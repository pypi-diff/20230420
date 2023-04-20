# Comparing `tmp/qtaf-5.5.9.tar.gz` & `tmp/qtaf-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.5.9.tar", last modified: Tue Aug  2 08:55:00 2022, max compression
+gzip compressed data, was "qtaf-5.6.0.tar", last modified: Thu Apr 20 01:20:36 2023, max compression
```

## Comparing `qtaf-5.5.9.tar` & `qtaf-5.6.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.742926 qtaf-5.5.9/
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-08-02 08:54:46.000000 qtaf-5.5.9/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-02 08:54:46.000000 qtaf-5.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-08-02 08:55:00.742926 qtaf-5.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-08-02 08:54:46.000000 qtaf-5.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-02 08:54:46.000000 qtaf-5.5.9/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.730926 qtaf-5.5.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-02 08:54:46.000000 qtaf-5.5.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-02 08:54:46.000000 qtaf-5.5.9/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.730926 qtaf-5.5.9/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (121)     4473 2022-08-02 08:54:46.000000 qtaf-5.5.9/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     6582 2022-08-02 08:54:46.000000 qtaf-5.5.9/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 08:54:46.000000 qtaf-5.5.9/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1968182 2022-08-02 08:54:46.000000 qtaf-5.5.9/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.734926 qtaf-5.5.9/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-02 08:55:00.000000 qtaf-5.5.9/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-08-02 08:54:46.000000 qtaf-5.5.9/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-02 08:54:46.000000 qtaf-5.5.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 08:55:00.742926 qtaf-5.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-08-02 08:54:46.000000 qtaf-5.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.738926 qtaf-5.5.9/testbase/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25637 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)    11882 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (121)    10507 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    11944 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3292 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    31221 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (121)    11638 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    34337 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (121)    24520 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (121)    41124 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    47878 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (121)    27419 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    25689 2022-08-02 08:54:46.000000 qtaf-5.5.9/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-02 08:55:00.000000 qtaf-5.5.9/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:55:00.742926 qtaf-5.5.9/tuia/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (121)    16530 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-08-02 08:54:46.000000 qtaf-5.5.9/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-02 08:54:59.000000 qtaf-5.5.9/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.331433 qtaf-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 01:20:26.000000 qtaf-5.6.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 01:20:26.000000 qtaf-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 01:20:36.331433 qtaf-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-20 01:20:26.000000 qtaf-5.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-20 01:20:26.000000 qtaf-5.6.0/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.323433 qtaf-5.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 01:20:26.000000 qtaf-5.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.323433 qtaf-5.6.0/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.327433 qtaf-5.6.0/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 01:20:26.000000 qtaf-5.6.0/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 01:20:26.000000 qtaf-5.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 01:20:36.331433 qtaf-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-20 01:20:26.000000 qtaf-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.327433 qtaf-5.6.0/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35361 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 01:20:36.000000 qtaf-5.6.0/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.331433 qtaf-5.6.0/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 01:20:35.000000 qtaf-5.6.0/version.txt
```

### Comparing `qtaf-5.5.9/LICENSE.TXT` & `qtaf-5.6.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.5.9/PKG-INFO` & `qtaf-5.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.5.9
+Version: 5.6.0
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # QTAF
 
@@ -80,9 +79,7 @@
 TUIA (Tencent UI Automation)是UI自动化基础库，为QTA各个平台下的客户端UI测试Driver所使用。
 
 快速入门、使用和接口文档请参考《[TUIA文档](http://qta-tuia.readthedocs.io/zh/latest/index.html)》。
 
 ------------------------------
 
 欢迎加入QQ群（432699528）交流使用和反馈
-
-
```

### Comparing `qtaf-5.5.9/README.md` & `qtaf-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.5.9/__main__.py` & `qtaf-5.6.0/qta-manage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''QTAF执行入口
-'''
-
 from testbase.management import qta_manage_main
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     qta_manage_main()
-    
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qtaf-5.5.9/qta-manage.py` & `qtaf-5.6.0/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,14 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
+"""QTAF执行入口
+"""
+
 from testbase.management import qta_manage_main
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     qta_manage_main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtaf-5.5.9/qta_statics/TestReport.xsl` & `qtaf-5.6.0/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.5.9/qta_statics/TestResult.xsl` & `qtaf-5.6.0/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.5.9/qta_statics/qta-report.html` & `qtaf-5.6.0/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.5.9/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.0/qtaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.5.9
+Version: 5.6.0
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # QTAF
 
@@ -80,9 +79,7 @@
 TUIA (Tencent UI Automation)是UI自动化基础库，为QTA各个平台下的客户端UI测试Driver所使用。
 
 快速入门、使用和接口文档请参考《[TUIA文档](http://qta-tuia.readthedocs.io/zh/latest/index.html)》。
 
 ------------------------------
 
 欢迎加入QQ群（432699528）交流使用和反馈
-
-
```

### Comparing `qtaf-5.5.9/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.0/qtaf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 testbase/resource.py
 testbase/retry.py
 testbase/runner.py
 testbase/serialization.py
 testbase/test.py
 testbase/testcase.py
 testbase/testresult.py
+testbase/testsuite.py
 testbase/types.py
 testbase/util.py
 testbase/version.py
 tuia/__init__.py
 tuia/_tif.py
 tuia/accessible.py
 tuia/app.py
```

### Comparing `qtaf-5.5.9/qtaf_settings.py` & `qtaf-5.6.0/tuia/testcase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,22 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
-QTAF配置文件
-'''
-# -----------------------------------
-# 调试模式开关
-# -----------------------------------
-DEBUG = False
- 
-# -----------------------------------
-# 全局数据驱动配置
-# -----------------------------------
-DATA_DRIVE = False
-DATA_SOURCE = 'test/data/server.py'
-
-# -----------------------------------
-# 项目配置
-# -----------------------------------
-PROJECT_NAME = 'qtaf'
-PROJECT_MODE = 'standalone' #choices: standard/standalone
-PROJECT_ROOT = None#os.path.dirname(__file__)
-INSTALLED_APPS = []
-
 
-# -----------------------------------
-# Assert 
-# -----------------------------------
-QTAF_REWRITE_ASSERT = True
+import warnings
 
+warnings.warn(
+    "`tuia.testcase` is depressed, please use `qt4c.testcase` instead",
+    DeprecationWarning,
+)
+from qt4c.testcase import *  # pylint: disable=wildcard-import
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qtaf-5.5.9/setup.py` & `qtaf-5.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,53 +23,66 @@
 def generate_version():
     version = "1.0.0"
     if os.path.isfile(os.path.join(BASE_DIR, "version.txt")):
         with codecs.open("version.txt", "r", encoding="utf-8") as fd:
             content = fd.read().strip()
             if content:
                 version = content
-    with codecs.open(os.path.join(BASE_DIR, "testbase", "version.py"), "w", encoding="utf-8") as fd:
+    with codecs.open(
+        os.path.join(BASE_DIR, "testbase", "version.py"), "w", encoding="utf-8"
+    ) as fd:
         fd.write('version = "%s"\n' % version)
     return str(version)
 
 
 def parse_requirements():
     reqs = []
     if os.path.isfile(os.path.join(BASE_DIR, "requirements.txt")):
-        with codecs.open(os.path.join(BASE_DIR, "requirements.txt"), 'r', encoding="utf-8") as fd:
+        with codecs.open(
+            os.path.join(BASE_DIR, "requirements.txt"), "r", encoding="utf-8"
+        ) as fd:
             for line in fd.readlines():
                 line = line.strip()
                 if line:
                     reqs.append(line)
         return reqs
 
 
 def get_description():
     with codecs.open(os.path.join(BASE_DIR, "README.md"), "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 if __name__ == "__main__":
     setup(
-      version=generate_version(),
-      name="qtaf",
-      packages=find_packages(exclude=("tests", "tests.*",)),
-      py_modules=["qtaf_settings", "__main__", "qta-manage"],
-      include_package_data=True,
-      package_data={'':['*.txt', '*.TXT'], },
-      description="Basic test automation framework for QTA",
-      long_description=get_description(),
-      long_description_content_type="text/markdown",
-      author="Tencent",
-      license="Copyright(c)2010-2018 Tencent All Rights Reserved. ",
-      install_requires=parse_requirements(),
-      entry_points={'console_scripts': ['qta-manage = testbase.management:qta_manage_main'], },
-      classifiers=[
-        "Programming Language :: Python :: 2.7",
-        "Operating System :: OS Independent",
-      ],
-      url="https://github.com/Tencent/QTAF",
-      project_urls={
-          "TestBase Documentation": "https://qta-testbase.readthedocs.io/zh/latest/",
-          "TUIA Documentation": "https://qta-tuia.readthedocs.io/zh/latest/"
-      },
+        version=generate_version(),
+        name="qtaf",
+        packages=find_packages(
+            exclude=(
+                "tests",
+                "tests.*",
+            )
+        ),
+        py_modules=["qtaf_settings", "__main__", "qta-manage"],
+        include_package_data=True,
+        package_data={
+            "": ["*.txt", "*.TXT"],
+        },
+        description="Basic test automation framework for QTA",
+        long_description=get_description(),
+        long_description_content_type="text/markdown",
+        author="Tencent",
+        license="Copyright(c)2010-2018 Tencent All Rights Reserved. ",
+        install_requires=parse_requirements(),
+        entry_points={
+            "console_scripts": ["qta-manage = testbase.management:qta_manage_main"],
+        },
+        classifiers=[
+            "Programming Language :: Python :: 2.7",
+            "Operating System :: OS Independent",
+        ],
+        url="https://github.com/Tencent/QTAF",
+        project_urls={
+            "TestBase Documentation": "https://qta-testbase.readthedocs.io/zh/latest/",
+            "TUIA Documentation": "https://qta-tuia.readthedocs.io/zh/latest/",
+        },
     )
```

### Comparing `qtaf-5.5.9/testbase/__init__.py` & `qtaf-5.6.0/testbase/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''测试框架类库
-'''
+"""测试框架类库
+"""
 
 from .testcase import TestCase, TestCaseStatus, TestCasePriority
-from .version import version
+from .version import version
```

### Comparing `qtaf-5.5.9/testbase/assertion.py` & `qtaf-5.6.0/testbase/assertion.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 from __future__ import print_function, absolute_import
 
 import ast
 import copy
 import inspect
 import itertools
 import pprint
-import six
 import sys
 import threading
 import traceback
 import types
 
+import six
+
 from testbase.util import Singleton, get_method_defined_class, smart_text
-from testbase.conf import settings
 
 unary_map = {ast.Not: "not %s", ast.Invert: "~%s", ast.USub: "-%s", ast.UAdd: "+%s"}
 
 binop_map = {
     ast.BitOr: "|",
     ast.BitXor: "^",
     ast.BitAnd: "&",
@@ -55,25 +55,26 @@
     ast.Is: "is",
     ast.IsNot: "is not",
     ast.In: "in",
     ast.NotIn: "not in",
 }
 
 if sys.version_info >= (3, 5):
-    ast_Call = ast.Call
+    ast_Call = ast.Call  # pylint: disable=invalid-name
 else:
 
-    def ast_Call(a, b, c):
+    def ast_Call(a, b, c):  # pylint: disable=invalid-name
         return ast.Call(a, b, c, None, None)
 
+
 if hasattr(ast, "NameConstant"):
-    _NameConstant = ast.NameConstant
+    _NameConstant = ast.NameConstant  # pylint: disable=invalid-name
 else:
 
-    def _NameConstant(c):
+    def _NameConstant(c):  # pylint: disable=invalid-name
         return ast.Name(str(c), ast.Load())
 
 
 def set_location(node, lineno, col_offset):
     """Set node location information recursively."""
 
     def _fix(node, lineno, col_offset):
@@ -104,21 +105,20 @@
             func.__code__ = copy.deepcopy(item)
             break
     else:
         raise RuntimeError("no match name function for %s" % code.co_name)
 
 
 class AssertionRewriter(ast.NodeVisitor):
-    """assert rewriter
-    """
+    """assert rewriter"""
 
     def rewrite(self, item):
         try:
             self.rewrite_(item)
-        except:
+        except Exception:  # pylint: disable=broad-except
             stack = traceback.format_exc()
             msg = "[WARN]rewrite item %s failed: %s" % (item, stack)
             print(msg, file=sys.stderr)
 
     def rewrite_(self, item):
         """Find all assert statements in *mod* and rewrite them."""
         func = item
@@ -126,31 +126,63 @@
             return
 
         mod, func_node = get_func_mod_and_node(func)
         if mod is None and func_node is None:
             _AssertHookedCache().add(func)
             return
 
+        pos = 0
+        lineno = func_node.lineno
+        col_offset = func_node.col_offset
         # compatibility with py 2 and 3
         if sys.version_info[0] == 3:
             builtins_mod = "builtins"
         else:
             builtins_mod = "__builtin__"
-        aliases = [
-            ast.alias(builtins_mod, "_py_builtins_"),
-            ast.alias("testbase.assertion", "_qtaf_assert_"),
-        ]
-        pos = 0
-        lineno = func_node.lineno
-        col_offset = func_node.col_offset
+        # Now actually insert the special imports.
+        if sys.version_info >= (3, 10):
+            aliases = [
+                ast.alias(builtins_mod, "_py_builtins_", lineno=lineno, col_offset=0),
+                ast.alias(
+                    "testbase.assertion",
+                    "_qtaf_assert_",
+                    lineno=lineno,
+                    col_offset=0,
+                ),
+            ]
+        else:
+            aliases = [
+                ast.alias(builtins_mod, "_py_builtins_"),
+                ast.alias("testbase.assertion", "_qtaf_assert_"),
+            ]
 
         imports = [
-            ast.Import([alias], lineno=lineno, col_offset=col_offset) for alias in aliases
+            ast.Import([alias], lineno=lineno, col_offset=col_offset)
+            for alias in aliases
         ]
-        imports.append(ast.ImportFrom(module="testbase.testresult", names=[ast.alias('EnumLogLevel', None)], level=0, lineno=lineno, col_offset=col_offset))
+        if sys.version_info >= (3, 10):
+            imports.append(
+                ast.ImportFrom(
+                    module="testbase.testresult",
+                    names=[ast.alias("EnumLogLevel", None, lineno=lineno, col_offset=0)],
+                    level=0,
+                    lineno=lineno,
+                    col_offset=col_offset,
+                )
+            )
+        else:
+            imports.append(
+                ast.ImportFrom(
+                    module="testbase.testresult",
+                    names=[ast.alias("EnumLogLevel", None)],
+                    level=0,
+                    lineno=lineno,
+                    col_offset=col_offset,
+                )
+            )
         func_node.body[pos:pos] = imports
         nodes = [func_node]
         self.rewrite_code = False
         while nodes:
             node = nodes.pop()
             self.iter_ast_node(node)
         if self.rewrite_code:
@@ -171,29 +203,28 @@
                         new_nodes.append(child)
                     else:
                         new_nodes.append(child)
                 setattr(node, field, new_nodes)
             if isinstance(value, ast.Expr):
                 self.visit(value)
 
-    def visit_Expr(self, expr):
+    def visit_Expr(self, expr):  # pylint: disable=invalid-name
         value = expr.value
         if isinstance(value, ast.Call):
             if isinstance(value.func, ast.Attribute):
                 if value.func.attr == "assert_":
                     return self.rewrite_assert_(expr)
             elif isinstance(value.func, ast.Name):
                 if value.func.id == "assert_":
                     return self.rewrite_assert_(value)
 
         return [expr]
 
     def rewrite_assert_(self, elem):
-        """rewrite the assert_ expression
-        """
+        """rewrite the assert_ expression"""
         self.rewrite_code = True
         self.statements = []
         self.variables = []
         self.variable_counter = itertools.count()
         self.stack = []
         self.on_failure = []
         self.push_format_context()
@@ -214,17 +245,18 @@
         self.statements.append(ast.If(negation, body, []))
         assertmsg = self.helper("format_assertmsg", msg_arg)
         explanation = " " + explanation
         template = ast.BinOp(assertmsg, ast.Add(), ast.Str(explanation))
         msg = self.pop_format_context(template)
         fmt = self.helper("format_explanation", msg)
         log_record = ast.Attribute(
-                                value=ast.Name(id=caller_id, ctx=ast.Load()),
-                                attr='_log_assert_failed',
-                                ctx=ast.Load())
+            value=ast.Name(id=caller_id, ctx=ast.Load()),
+            attr="_log_assert_failed",
+            ctx=ast.Load(),
+        )
         args = [fmt]
         exc = ast_Call(log_record, args, [])
         log_record_expr = ast.Expr(value=exc)
         body.append(log_record_expr)
         # Clear temporary variables by setting them to None.
         if self.variables:
             variables = [ast.Name(name, ast.Store()) for name in self.variables]
@@ -311,25 +343,25 @@
 
     def generic_visit(self, node):
         """Handle expressions we don't have custom code for."""
         assert isinstance(node, ast.expr)
         res = self.assign(node)
         return res, self.explanation_param(self.display(res))
 
-    def visit_Name(self, name):
+    def visit_Name(self, name):  # pylint: disable=invalid-name
         # Display the repr of the name if it's a local variable or
         # _should_repr_global_name() thinks it's acceptable.
         locs = ast_Call(self.builtin("locals"), [], [])
         inlocs = ast.Compare(ast.Str(name.id), [ast.In()], [locs])
         dorepr = self.helper("should_repr_global_name", name)
         test = ast.BoolOp(ast.Or(), [inlocs, dorepr])
         expr = ast.IfExp(test, self.display(name), ast.Str(name.id))
         return name, self.explanation_param(expr)
 
-    def visit_BoolOp(self, boolop):
+    def visit_BoolOp(self, boolop):  # pylint: disable=invalid-name
         res_var = self.variable()
         expl_list = self.assign(ast.List([], ast.Load()))
         app = ast.Attribute(expl_list, "append", ast.Load())
         is_or = int(isinstance(boolop.op, ast.Or))
         body = save = self.statements
         fail_save = self.on_failure
         levels = len(boolop.values) - 1
@@ -357,29 +389,29 @@
                 self.statements = body = inner
         self.statements = save
         self.on_failure = fail_save
         expl_template = self.helper("format_boolop", expl_list, ast.Num(is_or))
         expl = self.pop_format_context(expl_template)
         return ast.Name(res_var, ast.Load()), self.explanation_param(expl)
 
-    def visit_UnaryOp(self, unary):
+    def visit_UnaryOp(self, unary):  # pylint: disable=invalid-name
         pattern = unary_map[unary.op.__class__]
         operand_res, operand_expl = self.visit(unary.operand)
         res = self.assign(ast.UnaryOp(unary.op, operand_res))
         return res, pattern % (operand_expl,)
 
-    def visit_BinOp(self, binop):
+    def visit_BinOp(self, binop):  # pylint: disable=invalid-name
         symbol = binop_map[binop.op.__class__]
         left_expr, left_expl = self.visit(binop.left)
         right_expr, right_expl = self.visit(binop.right)
         explanation = "(%s %s %s)" % (left_expl, symbol, right_expl)
         res = self.assign(ast.BinOp(left_expr, binop.op, right_expr))
         return res, explanation
 
-    def visit_Call_35(self, call):
+    def visit_Call_35(self, call):  # pylint: disable=invalid-name
         """
         visit `ast.Call` nodes on Python3.5 and after
         """
         new_func, func_expl = self.visit(call.func)
         arg_expls = []
         new_args = []
         new_kwargs = []
@@ -398,20 +430,20 @@
         expl = "%s(%s)" % (func_expl, ", ".join(arg_expls))
         new_call = ast.Call(new_func, new_args, new_kwargs)
         res = self.assign(new_call)
         res_expl = self.explanation_param(self.display(res))
         outer_expl = "%s\n{%s = %s\n}" % (res_expl, res_expl, expl)
         return res, outer_expl
 
-    def visit_Starred(self, starred):
+    def visit_Starred(self, starred):  # pylint: disable=invalid-name
         # From Python 3.5, a Starred node can appear in a function call
         _, expl = self.visit(starred.value)
         return starred, "*" + expl
 
-    def visit_Call_legacy(self, call):
+    def visit_Call_legacy(self, call):  # pylint: disable=invalid-name
         """
         visit `ast.Call nodes on 3.4 and below`
         """
         new_func, func_expl = self.visit(call.func)
         arg_expls = []
         new_args = []
         new_kwargs = []
@@ -437,29 +469,29 @@
         outer_expl = "%s\n{%s = %s\n}" % (res_expl, res_expl, expl)
         return res, outer_expl
 
     # ast.Call signature changed on 3.5,
     # conditionally change  which methods is named
     # visit_Call depending on Python version
     if sys.version_info >= (3, 5):
-        visit_Call = visit_Call_35
+        visit_Call = visit_Call_35  # pylint: disable=invalid-name
     else:
-        visit_Call = visit_Call_legacy
+        visit_Call = visit_Call_legacy  # pylint: disable=invalid-name
 
-    def visit_Attribute(self, attr):
+    def visit_Attribute(self, attr):  # pylint: disable=invalid-name
         if not isinstance(attr.ctx, ast.Load):
             return self.generic_visit(attr)
         value, value_expl = self.visit(attr.value)
         res = self.assign(ast.Attribute(value, attr.attr, ast.Load()))
         res_expl = self.explanation_param(self.display(res))
         pat = "%s\n{%s = %s.%s\n}"
         expl = pat % (res_expl, res_expl, value_expl, attr.attr)
         return res, expl
 
-    def visit_Compare(self, comp):
+    def visit_Compare(self, comp):  # pylint: disable=invalid-name
         self.push_format_context()
         left_res, left_expl = self.visit(comp.left)
         if isinstance(comp.left, (ast.Compare, ast.BoolOp)):
             left_expl = "({})".format(left_expl)
         res_variables = [self.variable() for i in range(len(comp.ops))]
         load_names = [ast.Name(v, ast.Load()) for v in res_variables]
         store_names = [ast.Name(v, ast.Store()) for v in res_variables]
@@ -494,15 +526,15 @@
         return res, self.explanation_param(self.pop_format_context(expl_call))
 
 
 def _call_reprcompare(ops, results, expls, each_obj):
     for _, res, expl in zip(range(len(ops)), results, expls):
         try:
             done = not res
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             done = True
         if done:
             break
     return expl
 
 
 def _saferepr(obj):
@@ -540,15 +572,15 @@
     newlines.  For other objects py.io.saferepr() is used first.
 
     """
     # reprlib appears to have a bug which means that if a string
     # contains a newline it gets escaped, however if an object has a
     # .__repr__() which contains newlines it does not get escaped.
     # However in either case we want to preserve the newline.
-#     if isinstance(obj, six.text_type) or isinstance(obj, six.binary_type):
+    #     if isinstance(obj, six.text_type) or isinstance(obj, six.binary_type):
     if isinstance(obj, six.string_types):
         s = smart_text(obj)
         is_repr = False
     else:
         s = pprint.saferepr(obj)
         is_repr = True
     t = str
@@ -564,48 +596,48 @@
     Normally all embedded newlines are escaped, however there are
     three exceptions: \n{, \n} and \n~.  The first two are intended
     cover nested explanations, see function and attribute explanations
     for examples (.visit_Call(), visit_Attribute()).  The last one is
     for when one explanation needs to span multiple lines, e.g. when
     displaying diffs.
     """
-    raw_lines = (explanation or '').split('\n')
+    raw_lines = (explanation or "").split("\n")
     # escape newlines not followed by {, } and ~
     msg = raw_lines[0]
     raw_lines = raw_lines[1:]
     lines = raw_lines[:1]
     for l in raw_lines[1:]:
-        if l.startswith('{') or l.startswith('}') or l.startswith('~'):
+        if l.startswith("{") or l.startswith("}") or l.startswith("~"):
             lines.append(l)
         else:
-            lines[-1] += '\\n' + l
+            lines[-1] += "\\n" + l
 
     result = lines[:1]
     stack = [0]
     stackcnt = [0]
     for line in lines[1:]:
-        if line.startswith('{'):
+        if line.startswith("{"):
             if stackcnt[-1]:
-                s = 'and   '
+                s = "and   "
             else:
-                s = 'where '
+                s = "where "
             stack.append(len(result))
             stackcnt[-1] += 1
             stackcnt.append(0)
-            result.append(' +' + '  ' * (len(stack) - 1) + s + line[1:])
-        elif line.startswith('}'):
+            result.append(" +" + "  " * (len(stack) - 1) + s + line[1:])
+        elif line.startswith("}"):
             stack.pop()
             stackcnt.pop()
             result[stack[-1]] += line[1:]
         else:
-            assert line.startswith('~')
-            result.append('  ' * len(stack) + line[1:])
+            assert line.startswith("~")
+            result.append("  " * len(stack) + line[1:])
     assert len(stack) == 1
     result[0] = " [%s] assert " % msg + result[0]
-    return '\n'.join(result)
+    return "\n".join(result)
 
 
 def get_func_name(func):
     if isinstance(func, types.MethodType):
         if sys.version_info[0] == 3:
             return func.__func__.__name__
         else:
@@ -656,15 +688,18 @@
 
 def get_func_compiled_code(func, new_code):
     func_name = get_func_name(func)
     if isinstance(func, types.MethodType):
         for item in new_code.co_consts:
             if isinstance(item, types.CodeType):
                 for sub_item in item.co_consts:
-                    if isinstance(sub_item, types.CodeType) and sub_item.co_name == func_name:
+                    if (
+                        isinstance(sub_item, types.CodeType)
+                        and sub_item.co_name == func_name
+                    ):
                         return sub_item
     elif isinstance(func, types.FunctionType):
         for item in new_code.co_consts:
             if isinstance(item, types.CodeType) and item.co_name == func_name:
                 return item
     else:
         raise RuntimeError("%s not supported yet" % repr(func))
@@ -678,15 +713,14 @@
         else:
             func.__func__.__code__ = new_func_code
     else:
         func.__code__ = new_func_code
 
 
 class _AssertHookedCache(six.with_metaclass(Singleton, object)):
-
     def __init__(self):
         self._lock = threading.Lock()
         self.__cache = set()
 
     def add(self, func):
         with self._lock:
             self.__cache.add(self._hash_func(func))
@@ -700,10 +734,13 @@
 
     def _hash_func(self, func):
         if isinstance(func, (types.FunctionType, types.MethodType)):
             return func
         else:
             raise ValueError("func must be a callable type or object")
 
+    def clear(self):
+        self.__cache.clear()
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `qtaf-5.5.9/testbase/conf.py` & `qtaf-5.6.0/testbase/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''配置接口
+"""配置接口
 
 一、配置格式
 配置文件名默认为settings.py，可以通过环境变量指定用户配置文件的路径
 qtaf相关配置的环境变量为：
 QTAF_EXLIB_PATH: 指定exlib的路径，exlib下放置对应的qtaf、qt4s、installed_libs.txt等文件
 QTAF_INSTALLED_LIBS: 指定已经安装的库的列表，以分号分隔，例如qt4s，用来代替不使用installed_libs.txt的场景
 QTAF_SETTINGS_MODULE: 指定用户自定义的配置文件的路径，最后加载，会覆盖已经存在的配置
@@ -36,15 +36,15 @@
 注意 settings的值都是只读的，不可以修改，如果尝试修改会导致异常
 
 三、配置优先级
 配置存在2个优先级，当存在名字冲突时，使用高优先级的配置的值。优先级自低到高分别为：
 1、QTAF配置                     固定为：test_proj/exlib/qtaf.egg/qtaf_settings.py
 2、lib配置                      已经配置在test_proj/exlib/installed_libs.txt的包中的settings模块
 3、用户自定义配置          固定为：test_proj/settings.py
-'''
+"""
 
 import imp
 import os
 import sys
 import traceback
 
 import qtaf_settings
@@ -52,153 +52,162 @@
 from testbase import logger
 from testbase.exlib import ExLibManager
 
 _DEFAULT_SETTINSG_MODULE = "settings"
 
 
 class _Settings(object):
-    '''配置读取接口
-    '''
+    """配置读取接口"""
 
     def __init__(self):
         self.__keys = set()
         self.__sealed = False
         self.__loaded = False
 
     def _load(self):
-        '''加载配置
+        """加载配置
         :returns: Settings - 设置读取接口
-        '''
+        """
         # get PROJECT_MODE from user settings
-        default_mode = getattr(qtaf_settings, 'PROJECT_MODE', None)
+        default_mode = getattr(qtaf_settings, "PROJECT_MODE", None)
         try:
             pre_settings = self._load_proj_settings_module("testbase.conf.pre_settings")
             mode = getattr(pre_settings, "PROJECT_MODE", default_mode)
         except ImportError as e:
             pre_settings = None
             if os.path.isfile(__file__):
                 mode = "standard"
             else:
                 mode = "standalone"
 
         if mode == "standard":  # library mode
             proj_root = getattr(pre_settings, "PROJECT_ROOT", os.getcwd())
-            installed_apps = getattr(pre_settings, "INSTALLED_APPS", getattr(qtaf_settings, 'INSTALLED_APPS', []))
+            installed_apps = getattr(
+                pre_settings,
+                "INSTALLED_APPS",
+                getattr(qtaf_settings, "INSTALLED_APPS", []),
+            )
 
         else:  # egg mode
             proj_root = self._get_standalone_project_root(pre_settings)
             installed_apps = ExLibManager(proj_root).list_names()
 
         # load settings from qtaf
         self._load_setting_from_module(qtaf_settings)
 
         # load settings from installed apps
         for appname in installed_apps:
             modname = "%s.settings" % appname
             try:
                 __import__(modname)
-            except:
+            except Exception:  # pylint: disable=broad-except
                 stack = traceback.format_exc()
-                logger.warn("[WARN]load library settings module \"%s\" failed:\n%s" % (modname, stack))
+                logger.warn(
+                    '[WARN]load library settings module "%s" failed:\n%s'
+                    % (modname, stack)
+                )
             else:
                 self._load_setting_from_module(sys.modules[modname])
 
         # load settings from user settings
         try:
             proj_settings = self._load_proj_settings_module("testbase.conf.settings")
         except ImportError as e:
-            if e.args[0] not in ["No module named settings", "No module named 'settings'"]:
+            if e.args[0] not in [
+                "No module named settings",
+                "No module named 'settings'",
+            ]:
                 # project settings found and there was an error
                 stack = traceback.format_exc()
                 logger.warn("[WARN]load project settings failed:\n%s" % stack)
         else:
             self._load_setting_from_module(proj_settings)
 
         # trying to set project root automatically
         setattr(self, "PROJECT_ROOT", proj_root)
         setattr(self, "INSTALLED_APPS", installed_apps)
 
     def _load_proj_settings_module(self, import_name):
-        '''加载项目配置文件
-        '''
+        """加载项目配置文件"""
         user_settings = os.environ.get("QTAF_SETTINGS_MODULE", None)
         if user_settings:
-            parts = user_settings.split('.')
+            parts = user_settings.split(".")
             parts_temp = parts[:]
             dir_path = None
             while parts_temp:
                 if dir_path:
                     fd, dir_path, desc = imp.find_module(parts_temp[0], [dir_path])
                 else:
                     fd, dir_path, desc = imp.find_module(parts_temp[0])
                 del parts_temp[0]
         else:
             fd, dir_path, desc = imp.find_module(_DEFAULT_SETTINSG_MODULE)
         return imp.load_module(import_name, fd, dir_path, desc)
 
     def _load_setting_from_module(self, module):
-        '''从模块中加载设置
-        '''
+        """从模块中加载设置"""
         for name in dir(module):
-            if name.startswith('__'):
+            if name.startswith("__"):
                 continue
             if name.islower():
                 continue
             self.__keys.add(name)
             setattr(self, name, getattr(module, name))
 
     def _get_standalone_project_root(self, pre_settings):
-        '''获取独立模式下的项目的根目录
-        '''
+        """获取独立模式下的项目的根目录"""
         proj_root = getattr(pre_settings, "PROJECT_ROOT", None)
         if proj_root:
             return proj_root
         if os.path.isfile(__file__):  # 没使用qtaf.egg包
             cwd = os.getcwd()
             # 使用外链或拷贝文件的方式
-            dst_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..')
+            dst_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "..")
             if cwd.find(dst_path) >= 0:
                 return os.path.abspath(dst_path)
 
             # eclipse调试使用工程引用的方式
-            if 'PYTHONPATH' not in os.environ:
+            if "PYTHONPATH" not in os.environ:
                 return cwd
-            py_paths = os.environ['PYTHONPATH']
+            py_paths = os.environ["PYTHONPATH"]
             paths = py_paths.split(";")
             if len(paths) > 2:
                 dst_path = paths[1]
             if cwd.find(dst_path) >= 0:
                 return dst_path
 
             # 非预期的情况，返回当前工作目录
             return cwd
         else:  # 使用的egg包，qtaf.egg包在exlib目录中
-            exlib_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', '..')
-            proj_root = os.path.abspath(os.path.join(exlib_dir, '..'))
+            exlib_dir = os.path.join(
+                os.path.dirname(os.path.abspath(__file__)), "..", ".."
+            )
+            proj_root = os.path.abspath(os.path.join(exlib_dir, ".."))
             return proj_root
 
     def get(self, name, *default_value):
-        '''获取配置
-        '''
+        """获取配置"""
         if len(default_value) > 1:
-            raise TypeError("get expected at most 3 arguments, got %s" % (len(default_value) + 2))
+            raise TypeError(
+                "get expected at most 3 arguments, got %s" % (len(default_value) + 2)
+            )
         if default_value:
             return getattr(self, name, default_value[0])
         else:
             return getattr(self, name)
 
     def __ensure_loaded(self):
         if not self.__loaded:
             self.__loaded = True
             self._load()
             self.__sealed = True
 
     def __setattr__(self, name, value):
-        if not name.startswith('_Settings__') and self.__sealed:
-            raise RuntimeError("尝试动态修改配置项\"%s\"" % name)
+        if not name.startswith("_Settings__") and self.__sealed:
+            raise RuntimeError('尝试动态修改配置项"%s"' % name)
         else:
             super(_Settings, self).__setattr__(name, value)
 
     def __getattribute__(self, name):
         try:
             return super(_Settings, self).__getattribute__(name)
         except AttributeError:
@@ -214,16 +223,15 @@
         return key in self.__keys
 
 
 settings = _Settings()
 
 
 class _InnerSettings(object):
-    """inner settings for a SettingsMixin class
-    """
+    """inner settings for a SettingsMixin class"""
 
     def __init__(self, defined_class):
         self.__tailer_names = {}
         self.__visited_settings_class = set()
         self.__allowed_prefix = set()
         self.__sealed = False
         self.__load_settings(defined_class)
@@ -261,51 +269,56 @@
                 if key in settings:
                     value = settings.get(key)
                 else:
                     value = getattr(inner_settings_cls, key)
                 setattr(self, key, value)
 
                 # handle legacy
-                tailor_name = key[len(prefix):]
+                tailor_name = key[len(prefix) :]
                 if tailor_name in self.__tailer_names:
                     for base_prefix in self.__tailer_names[tailor_name][:]:
                         base_name = base_prefix + tailor_name
                         setattr(self, base_name, value)
                         self.__tailer_names[tailor_name].append(prefix)
                 else:
                     self.__tailer_names[tailor_name] = [prefix]
 
             elif not key.startswith("_"):
                 for item in self.__allowed_prefix:
                     if key.startswith(item):
-                        tailor_name = key[len(item) + 1:]
+                        tailor_name = key[len(item) + 1 :]
                         break
                 else:
                     tailor_name = key.upper()
-                err_msg = "%s's Settings item `%s` must start with %s like %s%s" % (class_path, key, prefix, prefix, tailor_name)
+                err_msg = "%s's Settings item `%s` must start with %s like %s%s" % (
+                    class_path,
+                    key,
+                    prefix,
+                    prefix,
+                    tailor_name,
+                )
                 raise RuntimeError(err_msg)
 
     def __setattr__(self, name, value):
-        if not name.startswith('_InnerSettings__') and self.__sealed:
+        if not name.startswith("_InnerSettings__") and self.__sealed:
             raise RuntimeError("dynamicly modifying value is not allowed.")
         super(_InnerSettings, self).__setattr__(name, value)
 
     def __getattribute__(self, name):
         try:
             return super(_InnerSettings, self).__getattribute__(name)
         except AttributeError:
             if name in settings:
                 return settings.get(name)
             else:
                 raise
 
 
 class SettingsMixin(object):
-    """a mixin class coordinate with qtaf settings
-    """
+    """a mixin class coordinate with qtaf settings"""
 
     @property
     def settings(self):
         cls = type(self)
         settings_key = "_%s_settings" % cls.__name__
         if not hasattr(cls, settings_key):
             if not hasattr(cls, "Settings"):
```

### Comparing `qtaf-5.5.9/testbase/context.py` & `qtaf-5.6.0/testbase/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 测试用例执行时上下文
-'''
+"""
 
 from testbase.util import ThreadGroupLocal
 
+
 def current_testcase():
-    '''当前正在执行的用例
-    
+    """当前正在执行的用例
+
     :returns: TestCase
-    '''
-    return getattr(ThreadGroupLocal(), 'testcase', None)
+    """
+    return getattr(ThreadGroupLocal(), "testcase", None)
+
 
 def current_testresult():
-    '''当前正在执行的用例对应的测试结果
-    
+    """当前正在执行的用例对应的测试结果
+
     :returns: TestResult
-    '''
-    return getattr(ThreadGroupLocal(), 'testresult', None)
+    """
+    return getattr(ThreadGroupLocal(), "testresult", None)
+
 
 def current_testcase_local():
-    return ThreadGroupLocal()
+    return ThreadGroupLocal()
```

### Comparing `qtaf-5.5.9/testbase/datadrive.py` & `qtaf-5.6.0/testbase/datadrive.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,17 +80,18 @@
 
     if __name__ == '__main__':
         MyTest().run()
 
 '''
 from __future__ import absolute_import
 
-import six
 import types
 
+import six
+
 from testbase import logger
 from testbase.conf import settings
 from testbase.testcase import TestCase
 from testbase.util import translate_bad_char, has_bad_char, smart_text
 
 
 def translate_bad_char4exclude_keys(data_key):
@@ -98,78 +99,76 @@
         data_key = smart_text(data_key)
     else:
         data_key = str(data_key)
     data_key = translate_bad_char(data_key)
     return data_key
 
 
-
 class DataDrive(object):
-    '''数据驱动类修饰器，标识一个测试用例类使用数据驱动
-    '''
+    """数据驱动类修饰器，标识一个测试用例类使用数据驱动"""
 
     def __init__(self, case_data):
-        '''构造函数
+        """构造函数
 
         :param case_datas: 数据驱动测试数据集
         :type case_datas: list/tuple/dict
-        '''
+        """
         self._case_data = case_data
 
     def __call__(self, testcase_class):
-        '''修饰器
+        """修饰器
 
         :param testcase_class: 要修饰的测试用例
         :type testcase_class: TestCase
-        '''
+        """
         if not issubclass(testcase_class, TestCase):
-            raise TypeError('data driver decorator cannot be applied to non-TestCase type')
+            raise TypeError(
+                "data driver decorator cannot be applied to non-TestCase type"
+            )
         testcase_class.__qtaf_datadrive__ = self
         return testcase_class
 
     def __iter__(self):
-        '''遍历全部的数据名
-        '''
+        """遍历全部的数据名"""
         if isinstance(self._case_data, types.GeneratorType):
             self._case_data = list(self._case_data)
         if isinstance(self._case_data, list) or isinstance(self._case_data, tuple):
             for it in range(len(self._case_data)):
                 yield it
         else:
             for it in self._case_data:
                 yield it
 
     def __getitem__(self, name):
-        '''获取对应名称的数据
-        '''
+        """获取对应名称的数据"""
         return self._case_data[name]
 
     def __len__(self):
         return len(self._case_data)
 
 
 def is_datadrive(obj):
-    '''是否为数据驱动用例
+    """是否为数据驱动用例
 
     :param obj: 测试用例或测试用例类
     :type obj: TestCase/type
 
     :returns boolean
-    '''
-    return hasattr(obj, '__qtaf_datadrive__')
+    """
+    return hasattr(obj, "__qtaf_datadrive__")
 
 
 def get_datadrive(obj):
-    '''获取对应用例的数据驱动
+    """获取对应用例的数据驱动
 
     :param obj: 测试用例或测试用例类
     :type obj: TestCase/type
 
     :returns DataDrive
-    '''
+    """
     return obj.__qtaf_datadrive__
 
 
 def _get_translated_in_datadrive(name, dd):
     if isinstance(name, six.string_types):
         name = smart_text(name)
     else:
@@ -192,38 +191,40 @@
     else:
         data_key = str(data_key)
     data_key = translate_bad_char(data_key)
     return data_key
 
 
 def load_datadrive_tests(cls, name=None, exclude_data_key=None, attrs=None):
-    '''加载对应数据驱动测试用例类的数据驱动用例
-    '''
+    """加载对应数据驱动测试用例类的数据驱动用例"""
     if is_datadrive(cls):
         dd = get_datadrive(cls)
     else:
         if not settings.DATA_DRIVE:
             raise RuntimeError("DATA_DRIVE is not set to True")
 
         from testbase.loader import TestDataLoader
+
         dd = TestDataLoader().load()
 
     if name:
         if name in dd:
-            drive_data = {name : dd[name]}
+            drive_data = {name: dd[name]}
         else:
             drive_value = _get_translated_in_datadrive(name, dd)
-            drive_data = {name : drive_value}
+            drive_data = {name: drive_value}
     else:
         drive_data = dd
 
     if exclude_data_key is None:
         exclude_data_key = []
 
-    exclude_data_key = [_translate_bad_char4exclude_keys(item) for item in exclude_data_key]
+    exclude_data_key = [
+        _translate_bad_char4exclude_keys(item) for item in exclude_data_key
+    ]
 
     tests = []
     for item in drive_data:
         # 如果有排除标签
         exclude_item = _translate_bad_char4exclude_keys(item)
         if exclude_data_key is not None and exclude_item in exclude_data_key:
             continue
@@ -231,15 +232,18 @@
         if isinstance(item, six.string_types):
             item = smart_text(item)
         else:
             item = str(item)
         casedata_name = item
         if has_bad_char(item):
             casedata_name = translate_bad_char(item)
-            warn_msg = "[WARNING]%r's drive data key should use \"%s\" instead of \"%s\"" % (cls, casedata_name, item)
+            warn_msg = (
+                '[WARNING]%r\'s drive data key should use "%s" instead of "%s"'
+                % (cls, casedata_name, item)
+            )
             logger.warn(warn_msg)
 
         if isinstance(testdata, dict) and "__attrs__" in testdata:
             new_attrs = testdata.get("__attrs__")
         else:
             new_attrs = None
 
@@ -247,8 +251,7 @@
             if not new_attrs:
                 new_attrs = attrs
             else:
                 new_attrs.update(attrs)
 
         tests.append(cls(testdata, casedata_name, new_attrs))
     return tests
-
```

### Comparing `qtaf-5.5.9/testbase/dist.py` & `qtaf-5.6.0/testbase/dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 """
 
 import os
 import sys
 import re
 import shutil
 import zipfile
-import pkg_resources
 import subprocess
 
+import pkg_resources
+
 from testbase import resource
 from testbase.conf import settings
 from testbase.util import codecs_open
 
 SETUP_PY_TEMPLATE = """
 from setuptools import setup, find_packages
 
@@ -167,38 +168,40 @@
         self._version = version
 
     def run(self, exclude_resources):
         self._generate_sdist(exclude_resources=exclude_resources)
 
     def _merge_requirements(self):
         """Merge exlib & requirements.txt"""
-        exlib = os.path.join(settings.PROJECT_ROOT, 'exlib')
-        egg_pattern = re.compile(r"(?P<name>[a-zA-Z0-9_]+)(\-(?P<version>[0-9a-zA-Z_\.]+)|)(\-.*|)\.egg$")
+        exlib = os.path.join(settings.PROJECT_ROOT, "exlib")
+        egg_pattern = re.compile(
+            r"(?P<name>[a-zA-Z0-9_]+)(\-(?P<version>[0-9a-zA-Z_\.]+)|)(\-.*|)\.egg$"
+        )
         reqs_dict = {}
 
         req_txt = os.path.join(settings.PROJECT_ROOT, "requirements.txt")
         if os.path.isfile(req_txt):
-            with codecs_open(req_txt, 'r', encoding="utf-8") as fd:
+            with codecs_open(req_txt, "r", encoding="utf-8") as fd:
                 for it in pkg_resources.parse_requirements(fd.read()):
                     reqs_dict[it.name] = str(it)
 
         elif os.path.isdir(exlib):
             for filename in os.listdir(exlib):
                 if not filename.endswith(".egg"):
                     continue
                 result = egg_pattern.match(filename)
                 if not result:
                     continue
-                name, version = result.group('name'), result.group('version')
+                name, version = result.group("name"), result.group("version")
                 if version:
                     reqs_dict[name] = "%s==%s" % (name, version)
                 else:
                     reqs_dict[name] = name
 
-        if 'qtaf' not in reqs_dict:
+        if "qtaf" not in reqs_dict:
             reqs_dict["qtaf"] = "qtaf"
         return reqs_dict.values()
 
     def _generate_sdist(self, exclude_resources):
         """Call setuptools to generate source dist"""
         reqs = self._merge_requirements()
         setup_py = os.path.join(settings.PROJECT_ROOT, "setup.py")
@@ -206,21 +209,24 @@
             template = SETUP_PY_TEMPLATE
             cmd = "sdist"
         else:
             template = SETUP_PY_TEMPLATE_INCLUDE_RESOURCE
             cmd = "sdist_qta"
 
         with codecs_open(setup_py, "w", encoding="utf-8") as fd:
-            fd.write(template % dict(
-                version=self._version,
-                name=settings.PROJECT_NAME,
-                requirements=repr(reqs),
-                python_main_ver=sys.version_info[0],
-                python_vice_ver=sys.version_info[1]
-            ))
+            fd.write(
+                template
+                % dict(
+                    version=self._version,
+                    name=settings.PROJECT_NAME,
+                    requirements=repr(reqs),
+                    python_main_ver=sys.version_info[0],
+                    python_vice_ver=sys.version_info[1],
+                )
+            )
 
         subprocess.call(["python", "setup.py", cmd], cwd=settings.PROJECT_ROOT)
         os.remove(setup_py)
 
     def _generate_resource_pkg(self):
         filename = "%s-%s-resource.zip" % (settings.PROJECT_NAME, self._version)
         filepath = os.path.join(settings.PROJECT_ROOT, "dist", filename)
@@ -229,16 +235,15 @@
                 for dirpath, _, filenames in os.walk(res_path):
                     for filename in filenames:
                         src = os.path.join(dirpath, filename)
                         zf.write(src, os.path.relpath(src, res_path))
 
 
 class VirtuelEnv(object):
-    """virtual env for QTA test project
-    """
+    """virtual env for QTA test project"""
 
     VENV_ENV_NAME = "QTAF_VENV"
 
     def __init__(self, dist_pkg_path, path=None, recreate=False):
         self._dist_pkg_path = dist_pkg_path
         self._venv = path
         self._recreate_venv = recreate
@@ -267,24 +272,24 @@
             venv_path = self._venv
         else:
             venv_path = os.path.basename(self._dist_pkg_path)
             if venv_path.endswith(".zip"):
                 venv_path = venv_path.rsplit(".", 1)[0]
             elif venv_path.endswith(".tar.gz"):
                 venv_path = venv_path.rsplit(".", 2)[0]
-            venv_path = venv_path + '_venv'
+            venv_path = venv_path + "_venv"
         if (not os.path.isdir(venv_path)) or self._recreate_venv:
             if os.path.isdir(venv_path):
                 shutil.rmtree(venv_path)
             virtualenv.create_environment(venv_path, site_packages=True)
             created = True
         else:
             created = False
         _, _, _, bin_dir = virtualenv.path_locations(venv_path)
-        activation_script = os.path.join(bin_dir, 'activate_this.py')
+        activation_script = os.path.join(bin_dir, "activate_this.py")
         with open(activation_script) as fd:
             exec(fd.read(), dict(__file__=activation_script))
         if created:
             subprocess.call(["pip", "install", self._dist_pkg_path], close_fds=True)
 
         os.environ[self.VENV_ENV_NAME] = "1"
         argv = list(sys.argv)
```

### Comparing `qtaf-5.5.9/testbase/exlib.py` & `qtaf-5.6.0/testbase/exlib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,141 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 扩展库管理（仅独立模式使用）
-'''
+"""
 
 import os
 import zipfile
 import shutil
 import logging
 import xml.dom.minidom as dom
 
 from testbase.util import codecs_open
 
+
 class ExLibManager(object):
-    '''扩展库管理器
-    '''
-    def __init__(self, proj_root ):
+    """扩展库管理器"""
+
+    def __init__(self, proj_root):
         self._top_dir = proj_root
-        self._installed_libs = os.path.join(self._top_dir, 'exlib', 'installed_libs.txt')
-    
-    def _get_egg_name(self, egg_path ):
-        '''获取egg包名称
-        '''
-        with zipfile.ZipFile(egg_path, 'r') as egg:
-            with egg.open('EGG-INFO/PKG-INFO', 'r') as fd:
+        self._installed_libs = os.path.join(
+            self._top_dir, "exlib", "installed_libs.txt"
+        )
+
+    def _get_egg_name(self, egg_path):
+        """获取egg包名称"""
+        with zipfile.ZipFile(egg_path, "r") as egg:
+            with egg.open("EGG-INFO/PKG-INFO", "r") as fd:
                 for line in fd.readlines():
-                    if line.startswith('Name:'):
-                        return line.split(':')[1].strip()
+                    if line.startswith("Name:"):
+                        return line.split(":")[1].strip()
 
-    def install(self, egg_path ):
-        '''安装
-        '''
-        #获取全部的顶级package
+    def install(self, egg_path):
+        """安装"""
+        # 获取全部的顶级package
         toplv_pkgs = []
-        with zipfile.ZipFile(egg_path, 'r') as egg:
+        with zipfile.ZipFile(egg_path, "r") as egg:
             for f in egg.filelist:
-                items = f.filename.split('/')
-                if len(items) == 2 and items[1].lower() == '__init__.py':
+                items = f.filename.split("/")
+                if len(items) == 2 and items[1].lower() == "__init__.py":
                     toplv_pkgs.append(items[0])
-        
-        exlib_dir = os.path.join(self._top_dir, 'exlib')
+
+        exlib_dir = os.path.join(self._top_dir, "exlib")
         if not os.path.isdir(exlib_dir):
             os.makedirs(exlib_dir)
-        
-        #移除老的包
+
+        # 移除老的包
         egg_name = self._get_egg_name(egg_path)
         egg_paths_remove = []
         if egg_name:
             for file_name in os.listdir(exlib_dir):
-                if not file_name.lower().endswith('.egg'):
+                if not file_name.lower().endswith(".egg"):
                     continue
                 file_path = os.path.join(exlib_dir, file_name)
                 if not os.path.isfile(file_path):
                     continue
                 if egg_name == self._get_egg_name(file_path):
                     os.remove(file_path)
                     egg_paths_remove.append(file_path)
-        
-        #拷贝包
+
+        # 拷贝包
         shutil.copy(egg_path, exlib_dir)
-        
-        #记录到installed_libs.txt
+
+        # 记录到installed_libs.txt
         installed_pkgs = self.list_names()
         for pkg in toplv_pkgs[:]:
             if pkg in installed_pkgs:
                 toplv_pkgs.remove(pkg)
         if toplv_pkgs:
-            with codecs_open(self._installed_libs, 'a+') as fd:
+            with codecs_open(self._installed_libs, "a+") as fd:
                 for pkg in toplv_pkgs:
-                    fd.write(pkg+'\n')
-                    
+                    fd.write(pkg + "\n")
+
         self._update_pydev_conf(egg_path, egg_paths_remove)
-                    
+
     def _update_pydev_conf(self, egg_path, egg_paths_remove):
-        '''修改pydev配置
-        '''
+        """修改pydev配置"""
         egg_names_remove = []
         for it in egg_paths_remove:
             egg_names_remove.append(os.path.basename(it).lower())
         egg_name = os.path.basename(egg_path)
-        
-#         if len(egg_names_remove) == 1 and egg_names_remove[0] == egg_name:
-#             return
-        
-        pydev_path = os.path.join(self._top_dir, '.pydevproject')
+
+        #         if len(egg_names_remove) == 1 and egg_names_remove[0] == egg_name:
+        #             return
+
+        pydev_path = os.path.join(self._top_dir, ".pydevproject")
         if not os.path.isfile(pydev_path):
-            logging.warn('pydev configure file not found')
+            logging.warn("pydev configure file not found")
             return
         doc = dom.parse(pydev_path)
-        for propnode in doc.getElementsByTagName('pydev_pathproperty'):
-            if propnode.getAttribute('name') == 'org.python.pydev.PROJECT_SOURCE_PATH':
+        for propnode in doc.getElementsByTagName("pydev_pathproperty"):
+            if propnode.getAttribute("name") == "org.python.pydev.PROJECT_SOURCE_PATH":
                 break
         else:
-            propnode = doc.createElement('pydev_pathproperty')
-            propnode.setAttribute('name', 'org.python.pydev.PROJECT_SOURCE_PATH')
-            projnodes = doc.getElementsByTagName('pydev_project')
+            propnode = doc.createElement("pydev_pathproperty")
+            propnode.setAttribute("name", "org.python.pydev.PROJECT_SOURCE_PATH")
+            projnodes = doc.getElementsByTagName("pydev_project")
             if not projnodes:
-                logging.warn('pydev configure file corrupted')
+                logging.warn("pydev configure file corrupted")
                 return
             projnodes[0].AppendChild(propnode)
-        
 
-        for pathnode in propnode.getElementsByTagName('path'):
-            file_path =  pathnode.childNodes[0].data
-            name = file_path[file_path.rfind('/')+1:]
+        for pathnode in propnode.getElementsByTagName("path"):
+            file_path = pathnode.childNodes[0].data
+            name = file_path[file_path.rfind("/") + 1 :]
             if name.lower() in egg_names_remove:
                 propnode.removeChild(pathnode)
-                
-        pathnode = doc.createElement('path')
+
+        pathnode = doc.createElement("path")
         print(egg_name)
-        pathnode.appendChild(doc.createTextNode('/${PROJECT_DIR_NAME}/exlib/%s'%egg_name))
+        pathnode.appendChild(
+            doc.createTextNode("/${PROJECT_DIR_NAME}/exlib/%s" % egg_name)
+        )
         propnode.appendChild(pathnode)
-        with codecs_open(pydev_path, 'w', 'utf8') as fd:
-            fd.write(doc.toxml(encoding='UTF-8'))
-        
-                    
+        with codecs_open(pydev_path, "w", "utf8") as fd:
+            fd.write(doc.toxml(encoding="UTF-8"))
+
     def list_names(self):
-        '''获取全部的扩展包的名字
-        '''
+        """获取全部的扩展包的名字"""
         if not os.path.isfile(self._installed_libs):
             return []
         names = []
-        with codecs_open(self._installed_libs, 'r', encoding="utf-8") as fd:
+        with codecs_open(self._installed_libs, "r", encoding="utf-8") as fd:
             for libname in fd.readlines():
-                libname = libname.strip('\r\n ')
+                libname = libname.strip("\r\n ")
                 if not libname:
                     continue
                 names.append(libname)
-        return names
+        return names
```

### Comparing `qtaf-5.5.9/testbase/loader.py` & `qtaf-5.6.0/testbase/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,72 +8,72 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 测试用例加载
-'''
+"""
 from __future__ import absolute_import
 
 import imp
 import pkgutil
 import os
-import six
 import sys
 import traceback
 import types
 
 from collections import OrderedDict
+
+import six
+
 from testbase import datadrive
-from testbase.testcase import TestCase, SeqTestSuite
+from testbase.testcase import TestCase
+from testbase.testsuite import SeqTestSuite, TestSuite
 from testbase.conf import settings
 from testbase.util import smart_text
 
 
 class TestLoader(object):
-    '''测试用例加载器
-    '''
+    """测试用例加载器"""
 
     def __init__(self, filter_func=None):
-        '''构造函数
+        """构造函数
         :param filter: 用例过滤函数，函数原型为 filter_func(testcase_obj)，返回None/False表示不过滤此用例
         :type filter: callable
-        '''
+        """
         self._filter = filter_func
         self._module_errs = {}
         self._filtered_tests = {}
 
     def get_last_errors(self):
-        '''返回最后一次load调用时加载失败的全部模块和对应错误信息
+        """返回最后一次load调用时加载失败的全部模块和对应错误信息
 
         :returns dict: 模块和对应的错误信息
-        '''
+        """
         return self._module_errs
 
     def get_filtered_tests(self):
-        '''返回最后一次load调用时被过滤掉的测试用例
-        '''
+        """返回最后一次load调用时被过滤掉的测试用例"""
         return list(self._filtered_tests.keys())
 
     def get_filtered_tests_with_reason(self):
-        '''返回最后一次load调用时被过滤掉的测试用例和过滤原因
-        '''
+        """返回最后一次load调用时被过滤掉的测试用例和过滤原因"""
         return self._filtered_tests
 
     def load(self, testname):
-        '''通过名字加载测试用例
+        """通过名字加载测试用例
 
         :param name: 用例或用例名称
         :type name: string/list
 
         :returns list - 测试用例对象列表
-        '''
+        """
 
         if isinstance(testname, list):
             testnames = testname
         else:
             testnames = [testname]
 
         self._module_errs = {}
@@ -86,162 +86,218 @@
             if isinstance(testname, dict):
                 parameters = testname.get("parameters", {})
                 exclude_data_keys = testname.get("exclude_data_keys")
                 testname = testname.get("name")
             testname = smart_text(testname)
             if settings.DATA_DRIVE:
                 self._dataset = TestDataLoader().load()
-            if '/' in testname:
-                testname, data_key = testname.split('/', 1)
+            if "/" in testname:
+                testname, data_key = testname.split("/", 1)
             else:
                 data_key = None
 
             obj = self._load(testname)
 
             if isinstance(obj, types.ModuleType):
-                if hasattr(obj, '__path__'):
-                    testcases += self._load_from_package(obj, data_key, exclude_data_keys, parameters)
+                if hasattr(obj, "__path__"):
+                    testcases += self._load_from_package(
+                        obj, data_key, exclude_data_keys, parameters
+                    )
                 else:
-                    testcases += self._load_from_module(obj, data_key, exclude_data_keys, parameters)
+                    testcases += self._load_from_module(
+                        obj, data_key, exclude_data_keys, parameters
+                    )
             elif isinstance(obj, type):
-                testcases += self._load_from_class(obj, data_key, exclude_data_keys, parameters)
+                if issubclass(obj, TestCase):
+                    testcases += self._load_from_class(
+                        obj, data_key, exclude_data_keys, parameters
+                    )
+                elif issubclass(obj, TestSuite):
+                    testcases += self._load_from_testsuite(
+                        obj, data_key, exclude_data_keys, parameters
+                    )
 
         # 过滤掉重复的用例
         testcase_dict = OrderedDict()
         for testcase in testcases:
             testcase_dict[testcase.test_name] = testcase
 
         return list(testcase_dict.values())
 
     def _load(self, testname):
-        '''加载对应的对象
+        """加载对应的对象
 
         :param name: 用例或用例集名称
         :type name: string
         :returns - Type/ModuleType
-        '''
-        parts = testname.split('.')
+        """
+        parts = testname.split(".")
         module = None
         parts_imp = parts[:]
         while parts_imp:
             try:
-                modulename = '.'.join(parts_imp)
+                modulename = ".".join(parts_imp)
                 __import__(modulename)  # __import__得到的是最外层模块的object
                 module = sys.modules[modulename]
                 break
             except ImportError:
                 del parts_imp[-1]
-            except:
+            except Exception:  # pylint: disable=broad-except
                 del parts_imp[-1]
                 break
 
         obj = module
 
         if parts_imp == parts:  # 为一个包或模块
             return obj
 
         elif parts_imp == parts[0:-1] and hasattr(module, parts[-1]):  # 为一个类
             try:
                 testclass = getattr(module, parts[-1])
-                if not self._is_testcase_class(testclass):
-                    raise TypeError("%s不是一个有效的测试用例" % testname)
-            except:
+                if not self._is_testcase_class(
+                    testclass
+                ) and not self._is_testsuite_class(testclass):
+                    raise TypeError("%s不是一个有效的测试用例(套)" % testname)
+            except Exception:  # pylint: disable=broad-except
                 self._module_errs[testname] = traceback.format_exc()
                 return
             else:
                 return testclass
 
         else:  # 触发异常
             if parts_imp:
-                modulename = '.'.join(parts_imp)
-                modulename += '.'
+                modulename = ".".join(parts_imp)
+                modulename += "."
             else:
-                modulename = ''
+                modulename = ""
             modulename += parts[len(parts_imp)]
             try:
                 __import__(modulename)
-            except:
+            except Exception:  # pylint: disable=broad-except
                 self._module_errs[modulename] = traceback.format_exc()
 
     def _is_testcase_class(self, obj):
-        '''是否为测试用例类
+        """是否为测试用例类
 
         :returns bool - 是否为用例类
-        '''
-        return (isinstance(obj, type) and
-              issubclass(obj, TestCase) and
-              hasattr(obj, "runTest") and
-              getattr(obj, "priority", None))
+        """
+        return (
+            isinstance(obj, type)
+            and issubclass(obj, TestCase)
+            and hasattr(obj, "runTest")
+            and getattr(obj, "priority", None)
+        )
+
+    def _is_testsuite_class(self, obj):
+        """是否是测试用例套类
+
+        :returns bool - 是否为用例套类
+        """
+        return isinstance(obj, type) and issubclass(obj, TestSuite)
 
     def _walk_package_error(self, modulename):
-        '''walk_packages错误回调
-        '''
+        """walk_packages错误回调"""
         self._module_errs[modulename] = traceback.format_exc()
 
     def _load_from_package(self, pkg, data_key=None, exclude_data_key=None, attrs=None):
-        '''从一个python包加载测试用例
+        """从一个python包加载测试用例
 
         :param pkg: Python包
         :type pkg: ModuleType
         :returns list - 测试用例对象列表
-        '''
+        """
         tests = []
-        for _, modulename, ispkg in pkgutil.walk_packages(pkg.__path__, pkg.__name__ + '.', onerror=self._walk_package_error):
+        for _, modulename, ispkg in pkgutil.walk_packages(
+            pkg.__path__, pkg.__name__ + ".", onerror=self._walk_package_error
+        ):
             if ispkg:
                 continue
             try:
                 __import__(modulename)
-                tests += self._load_from_module(sys.modules[modulename], data_key, exclude_data_key=exclude_data_key, attrs=None)
-            except:
+                tests += self._load_from_module(
+                    sys.modules[modulename],
+                    data_key,
+                    exclude_data_key=exclude_data_key,
+                    attrs=None,
+                )
+            except Exception:  # pylint: disable=broad-except
                 self._module_errs[modulename] = traceback.format_exc()
         return tests
 
     def _load_from_module(self, mod, data_key=None, exclude_data_key=None, attrs=None):
-        '''从一个python模块加载测试用例
+        """从一个python模块加载测试用例
 
         :param mod: Python模块
         :type mod: ModuleType
         :returns list - 测试用例对象列表
-        '''
+        """
         tests = []
         for name in dir(mod):
             obj = getattr(mod, name)
             if self._is_testcase_class(obj):
-                tests += self._load_from_class(obj, data_key, exclude_data_key=exclude_data_key, attrs=attrs)
-        if hasattr(mod, '__qtaf_seq_tests__'):  # 测试用例需要顺序执行
+                tests += self._load_from_class(
+                    obj, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                )
+        if hasattr(mod, "__qtaf_seq_tests__"):  # 测试用例需要顺序执行
             seqdef = mod.__qtaf_seq_tests__
             if not isinstance(seqdef, list):
                 raise TypeError("__qtaf_seq_tests__必须为list类型")
             if len(seqdef) == 0:
                 raise ValueError("__qtaf_seq_tests__必须至少包含一个测试用例")
             for it in seqdef:
                 if type(it) != type(TestCase) or not issubclass(it, TestCase):
                     raise TypeError("__qtaf_seq_tests__的元素必须为测试用例类")
             test_dict = {}
             for test in tests:
                 if type(test) in test_dict:
                     test_dict[type(test)].append(test)
                 else:
-                    test_dict[type(test)] = [test, ]
+                    test_dict[type(test)] = [
+                        test,
+                    ]
             for it in seqdef:
                 if it not in test_dict:
                     raise RuntimeError("__qtaf_seq_tests__中的测试用例'%s'已被过滤" % it.__name__)
             tests_list = []
             for it in seqdef:
                 tests_list += test_dict[it]
             tests = [SeqTestSuite(tests_list)]
         return tests
 
+    def _load_from_testsuite(
+        self, cls, data_key=None, exclude_data_key=None, attrs=None
+    ):
+        """从测试用例套类加载测试用例"""
+        tests = []
+        for test in cls.testcases:
+            if isinstance(test, str):
+                test = self._load(test)
+            if not isinstance(test, type):
+                if hasattr(test, "__path__"):
+                    tests += self._load_from_package(
+                        test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                    )
+                else:
+                    tests += self._load_from_module(
+                        test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                    )
+            else:
+                tests += self._load_from_class(
+                    test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                )
+
+        return [cls([it for it in tests if not cls.filter(it)])]
+
     def _load_from_class(self, cls, data_key=None, exclude_data_key=None, attrs=None):
-        '''加载用例类
+        """加载用例类
 
         :param cls: Python类
         :type cls: Type
         :returns list - 测试用例对象列表
-        '''
+        """
         if exclude_data_key is None:
             exclude_data_key = []
         exclude_data_key = [smart_text(i) for i in exclude_data_key]
 
         tests = []
         if datadrive.is_datadrive(cls) or settings.DATA_DRIVE:
             tests = datadrive.load_datadrive_tests(cls, data_key, attrs)
@@ -259,71 +315,74 @@
                 else:
                     final_tests.append(it)
             tests = final_tests
         return tests
 
 
 class TestDataLoader(object):
-    '''测试数据加载器
-    '''
-    MODULE_NAME = 'testbase.loader.testdata'
+    """测试数据加载器"""
+
+    MODULE_NAME = "testbase.loader.testdata"
 
     def _load_dataset_module_from_file(self):
-        '''从文件中加载数据模块
-        '''
+        """从文件中加载数据模块"""
         if self.MODULE_NAME in sys.modules:
             return sys.modules[self.MODULE_NAME]
 
         if os.path.isfile(__file__):
-            qtaf_top_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..')
+            qtaf_top_dir = os.path.join(
+                os.path.dirname(os.path.abspath(__file__)), ".."
+            )
             top_dir = qtaf_top_dir
         else:  # 使用的egg包
-            qtaf_top_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..')
-            top_dir = os.path.join(qtaf_top_dir, '..', '..')
+            qtaf_top_dir = os.path.join(
+                os.path.dirname(os.path.abspath(__file__)), ".."
+            )
+            top_dir = os.path.join(qtaf_top_dir, "..", "..")
         top_dir = os.path.abspath(top_dir)
 
         py_path = os.path.join(top_dir, settings.DATA_SOURCE)
         if not os.path.isfile(py_path):
-            raise RuntimeError("指定的数据源文件\"%s\"不存在" % py_path)
+            raise RuntimeError('指定的数据源文件"%s"不存在' % py_path)
 
         module_name = os.path.basename(py_path)
-        module_name = module_name[0:module_name.rfind('.')]
+        module_name = module_name[0 : module_name.rfind(".")]
 
-        fd, pathname, desc = imp.find_module(module_name, [os.path.dirname(py_path), top_dir])
+        fd, pathname, desc = imp.find_module(
+            module_name, [os.path.dirname(py_path), top_dir]
+        )
         module = imp.load_module(self.MODULE_NAME, fd, pathname, desc)
         return module
 
     def _load_dataset_module_from_name(self):
-        '''根据模块名加载模块
-        '''
+        """根据模块名加载模块"""
         __import__(settings.DATA_SOURCE)
         return sys.modules[settings.DATA_SOURCE]
 
     def _load_dataset(self):
-        '''加载数据
-        '''
+        """加载数据"""
         if not settings.DATA_SOURCE:
             raise RuntimeError("DATA_DRIVE=True，但未指定的数据源文件")
 
         if isinstance(settings.DATA_SOURCE, six.string_types):
-            if settings.DATA_SOURCE.endswith('.py'):
+            if settings.DATA_SOURCE.endswith(".py"):
                 module = self._load_dataset_module_from_file()
             else:
                 module = self._load_dataset_module_from_name()
-            if not hasattr(module, 'DATASET'):
-                raise RuntimeError("数据源文件\"%s\"没有定义模块变量\"DATASET\"" % module)
+            if not hasattr(module, "DATASET"):
+                raise RuntimeError('数据源文件"%s"没有定义模块变量"DATASET"' % module)
             return module.DATASET
 
         else:
             return settings.DATA_SOURCE
 
     def load(self):
-        '''从数据源加载测试数据
+        """从数据源加载测试数据
         :returns list - 测试数据集
-        '''
+        """
         dataset = self._load_dataset()
         if isinstance(dataset, list) or isinstance(dataset, tuple):
             dataset_dict = OrderedDict()  # keep ordered
             for idx, it in enumerate(dataset):
                 dataset_dict[str(idx)] = it
             dataset = dataset_dict
         elif isinstance(dataset, dict):
```

### Comparing `qtaf-5.5.9/testbase/logger.py` & `qtaf-5.6.0/testbase/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,121 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''log模块
-'''
+"""log模块
+"""
 
 import logging
 import sys
 import traceback
 from testbase import context
 from testbase.util import ensure_binary_stream, smart_binary
-    
+
 _stream, _encoding = ensure_binary_stream(sys.stdout)
 
 class _Formatter(logging.Formatter):
     def format(self, record):
         s = super(_Formatter, self).format(record)
         return smart_binary(s, encoding=_encoding)
-    
-_stream_handler=logging.StreamHandler(_stream)
+
+
+_stream_handler = logging.StreamHandler(_stream)
 _stream_handler.terminator = b"\n"
 _stream_handler.setFormatter(_Formatter())
 
+
 class TestResultBridge(logging.Handler):
-    '''中转log信息到TestResult
-    '''
+    """中转log信息到TestResult"""
+
     def emit(self, log_record):
-        '''Log Handle 必须实现此函数
-        '''
+        """Log Handle 必须实现此函数"""
         testresult = context.current_testresult()
         if testresult is None:
             _stream_handler.emit(log_record)
             return
         record = {}
         if log_record.exc_info:
-            record['traceback'] = ''.join(traceback.format_tb(log_record.exc_info[2])) + '%s: %s' %(
-                                   log_record.exc_info[0].__name__, log_record.exc_info[1])
+            record["traceback"] = "".join(
+                traceback.format_tb(log_record.exc_info[2])
+            ) + "%s: %s" % (log_record.exc_info[0].__name__, log_record.exc_info[1])
         testresult.log_record(log_record.levelno, log_record.msg, record)
-        
+
+
 _LOGGER_NAME = "QTA_LOGGER"
 _logger = logging.getLogger(_LOGGER_NAME)
 _logger.setLevel(logging.DEBUG)
 _logger.addHandler(TestResultBridge())
 
-        
+
 def critical(msg, *args, **kwargs):
     _logger.error(msg, *args, **kwargs)
- 
+
+
 fatal = critical
 
+
 def error(msg, *args, **kwargs):
-    '''Log a message with severity 'ERROR' on the root logger.
-    '''
+    """Log a message with severity 'ERROR' on the root logger."""
     _logger.error(msg, *args, **kwargs)
 
+
 def exception(msg, *args):
-    '''Log a message with severity 'ERROR' on the root logger,with exception information.
-    '''
+    """Log a message with severity 'ERROR' on the root logger,with exception information."""
     _logger.exception(msg, *args)
 
+
 def warning(msg, *args, **kwargs):
-    '''Log a message with severity 'WARNING' on the root logger.
-    '''
+    """Log a message with severity 'WARNING' on the root logger."""
     _logger.warning(msg, *args, **kwargs)
 
+
 warn = warning
 
+
 def info(msg, *args, **kwargs):
-    '''Log a message with severity 'INFO' on the root logger.
-    '''
+    """Log a message with severity 'INFO' on the root logger."""
     _logger.info(msg, *args, **kwargs)
 
+
 def debug(msg, *args, **kwargs):
-    '''Log a message with severity 'DEBUG' on the root logger.
-    '''
+    """Log a message with severity 'DEBUG' on the root logger."""
     _logger.debug(msg, *args, **kwargs)
 
+
 def log(level, msg, *args, **kwargs):
-    '''Log 'msg % args' with the integer severity 'level' on the root logger.
-    '''
+    """Log 'msg % args' with the integer severity 'level' on the root logger."""
     _logger.log(level, msg, *args, **kwargs)
-    
-def addHandler(hdlr):
-    '''Add the specified handler to this logger.
-    '''
+
+
+def addHandler(hdlr):  # pylint: disable=invalid-name
+    """Add the specified handler to this logger."""
     _logger.addHandler(hdlr)
-    
-def removeHandler(hdlr):
-    '''Remove the specified handler from this logger.
-    '''
+
+
+def removeHandler(hdlr):  # pylint: disable=invalid-name
+    """Remove the specified handler from this logger."""
     _logger.removeHandler(hdlr)
+
+def set_formatter(fmt):
+    """Set the specified formatter to this logger.
+    """
+    class __formatter(_Formatter):
+        def __init__(self, fmt):
+            super(_Formatter, self).__init__(fmt)
+
+    _stream_handler.setFormatter(__formatter(fmt))
+
+def set_level(level):
+    """Set the specified log level to this logger.
+    """
+    _logger.setLevel(level)
```

### Comparing `qtaf-5.5.9/testbase/management.py` & `qtaf-5.6.0/testbase/management.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,185 +37,285 @@
 from testbase.runner import TestCaseSettings
 from testbase.report import test_list_types
 from testbase.types import runner_types, report_types, resmgr_backend_types
 from testbase.util import codecs_open, path_exists
 
 
 class ArgumentParser(object):
-    """参数解析
-    """
+    """参数解析"""
+
     USAGE = """Usage: %(ProgramName)s subcommand [options] [args]
 
 Options:
   -h, --help            show this help message and exit
 
 Type '%(ProgramName)s help <subcommand>' for help on a specific subcommand.
 
 Available subcommands:
 
 %(SubcmdList)s
 
 """
 
     def __init__(self, subcmd_classes):
-        """构造函数
-        """
+        """构造函数"""
         self.subcmd_classes = subcmd_classes
         self.prog = os.path.basename(sys.argv[0])
 
     def print_help(self):
-        """打印帮助文档
-        """
-        logger.info(self.USAGE % {"ProgramName": self.prog,
-                                 "SubcmdList": "\n".join([ '\t%s' % it.name for it in self.subcmd_classes])})
+        """打印帮助文档"""
+        logger.info(
+            self.USAGE
+            % {
+                "ProgramName": self.prog,
+                "SubcmdList": "\n".join(
+                    ["\t%s" % it.name for it in self.subcmd_classes]
+                ),
+            }
+        )
 
     def parse_args(self, args):
-        """解析参数
-        """
+        """解析参数"""
         if len(args) < 1:
             self.print_help()
             return 1
 
         subcmd = args[0]
         for it in self.subcmd_classes:
             if it.name == subcmd:
                 subcmd_class = it
                 parser = it.parser
                 break
         else:
-            logger.error("invalid subcommand \"%s\"\n" % subcmd)
+            logger.error('invalid subcommand "%s"\n' % subcmd)
             return 1
 
         ns = parser.parse_args(args[1:])
         subcmd = subcmd_class()
         subcmd.main_parser = self
         return subcmd, ns
 
-#     def add_subcommand(self, subcmd, parser ):
-#         """增加一个子命令
-#         """
-#         parser.prog = "%s help" % self.prog
-#         self._subcmd_parser_dict[subcmd] = parser
+    #     def add_subcommand(self, subcmd, parser ):
+    #         """增加一个子命令
+    #         """
+    #         parser.prog = "%s help" % self.prog
+    #         self._subcmd_parser_dict[subcmd] = parser
 
     def get_subcommand(self, name):
-        """获取子命令
-        """
+        """获取子命令"""
         for it in self.subcmd_classes:
             if it.name == name:
                 return it()
 
 
 class Command(object):
-    """一个命令
-    """
+    """一个命令"""
+
     name = None
     parser = None
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         raise NotImplementedError()
 
 
 class Help(Command):
-    """帮助命令
-    """
-    name = 'help'
+    """帮助命令"""
+
+    name = "help"
     parser = argparse.ArgumentParser("Display subcommand usage")
-    parser.add_argument('subcommand', nargs='?', help="target subcommand to display")
+    parser.add_argument("subcommand", nargs="?", help="target subcommand to display")
 
     def execute(self, args):
-        """执行过程
-        """
-        if args.subcommand == None:
+        """执行过程"""
+        if args.subcommand is None:
             self.main_parser.print_help()
         else:
             subcmd = self.main_parser.get_subcommand(args.subcommand)
             subcmd.parser.print_help()
 
 
 class RunScript(Command):
-    """执行一个脚本
-    """
-    name = 'runscript'
+    """执行一个脚本"""
+
+    name = "runscript"
     parser = argparse.ArgumentParser("Run python script")
-    parser.add_argument('script_path', help="target script to run")
+    parser.add_argument("script_path", help="target script to run")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         import runpy
+
         if not os.path.isfile(args.script_path):
             print("invalid file path: %s" % args.script_path)
             return 1
-        runpy.run_path(args.script_path, run_name='__main__')
+        runpy.run_path(args.script_path, run_name="__main__")
 
 
 class RunTest(Command):
-    """批量执行测试用例
-    """
-    name = 'runtest'
-    parser = argparse.ArgumentParser("Run QTA testcases")
-    parser.add_argument("tests", metavar="TEST", nargs='*', help="testcase set to executive, eg: zoo.xxx.HelloTest")
-    parser.add_argument('-w', '--working-dir', default=None, help="working directory to store all result files", dest="working_dir")
-    parser.add_argument('--priority', help="run test cases with specific priority, accept multiple options",
-                        dest="priorities", action="append",
-                        choices=[TestCasePriority.BVT, TestCasePriority.High, TestCasePriority.Normal, TestCasePriority.Low])
-    parser.add_argument('--status', default=None, help="run test cases with specific status, accept multiple options",
-                        dest="status", action="append",
-                        choices=[TestCaseStatus.Design, TestCaseStatus.Implement, TestCaseStatus.Ready, TestCaseStatus.Review, TestCaseStatus.Suspend])
-    parser.add_argument("--excluded-name", help="exclude test cases with specific name prefix , accept multiple options",
-                        action="append", dest="excluded_names", metavar="EXCLUDED_NAME")
-    parser.add_argument("--owner", help="run test cases with specific owner, accept multiple options",
-                        action="append", dest="owners", metavar="OWNER")
-    parser.add_argument("--tag", help="run test cases with specific tag, accept multiple options",
-                        action="append", dest="tags", metavar="TAG")
-    parser.add_argument("--excluded-tag", help="exclude test cases with specific name tag, accept multiple options",
-                        action="append", dest="excluded_tags", metavar="EXCLUDED_TAG")
-
-    parser.add_argument("--report-type", help="report type", choices=report_types.keys(), default="stream")
-    parser.add_argument("--report-args", help="additional arguments for specific report", default="")
-    parser.add_argument("--report-args-help", help="show help information for specific report arguemnts", choices=report_types.keys())
-
-    parser.add_argument("--resmgr-backend-type", help="test resource manager backend type", choices=resmgr_backend_types.keys(), default="local")
-
-    parser.add_argument("--runner-type", help="test runner type", choices=runner_types.keys(), default="basic")
-    parser.add_argument("--runner-args", help="additional arguments for specific runner", default="")
-    parser.add_argument("--runner-args-help", help="show help information for specific runner arguemnts", choices=runner_types.keys())
+    """批量执行测试用例"""
 
-    parser.add_argument("--execute-type", help="execute type", choices=["random", "sequential"], default="random")
+    name = "runtest"
+    parser = argparse.ArgumentParser("Run QTA testcases")
+    parser.add_argument(
+        "tests",
+        metavar="TEST",
+        nargs="*",
+        help="testcase set to executive, eg: zoo.xxx.HelloTest",
+    )
+    parser.add_argument(
+        "-w",
+        "--working-dir",
+        default=None,
+        help="working directory to store all result files",
+        dest="working_dir",
+    )
+    parser.add_argument(
+        "--priority",
+        help="run test cases with specific priority, accept multiple options",
+        dest="priorities",
+        action="append",
+        choices=[
+            TestCasePriority.BVT,
+            TestCasePriority.High,
+            TestCasePriority.Normal,
+            TestCasePriority.Low,
+        ],
+    )
+    parser.add_argument(
+        "--status",
+        default=None,
+        help="run test cases with specific status, accept multiple options",
+        dest="status",
+        action="append",
+        choices=[
+            TestCaseStatus.Design,
+            TestCaseStatus.Implement,
+            TestCaseStatus.Ready,
+            TestCaseStatus.Review,
+            TestCaseStatus.Suspend,
+        ],
+    )
+    parser.add_argument(
+        "--excluded-name",
+        help="exclude test cases with specific name prefix , accept multiple options",
+        action="append",
+        dest="excluded_names",
+        metavar="EXCLUDED_NAME",
+    )
+    parser.add_argument(
+        "--owner",
+        help="run test cases with specific owner, accept multiple options",
+        action="append",
+        dest="owners",
+        metavar="OWNER",
+    )
+    parser.add_argument(
+        "--tag",
+        help="run test cases with specific tag, accept multiple options",
+        action="append",
+        dest="tags",
+        metavar="TAG",
+    )
+    parser.add_argument(
+        "--excluded-tag",
+        help="exclude test cases with specific name tag, accept multiple options",
+        action="append",
+        dest="excluded_tags",
+        metavar="EXCLUDED_TAG",
+    )
+
+    parser.add_argument(
+        "--report-type",
+        help="report type",
+        choices=report_types.keys(),
+        default="stream",
+    )
+    parser.add_argument(
+        "--report-args", help="additional arguments for specific report", default=""
+    )
+    parser.add_argument(
+        "--report-args-help",
+        help="show help information for specific report arguemnts",
+        choices=report_types.keys(),
+    )
+
+    parser.add_argument(
+        "--resmgr-backend-type",
+        help="test resource manager backend type",
+        choices=resmgr_backend_types.keys(),
+        default="local",
+    )
+
+    parser.add_argument(
+        "--runner-type",
+        help="test runner type",
+        choices=runner_types.keys(),
+        default="basic",
+    )
+    parser.add_argument(
+        "--runner-args", help="additional arguments for specific runner", default=""
+    )
+    parser.add_argument(
+        "--runner-args-help",
+        help="show help information for specific runner arguemnts",
+        choices=runner_types.keys(),
+    )
+
+    parser.add_argument(
+        "--execute-type",
+        help="execute type",
+        choices=["random", "sequential"],
+        default="random",
+    )
+
+    parser.add_argument(
+        "--stop-on-failure",
+        action="store_true",
+        help="task stop on failure, default is False.",
+        dest="stop_on_failure",
+    )
 
     parser.add_argument("--share-data", help="share data", default="{}")
     parser.add_argument("--global-parameters", help="global parameters", default="")
 
     parser.add_argument("--config-file", help="runtime config file path")
 
+    COMPLEX_ARG_MAP = {
+        "priority": "priorities",
+        "excluded_name": "excluded_names",
+        "owner": "owners",
+        "tag": "tags",
+        "excluded_tag": "excluded_tags",
+    }
+
     def run_args_parser(self, runner_args):
         """兼容参数传入concurrency=5,retries=1，支持subprocess shell=False"""
-        regex_c = re.compile(r'(\w+=\w+)+')
+        regex_c = re.compile(r"(\w+=\w+)+")
         regex = regex_c.search(runner_args)
         if regex:
             # concurrency=5,retries=1
             ret = []
             args = regex_c.findall(runner_args)
             for arg in args:
                 tmp = arg.split("=")
                 ret.append("--%s %s" % (tmp[0], tmp[1]))
             return " ".join(ret)
         else:
             # --concurrency 5 --retries 1
             return runner_args
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         if args.config_file:
-            with open(args.config_file, 'r') as fp:
+            with open(args.config_file, "r") as fp:
                 data = json.load(fp)
                 for k, value in data.items():
+                    if k in self.COMPLEX_ARG_MAP.keys():
+                        k = self.COMPLEX_ARG_MAP[k]
                     setattr(args, k, value)
 
         if args.report_args_help:
             report_types[args.report_args_help].get_parser().print_help()
             return 1
         if args.runner_args_help:
             runner_types[args.runner_args_help].get_parser().print_help()
@@ -227,137 +327,225 @@
         if args.working_dir is None:
             args.working_dir = os.getcwd()
         prev_dir = os.getcwd()
         if not path_exists(args.working_dir):
             os.makedirs(args.working_dir)
         os.chdir(args.working_dir)
 
-        priorities = args.priorities or [TestCase.EnumPriority.Low,
-                                          TestCase.EnumPriority.Normal,
-                                          TestCase.EnumPriority.High,
-                                          TestCase.EnumPriority.BVT]
-
-        status = args.status or [TestCase.EnumStatus.Design,
-                                  TestCase.EnumStatus.Implement,
-                                  TestCase.EnumStatus.Review,
-                                  TestCase.EnumStatus.Ready]
+        priorities = args.priorities or [
+            TestCase.EnumPriority.Low,
+            TestCase.EnumPriority.Normal,
+            TestCase.EnumPriority.High,
+            TestCase.EnumPriority.BVT,
+        ]
+
+        status = args.status or [
+            TestCase.EnumStatus.Design,
+            TestCase.EnumStatus.Implement,
+            TestCase.EnumStatus.Review,
+            TestCase.EnumStatus.Ready,
+        ]
 
         if args.share_data and isinstance(args.share_data, six.string_types):
             args.share_data = json.loads(args.share_data)
 
-        if args.global_parameters and isinstance(args.global_parameters, six.string_types):
+        if args.global_parameters and isinstance(
+            args.global_parameters, six.string_types
+        ):
             args.global_parameters = json.loads(args.global_parameters)
 
-        test_conf = TestCaseSettings(names=args.tests,
-                                    excluded_names=args.excluded_names,
-                                    priorities=priorities,
-                                    status=status,
-                                    owners=args.owners,
-                                    tags=args.tags,
-                                    excluded_tags=args.excluded_tags,
-                                    share_data=args.share_data,
-                                    global_parameters=args.global_parameters)
+        test_conf = TestCaseSettings(
+            names=args.tests,
+            excluded_names=args.excluded_names,
+            priorities=priorities,
+            status=status,
+            owners=args.owners,
+            tags=args.tags,
+            excluded_tags=args.excluded_tags,
+            share_data=args.share_data,
+            global_parameters=args.global_parameters,
+            stop=args.stop_on_failure,
+        )
 
         report_type = report_types[args.report_type]
-        if args.report_type == 'xml':
+        if args.report_type == "xml":
 
             class VerboseXMLTestReport(report_types[args.report_type]):
-
                 def log_test_result(self, testcase, testresult):
-                    logger.info("run test case: %s(pass?:%s)" % (testcase.test_name, testresult.passed))
-                    super(VerboseXMLTestReport, self).log_test_result(testcase, testresult)
+                    logger.info(
+                        "run test case: %s(pass?:%s)"
+                        % (testcase.test_name, testresult.passed)
+                    )
+                    super(VerboseXMLTestReport, self).log_test_result(
+                        testcase, testresult
+                    )
 
             report_type = VerboseXMLTestReport
 
-        elif args.report_type == 'online':
+        elif args.report_type == "online":
 
             class VerboseOnlineTestReport(report_types[args.report_type]):
-
                 def log_test_result(self, testcase, testresult):
-                    logger.info("run test case: %s(pass?:%s)" % (testcase.test_name, testresult.passed))
-                    super(VerboseOnlineTestReport, self).log_test_result(testcase, testresult)
+                    logger.info(
+                        "run test case: %s(pass?:%s)"
+                        % (testcase.test_name, testresult.passed)
+                    )
+                    super(VerboseOnlineTestReport, self).log_test_result(
+                        testcase, testresult
+                    )
 
                 def begin_report(self):
                     super(VerboseOnlineTestReport, self).begin_report()
                     print("report url: %s" % self.url)
-                    with codecs_open(os.path.join(os.getcwd(), "report_url.txt"), "w", encoding="utf-8") as fd:
+                    with codecs_open(
+                        os.path.join(os.getcwd(), "report_url.txt"),
+                        "w",
+                        encoding="utf-8",
+                    ) as fd:
                         fd.write(self.url)
 
             report_type = VerboseOnlineTestReport
 
         report = report_type.parse_args(shlex.split(args.report_args))
         resmgr_backend = resmgr_backend_types[args.resmgr_backend_type]()
         execute_type = args.execute_type
 
         runner_type = runner_types[args.runner_type]
         # 解析runner_args参数, 用于支持命令行传入concurrency=5,retries=1
         runner_args = self.run_args_parser(args.runner_args)
-        runner = runner_type.parse_args(shlex.split(runner_args), report, resmgr_backend, execute_type)
+        runner = runner_type.parse_args(
+            shlex.split(runner_args), report, resmgr_backend, execute_type
+        )
 
         runner.run(test_conf)
         os.chdir(prev_dir)
-        if args.report_type == 'online':
+        if args.report_type == "online":
             if sys.platform == "win32" and os.environ.get("AUTO_OPEN_URL", "1") == "1":
                 logger.info("opening online report url:%s" % report.url)
                 os.system("start %s" % report.url)
             else:
                 logger.info("online report generated: %s" % report.url)
 
-        elif args.report_type == 'xml':
+        elif args.report_type == "xml":
             if sys.platform == "win32" and os.environ.get("AUTO_OPEN_URL", "1") == "1":
                 logger.info("opening XML report with IE...")
-                report_xml = os.path.abspath(os.path.join(args.working_dir, "TestReport.xml"))
+                report_xml = os.path.abspath(
+                    os.path.join(args.working_dir, "TestReport.xml")
+                )
                 os.system("start iexplore %s" % report_xml)
             else:
-                logger.info("XML report generated: %s" % os.path.abspath("TestReport.xml"))
+                logger.info(
+                    "XML report generated: %s" % os.path.abspath("TestReport.xml")
+                )
 
         if not report.is_passed():
             return 1
 
 
 class DiscoverTests(Command):
-    """discover tests
-    """
+    """discover tests"""
+
     name = "discover"
     parser = argparse.ArgumentParser("Discover tests")
-    parser.add_argument("tests", metavar="TEST", nargs='*', help="testcase set to executive, eg: zoo.xxx.HelloTest")
-    parser.add_argument('--priority', help="test cases with specific priority, accept multiple options, default is High and Normal",
-                        dest="priorities", action="append",
-                        choices=[TestCasePriority.BVT, TestCasePriority.High, TestCasePriority.Normal, TestCasePriority.Low])
-    parser.add_argument('--status', help="test cases with specific status, accept multiple options, default is Ready",
-                        dest="status", action="append",
-                        choices=[TestCaseStatus.Design, TestCaseStatus.Implement, TestCaseStatus.Ready, TestCaseStatus.Review, TestCaseStatus.Suspend])
-    parser.add_argument("--excluded-name", help="exclude test cases with specific name prefix , accept multiple options",
-                        action="append", dest="excluded_names", metavar="EXCLUDED_NAME")
-    parser.add_argument("--owner", help="test cases with specific owner, accept multiple options",
-                        action="append", dest="owners", metavar="OWNER")
-    parser.add_argument("--tag", help="test cases with specific tag, accept multiple options",
-                        action="append", dest="tags", metavar="TAG")
-    parser.add_argument("--excluded-tag", help="exclude test cases with specific name tag, accept multiple options",
-                        action="append", dest="excluded_tags", metavar="EXCLUDED_TAG")
-    parser.add_argument("--show", help="explicitly specify test case types to show, default will show all kinds of test cases",
-                        choices=["filtered", "error", "normal"], dest="shows", action="append")
-    parser.add_argument("--output-file", help="output file name, default is stdout", default=None)
-    parser.add_argument("--output-type", help="output type, default is stream", default="stream", choices=test_list_types.keys())
+    parser.add_argument(
+        "tests",
+        metavar="TEST",
+        nargs="*",
+        help="testcase set to executive, eg: zoo.xxx.HelloTest",
+    )
+    parser.add_argument(
+        "--priority",
+        help="test cases with specific priority, accept multiple options, default is High and Normal",
+        dest="priorities",
+        action="append",
+        choices=[
+            TestCasePriority.BVT,
+            TestCasePriority.High,
+            TestCasePriority.Normal,
+            TestCasePriority.Low,
+        ],
+    )
+    parser.add_argument(
+        "--status",
+        help="test cases with specific status, accept multiple options, default is Ready",
+        dest="status",
+        action="append",
+        choices=[
+            TestCaseStatus.Design,
+            TestCaseStatus.Implement,
+            TestCaseStatus.Ready,
+            TestCaseStatus.Review,
+            TestCaseStatus.Suspend,
+        ],
+    )
+    parser.add_argument(
+        "--excluded-name",
+        help="exclude test cases with specific name prefix , accept multiple options",
+        action="append",
+        dest="excluded_names",
+        metavar="EXCLUDED_NAME",
+    )
+    parser.add_argument(
+        "--owner",
+        help="test cases with specific owner, accept multiple options",
+        action="append",
+        dest="owners",
+        metavar="OWNER",
+    )
+    parser.add_argument(
+        "--tag",
+        help="test cases with specific tag, accept multiple options",
+        action="append",
+        dest="tags",
+        metavar="TAG",
+    )
+    parser.add_argument(
+        "--excluded-tag",
+        help="exclude test cases with specific name tag, accept multiple options",
+        action="append",
+        dest="excluded_tags",
+        metavar="EXCLUDED_TAG",
+    )
+    parser.add_argument(
+        "--show",
+        help="explicitly specify test case types to show, default will show all kinds of test cases",
+        choices=["filtered", "error", "normal"],
+        dest="shows",
+        action="append",
+    )
+    parser.add_argument(
+        "--output-file", help="output file name, default is stdout", default=None
+    )
+    parser.add_argument(
+        "--output-type",
+        help="output type, default is stream",
+        default="stream",
+        choices=test_list_types.keys(),
+    )
 
     def execute(self, args):
         if not args.tests:
             logger.info("no test set specified")
             return 1
         shows = args.shows or ["filtered", "error", "normal"]
-        priorities = args.priorities or [TestCase.EnumPriority.Normal, TestCase.EnumPriority.High]
+        priorities = args.priorities or [
+            TestCase.EnumPriority.Normal,
+            TestCase.EnumPriority.High,
+        ]
         status = args.status or [TestCase.EnumStatus.Ready]
 
-        test_conf = TestCaseSettings(names=args.tests,
-                                    excluded_names=args.excluded_names,
-                                    priorities=priorities,
-                                    status=status,
-                                    owners=args.owners,
-                                    tags=args.tags,
-                                    excluded_tags=args.excluded_tags)
+        test_conf = TestCaseSettings(
+            names=args.tests,
+            excluded_names=args.excluded_names,
+            priorities=priorities,
+            status=status,
+            owners=args.owners,
+            tags=args.tags,
+            excluded_tags=args.excluded_tags,
+        )
 
         loader = TestLoader(test_conf.filter)
         tests = loader.load(test_conf.names)
 
         test_list_output = test_list_types[args.output_type](args.output_file)
 
         if "filtered" in shows:
@@ -373,328 +561,470 @@
             error_tests = loader.get_last_errors().items()
             sorted_error_tests = sorted(error_tests, key=lambda x: x[0])
             test_list_output.output_error_tests(sorted_error_tests)
         test_list_output.end_output()
 
 
 class RunPlan(Command):
-    """执行测试计划
-    """
+    """执行测试计划"""
+
     name = "runplan"
     parser = argparse.ArgumentParser("Run QTA test plan")
-    parser.add_argument("--report-type", help="report type", choices=report_types.keys(), default="stream")
-    parser.add_argument("--report-args", help="additional arguments for specific report", default="")
-    parser.add_argument("--report-args-help", help="show help information for specific report arguemnts", choices=report_types.keys())
-
-    parser.add_argument("--runner-type", help="test runner type", choices=runner_types.keys(), default="basic")
-    parser.add_argument("--runner-args", help="additional arguments for specific runner", default="")
-    parser.add_argument("--runner-args-help", help="show help information for specific runner arguemnts", choices=runner_types.keys())
-
-    parser.add_argument("--resmgr-backend-type", help="test resource manager backend type", choices=resmgr_backend_types.keys(), default="local")
+    parser.add_argument(
+        "--report-type",
+        help="report type",
+        choices=report_types.keys(),
+        default="stream",
+    )
+    parser.add_argument(
+        "--report-args", help="additional arguments for specific report", default=""
+    )
+    parser.add_argument(
+        "--report-args-help",
+        help="show help information for specific report arguemnts",
+        choices=report_types.keys(),
+    )
+
+    parser.add_argument(
+        "--runner-type",
+        help="test runner type",
+        choices=runner_types.keys(),
+        default="basic",
+    )
+    parser.add_argument(
+        "--runner-args", help="additional arguments for specific runner", default=""
+    )
+    parser.add_argument(
+        "--runner-args-help",
+        help="show help information for specific runner arguemnts",
+        choices=runner_types.keys(),
+    )
+
+    parser.add_argument(
+        "--resmgr-backend-type",
+        help="test resource manager backend type",
+        choices=resmgr_backend_types.keys(),
+        default="local",
+    )
 
     parser.add_argument("plan", help="designate a test plan to run")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         if args.report_args_help:
             report_types[args.report_args_help].get_parser().print_help()
             return
         if args.runner_args_help:
             runner_types[args.runner_args_help].get_parser().print_help()
             return
 
         report_type = report_types[args.report_type]
         report = report_type.parse_args(shlex.split(args.report_args))
 
         resmgr_backend = resmgr_backend_types[args.resmgr_backend_type]()
 
         runner_type = runner_types[args.runner_type]
-        runner = runner_type.parse_args(shlex.split(args.runner_args), report, resmgr_backend)
+        runner = runner_type.parse_args(
+            shlex.split(args.runner_args), report, resmgr_backend
+        )
 
         planname = args.plan
         planmodulename, planclsname = planname.rsplit(".", 1)
         __import__(planmodulename)
         planmod = sys.modules[planmodulename]
         plancls = getattr(planmod, planclsname)
         runner.run(plancls())
         if not report.is_passed():
             return 1
 
 
 class InstallLib(Command):
-    """安装扩展库
-    """
-    name = 'installlib'
+    """安装扩展库"""
+
+    name = "installlib"
     parser = argparse.ArgumentParser("Install extend library")
     parser.add_argument("egg_path", help="egg file path")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         ExLibManager(settings.PROJECT_ROOT).install(args.egg_path)
 
 
 class CreateProject(Command):
-    """创建测试项目
-    """
-    name = 'createproject'
+    """创建测试项目"""
+
+    name = "createproject"
     parser = argparse.ArgumentParser("Create new QTA project")
-    parser.add_argument('name', help="project name")
-    parser.add_argument('--dest', default=None, help="target path to create project")
+    parser.add_argument("name", help="project name")
+    parser.add_argument("--dest", default=None, help="target path to create project")
     # parser.add_argument('--mode', default="standalone", help="project mode: standard or standalone")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         if args.dest is None:
             dest = os.getcwd()
         else:
             dest = args.dest
         if os.path.isfile(__file__):
             mode = project.EnumProjectMode.Standard
         else:
             mode = project.EnumProjectMode.Standalone
-        proj_path = os.path.join(dest, args.name.lower() + 'testproj')
-        logger.info('create %s mode test project: %s' % (mode, proj_path))
+        proj_path = os.path.join(dest, args.name.lower() + "testproj")
+        logger.info("create %s mode test project: %s" % (mode, proj_path))
         project.create_project(proj_path, args.name, mode)
 
 
 class UpgradeProject(Command):
-    """升级测试项目
-    """
-    name = 'upgradeproject'
+    """升级测试项目"""
+
+    name = "upgradeproject"
     parser = argparse.ArgumentParser("Upgrade QTA project")
-    parser.add_argument('proj_path', help="target path to upgrade project")
+    parser.add_argument("proj_path", help="target path to upgrade project")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         if os.path.isfile(__file__):
             logger.error("should run in egg mode")
             return 1
 
         qtaf_path = os.path.dirname(os.path.abspath(__file__))
         project.update_project_qtaf(args.proj_path, qtaf_path)
 
 
 class Shell(Command):
-    """Python Shell
-    """
-    name = 'shell'
+    """Python Shell"""
+
+    name = "shell"
     parser = argparse.ArgumentParser("open python shell")
 
     def execute(self, args):
-        """执行过程
-        """
+        """执行过程"""
         try:
             import readline  # optional, will allow Up/Down/History in the console
         except ImportError:
             pass
         import code
+
         varables = globals().copy()
         varables.update(locals())
         shell = code.InteractiveConsole(varables)
         shell.interact()
 
 
 class Distribute(Command):
-    """Generate distribution packages
-    """
-    name = 'dist'
+    """Generate distribution packages"""
+
+    name = "dist"
     parser = argparse.ArgumentParser("Generate distribution packages")
-    parser.add_argument("--version", help="assign distribution version", default="1.0.0")
-    parser.add_argument("--exclude-resources", action="store_true", help="do not package resource data in package", default=False)
+    parser.add_argument(
+        "--version", help="assign distribution version", default="1.0.0"
+    )
+    parser.add_argument(
+        "--exclude-resources",
+        action="store_true",
+        help="do not package resource data in package",
+        default=False,
+    )
 
     def execute(self, args):
         DistGenerator(args.version).run(args.exclude_resources)
 
 
 class RunTestDistPackage(Command):
-    """Run tests in distribution package
-    """
+    """Run tests in distribution package"""
+
     name = "runtest"
     parser = argparse.ArgumentParser("Run tests in distribution package")
-    parser.add_argument("--recreate-venv", action="store_true", help="force recreate virtualenv")
+    parser.add_argument(
+        "--recreate-venv", action="store_true", help="force recreate virtualenv"
+    )
     parser.add_argument("--venv", help="designate virtualenv path manually")
 
-    parser.add_argument("--priority", help="run test cases with specific priority, accept multiple options",
-                        choices=[TestCasePriority.BVT, TestCasePriority.High, TestCasePriority.Normal, TestCasePriority.Low],
-                        action="append", dest="priorities")
-    parser.add_argument("--status", help="run test cases with specific status, accept multiple options",
-                        choices=[TestCaseStatus.Design, TestCaseStatus.Implement, TestCaseStatus.Ready, TestCaseStatus.Review, TestCaseStatus.Suspend],
-                        action="append", dest="status")
-    parser.add_argument("--owner", help="run test cases with specific owner, accept multiple options", action="append", dest="owners")
-    parser.add_argument("--excluded-name", help="exclude test cases with specific name prefix , accept multiple options", action="append", dest="excluded_names")
-    parser.add_argument("--tag", help="run test cases with specific tag, accept multiple options", action="append", dest="tags")
-    parser.add_argument("--excluded-tag", help="exclude test cases with specific name tag , accept multiple options", action="append", dest="excluded_tags")
-
-    parser.add_argument("--report-type", help="report type", choices=report_types.keys(), default="stream")
-    parser.add_argument("--report-args", help="additional arguments for specific report", default="")
-    parser.add_argument("--report-args-help", help="show help information for specific report arguemnts", choices=report_types.keys())
-
-    parser.add_argument("--runner-type", help="test runner type", choices=runner_types.keys(), default="basic")
-    parser.add_argument("--runner-args", help="additional arguments for specific runner", default="")
-    parser.add_argument("--runner-args-help", help="show help information for specific runner arguemnts", choices=runner_types.keys())
-
-    parser.add_argument("--resmgr-backend-type", help="test resource manager backend type", choices=resmgr_backend_types.keys(), default="local")
-
-    parser.add_argument("--disable-run-on-child", help="do not create child process to run", action="store_true")
+    parser.add_argument(
+        "--priority",
+        help="run test cases with specific priority, accept multiple options",
+        choices=[
+            TestCasePriority.BVT,
+            TestCasePriority.High,
+            TestCasePriority.Normal,
+            TestCasePriority.Low,
+        ],
+        action="append",
+        dest="priorities",
+    )
+    parser.add_argument(
+        "--status",
+        help="run test cases with specific status, accept multiple options",
+        choices=[
+            TestCaseStatus.Design,
+            TestCaseStatus.Implement,
+            TestCaseStatus.Ready,
+            TestCaseStatus.Review,
+            TestCaseStatus.Suspend,
+        ],
+        action="append",
+        dest="status",
+    )
+    parser.add_argument(
+        "--owner",
+        help="run test cases with specific owner, accept multiple options",
+        action="append",
+        dest="owners",
+    )
+    parser.add_argument(
+        "--excluded-name",
+        help="exclude test cases with specific name prefix , accept multiple options",
+        action="append",
+        dest="excluded_names",
+    )
+    parser.add_argument(
+        "--tag",
+        help="run test cases with specific tag, accept multiple options",
+        action="append",
+        dest="tags",
+    )
+    parser.add_argument(
+        "--excluded-tag",
+        help="exclude test cases with specific name tag , accept multiple options",
+        action="append",
+        dest="excluded_tags",
+    )
+
+    parser.add_argument(
+        "--report-type",
+        help="report type",
+        choices=report_types.keys(),
+        default="stream",
+    )
+    parser.add_argument(
+        "--report-args", help="additional arguments for specific report", default=""
+    )
+    parser.add_argument(
+        "--report-args-help",
+        help="show help information for specific report arguemnts",
+        choices=report_types.keys(),
+    )
+
+    parser.add_argument(
+        "--runner-type",
+        help="test runner type",
+        choices=runner_types.keys(),
+        default="basic",
+    )
+    parser.add_argument(
+        "--runner-args", help="additional arguments for specific runner", default=""
+    )
+    parser.add_argument(
+        "--runner-args-help",
+        help="show help information for specific runner arguemnts",
+        choices=runner_types.keys(),
+    )
+
+    parser.add_argument(
+        "--resmgr-backend-type",
+        help="test resource manager backend type",
+        choices=resmgr_backend_types.keys(),
+        default="local",
+    )
+
+    parser.add_argument(
+        "--disable-run-on-child",
+        help="do not create child process to run",
+        action="store_true",
+    )
 
     parser.add_argument("package", help="QTA sdist package")
-    parser.add_argument("tests", nargs='*', help="designate test names to run")
+    parser.add_argument("tests", nargs="*", help="designate test names to run")
 
     def execute(self, args):
         if args.report_args_help:
             report_types[args.report_args_help].get_parser().print_help()
             return
         if args.runner_args_help:
             runner_types[args.runner_args_help].get_parser().print_help()
             return
 
-        venv = VirtuelEnv(
-            args.package,
-            args.venv,
-            args.recreate_venv)
+        venv = VirtuelEnv(args.package, args.venv, args.recreate_venv)
         venv.activate()
 
         report_type = report_types[args.report_type]
         report = report_type.parse_args(shlex.split(args.report_args))
 
         resmgr_backend = resmgr_backend_types[args.resmgr_backend_type]()
 
         runner_type = runner_types[args.runner_type]
         runner_args = args.runner_args + " "  # incase user input has no space
-        runner = runner_type.parse_args(shlex.split(runner_args), report, resmgr_backend)
+        runner = runner_type.parse_args(
+            shlex.split(runner_args), report, resmgr_backend
+        )
 
         test = TestCaseSettings(
-                args.tests,
-                args.excluded_names,
-                args.priorities,
-                args.status,
-                args.owners,
-                args.tags,
-                args.excluded_tags)
+            args.tests,
+            args.excluded_names,
+            args.priorities,
+            args.status,
+            args.owners,
+            args.tags,
+            args.excluded_tags,
+        )
 
         runner.run(test)
         if not report.is_passed():
             return 1
 
 
 class RunPlanDistPackage(Command):
-    """Run test plan in distribution package
-    """
+    """Run test plan in distribution package"""
+
     name = "runplan"
     parser = argparse.ArgumentParser("Run test plan in distribution package")
-    parser.add_argument("--recreate-venv", action="store_true", help="force recreate virtualenv")
+    parser.add_argument(
+        "--recreate-venv", action="store_true", help="force recreate virtualenv"
+    )
     parser.add_argument("--venv", help="designate virtualenv path manually")
 
-    parser.add_argument("--report-type", help="report type", choices=report_types.keys(), default="stream")
-    parser.add_argument("--report-args", help="additional arguments for specific report", default="")
-    parser.add_argument("--report-args-help", help="show help information for specific report arguemnts", choices=report_types.keys())
-
-    parser.add_argument("--runner-type", help="test runner type", choices=runner_types.keys(), default="basic")
-    parser.add_argument("--runner-args", help="additional arguments for specific runner", default="")
-    parser.add_argument("--runner-args-help", help="show help information for specific runner arguemnts", choices=runner_types.keys())
-
-    parser.add_argument("--resmgr-backend-type", help="test resource manager backend type", choices=resmgr_backend_types.keys(), default="local")
-
-    parser.add_argument("--disable-run-on-child", help="do not create child process to run", action="store_true")
+    parser.add_argument(
+        "--report-type",
+        help="report type",
+        choices=report_types.keys(),
+        default="stream",
+    )
+    parser.add_argument(
+        "--report-args", help="additional arguments for specific report", default=""
+    )
+    parser.add_argument(
+        "--report-args-help",
+        help="show help information for specific report arguemnts",
+        choices=report_types.keys(),
+    )
+
+    parser.add_argument(
+        "--runner-type",
+        help="test runner type",
+        choices=runner_types.keys(),
+        default="basic",
+    )
+    parser.add_argument(
+        "--runner-args", help="additional arguments for specific runner", default=""
+    )
+    parser.add_argument(
+        "--runner-args-help",
+        help="show help information for specific runner arguemnts",
+        choices=runner_types.keys(),
+    )
+
+    parser.add_argument(
+        "--resmgr-backend-type",
+        help="test resource manager backend type",
+        choices=resmgr_backend_types.keys(),
+        default="local",
+    )
+
+    parser.add_argument(
+        "--disable-run-on-child",
+        help="do not create child process to run",
+        action="store_true",
+    )
 
     parser.add_argument("package", help="QTA sdist package")
     parser.add_argument("plan", help="designate a test plan to run")
 
     def execute(self, args):
         if args.report_args_help:
             report_types[args.report_args_help].get_parser().print_help()
             return
         if args.runner_args_help:
             runner_types[args.runner_args_help].get_parser().print_help()
             return
 
-        venv = VirtuelEnv(
-            args.package,
-            args.venv,
-            args.recreate_venv)
+        venv = VirtuelEnv(args.package, args.venv, args.recreate_venv)
         venv.activate()
 
         report_type = report_types[args.report_type]
         report = report_type.parse_args(shlex.split(args.report_args))
 
         resmgr_backend = resmgr_backend_types[args.resmgr_backend_type]()
 
         runner_type = runner_types[args.runner_type]
-        runner = runner_type.parse_args(shlex.split(args.runner_args), report, resmgr_backend)
+        runner = runner_type.parse_args(
+            shlex.split(args.runner_args), report, resmgr_backend
+        )
 
         planname = args.plan
         planmodulename, planclsname = planname.rsplit(".", 1)
         __import__(planmodulename)
         planmod = sys.modules[planmodulename]
         plancls = getattr(planmod, planclsname)
         runner.run(plancls())
         if not report.is_passed():
             return 1
 
 
 class ManagementToolsConsole(object):
-    """管理工具交互模式
-    """
+    """管理工具交互模式"""
+
     prompt = "QTA> "
 
     def __init__(self, argparser):
         self._argparser = argparser
 
     def cmdloop(self):
-        logger.info("""QTAF %(qtaf_version)s (test project: %(proj_root)s [%(proj_mode)s mode])\n""" % {
-            'qtaf_version': version,
-            'proj_root': settings.PROJECT_ROOT,
-            'proj_mode': settings.PROJECT_MODE,
-        })
+        logger.info(
+            """QTAF %(qtaf_version)s (test project: %(proj_root)s [%(proj_mode)s mode])\n"""
+            % {
+                "qtaf_version": version,
+                "proj_root": settings.PROJECT_ROOT,
+                "proj_mode": settings.PROJECT_MODE,
+            }
+        )
         if six.PY3:
             raw_input_func = input
         else:
             raw_input_func = raw_input
         while 1:
             line = raw_input_func(self.prompt)
             args = shlex.split(line, posix="win" not in sys.platform)
             if not args:
                 continue
             subcmd = args[0]
             if not self._argparser.get_subcommand(subcmd):
-                sys.stderr.write("invalid command: \"%s\"\n" % subcmd)
+                sys.stderr.write('invalid command: "%s"\n' % subcmd)
                 continue
             try:
                 subcmd, ns = self._argparser.parse_args(args)
                 subcmd.execute(ns)
             except SystemExit:
                 logger.info("command exit")
-            except:
+            except Exception:  # pylint: disable=broad-except
                 traceback.print_exc()
 
 
 class ManagementTools(object):
-    """管理工具类入口
-    """
-    excluded_command_types = [CreateProject, UpgradeProject, RunTestDistPackage, RunPlanDistPackage]
+    """管理工具类入口"""
+
+    excluded_command_types = [
+        CreateProject,
+        UpgradeProject,
+        RunTestDistPackage,
+        RunPlanDistPackage,
+    ]
 
     def __init__(self):
         if settings.PROJECT_MODE == project.EnumProjectMode.Standard:
             self.excluded_command_types.append(InstallLib)
 
     def _load_cmds(self):
-        """加载全部的命令
-        """
+        """加载全部的命令"""
         cmds = []
         cmds += self._load_cmd_from_module(sys.modules[__name__])
         cmds += self._load_app_cmds()
         return cmds
 
     def _load_cmd_from_module(self, mod):
-        """加载一个模块里面的全部命令
-        """
+        """加载一个模块里面的全部命令"""
         cmds = []
         for objname in dir(mod):
             obj = getattr(mod, objname)
             if not inspect.isclass(obj):
                 continue
             if obj == Command:
                 continue
@@ -703,49 +1033,52 @@
             if issubclass(obj, Command):
                 cmds.append(obj)
 
         cmds.sort(key=lambda x: x.name)
         return cmds
 
     def _load_app_cmds(self):
-        """从应用lib中加载命令
-        """
+        """从应用lib中加载命令"""
         cmds = []
         for libname in settings.INSTALLED_APPS:
             if not libname:
                 continue
-            modname = '%s.cmds' % libname
+            modname = "%s.cmds" % libname
             try:
                 __import__(modname)
             except ImportError:
                 continue
             else:
                 for cmd in self._load_cmd_from_module(sys.modules[modname]):
-                    cmd.name = libname + '.' + cmd.name
+                    cmd.name = libname + "." + cmd.name
                     cmds.append(cmd)
         return cmds
 
     def run(self):
-        """执行入口
-        """
+        """执行入口"""
         cmds = self._load_cmds()
         argparser = ArgumentParser(cmds)
         if len(sys.argv) > 1:
             subcmd, args = argparser.parse_args(sys.argv[1:])
             return subcmd.execute(args) or 0
         else:
             ManagementToolsConsole(argparser).cmdloop()
             return 0
 
 
 def qta_manage_main():
-    """qta-manage工具入口
-    """
+    """qta-manage工具入口"""
     use_egg = not os.path.isfile(__file__)
     if use_egg:
-        cmds = [CreateProject, UpgradeProject, RunTestDistPackage, RunPlanDistPackage, Help]
+        cmds = [
+            CreateProject,
+            UpgradeProject,
+            RunTestDistPackage,
+            RunPlanDistPackage,
+            Help,
+        ]
     else:
         cmds = [CreateProject, RunTestDistPackage, RunPlanDistPackage, Help]
     argparser = ArgumentParser(cmds)
     subcmd, args = argparser.parse_args(sys.argv[1:])
     exit_code = subcmd.execute(args) or 0
     os._exit(exit_code)
```

### Comparing `qtaf-5.5.9/testbase/plan.py` & `qtaf-5.6.0/testbase/plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # governing permissions and limitations under the License.
 #
 """Test plan
 """
 
 
 class TestPlan(object):
-    """测试计划
-    """
+    """测试计划"""
+
     tests = None
     test_target_args = {}
 
     def get_tests(self):
         """获取测试用例定义
 
         :rtypes: str/list(str)/list(TestCase)/TestCaseSettings
@@ -35,37 +35,35 @@
         """获取被测对象
 
         :return: 被测对象信息
         :rtypes: dict
         """
         if isinstance(self.test_target_args, dict):
             return self.test_target_args
-        raise ValueError("`test_target_args` is not a dictionary, please overwrite `get_test_target` for your custom implenmentation")
+        raise ValueError(
+            "`test_target_args` is not a dictionary, please overwrite `get_test_target` for your custom implenmentation"
+        )
 
     def test_setup(self, report):
-        """测试初始化步骤
-        """
+        """测试初始化步骤"""
         pass
 
     def test_teardown(self, report):
-        """测试清理步骤
-        """
+        """测试清理步骤"""
         pass
 
     def resource_setup(self, report, restype, resource):
-        """测试资源初始化
-        """
+        """测试资源初始化"""
         pass
 
     def resource_teardown(self, report, restype, resource):
-        """测试资源清理
-        """
+        """测试资源清理"""
         pass
 
     def debug_run(self, report=None, resmgr_backend=None):
-        """调试执行
-        """
+        """调试执行"""
         from testbase.runner import TestRunner
         from testbase.report import StreamTestReport
+
         if report is None:
             report = StreamTestReport()
         return TestRunner(report, resmgr_backend=resmgr_backend).run(self)
```

### Comparing `qtaf-5.5.9/testbase/project.py` & `qtaf-5.6.0/testbase/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,36 +156,33 @@
 <path>/${PROJECT_DIR_NAME}</path>
 </pydev_pathproperty>
 </pydev_project>
 """
 
 
 class EnumProjectMode(object):
-    """测试项目运行模式
-    """
+    """测试项目运行模式"""
 
     Standard = "standard"  # Python标准模式，QTAF和扩展库安装到Python Libs中
     Standalone = "standalone"  # 独立模式，QTAF和扩展库安装到测试项目的exlib目录中
 
 
 def _create_initpy(dir_path, doc):
-    """创建一个__init__.py
-        """
+    """创建一个__init__.py"""
     with codecs_open(os.path.join(dir_path, "__init__.py"), "wb") as fd:
         fd.write(
             (
                 INITPY_CONTENT
                 % {"Doc": doc, "Date": datetime.date.today().strftime("%Y/%m/%d")}
             ).encode("utf8")
         )
 
 
 def _create_settingspy(proj_path, proj_name, mode):
-    """创建settings.py文件
-    """
+    """创建settings.py文件"""
     if mode == EnumProjectMode.Standalone:
         content = SETTINGS_CONTENT_STANDALONE
     else:
         content = SETTINGS_CONTENT_STANDARD
     with codecs_open(os.path.join(proj_path, "settings.py"), "wb") as fd:
         fd.write(
             (
@@ -195,27 +192,25 @@
                     "ProjectName": proj_name,
                 }
             ).encode("utf8")
         )
 
 
 def _create_managepy(proj_path):
-    """创建manage.py文件
-    """
+    """创建manage.py文件"""
     with codecs_open(os.path.join(proj_path, "manage.py"), "wb") as fd:
         fd.write(
             (
                 MANAGE_CONTENT % {"Date": datetime.date.today().strftime("%Y/%m/%d")}
             ).encode("utf8")
         )
 
 
 def _create_sample_test(dir_path, proj_name):
-    """创建示例测试用例
-    """
+    """创建示例测试用例"""
     with codecs_open(os.path.join(dir_path, "hello.py"), "wb") as fd:
         fd.write(
             (
                 TESTCASE_CONTENT
                 % {
                     "Date": datetime.date.today().strftime("%Y/%m/%d"),
                     "ProjectName": proj_name,
@@ -223,53 +218,49 @@
                     "UserName": getpass.getuser(),
                 }
             ).encode("utf8")
         )
 
 
 def _create_sample_lib(dir_path, proj_name):
-    """创建示例lib
-    """
+    """创建示例lib"""
     with codecs_open(os.path.join(dir_path, "testcase.py"), "wb") as fd:
         fd.write(
             (
                 TESTLIB_CONTENT
                 % {
                     "Date": datetime.date.today().strftime("%Y/%m/%d"),
                     "ProjectName": proj_name,
                     "ProjectNameCapUp": proj_name[0].upper() + proj_name[1:],
                 }
             ).encode("utf8")
         )
 
 
 def _copy_qtaf_egg(egg_path, dir_path):
-    """拷贝QTAF egg包
-    """
+    """拷贝QTAF egg包"""
     shutil.copy(egg_path, dir_path)
     with zipfile.ZipFile(egg_path) as zfile:
         try:
             zfile.getinfo("doc/qtaf.chm")  # chm可能不存在
         except KeyError:
             return
         else:
             with codecs_open(os.path.join(dir_path, "qtaf.chm"), "wb") as fd:
                 fd.write(zfile.read("doc/qtaf.chm"))
 
 
 def _create_eclipse_projfile(proj_path, proj_name):
-    """创建eclispe项目文件
-    """
+    """创建eclispe项目文件"""
     with codecs_open(os.path.join(proj_path, ".project"), "wb") as fd:
         fd.write((ECLIPSE_PROJ_CONTENT % {"ProjectName": proj_name}).encode("utf8"))
 
 
 def _create_pydev_conffile(proj_path, mode):
-    """创建pydev配置文件
-    """
+    """创建pydev配置文件"""
     with codecs_open(os.path.join(proj_path, ".pydevproject"), "wb") as fd:
         if mode == EnumProjectMode.Standalone:
             qtaf_egg_path = os.path.join(
                 os.path.dirname(os.path.abspath(__file__)), ".."
             )
             qtaf_egg_path = os.path.abspath(qtaf_egg_path)
             fd.write(
@@ -279,16 +270,15 @@
                 ).encode("utf8")
             )
         else:
             fd.write(PYDEV_CONF_CONTENT_STANDARD.encode("utf8"))
 
 
 def _update_pydev_conffile(proj_path, egg_name):
-    """更新pydev配置文件中的Egg名称
-    """
+    """更新pydev配置文件中的Egg名称"""
     with codecs_open(
         os.path.join(proj_path, ".pydevproject"), "r", encoding="utf-8"
     ) as fd:
         doc = dom.parse(fd)
         nodes = doc.getElementsByTagName("pydev_pathproperty")
         if len(nodes) == 0:
             propsnode = doc.createElement("pydev_pathproperty")
@@ -311,16 +301,15 @@
         propsnode.appendChild(pathnode)
 
     with codecs_open(os.path.join(proj_path, ".pydevproject"), "wb", "utf8") as fd:
         fd.write(doc.toxml(encoding="UTF-8"))
 
 
 def create_project(dest_path, proj_name, mode):
-    """创建项目
-    """
+    """创建项目"""
     if not os.path.isdir(dest_path):
         os.makedirs(dest_path)
 
     lib_dir = os.path.join(dest_path, "%slib" % proj_name)
     if not os.path.isdir(lib_dir):
         os.mkdir(lib_dir)
         _create_initpy(lib_dir, "测试lib")
@@ -349,35 +338,32 @@
     _create_settingspy(dest_path, proj_name, mode)
     _create_managepy(dest_path)
     _create_eclipse_projfile(dest_path, proj_name)
     _create_pydev_conffile(dest_path, mode)
 
 
 def update_project_qtaf(proj_path, qtaf_egg_path):
-    """升级项目的QTAF
-    """
+    """升级项目的QTAF"""
     exlib_dir = os.path.join(proj_path, "exlib")
     for name in os.listdir(exlib_dir):
         if name.startswith("qtaf-") and name.endswith(".egg"):
             os.remove(os.path.join(exlib_dir, name))
     _copy_qtaf_egg(qtaf_egg_path, exlib_dir)
     _update_pydev_conffile(proj_path, os.path.basename(qtaf_egg_path))
 
 
 class Project(object):
-    """一个项目（废弃接口，存在是为了兼容）
-    """
+    """一个项目（废弃接口，存在是为了兼容）"""
 
     def __init__(self, root):
         self._root = root
 
     @property
     def path(self):
         return self._root
 
 
 def current_project():
-    """获取当前项目（废弃接口，存在是为了兼容）
-    """
+    """获取当前项目（废弃接口，存在是为了兼容）"""
     from testbase.conf import settings
 
     return Project(settings.PROJECT_ROOT)
```

### Comparing `qtaf-5.5.9/testbase/report.py` & `qtaf-5.6.0/testbase/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 """
 
 import sys
 import socket
 import os
 import shutil
 import json
-import getpass
 import locale
 import argparse
 import xml.dom.minidom as dom
 import xml.sax.saxutils as saxutils
 
 from datetime import datetime
 
@@ -39,14 +38,15 @@
     codecs_open,
     get_os_version,
     get_inner_resource,
 )
 from testbase.version import version
 
 os_encoding = locale.getdefaultlocale()[1]
+# pylint: disable=invalid-name
 report_usage = (
     'runtest <test ...> --report-type <report-type> [--report-args "<report-args>"]'
 )
 
 
 class ITestReport(object):
     """测试报告接口"""
@@ -125,14 +125,26 @@
         """记录被测对象
 
         :param test_target: 被测对象详情
         :type test_target: any
         """
         pass
 
+    def log_not_run_test(self, testcase, testresult_type, reason=""):
+        """记录没有执行的用例
+
+        :param testcase: 测试用例
+        :type testcase: TestCase
+        :param testresult_type: 自定义测试结果类型
+        :type testresult_type: TestResultType
+        :param reason: 原因
+        :type reason: str
+        """
+        pass
+
     def log_resource(self, res_type, resource):
         """记录测试使用的资源
 
         :param res_type: 资源类型
         :type res_type: str
         :param resource: 资源详情
         :type resource: dict
@@ -257,14 +269,29 @@
     def is_passed(self):
         """报告中是否所有用例都通过，兼容已有EmptyTestReport，若用例数为0，也认为不通过
 
         :return: boolean
         """
         return all(self._cases_passed.values()) and len(self._cases_passed) > 0
 
+    def log_not_run_test(self, testcase, testresult_type, reason=""):
+        """记录没有执行的用例
+
+        :param testcase: 测试用例
+        :type testcase: TestCase
+        :param testresult_type: 自定义测试结果类型
+        :type testresult_type: TestResultType
+        :param reason: 原因
+        :type reason: str
+        """
+        result = self.get_testresult_factory().create(testcase)
+        result.customize_result(testresult_type, reason)
+        result.begin_test(testcase)
+        result.end_test()
+
 
 class ITestResultFactory(object):
     """TestResult工厂接口"""
 
     def create(self, testcase):
         """创建TestResult对象
         :param testcase: 测试用例
@@ -484,15 +511,15 @@
             self._passed_testresults.append(testresult)
         else:
             self._failed_testresults.append(testresult)
         self._write(
             "run test case: %s(pass?:%s)\n" % (testcase.test_name, testresult.passed)
         )
 
-    def log_record(self, level, tag, msg, record={}):
+    def log_record(self, level, tag, msg, record=None):
         """增加一个记录
         :param level: 日志级别
         :param msg: 日志消息
         :param tag: 日志标签
         :param record: 日志记录信息
         :type level: string
         :type tag: string
@@ -645,30 +672,33 @@
         """ % (
             testresult.passed,
             testresult.file_path,
             testcase.status,
             casemark,
         )
         doc2 = dom.parseString(smart_binary(nodestr))
-        resultNode = doc2.childNodes[0]
-        resultNode.setAttribute("name", smart_text(saxutils.escape(testcase.test_name)))
-        resultNode.setAttribute("owner", smart_text(saxutils.escape(testcase.owner)))
-        self._runrstnode.appendChild(resultNode)
+        result_node = doc2.childNodes[0]
+        result_node.setAttribute(
+            "name", smart_text(saxutils.escape(testcase.test_name))
+        )
+        result_node.setAttribute("owner", smart_text(saxutils.escape(testcase.owner)))
+        self._runrstnode.appendChild(result_node)
 
-    def log_record(self, level, tag, msg, record={}):
+    def log_record(self, level, tag, msg, record=None):
         """增加一个记录
         :param level: 日志级别
         :param msg: 日志消息
         :param tag: 日志标签
         :param record: 日志记录信息
         :type level: string
         :type tag: string
         :type msg: string
         :type record: dict
         """
+        record = record or {}
         if tag == "LOADER" and level == EnumLogLevel.ERROR:
             if "error_testname" in record and "error" in record:
                 testname = record["error_testname"]
                 mdfailsnode = self._xmldoc.createElement("LoadFailure")
                 self._runrstnode.appendChild(mdfailsnode)
                 logfile = "%s.log" % testname
                 xmltpl = """<Module name="%s" log="%s"/>""" % (testname, logfile)
@@ -687,16 +717,16 @@
         """
         nodestr = """<FilterTest name="%s" reason="%s"></FilterTest>
         """ % (
             smart_text(saxutils.escape(testcase.test_name)),
             smart_text(saxutils.escape(reason)),
         )
         doc2 = dom.parseString(nodestr)
-        filterNode = doc2.childNodes[0]
-        self._runrstnode.appendChild(filterNode)
+        filter_node = doc2.childNodes[0]
+        self._runrstnode.appendChild(filter_node)
 
     def log_load_error(self, loader, name, error):
         """记录一个加载失败的用例或用例集
         :param loader: 用例加载器
         :type loader: TestLoader
         :param name: 名称
         :type name: str
@@ -706,16 +736,16 @@
         log_file = "%s.log" % name
         nodestr = """<LoadTestError name="%s" log="%s"></LoadTestError>
         """ % (
             smart_text(saxutils.escape(name)),
             log_file,
         )
         doc2 = dom.parseString(nodestr)
-        errNode = doc2.childNodes[0]
-        self._runrstnode.appendChild(errNode)
+        err_node = doc2.childNodes[0]
+        self._runrstnode.appendChild(err_node)
         with codecs_open(log_file, "wb") as fd:
             fd.write(smart_binary(error))
 
     def get_testresult_factory(self):
         """获取对应的TestResult工厂
         :returns ITestResultFactory
         """
@@ -930,16 +960,17 @@
         fd = codecs_open(args.output, "w", encoding="utf-8")
         return cls(fd, title=args.title)
 
 
 class HtmlTestReport(JSONTestReportBase):
     """html test report"""
 
-    def __init__(self, title="调试测试", displays=["failed", "error"]):
+    def __init__(self, title="调试测试", displays=None):
         super(HtmlTestReport, self).__init__(title=title)
+        displays = displays or ["failed", "error"]
         self._data["displays"] = displays
 
     def get_testresult_factory(self):
         """获取对应的TestResult工厂
         :returns ITestResultFactory
         """
         return HtmlTestResultFactory()
```

### Comparing `qtaf-5.5.9/testbase/resource.py` & `qtaf-5.6.0/testbase/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,51 +28,48 @@
 import testbase.logger as logger
 from testbase.conf import settings
 from testbase.util import smart_text, codecs_open
 from testbase.testresult import EnumLogLevel
 
 os_encoding = locale.getdefaultlocale()[1]
 if not os_encoding:
-    os_encoding = 'utf8'
+    os_encoding = "utf8"  # pylint: disable=invalid-name
 
 
 class ResourceNotAvailable(Exception):
-    """没有可用的资源
-    """
+    """没有可用的资源"""
+
     pass
 
 
 class DownloadFileError(Exception):
-    """download file failed
-    """
+    """download file failed"""
 
     def __init__(self, url, status_code, msg, headers, data):
         self.url = url
         self.status_code = status_code
         self.msg = msg
         self.headers = headers
         self.data = data
 
     def __str__(self):
-        return "downloading file failed for: %s %s %s\nheaders=%s\nbody=%s" % (self.url,
-                                                             self.status_code,
-                                                             self.msg,
-                                                             self.headers,
-                                                             smart_text(self.data))
-
-
+        return "downloading file failed for: %s %s %s\nheaders=%s\nbody=%s" % (
+            self.url,
+            self.status_code,
+            self.msg,
+            self.headers,
+            smart_text(self.data),
+        )
 
 
 class Session(object):
-    """会话
-    """
+    """会话"""
 
     def __init__(self, backend, session_id):
-        """构造函数
-        """
+        """构造函数"""
         self._backend = backend
         self._id = session_id
 
     def acquire_resource(self, res_type, res_group=None, condition=None):
         """申请资源
 
         :param res_type: 资源类型
@@ -82,44 +79,56 @@
         :param condition: 资源属性匹配
         :type condition: dict
         :returns: 资源
         :rtypes: dict
         """
         tc = context.current_testresult()
         try:
-            resource = self._backend.acquire_resource(self._id, res_type, res_group, condition)
+            resource = self._backend.acquire_resource(
+                self._id, res_type, res_group, condition
+            )
         except ResourceNotAvailable:
             if tc:
-                tc.log_record(EnumLogLevel.RESNOTREADY, "acquire resource (res_type:%s, res_group:%s, condition:%s) failed" % (res_type, res_group, condition))
+                tc.log_record(
+                    EnumLogLevel.RESNOTREADY,
+                    "acquire resource (res_type:%s, res_group:%s, condition:%s) failed"
+                    % (res_type, res_group, condition),
+                )
             raise
         else:
             if tc:
                 extra = {}
                 extra["res_type"] = res_type
                 if not isinstance(resource, dict):
                     raise ValueError("Resource record should be a dictionary")
                 if "id" not in resource:
-                    raise ValueError("Resource record should be a dictionary with key 'id'")
+                    raise ValueError(
+                        "Resource record should be a dictionary with key 'id'"
+                    )
                 extra["resource_id"] = resource["id"]
-                tc.log_record(EnumLogLevel.RESOURCE, "acquire resource (res_type:%s, res_group:%s, condition:%s) successfully" % (res_type, res_group, condition), extra)
+                tc.log_record(
+                    EnumLogLevel.RESOURCE,
+                    "acquire resource (res_type:%s, res_group:%s, condition:%s) successfully"
+                    % (res_type, res_group, condition),
+                    extra,
+                )
             return resource
 
     def release_resource(self, res_type, resource_id):
         """释放资源
 
         :param res_type: 资源类型
         :type res_type: str
         :param resource_id: 资源ID
         :type resource_id: str
         """
         return self._backend.release_resource(self._id, res_type, resource_id)
 
     def destroy(self):
-        """销毁该会话（全部占用的资源会释放）
-        """
+        """销毁该会话（全部占用的资源会释放）"""
         if not self._id:
             return
         res = self._backend.destroy_session(self._id)
         self._id = None
         return res
 
     def get_file(self, path):
@@ -131,15 +140,15 @@
         """
         return self._backend.get_file(path)
 
     def list_dir(self, path):
         """获取目录下文件列表
 
         :param path: 目录引用路径（相对路径）
-        :returns: 一个包含该目录下所有文件的绝对路径的list 
+        :returns: 一个包含该目录下所有文件的绝对路径的list
         :rtypes: list[str]
         """
         return self._backend.list_dir(path)
 
     def walk(self, path):
         """获取目录下文件列表
 
@@ -148,16 +157,15 @@
         :return iterators: iterator of (dir_path, dirnames, filenames) tuples
         :type   iterators: iterator
         """
         return self._backend.walk(path)
 
 
 class IResourceManagerBackend(object):
-    """测试资源管理后端接口定义
-    """
+    """测试资源管理后端接口定义"""
 
     def create_session(self, testcase=None):
         """创建会话
 
         :param testcase: 使用的测试用例
         :type testcase: TestCase
         :returns: 会话ID
@@ -263,16 +271,15 @@
         :returns: iterator of (res_type, resource)
         :rtypes: iterator(str, dict)
         """
         return self._backend.iter_managed_resource()
 
 
 class LocalResourceLock(object):
-    """本地资源锁
-    """
+    """本地资源锁"""
 
     _lock_cache = {}
 
     def __init__(self, res_type, resource_id):
         self._res_type = res_type
         self._resource_id = resource_id
         if sys.platform == "win32":
@@ -297,23 +304,23 @@
             return False
         if self._os_try_acquire():
             self._lock_cache[self._file_path] = self
             return True
         return False
 
     def release(self):
-        """释放
-        """
+        """释放"""
         if self._fd is None:
             raise RuntimeError("lock is not acquired")
         del self._lock_cache[self._file_path]
         return self._os_release()
 
     def _win_try_acquire(self):
         import msvcrt
+
         try:
             fd = os.open(self._file_path, os.O_RDWR | os.O_CREAT | os.O_TRUNC)
         except OSError:
             pass
         else:
             try:
                 msvcrt.locking(fd, msvcrt.LK_NBLCK, 1)
@@ -322,57 +329,59 @@
             else:
                 self._fd = fd
                 return True
         return False
 
     def _win_release(self):
         import msvcrt
+
         msvcrt.locking(self._fd, msvcrt.LK_UNLCK, 1)
         os.close(self._fd)
         try:
             os.remove(self._file_path)
         except OSError:
             pass
         self._fd = None
 
     def _unix_try_acquire(self):
         import fcntl
+
         fd = os.open(self._file_path, os.O_RDWR | os.O_CREAT | os.O_TRUNC)
         try:
             fcntl.flock(fd, fcntl.LOCK_EX | fcntl.LOCK_NB)
         except (IOError, OSError):
             os.close(fd)
         else:
             self._fd = fd
             return True
         return False
 
     def _unix_release(self):
         import fcntl
+
         fcntl.flock(self._fd, fcntl.LOCK_UN)
         os.close(self._fd)
         self._fd = None
 
 
 class LocalResourceHandler(object):
-    """本地资源处理句柄
-    """
+    """本地资源处理句柄"""
 
     def __init__(self, resource_lock_type=LocalResourceLock):
         """构造函数
 
         :param resource_lock_type: 资源锁类型
         :type resource_lock_type: type
         """
         self._lock_type = LocalResourceLock
         self._res_locks = {}
 
     def acquire_resource(self, session_id, res_type, res_group, condition):
         """申请资源
-    
+
         :param session_id: 会话ID
         :type session_id: str
         :param res_type: 资源类型
         :type res_type: str
         :param res_group: 资源分组
         :type res_group: str
         :param condition: 资源属性匹配
@@ -402,15 +411,17 @@
         :param res_type: 资源类型
         :type res_type: str
         :param resource_id: 资源ID
         :type resource_id: str
         """
         if session_id not in self._res_locks:
             raise ValueError("invalid session")
-        for idx, (_res_type, _resource_id, lock) in enumerate(self._res_locks[session_id]):
+        for idx, (_res_type, _resource_id, lock) in enumerate(
+            self._res_locks[session_id]
+        ):
             if _res_type == res_type and _resource_id == resource_id:
                 lock.release()
             del self._res_locks[session_id][idx]
             break
         else:
             raise ValueError("resource is not acquired yet")
 
@@ -457,16 +468,15 @@
         :returns: iterator of resource
         :rtypes: iterator(dict)
         """
         return self.iter_resource(res_type)
 
 
 class LocalCSVResourceHandler(LocalResourceHandler):
-    """基于本地CSV文件管理资源
-    """
+    """基于本地CSV文件管理资源"""
 
     def __init__(self, csv_path, resource_lock_type=LocalResourceLock):
         """构造函数
 
         :param csv_path: CSV文件
         :type csv_path: str
         :param resource_lock_type: 资源锁类型
@@ -491,83 +501,84 @@
             for rowid, row in enumerate(csv.DictReader(fd)):
                 if "id" not in row:
                     row["id"] = rowid
                     yield row
 
 
 class LocalResourceManagerBackend(IResourceManagerBackend):
-    """基本本地文件的方式的资源管理
-    """
+    """基本本地文件的方式的资源管理"""
+
     _res_type_map = {}
 
     @classmethod
     def register_resource_type(cls, res_type, handler):
-        """注册一个资源类型
-        """
+        """注册一个资源类型"""
         cls._res_type_map[res_type] = handler
 
     def __init__(self):
         self._resources_dirs = iter_resource_paths()
-        self._session_path = os.path.join(settings.PROJECT_ROOT, 'sessions')
+        self._session_path = os.path.join(settings.PROJECT_ROOT, "sessions")
 
     def _adjust_path(self, path):
-        """根据操作系统转换文件分隔符
-        """
-        if os.sep == '/':
-            return path.replace('\\', os.sep)
+        """根据操作系统转换文件分隔符"""
+        if os.sep == "/":
+            return path.replace("\\", os.sep)
         else:
-            return path.replace('/', os.sep)
+            return path.replace("/", os.sep)
 
     def _download_file(self, url, target_path):
         from six.moves.urllib import request, error
+
         try:
             rsp = request.urlopen(url, timeout=300)
             rspbuf = rsp.read()
         except error.HTTPError as e:
             raise DownloadFileError(url, e.code, e.msg, e.headers, e.read())
         with codecs_open(target_path, "wb") as fd:
             fd.write(rspbuf)
 
     def _resolve_link_file(self, remote_path, prefer_local_path):
-        """获取链接的真正的文件
-        """
+        """获取链接的真正的文件"""
         if os.path.isfile(remote_path):
             return remote_path
         elif remote_path.startswith("http://") or remote_path.startswith("https://"):
             self._download_file(remote_path, prefer_local_path)
             return prefer_local_path
         else:
             raise ValueError("Invalid link file path: %s" % remote_path)
 
     def abs_path(self, relative_path):
         """get resource absolute path
-:        type relative_path:string
-        :param relative_path: ，资源文件相对描述符，相对于setting下的资源目录的路径,支持多级目录
-        :return:返回资源文件的绝对路径
+        :        type relative_path:string
+                :param relative_path: ，资源文件相对描述符，相对于setting下的资源目录的路径,支持多级目录
+                :return:返回资源文件的绝对路径
         """
         relative_path = self._adjust_path(relative_path)
         if relative_path.startswith(os.sep):
             relative_path = relative_path[1:]
 
         found_paths = []
         for it in self._resources_dirs:
             file_path = self._adjust_path(os.path.join(it, relative_path))
             file_path = smart_text(file_path)
-            file_link = smart_text(file_path + '.link')
+            file_link = smart_text(file_path + ".link")
             if os.path.exists(file_path):
                 found_paths.append(file_path)
             elif os.path.exists(file_link):
                 with codecs_open(file_link, encoding="utf-8") as f:
                     remote_path = f.read()
                     file_path = self._resolve_link_file(remote_path, file_path)
                     found_paths.append(file_path)
         if len(found_paths) == 0:
             raise Exception("relative_path=%s not found" % relative_path)
         if len(found_paths) > 1:
-            raise Exception("relative_path=%s got multiple results:\n%s" % (relative_path, "\n".join(found_paths)))
+            raise Exception(
+                "relative_path=%s got multiple results:\n%s"
+                % (relative_path, "\n".join(found_paths))
+            )
         return os.path.abspath(found_paths[0])
 
     def get_file(self, relative_path):
         """查找某个文件
 
         :type relative_path:string
         :param relative_path: 资源文件相对描述符，相对于setting下的资源目录的路径,支持多级目录
@@ -608,57 +619,53 @@
         for dir_path, dir_names, file_names in os.walk(abs_path):
             for index, file_name in enumerate(file_names):
                 if file_name.endswith(".link"):
                     file_names[index] = file_name[-5:]
             yield dir_path[base_len:], dir_names, file_names
 
     def _clean_cache(self):
-        """清理缓存文件
-        """
+        """清理缓存文件"""
         for it in self._resources_dirs:
             self._rm_cachefile_recursively(it)
 
     def _rm_cachefile_recursively(self, path):
-        """递归删除目录下的缓存文件
-        """
+        """递归删除目录下的缓存文件"""
         for root, _, files in os.walk(path):
             for it in files:
-                if it.endswith('.link'):
+                if it.endswith(".link"):
                     try:
                         os.remove(os.path.join(root, it)[0:-5])
                     except OSError:
                         pass
 
     def create_session(self, testcase=None):
-        """创建会话
-        """
+        """创建会话"""
         session_id = str(uuid.uuid4())
-        timeout = 300 if testcase is None else (testcase.timeout * 60 + 300 + 5)  # 300为用例超时时的Cleanup超时时间
+        timeout = (
+            300 if testcase is None else (testcase.timeout * 60 + 300 + 5)
+        )  # 300为用例超时时的Cleanup超时时间
         for handler in self._res_type_map.values():
             handler.session_created(session_id, timeout, testcase)
         return session_id
 
     def destroy_session(self, sessionid):
-        """销毁会话
-        """
+        """销毁会话"""
         self._clean_cache()
         for handler in self._res_type_map.values():
             handler.session_destroyed(sessionid)
 
     def acquire_resource(self, session_id, res_type, res_group, condition):
-        """申请资源
-        """
+        """申请资源"""
         handler = self._res_type_map.get(res_type)
         if handler is None:
             raise ValueError("resource type '%s' it not registered")
         return handler.acquire_resource(session_id, res_type, res_group, condition)
 
     def release_resource(self, session_id, res_type, resource_id):
-        """释放资源
-        """
+        """释放资源"""
         handler = self._res_type_map.get(res_type)
         if handler is None:
             raise ValueError("resource type '%s' it not registered")
         return handler.release_resource(session_id, res_type, resource_id)
 
     def iter_managed_resource(self):
         """查询全部托管的资源（支持初始化&反初始化）
@@ -694,15 +701,15 @@
     :returns :返回一个包含资源目录下所有文件或者文件下的绝对路径的list
     """
     return _current_resmgr_session().list_dir(path)
 
 
 def walk(path):
     """遍历某个路径
-    
+
     :param path: 相对于resources目录的路径，用于遍历文件夹
     :type  path: str
     :return iterators: iterator of (dir_path, dirnames, filenames) tuples
     :type   iterators: iterator
     """
     return _current_resmgr_session().walk(path)
 
@@ -732,16 +739,15 @@
     """
     return _current_resmgr_session().release_resource(res_type, resource_id)
 
 
 def iter_resource_paths():
     """返回测试项目的全部resources目录
 
-    :return: 
+    :return:
     """
     resource_paths = []
     for dirpath, dirnames, _ in os.walk(settings.PROJECT_ROOT):
         for dirname in dirnames:
-            if dirname == 'resources':
+            if dirname == "resources":
                 resource_paths.append(os.path.join(dirpath, dirname))
     return resource_paths
-
```

### Comparing `qtaf-5.5.9/testbase/retry.py` & `qtaf-5.6.0/testbase/retry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,137 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 """重试机制实现
 """
 
 import time
-    
+
+
 class _RetryItem(object):
-    """
-    """
+    """ """
+
     def __init__(self, iteration, timestamps=None):
         self.__iteration = iteration
         self.__ts = timestamps
 
     @property
     def iteration(self):
         return self.__iteration
-    
+
     @property
     def ts(self):
         return self.__ts
-    
+
     def __str__(self):
-        return "<%s iter=%s, ts=%s>" % (self.__class__.__name__, self.__iteration, self.__ts)
-            
-    
+        return "<%s iter=%s, ts=%s>" % (
+            self.__class__.__name__,
+            self.__iteration,
+            self.__ts,
+        )
+
+
 class _RetryWithTimeout(object):
-    """retry mechanism with timeout
-    """
-    def __init__(self,interval=5, timeout=60, raise_error=True):
+    """retry mechanism with timeout"""
+
+    def __init__(self, interval=5, timeout=60, raise_error=True):
         self.interval = interval
         self.timeout = timeout
         self.raise_error = raise_error
         self.__start_time = None
         self.__count = 0
-    
+
     def __iter__(self):
         return self
-    
+
     def next(self):
-        if self.__start_time == None:
+        if self.__start_time is None:
             self.__count += 1
             self.__start_time = time.time()
             return _RetryItem(self.__count, self.__start_time)
         else:
             time.sleep(self.interval)
             ts = time.time()
             if ts - self.__start_time < self.timeout:
                 self.__count += 1
                 return _RetryItem(self.__count, ts)
             else:
                 if self.raise_error:
-                    raise RetryLimitExcceeded("Procedure retried %s times in %ss" % (self.__count, self.timeout))
+                    raise RetryLimitExcceeded(
+                        "Procedure retried %s times in %ss"
+                        % (self.__count, self.timeout)
+                    )
                 else:
                     raise StopIteration
-                
+
     __next__ = next
-        
-        
+
+
 class _RetryWithCount(object):
-    """retry mechanism with count
-    """
-    def __init__(self, limit=3, interval=0,raise_error=True):
+    """retry mechanism with count"""
+
+    def __init__(self, limit=3, interval=0, raise_error=True):
         self.limit = limit
         self.raise_error = raise_error
         self.interval = interval
         self.__count = 0
-        
+
     def __iter__(self):
         return self
-    
+
     def next(self):
         self.__count += 1
         if self.__count <= self.limit:
-            if self.__count !=1 and self.interval:
+            if self.__count != 1 and self.interval:
                 time.sleep(self.interval)
             return _RetryItem(self.__count, time.time())
         if self.raise_error:
-            raise RetryLimitExcceeded("Procedure retried for %s times with interval=%ss" % (self.limit, self.interval))
+            raise RetryLimitExcceeded(
+                "Procedure retried for %s times with interval=%ss"
+                % (self.limit, self.interval)
+            )
         else:
             raise StopIteration
-        
+
     __next__ = next
 
-        
+
 class RetryLimitExcceeded(Exception):
-    """maxmium retry limit excceeded error
-    """
+    """maxmium retry limit excceeded error"""
+
     pass
 
- 
+
 class Retry(object):
-    """retry mechanism with timeout or limit
-    """
+    """retry mechanism with timeout or limit"""
+
     def __init__(self, timeout=10, limit=None, interval=0.5, raise_error=True):
         if limit:
-            self._retry = _RetryWithCount(limit=limit, interval=interval, raise_error=raise_error)
+            self._retry = _RetryWithCount(
+                limit=limit, interval=interval, raise_error=raise_error
+            )
         else:
-            self._retry = _RetryWithTimeout(timeout=timeout, interval=interval, raise_error=raise_error)
-        
+            self._retry = _RetryWithTimeout(
+                timeout=timeout, interval=interval, raise_error=raise_error
+            )
+
     def __iter__(self):
         return self._retry.__iter__()
-    
+
     def call(self, callee, *args, **kwargs):
         if not hasattr(callee, "__call__"):
             raise ValueError("callee must be a function instance")
         for _ in self:
             r = callee(*args, **kwargs)
             if r:
                 return r
```

### Comparing `qtaf-5.5.9/testbase/runner.py` & `qtaf-5.6.0/testbase/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,68 +8,82 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 TestRunner负责多个测试用例，目前提供三种方式:
 
     - 单线程执行 TestRunner
     - 多线程执行 ThreadingTestRunner
     - 多进程执行 MultiProcessTestRunner
 
 整个执行逻辑可以用以下伪代码来理解::
 
     for test in tests:
         report.begin_test(test)
         result = report.get_testresult_factory().create(test)
         report.end_test(test, result)
 
-'''
+"""
 from __future__ import absolute_import
 
-import threading
-import multiprocessing
-import traceback
+import argparse
 import collections
+import itertools
+import multiprocessing
 import random
 import re
-import types
-import sys
-import argparse
 import socket
+import sys
+import threading
+import traceback
+import types
 import uuid
-import itertools
-import json
+
 import six
 
 from six.moves import queue
 
 from testbase import logger
 from testbase.loader import TestLoader
 from testbase import serialization
-from testbase.testcase import TestCase, TestCaseRunner, TestSuite
 from testbase.report import TestReportBase
-from testbase.testresult import TestResultCollection
+from testbase.testcase import TestCase, TestCaseRunner
+from testbase.testsuite import TestSuiteBase
+from testbase.testresult import TestResultCollection, TestResultType
 from testbase.resource import TestResourceManager, LocalResourceManagerBackend
 from testbase.plan import TestPlan
 from testbase.util import ShareDataManager
 
-runner_usage = 'runtest <test ...> --runner-type <runner-type> [--runner-args "<runner-args>"]'
+# pylint: disable=invalid-name
+runner_usage = (
+    'runtest <test ...> --runner-type <runner-type> [--runner-args "<runner-args>"]'
+)
 
 
 class TestCaseSettings(object):
-    '''目标测试用例配置
-    '''
+    """目标测试用例配置"""
 
-    def __init__(self, names=None, excluded_names=None, priorities=None, status=None, owners=None,
-                tags=None, excluded_tags=None, share_data={}, global_parameters={}):
-        '''构造函数
+    def __init__(
+        self,
+        names=None,
+        excluded_names=None,
+        priorities=None,
+        status=None,
+        owners=None,
+        tags=None,
+        excluded_tags=None,
+        share_data=None,
+        global_parameters=None,
+        stop=False
+    ):
+        """构造函数
 
         :param names: 测试用例名
         :type names: list
         :param excluded_names: 排除测试用例名
         :type excluded_names: list
         :param priorities: 指定用例优先级，如果不指定则默认全部优先级
         :type priorities: list
@@ -77,28 +91,38 @@
         :type status: list
         :param owners: 指定用户名进行过滤
         :type owners: list
         :param tags: 指定标签选择用例
         :type tags: list
         :param excluded_tags: 指定标签排除用例
         :type tags: list
-        '''
+        :param stop: 遇见执行失败时，是否停止测试，如果True则支持，默认False
+        :type stop: bool
+        """
+        share_data = share_data or {}
+        global_parameters = global_parameters or {}
+        self.stop = stop
         if names is None:
             self.names = []
         else:
             # self.names = list(names)
-            self.names = [name if isinstance(name, dict) else {"name": self._generate_testcase_names(name)} for name in names]
+            self.names = [
+                name
+                if isinstance(name, dict)
+                else {"name": self._generate_testcase_names(name)}
+                for name in names
+            ]
 
         for case in self.names:
             if "parameters" in case:
                 for parameter in global_parameters:
-                    if parameter not in case['parameters']:
-                        case['parameters'][parameter] = global_parameters[parameter]
+                    if parameter not in case["parameters"]:
+                        case["parameters"][parameter] = global_parameters[parameter]
             else:
-                case['parameters'] = global_parameters
+                case["parameters"] = global_parameters
 
         if owners is None:
             self.owners = []
         else:
             self.owners = list(owners)
 
         if excluded_names is None:
@@ -107,25 +131,29 @@
             excluded_names = list(excluded_names)
         self.excluded_names = []
         for it in excluded_names:
             if it:
                 self.excluded_names.append(it)
 
         if priorities is None:
-            priorities = [TestCase.EnumPriority.BVT,
-                          TestCase.EnumPriority.High,
-                          TestCase.EnumPriority.Normal,
-                          TestCase.EnumPriority.Low]
+            priorities = [
+                TestCase.EnumPriority.BVT,
+                TestCase.EnumPriority.High,
+                TestCase.EnumPriority.Normal,
+                TestCase.EnumPriority.Low,
+            ]
 
         if status is None:
-            status = [TestCase.EnumStatus.Design,
-                      TestCase.EnumStatus.Implement,
-                      TestCase.EnumStatus.Ready,
-                      TestCase.EnumStatus.Review,
-                      TestCase.EnumStatus.Suspend]
+            status = [
+                TestCase.EnumStatus.Design,
+                TestCase.EnumStatus.Implement,
+                TestCase.EnumStatus.Ready,
+                TestCase.EnumStatus.Review,
+                TestCase.EnumStatus.Suspend,
+            ]
         self.priorities = priorities
         self.status = status
 
         self.excluded_cls_names = []
         self.excluded_mod_names = []
         for it in self.excluded_names:
             if self._is_test_class(it):
@@ -135,51 +163,50 @@
 
         self.tags = set(tags) if tags else None
         self.excluded_tags = set(excluded_tags) if excluded_tags else None
         self.share_data = share_data
 
     def _generate_testcase_names(self, testcase):
         if testcase.endswith(".py"):
-            testcase = re.sub(r'\\|/', '.', testcase)
-            testcase = re.sub(r'\.py$', '', testcase)
+            testcase = re.sub(r"\\|/", ".", testcase)
+            testcase = re.sub(r"\.py$", "", testcase)
         return testcase
 
     def _is_test_class(self, name):
-        '''判断路径是否是一个类名
-        '''
-        if '/' in name:  # 数据驱动相关的类
+        """判断路径是否是一个类名"""
+        if "/" in name:  # 数据驱动相关的类
             return True
-        if '.' not in name:  # 不可能直接引用类名
+        if "." not in name:  # 不可能直接引用类名
             return False
 
         try:
             __import__(name)
             return False  # 为模块
-        except ImportError:
-            modname, clsname = name.rsplit('.', 1)
+        except ImportError:  # pylint: disable=broad-except
+            modname, clsname = name.rsplit(".", 1)
             try:
                 __import__(modname)
                 mod = sys.modules[modname]
-            except:
+            except Exception:  # pylint: disable=broad-except
                 return False  # 不存在的模块
             else:
                 return hasattr(mod, clsname)
 
     def filter(self, testcase):
-        '''测试用例过滤函数
+        """测试用例过滤函数
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
+        """
         name = testcase.test_name
         for it in self.excluded_cls_names:
             if name.startswith(it):
                 return "match excluded list: '%s'" % it
         for it in self.excluded_mod_names:
-            if name.startswith(it + '.'):
+            if name.startswith(it + "."):
                 return "match excluded list: '%s'" % it
         if testcase.status not in self.status:
             return "testcase with status '%s' is excluded" % testcase.status
         if testcase.priority not in self.priorities:
             return "testcase with priority '%s' is excluded" % testcase.priority
         if self.owners and testcase.owner not in self.owners:
             return "testcase with owner '%s' is excluded" % testcase.owner
@@ -187,92 +214,104 @@
             return "testcase is not tagged with %s" % ("/".join(self.tags))
         if self.excluded_tags and not self.excluded_tags.isdisjoint(testcase.tags):
             return "testcase is tag with %s" % ("/".join(self.excluded_tags))
         return False
 
 
 class BaseTestRunner(object):
-    '''测试执行器基类
-    '''
+    """测试执行器基类"""
 
     def __init__(self, report, resmgr_backend=None, execute_type="random"):
-        '''构造函数
+        """构造函数
 
         :param report: 测试报告
         :type report: ITestReport
-        '''
+        """
         self.__report = report
+        self.stop = False
         if resmgr_backend is None:
             resmgr_backend = LocalResourceManagerBackend()
         self._resmgr = TestResourceManager(resmgr_backend)
         self._execute_type = execute_type
 
+        self._not_run = []  # 未执行的用例
+        self._error_msg = ""    # 错误信息，目前用于未执行的用例
+
         self._share_data_mgr = ShareDataManager()
 
     @property
     def report(self):
-        '''对应的测试报告
+        """对应的测试报告
 
         :returns: ITestReport
-        '''
+        """
         return self.__report
 
     def load_share_data(self, data):
         if not isinstance(data, dict):
-            logger.warn("share_data expected dict instance, %s found" % type(data).__name__)
+            logger.warn(
+                "share_data expected dict instance, %s found" % type(data).__name__
+            )
             return
         for key, value in data.items():
             self._share_data_mgr.set(key, value)
 
     def get_share_data(self, key):
         return self._share_data_mgr.get(key)
 
     def add_share_data(self, key, value, level=0):
         self._share_data_mgr.set(key, value, level)
 
     def remove_share_data(self, name):
         self._share_data_mgr.remove(name)
 
     def load(self, target):
-        '''加载测试用例
+        """加载测试用例
 
         :param target: 指定要执行的测试用例
         :type target: list(TestCase) or list(string) or string or TestCaseSettings
         :returns: 测试用例列表
-        '''
+        """
         if isinstance(target, str):
             target = TestCaseSettings(names=target.split(" "))
-        elif isinstance(target, list) and len(target) and isinstance(target[0], six.string_types):
+        elif (
+            isinstance(target, list)
+            and target
+            and isinstance(target[0], six.string_types)
+        ):
             target = TestCaseSettings(names=target)
 
         if isinstance(target, TestCaseSettings):
             loader = TestLoader(target.filter)
             tests = loader.load(target.names)
             self.__report.log_loaded_tests(loader, tests)
             filtered_tests = loader.get_filtered_tests_with_reason().items()
             for test, reason in filtered_tests:
                 self.__report.log_filtered_test(loader, test, reason)
             for testname, error in loader.get_last_errors().items():
                 self.__report.log_load_error(loader, testname, error)
-            self.__report.info('Loader', 'filter %s testcases totally' % len(filtered_tests))
-            self.__report.info("Loader", 'load %s testcases totally' % len(tests))
+            self.__report.info(
+                "Loader", "filter %s testcases totally" % len(filtered_tests)
+            )
+            self.__report.info("Loader", "load %s testcases totally" % len(tests))
         else:
             tests = target
         return tests
 
     def run(self, target):
-        '''运行测试
+        """运行测试
 
         :param target: 指定要执行的测试
         :type target: list(TestCase) or list(string) or string or TestCaseSettings or TestPlan
-        '''
+        """
         if isinstance(target, TestPlan):
             plan = target
             target = plan.get_tests()
         else:
+            self.stop = getattr(target, "stop", False)  # TestCaseSettings stop
 
             class SimplePlan(TestPlan):
                 tests = target
                 test_target_args = {}
 
             plan = SimplePlan()
 
@@ -280,351 +319,382 @@
             self.load_share_data(target.share_data)
 
         self.__report.begin_report()
         plan.test_setup(self.__report)
         self.__report.log_test_target(plan.get_test_target())
         self.resource_setup(plan)
         self.run_all_tests(self.load(target))
+        if self._not_run:
+            for testcase in self._not_run:
+                self.__report.log_not_run_test(testcase, TestResultType.FILTERED, self._error_msg)
         self.resource_teardown(plan)
         plan.test_teardown(self.__report)
         self.__report.end_report()
         self.clean_up()
         return self.__report
 
     def resource_setup(self, plan):
-        '''资源初始化
+        """资源初始化
 
         :param plan: 测试计划
         :type plan: TestPlan
-        '''
-        for res_type, resource in itertools.chain([("node", {"host": socket.gethostname(), "id": uuid.getnode() })],
-                                                  self._resmgr.iter_managed_resource()):
+        """
+        for res_type, resource in itertools.chain(
+            [("node", {"host": socket.gethostname(), "id": uuid.getnode()})],
+            self._resmgr.iter_managed_resource(),
+        ):
             ret_resource = plan.resource_setup(self.__report, res_type, resource)
             if ret_resource:
                 resource = ret_resource
             self.__report.log_resource(res_type, resource)
 
     def resource_teardown(self, plan):
-        '''资源清理
+        """资源清理
 
         :param plan: 测试计划
         :type plan: TestPlan
-        '''
+        """
         for res_type, resource in self._resmgr.iter_managed_resource():
             plan.resource_teardown(self.__report, res_type, resource)
-        plan.resource_teardown(self.__report, "node", {"host": socket.gethostname(), "id": uuid.getnode() })
+        plan.resource_teardown(
+            self.__report, "node", {"host": socket.gethostname(), "id": uuid.getnode()}
+        )
 
     def run_all_tests(self, tests):
-        '''执行全部的测试用例
+        """执行全部的测试用例
 
         :param tests: 测试用例对象列表
         :type tests: list
-        '''
+        """
         if self._execute_type == "random":
             random.shuffle(tests)
         for test in tests:
             self.run_test(test)
 
     def run_test(self, test):
-        '''执行一个测试用例
+        """执行一个测试用例
 
         :param test: 测试用例
         :type test: TestCase
         :returns: boolean - 测试是否通过
-        '''
+        """
         test.test_resmgr = self._resmgr
         if isinstance(test, TestCase):
             test.share_data_mgr = self._share_data_mgr  # 用于传递共享数据
-        elif isinstance(test, TestSuite):
+        elif isinstance(test, TestSuiteBase):
+            test.share_data_mgr = self._share_data_mgr
             for it in test:
                 it.share_data_mgr = self._share_data_mgr
 
-        runner = getattr(test, 'case_runner', TestCaseRunner())
+        runner = getattr(test, "case_runner", TestCaseRunner())
         result = runner.run(test, self.__report.get_testresult_factory())
         if isinstance(result, TestResultCollection):
             self._log_collection_result(result)
         else:
             self.__report.log_test_result(result.testcase, result)
         return result.passed
 
     def clean_up(self):
-        '''执行清理动作
-        '''
+        """执行清理动作"""
         pass
 
     def _log_collection_result(self, result_collection):
-        '''记录结果集合
-        '''
+        """记录结果集合"""
         for it in result_collection:
             if isinstance(it, TestResultCollection):
                 self._log_collection_result(it)
             else:
                 self.__report.log_test_result(it.testcase, it)
 
     @classmethod
     def get_parser(cls):
-        '''获取命令行参数解析器（如果实现）
+        """获取命令行参数解析器（如果实现）
 
         :returns: 解析器对象
         :rtype: argparse.ArgumentParser
-        '''
+        """
         raise NotImplementedError()
 
     @classmethod
     def parse_args(cls, args_string, report, resmgr_backend, execute_type):
-        '''通过命令行参数构造对象
+        """通过命令行参数构造对象
 
         :returns: 测试报告
         :rtype: cls
-        '''
+        """
         raise NotImplementedError()
 
+    def handle_result(self, test, tests_queue, passed, tests_retry_dict):
+        if not passed:
+            if self.stop:
+                if len(tests_queue) <= 0:
+                    return
+                while len(tests_queue) > 0:
+                    testcase = tests_queue.popleft()
+                    self._error_msg = "some testcase failed, stop on failure."
+                    self._not_run.append(testcase)
+                return
+            tests_retry_dict.setdefault(test, 0)
+            if tests_retry_dict[test] < self._retries:
+                tests_retry_dict[test] += 1
+                tests_queue.append(test)
+
 
 class TestRunner(BaseTestRunner):
-    '''测试执行器
-    '''
+    """测试执行器"""
 
     def __init__(self, report, retries=0, resmgr_backend=None, execute_type="random"):
-        '''构造函数
+        """构造函数
 
         :param result: 测试报告
         :type result: ITestReport
         :param retries: 用例失败时重试次数
         :type retries: int
-        '''
+        """
         super(TestRunner, self).__init__(report, resmgr_backend, execute_type)
         self._retries = retries
 
     def run_all_tests(self, tests):
-        '''执行全部的测试用例
+        """执行全部的测试用例
 
         :param test: 测试用例对象列表
         :type tests: list
-        '''
+        """
         if self._execute_type == "random":
             random.shuffle(tests)
         tests_queue = collections.deque(tests)
         tests_retry_dict = {}
         while len(tests_queue) > 0:
             test = tests_queue.popleft()
             passed = self.run_test(test)
-            if not passed:
-                tests_retry_dict.setdefault(test, 0)
-                if tests_retry_dict[test] < self._retries:
-                    tests_retry_dict[test] += 1
-                    tests_queue.append(test)
+            self.handle_result(test=test,
+                             tests_queue=tests_queue,
+                             passed=passed,
+                             tests_retry_dict=tests_retry_dict)
 
     @classmethod
     def get_parser(cls):
-        '''获取命令行参数解析器（如果实现）
+        """获取命令行参数解析器（如果实现）
 
         :returns: 解析器对象
         :rtype: argparse.ArgumentParser
-        '''
+        """
         parser = argparse.ArgumentParser(usage=runner_usage)
-        parser.add_argument("--retries", type=int, default=0, help="retry count while test case failed")
+        parser.add_argument(
+            "--retries", type=int, default=0, help="retry count while test case failed"
+        )
         return parser
 
     @classmethod
     def parse_args(cls, args_string, report, resmgr_backend, execute_type):
-        '''通过命令行参数构造对象
+        """通过命令行参数构造对象
 
         :returns: 测试报告
         :rtype: cls
-        '''
+        """
         args = cls.get_parser().parse_args(args_string)
         return cls(report, args.retries, resmgr_backend, execute_type)
 
 
 class ThreadSafetyReport(TestReportBase):
-    '''TestReport修饰器，保证线程安全
-    '''
+    """TestReport修饰器，保证线程安全"""
 
     def __init__(self, report):
-        '''构造函数
+        """构造函数
 
         :param result: 测试报告
         :type result: ITestReport
-        '''
+        """
         super(ThreadSafetyReport, self).__init__()
         self._lock = threading.Lock()
         self._report = report
 
     def begin_report(self):
-        '''开始测试执行
-        '''
+        """开始测试执行"""
         with self._lock:
             return self._report.begin_report()
 
     def end_report(self):
-        '''结束测试执行
+        """结束测试执行
 
         :param passed: 测试是否通过
         :type passed: boolean
-        '''
+        """
         with self._lock:
             return self._report.end_report()
 
     def log_test_result(self, testcase, testresult):
-        '''记录一个测试结果
+        """记录一个测试结果
 
         :param testcase: 测试用例
         :type testcase: TestCase
         :param testresult: 测试结果
         :type testresult: TestResult
-        '''
+        """
         with self._lock:
             super(ThreadSafetyReport, self).log_test_result(testcase, testresult)
             return self._report.log_test_result(testcase, testresult)
 
     def log_loaded_tests(self, loader, testcases):
-        '''记录加载成功的用例
+        """记录加载成功的用例
 
         :param loader: 用例加载器
         :type loader: TestLoader
         :param testcases: 测试用例列表
         :type testcases: list
-        '''
+        """
         with self._lock:
             return self._report.log_loaded_tests(loader, testcases)
 
     def log_filtered_test(self, loader, testcase, reason):
-        '''记录一个被过滤的测试用例
+        """记录一个被过滤的测试用例
         :param loader: 用例加载器
         :type loader: TestLoader
         :param testcase: 测试用例
         :type testcase: TestCase
         :param reason: 过滤原因
         :type reason: str
-        '''
+        """
         with self._lock:
             return self._report.log_filtered_test(loader, testcase, reason)
 
     def log_load_error(self, loader, name, error):
-        '''记录一个加载失败的用例或用例集
+        """记录一个加载失败的用例或用例集
         :param loader: 用例加载器
         :type loader: TestLoader
         :param name: 名称
         :type name: str
         :param error: 错误信息
         :type error: str
-        '''
+        """
         with self._lock:
             return self._report.log_load_error(loader, name, error)
 
     def get_testresult_factory(self):
-        '''获取对应的TestResult工厂
+        """获取对应的TestResult工厂
 
         :returns: ITestResultFactory
-        '''
+        """
         with self._lock:
             return self._report.get_testresult_factory()
 
     def log_record(self, level, tag, msg, record):
-        '''增加一个记录
+        """增加一个记录
 
         :param level: 日志级别
         :param msg: 日志消息
         :param tag: 日志标签
         :param record: 日志记录信息
         :type level: string
         :type tag: string
         :type msg: string
         :type record: dict
-        '''
+        """
         with self._lock:
             return self._report.log_record(level, tag, msg, record)
 
 
 class ThreadingTestRunner(BaseTestRunner):
-    '''使用多线程并发执行用例
-    '''
+    """使用多线程并发执行用例"""
 
-    def __init__(self, report, thread_cnt=0, retries=0, resmgr_backend=None, execute_type="random"):
-        '''构造函数
+    def __init__(
+        self,
+        report,
+        thread_cnt=0,
+        retries=0,
+        resmgr_backend=None,
+        execute_type="random",
+    ):
+        """构造函数
 
         :param report: 测试报告
         :type report: ITestReport
         :param thread_cnt: 线程数
         :type thread_cnt: int
         :param retries: 用例失败时重试次数
         :type retries: int
-        '''
+        """
         self.concurrency = int(thread_cnt) or multiprocessing.cpu_count()
         self._retries = retries
         self._lock = threading.Lock()
         if self.concurrency > 1:
             report = ThreadSafetyReport(report)
         super(ThreadingTestRunner, self).__init__(report, resmgr_backend, execute_type)
 
     def run_all_tests(self, tests):
-        '''执行全部的测试用例
+        """执行全部的测试用例
 
         :param test: 测试用例对象列表
         :type tests: list
-        '''
+        """
         if self._execute_type == "random":
             random.shuffle(tests)
         tests_queue = collections.deque(tests)
         tests_retry_dict = {}
         threads = []
         for _ in range(self.concurrency):
-            thread = threading.Thread(target=self._run_test_from_queue, args=(tests_queue, tests_retry_dict))
+            thread = threading.Thread(
+                target=self._run_test_from_queue, args=(tests_queue, tests_retry_dict)
+            )
             thread.start()
             threads.append(thread)
         for thread in threads:
             thread.join()
 
     def _run_test_from_queue(self, tests_queue, tests_retry_dict):
-        '''从队列中不断取用例并执行
+        """从队列中不断取用例并执行
 
         :param tests_queue: 测试用例队列
         :type tests_queue: deque
         :param tests_retry_dict: 测试用例重跑记录
         :type tests_retry_dict: dict
-        '''
-        while len(tests_queue) > 0 :
+        """
+        while len(tests_queue) > 0:
             with self._lock:
                 if len(tests_queue) <= 0:
                     break
                 test = tests_queue.pop()
             passed = self.run_test(test)
             with self._lock:
-                if not passed:
-                    tests_retry_dict.setdefault(test, 0)
-                    if tests_retry_dict[test] < self._retries:
-                        tests_retry_dict[test] += 1
-                        tests_queue.append(test)
+                self.handle_result(test=test,
+                                 tests_queue=tests_queue,
+                                 passed=passed,
+                                 tests_retry_dict=tests_retry_dict)
+
 
     @classmethod
     def get_parser(cls):
-        '''获取命令行参数解析器（如果实现）
+        """获取命令行参数解析器（如果实现）
 
         :returns: 解析器对象
         :rtype: argparse.ArgumentParser
-        '''
+        """
         parser = argparse.ArgumentParser(usage=runner_usage)
-        parser.add_argument("--retries", type=int, default=0, help="retry count while test case failed")
-        parser.add_argument("--concurrency", type=int, default=0, help="number of concurrent thread")
+        parser.add_argument(
+            "--retries", type=int, default=0, help="retry count while test case failed"
+        )
+        parser.add_argument(
+            "--concurrency", type=int, default=0, help="number of concurrent thread"
+        )
         return parser
 
     @classmethod
     def parse_args(cls, args_string, report, resmgr_backend, execute_type):
-        '''通过命令行参数构造对象
+        """通过命令行参数构造对象
 
         :returns: 测试报告
         :rtype: cls
-        '''
+        """
         args = cls.get_parser().parse_args(args_string)
         return cls(report, args.concurrency, args.retries, resmgr_backend, execute_type)
 
 
 class EnumProcessMsgType(object):
-    '''多进程间通信用的消息类型
-    '''
+    """多进程间通信用的消息类型"""
+
     Worker_Quit = 0
     Worker_RunTest = 1
     Worker_Idle = 2
     Worker_Error = 3
 
     Result_GetAttr = 4
     Result_AttrValue = 5
@@ -635,267 +705,303 @@
     Result_Raise = 10
 
     Report_LogTestResult = 12
     Report_LogRecord = 13
 
 
 class TestResultFunctionProxy(object):
-    '''测试结果函数代理
-    '''
+    """测试结果函数代理"""
 
     def __init__(self, from_worker, obj_id, func_name):
-        '''构造函数
+        """构造函数
 
         :param from_worker: 所属的工作者
         :type from_worker: TestWorker
         :param obj_id: 对象ID
         :type obj_id: int
         :param func_name: 函数名
         :type func_name: string
-        '''
+        """
         self._worker = from_worker
         self._objid = obj_id
         self._func_name = func_name
 
     def __call__(self, *args, **kwargs):
-        self._worker.send_message((EnumProcessMsgType.Result_CallFunc, self._objid, self._func_name,
-                                   args, kwargs))
+        self._worker.send_message(
+            (
+                EnumProcessMsgType.Result_CallFunc,
+                self._objid,
+                self._func_name,
+                args,
+                kwargs,
+            )
+        )
         msg = self._worker.recv_message(5)
         msg_type = msg[0]
         if msg_type == EnumProcessMsgType.Result_Return:
             return msg[1]
         elif msg_type == EnumProcessMsgType.Result_Raise:
             raise RuntimeError(str(msg[1]))
         else:
             raise RuntimeError("unexpect message: %s" % msg)
 
 
 class TestResultProxy(object):
-    '''测试结果代理
-    '''
+    """测试结果代理"""
 
     def __init__(self, from_worker, obj_id, passed, testcase):
-        '''构造函数
+        """构造函数
 
         :param from_worker: 来源的工作者
         :type from_worker: TestWorker
         :param obj_id: 对象ID
         :type obj_id: int
         :param passed: 测试是否通过
         :type passed: boolean
         :param testcase: 对应测试用例
         :type testcase: TestCase
-        '''
+        """
         self.__worker = from_worker
         self.__passed = passed
         self.__objid = obj_id
         self.__testcase = testcase
 
     def __getattr__(self, name):
-        if name.startswith('_TestResultProxy__'):
+        if name.startswith("_TestResultProxy__"):
             return super(TestResultProxy, self).__getattr__(name)
-        if name == 'passed':  # shortcut
+        if name == "passed":  # shortcut
             return self.__passed
-        if name == 'testcase':
+        if name == "testcase":
             return self.__testcase
-        self.__worker.send_message((EnumProcessMsgType.Result_GetAttr, self.__objid, name))
+        self.__worker.send_message(
+            (EnumProcessMsgType.Result_GetAttr, self.__objid, name)
+        )
         msg = self.__worker.recv_message(5)
         msg_type = msg[0]
         if msg_type == EnumProcessMsgType.Result_AttrValue:
             return msg[1]
         elif msg_type == EnumProcessMsgType.Result_Func:
             return TestResultFunctionProxy(self.__worker, self.__objid, name)
         elif EnumProcessMsgType.Result_AttrError:
             raise AttributeError(msg[1])
         else:
             raise RuntimeError("unexpect message: %s" % msg)
 
     def __setattr__(self, name, value):
-        if name.startswith('_TestResultProxy__'):
+        if name.startswith("_TestResultProxy__"):
             super(TestResultProxy, self).__setattr__(name, value)
         else:
             raise RuntimeError("read only")
 
 
 class TestReportProxy(TestReportBase):
-    '''测试报告代理
-    '''
+    """测试报告代理"""
 
     def __init__(self, worker_id, ctrl_msg_queue, result_factory, result_manager):
-        '''构造函数
+        """构造函数
 
         :param worker_id: 工作者ID
         :type worker_id: string
         :param ctrl_msg_queue: 控制进程的消息队列
         :type ctrl_msg_queue: multiprocessing.Queue
         :param result_factory: 测试结果工厂
         :type result_factory: ITestResultFactory
         :param result_manager: 测试结果残根管理器
         :type result_manager：TestResultStubManager
-        '''
+        """
         super(TestReportProxy, self).__init__()
         self._worker_id = worker_id
         self._ctrl_msg_queue = ctrl_msg_queue
         self._result_factory = result_factory
         self._result_manager = result_manager
 
     def begin_report(self):
-        '''开始测试执行
-        '''
+        """开始测试执行"""
         raise RuntimeError("should not call this")
 
     def end_report(self):
-        '''结束测试执行
+        """结束测试执行
 
         :param passed: 测试是否通过
         :type passed: boolean
-        '''
+        """
         raise RuntimeError("should not call this")
 
     def log_test_result(self, testcase, testresult):
-        '''记录一个测试结果
+        """记录一个测试结果
 
         :param testcase: 测试用例
         :type testcase: TestCase
         :param testresult: 测试结果
         :type testresult: TestResult
-        '''
+        """
         super(TestReportProxy, self).log_test_result(testcase, testresult)
         objid = self._result_manager.add_result(testresult)
-        self._ctrl_msg_queue.put((EnumProcessMsgType.Report_LogTestResult,
-                                  self._worker_id, serialization.dumps(testcase), objid, testresult.passed))
+        self._ctrl_msg_queue.put(
+            (
+                EnumProcessMsgType.Report_LogTestResult,
+                self._worker_id,
+                serialization.dumps(testcase),
+                objid,
+                testresult.passed,
+            )
+        )
 
     def log_record(self, level, tag, msg, record):
-        '''增加一个记录
+        """增加一个记录
 
         :param level: 日志级别
         :param tag: 日志标签
         :param msg: 日志消息
         :param record: 日志记录信息
         :type level: string
         :type tag: string
         :type msg: string
         :type record: dict
-        '''
-        self._ctrl_msg_queue.put((EnumProcessMsgType.Report_LogRecord, (level, tag, msg, record)))
+        """
+        self._ctrl_msg_queue.put(
+            (EnumProcessMsgType.Report_LogRecord, (level, tag, msg, record))
+        )
 
     def get_testresult_factory(self):
-        '''获取对应的TestResult工厂
+        """获取对应的TestResult工厂
 
         :returns: ITestResultFactory
-        '''
+        """
         return self._result_factory
 
 
 class _EmptyClass(object):
     pass
 
 
 class TestResultStubManager(object):
-    '''测试结果桩管理器
-    '''
+    """测试结果桩管理器"""
 
     def __init__(self, rsp_queue):
-        '''构造函数
+        """构造函数
 
         :param rsp_queue: 对工作者请求结果的答复消息队列
         :type rsp_queue:  multiprocessing.Queue
-        '''
+        """
         self._rsp_queue = rsp_queue
         self._result_dict = {}
 
     def add_result(self, result):
-        '''增加一个测试结果
-        '''
+        """增加一个测试结果"""
         self._result_dict[id(result)] = result
         return id(result)
 
     def get_result_attr(self, objid, attrname):
-        '''获取一个测试结果的属性值
+        """获取一个测试结果的属性值
 
         :param objid: 对象ID
         :type objid: int
         :param attrname: 属性名
         :type attrname: string
-        '''
+        """
         result = self._result_dict[objid]
         try:
             attr = getattr(result, attrname)
             if not isinstance(attr, types.MethodType):
                 rsp = EnumProcessMsgType.Result_AttrValue, attr
             else:
-                rsp = EnumProcessMsgType.Result_Func,
+                rsp = (EnumProcessMsgType.Result_Func,)
             self._rsp_queue.put(rsp)
-        except:
-            self._rsp_queue.put((EnumProcessMsgType.Result_AttrError,
-                                 "'%s' object has no attribute '%s'" % (type(result).__name__, attrname)))
+        except Exception:  # pylint: disable=broad-except
+            self._rsp_queue.put(
+                (
+                    EnumProcessMsgType.Result_AttrError,
+                    "'%s' object has no attribute '%s'"
+                    % (type(result).__name__, attrname),
+                )
+            )
 
     def call_result_func(self, objid, funcname, args, kwargs):
-        '''调用一个测试结果的函数
+        """调用一个测试结果的函数
 
         :param objid: 对象ID
         :type objid: int
         :param funcname: 函数名
         :type funcname: string
         :param args: 参数
         :type args: tuple
         :param kwargs: 参数
         :type kwargs: dict
-        '''
+        """
         result = self._result_dict[objid]
         try:
-            rsp = EnumProcessMsgType.Result_Return, getattr(result, funcname)(*args, **kwargs)
-        except:
+            rsp = EnumProcessMsgType.Result_Return, getattr(result, funcname)(
+                *args, **kwargs
+            )
+        except Exception:  # pylint: disable=broad-except
             rsp = EnumProcessMsgType.Result_Raise, traceback.format_exc()
         self._rsp_queue.put(rsp)
 
 
 def _log_collection_result(testreport, result_collection):
-    '''记录结果集合
-    '''
+    """记录结果集合"""
     for it in result_collection:
         if isinstance(it, TestResultCollection):
             _log_collection_result(testreport, it)
         else:
             testreport.log_test_result(it.testcase, it)
 
 
-def _run_test_thread(worker_id, ctrl_msg_queue, testcase, testreport, resmgr, share_data_mgr=None):
-    '''执行测试用例的线程
+def _run_test_thread(
+    worker_id, ctrl_msg_queue, testcase, testreport, resmgr, share_data_mgr=None
+):
+    """执行测试用例的线程
 
     :param worker_id: 工作者ID
     :type worker_id: string
     :param ctrl_msg_queue: 控制进程的消息队列
     :type ctrl_msg_queue: multiprocessing.Queue
     :param testcase: 测试用例
     :type testcase: TestCase
     :param testreport: 测试报告
     :type testreport: ITestReport
     :param resmgr: 资源管理器
     :type resmgr: TestResourceManager
-    '''
+    """
     try:
-        case_runner = getattr(testcase, 'case_runner', TestCaseRunner())
+        case_runner = getattr(testcase, "case_runner", TestCaseRunner())
         testcase.test_resmgr = resmgr
         testcase.share_data_mgr = share_data_mgr
         result = case_runner.run(testcase, testreport.get_testresult_factory())
         if isinstance(result, TestResultCollection):
             _log_collection_result(testreport, result)
         else:
             testreport.log_test_result(result.testcase, result)
 
-        ctrl_msg_queue.put((EnumProcessMsgType.Worker_Idle, worker_id, serialization.dumps(testcase), result.passed))
-    except:
-        ctrl_msg_queue.put((EnumProcessMsgType.Worker_Error, worker_id, traceback.format_exc()))
-
-
-def _worker_process(worker_id,
-                     ctrl_msg_queue, msg_queue, rsp_queue,
-                     result_factory_type, result_factory_data, resmgr, share_data_mgr=None):
-    '''执行测试的子进程过程
+        ctrl_msg_queue.put(
+            (
+                EnumProcessMsgType.Worker_Idle,
+                worker_id,
+                serialization.dumps(testcase),
+                result.passed,
+            )
+        )
+    except Exception:  # pylint: disable=broad-except
+        ctrl_msg_queue.put(
+            (EnumProcessMsgType.Worker_Error, worker_id, traceback.format_exc())
+        )
+
+
+def _worker_process(
+    worker_id,
+    ctrl_msg_queue,
+    msg_queue,
+    rsp_queue,
+    result_factory_type,
+    result_factory_data,
+    resmgr,
+    share_data_mgr=None,
+):
+    """执行测试的子进程过程
 
     :param worker_id: 工作者ID，全局唯一
     :type worker_id: string
     :param ctrl_msg_queue: 控制进程通信的消息队列
     :type ctrl_msg_queue: multiprocessing.Queue
     :param msg_queue: 本进程的消息队列
     :type msg_queue: multiprocessing.Queue
@@ -903,231 +1009,280 @@
     :type rsp_queue:  multiprocessing.Queue
     :param result_factory_type: 测试结果工厂类
     :type result_factory_type: type
     :param result_factory_data: 测试结果工厂序列化后数据
     :type result_factory_data: object
     :param resmgr: 资源管理器
     :type resmgr: TestResourceManager
-    '''
+    """
     try:
         result_factory = _EmptyClass()
         result_factory.__class__ = result_factory_type
         result_factory.loads(result_factory_data)
         result_manager = TestResultStubManager(rsp_queue)
-        report = TestReportProxy(worker_id, ctrl_msg_queue, result_factory, result_manager)
+        report = TestReportProxy(
+            worker_id, ctrl_msg_queue, result_factory, result_manager
+        )
         while True:
             msg = msg_queue.get()
             msg_type = msg[0]
             msg_data = msg[1:]
 
             if msg_type == EnumProcessMsgType.Worker_Quit:
                 break
 
             elif msg_type == EnumProcessMsgType.Worker_RunTest:
                 testcase = serialization.loads(msg_data[0])
-                t = threading.Thread(target=_run_test_thread,
-                                     args=(worker_id, ctrl_msg_queue, testcase, report, resmgr, share_data_mgr))
+                t = threading.Thread(
+                    target=_run_test_thread,
+                    args=(
+                        worker_id,
+                        ctrl_msg_queue,
+                        testcase,
+                        report,
+                        resmgr,
+                        share_data_mgr,
+                    ),
+                )
                 t.daemon = True
                 t.start()
 
             elif msg_type == EnumProcessMsgType.Result_GetAttr:
                 objid, name = msg_data
                 result_manager.get_result_attr(objid, name)
 
             elif msg_type == EnumProcessMsgType.Result_CallFunc:
                 objid, func, args, kwargs = msg_data
                 result_manager.call_result_func(objid, func, args, kwargs)
-    except:
-        ctrl_msg_queue.put((EnumProcessMsgType.Worker_Error, worker_id, traceback.format_exc()))
+    except Exception:  # pylint: disable=broad-except
+        ctrl_msg_queue.put(
+            (EnumProcessMsgType.Worker_Error, worker_id, traceback.format_exc())
+        )
 
 
 class TestWorker(object):
-    '''多进程执行用例时，执行测试的子进程
-    '''
+    """多进程执行用例时，执行测试的子进程"""
 
-    def __init__(self, worker_id, ctrl_msg_queue, result_factory, resmgr, share_data_mgr=None):
-        '''构造函数
+    def __init__(
+        self, worker_id, ctrl_msg_queue, result_factory, resmgr, share_data_mgr=None
+    ):
+        """构造函数
 
         :param worker_id: 工作者ID，全局唯一
         :type worker_id: string
         :param ctrl_msg_queue: 控制进程的消息队列
         :type msg_queue: multiprocessing.Queue
         :param result_factory: 测试结果工厂
         :type result_factory: ITestResultFactory
         :param resmgr: 资源管理器
         :type resmgr: TestResourceManager
-        '''
+        """
         self._worker_id = worker_id
         self._result_factory = result_factory
         self._ctrl_msg_queue = ctrl_msg_queue
         self._resmgr = resmgr
         self._share_data_mgr = share_data_mgr
         self._reset()
 
     def _reset(self):
-        '''重置内部状态
-        '''
+        """重置内部状态"""
         self._rsp_queue = multiprocessing.Queue()
         self._msg_queue = multiprocessing.Queue()
-        self._process = multiprocessing.Process(target=_worker_process,
-                                                args=(self._worker_id,
-                                                      self._ctrl_msg_queue,
-                                                      self._msg_queue,
-                                                      self._rsp_queue,
-                                                      type(self._result_factory),
-                                                      self._result_factory.dumps(),
-                                                      self._resmgr,
-                                                      self._share_data_mgr))
+        self._process = multiprocessing.Process(
+            target=_worker_process,
+            args=(
+                self._worker_id,
+                self._ctrl_msg_queue,
+                self._msg_queue,
+                self._rsp_queue,
+                type(self._result_factory),
+                self._result_factory.dumps(),
+                self._resmgr,
+                self._share_data_mgr,
+            ),
+        )
         self._monitor = threading.Thread(target=self._process_monitor)
         self._monitor.daemon = True
         self._testcase = None
         self._stopping = False
 
     def _process_monitor(self):
-        '''监控线程
-        '''
+        """监控线程"""
         self._process.join()
         if not self._stopping:
-            self._ctrl_msg_queue.put((EnumProcessMsgType.Worker_Error, self._worker_id, 'process exit unexpectedly'))
+            self._ctrl_msg_queue.put(
+                (
+                    EnumProcessMsgType.Worker_Error,
+                    self._worker_id,
+                    "process exit unexpectedly",
+                )
+            )
 
     def start(self):
-        '''开始执行
-        '''
+        """开始执行"""
         self._process.start()
         self._monitor.start()
 
     def stop(self):
-        '''结束执行
-        '''
+        """结束执行"""
         self._stopping = True
         self.send_message((EnumProcessMsgType.Worker_Quit,))
         self._process.join(5)
         if self._process.is_alive():
             self._process.terminate()
 
     def restart(self):
-        '''重新开始执行
-        '''
+        """重新开始执行"""
         self._reset()
         self.start()
 
     def run_testcase(self, testcase):
-        '''分配一个测试用例
+        """分配一个测试用例
 
         :param testcase: 要执行的测试用例
         :type testcase: TestCase
-        '''
-        self.send_message((EnumProcessMsgType.Worker_RunTest, serialization.dumps(testcase)))
+        """
+        self.send_message(
+            (EnumProcessMsgType.Worker_RunTest, serialization.dumps(testcase))
+        )
         self._testcase = testcase
 
     def current_testcase(self):
-        '''当前正在执行的测试用例
+        """当前正在执行的测试用例
 
         :returns: TestCase
-        '''
+        """
         return self._testcase
 
     def send_message(self, msg):
-        '''发送消息到工作者
+        """发送消息到工作者
 
         :param msg: 消息
         :type msg: tuple
-        '''
+        """
         self._msg_queue.put(msg)
 
     def recv_message(self, timeout=None):
-        '''接收工作者的答复消息
-        '''
+        """接收工作者的答复消息"""
         if timeout is None:
             return self._rsp_queue.get()
         else:
             try:
                 return self._rsp_queue.get(timeout=timeout)
             except queue.Empty:
                 raise RuntimeError("waiting response message from worker timeout")
 
 
 class MultiProcessTestRunner(BaseTestRunner):
-    '''使用多进程并发执行用例
+    """使用多进程并发执行用例
 
     多进程并发时，有两个特殊的问题需要处理：
 
     1、测试执行工作进程需要通知TestReport测试用例的执行情况等，
     解决方案是：
     为每个工作进程提供一个TestReportProxy，TestReportProxy通过消息机制通知
     真正的TestReport
 
     2、TestReport需要访问在工作进程的TestResult对象，
     解决方案是：
     每个工作进程有一个TestResultStubManager，提供给TestReport的是一个TestResultProxy
     对象，TestResultProxy通过消息机制和TestResultStubManager通信，来获取真正的TestResult
     的信息
 
-    '''
+    """
 
-    def __init__(self, report, process_cnt=0, retries=0, resmgr_backend=None, execute_type="random"):
-        '''构造函数
+    def __init__(
+        self,
+        report,
+        process_cnt=0,
+        retries=0,
+        resmgr_backend=None,
+        execute_type="random",
+    ):
+        """构造函数
 
         :param report: 测试报告
         :type report: ITestReport
         :param process_cnt: 进程数
         :type process_cnt: int
         :param retries: 失败重跑次数上限
         :type retries: int
-        '''
+        """
         self.concurrency = int(process_cnt) or multiprocessing.cpu_count()
         self._retries = retries
         self._workers_dict = {}
-        super(MultiProcessTestRunner, self).__init__(report, resmgr_backend, execute_type)
-
-        self._share_data_mgr = ShareDataManager(lock=multiprocessing.Lock(), data=multiprocessing.Manager().dict())
+        super(MultiProcessTestRunner, self).__init__(
+            report, resmgr_backend, execute_type
+        )
+
+        self._share_data_mgr = ShareDataManager(
+            lock=multiprocessing.Lock(), data=multiprocessing.Manager().dict()
+        )
 
     def run_all_tests(self, tests):
-        '''执行全部的测试用例
+        """执行全部的测试用例
 
         :param test: 测试用例对象列表
         :type tests: list
-        '''
+        """
         if len(tests) == 0:
             return
         if len(tests) < self.concurrency:
             self.concurrency = len(tests)
 
         if self._execute_type == "random":
             random.shuffle(tests)
         tests_queue = collections.deque(tests)
         tests_retry_dict = {}
         msg_queue = multiprocessing.Queue()
         result_factory = self.report.get_testresult_factory()
         for i in range(self.concurrency):
-            worker = TestWorker(i, msg_queue, result_factory, self._resmgr, self._share_data_mgr)
+            worker = TestWorker(
+                i, msg_queue, result_factory, self._resmgr, self._share_data_mgr
+            )
             worker.start()
             worker.run_testcase(tests_queue.popleft())
             self._workers_dict[i] = worker
 
         idle_workers = []
         error_counts = {}
         while True:
             msg = msg_queue.get()
             msg_type = msg[0]
 
             if msg_type == EnumProcessMsgType.Report_LogTestResult:
                 worker = self._workers_dict[msg[1]]
                 testcase = serialization.loads(msg[2])
                 objid, passed = msg[3], msg[4]
-                self.report.log_test_result(testcase, TestResultProxy(worker, objid, passed, testcase))
+                self.report.log_test_result(
+                    testcase, TestResultProxy(worker, objid, passed, testcase)
+                )
 
             elif msg_type == EnumProcessMsgType.Report_LogRecord:
                 self.report.log_record(msg[1], msg[2], msg[3], msg[4])
 
             elif msg_type == EnumProcessMsgType.Worker_Idle:
                 worker = self._workers_dict[msg[1]]
                 test = serialization.loads(msg[2])
                 passed = msg[3]
                 if not passed:
+                    if self.stop:   # 如果当前有用例执行失败，配置了stop_on_failure时，停止测试
+                        for index in list(self._workers_dict.keys())[::-1]:
+                            _worker = self._workers_dict[index]
+                            current_case = _worker.current_testcase()
+                            if worker != _worker:
+                                self._not_run.append(current_case)
+                                self._error_msg = "some testcase failed, stop on failure."  # 其它进程的用例也进入not_run list
+                        if len(tests_queue) <= 0:
+                            return
+                        while len(tests_queue) > 0:
+                            testcase = tests_queue.popleft()
+                            self._error_msg = "some testcase failed, stop on failure."
+                            self._not_run.append(testcase)
+                        return
                     tests_retry_dict.setdefault(test.test_name, 0)
                     if tests_retry_dict[test.test_name] < self._retries:
                         tests_retry_dict[test.test_name] += 1
                         tests_queue.append(test)
 
                 if len(tests_queue) > 0:
                     worker.run_testcase(tests_queue.popleft())
@@ -1137,18 +1292,25 @@
                         break
 
             elif msg_type == EnumProcessMsgType.Worker_Error:
                 if msg[1] not in self._workers_dict:
                     continue
                 worker = self._workers_dict[msg[1]]
                 err_msg = msg[2]
-                self.report.error('RUNNER', 'runner process %s error occurred: %s' % (msg[1], err_msg), record=dict(err_msg=err_msg))
+                self.report.error(
+                    "RUNNER",
+                    "runner process %s error occurred: %s" % (msg[1], err_msg),
+                    record=dict(err_msg=err_msg),
+                )
                 error_count = error_counts.get(msg[1], 0)
                 if error_count >= 4:
-                    self.report.error('RUNNER', 'worker with id=%s failed to run for up 3 times' % msg[1])
+                    self.report.error(
+                        "RUNNER",
+                        "worker with id=%s failed to run for up 3 times" % msg[1],
+                    )
                     worker.stop()
                     del self._workers_dict[msg[1]]
                     if len(idle_workers) == len(self._workers_dict):
                         break
                 else:
                     error_counts[msg[1]] = error_count + 1
                     if worker not in idle_workers:
@@ -1159,26 +1321,30 @@
     def clean_up(self):
         BaseTestRunner.clean_up(self)
         for it in self._workers_dict.values():
             it.stop()
 
     @classmethod
     def get_parser(cls):
-        '''获取命令行参数解析器（如果实现）
+        """获取命令行参数解析器（如果实现）
 
         :returns: 解析器对象
         :rtype: argparse.ArgumentParser
-        '''
+        """
         parser = argparse.ArgumentParser(usage=runner_usage)
-        parser.add_argument("--retries", type=int, default=0, help="retry count while test case failed")
-        parser.add_argument("--concurrency", type=int, default=0, help="number of concurrent thread")
+        parser.add_argument(
+            "--retries", type=int, default=0, help="retry count while test case failed"
+        )
+        parser.add_argument(
+            "--concurrency", type=int, default=0, help="number of concurrent thread"
+        )
         return parser
 
     @classmethod
     def parse_args(cls, args_string, report, resmgr_backend, execute_type):
-        '''通过命令行参数构造对象
+        """通过命令行参数构造对象
 
         :returns: 测试报告
         :rtype: cls
-        '''
+        """
         args = cls.get_parser().parse_args(args_string)
         return cls(report, args.concurrency, args.retries, resmgr_backend, execute_type)
```

### Comparing `qtaf-5.5.9/testbase/serialization.py` & `qtaf-5.6.0/testbase/serialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,67 +8,64 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 测试用例序列化和反序列化
-'''
+"""
 
 import sys
 import pickle
-from testbase.testcase import TestSuite
+from testbase.testsuite import TestSuiteBase
 
 
 class _EmptyClass(object):
     pass
 
 
 def dumps(testcase):
     """序列化测试用例
-    
+
     :param testcase: 测试用例
     :type testcase: TestCase
     """
-    if isinstance(testcase, TestSuite):
-        return {
-            'id': testcase.suite_class_name,
-            'data': pickle.dumps(testcase.dumps())
-        }
+    if isinstance(testcase, TestSuiteBase):
+        return {"id": testcase.suite_class_name, "data": pickle.dumps(testcase.dumps())}
     else:
         return {
-            'id': testcase.test_class_name,
-            'data': pickle.dumps(testcase.casedata),
-            'dname': testcase.casedataname,
+            "id": testcase.test_class_name,
+            "data": pickle.dumps(testcase.casedata),
+            "dname": testcase.casedataname,
         }
 
 
 def loads(buf):
     """反序列化测试用例
-    
+
     :param buf: 测试用例序列化数据
     :type buf: dict
     :returns: TestCase
     """
-    testname = buf['id']
-    items = testname.split('.')
+    testname = buf["id"]
+    items = testname.split(".")
     classname = items[-1]
-    modulename = '.'.join(items[0:-1])
+    modulename = ".".join(items[0:-1])
     if not modulename:  # main module
         modulename = "__main__"
     else:
         __import__(modulename)
     module = sys.modules[modulename]
     testclass = getattr(module, classname)
-    data = pickle.loads(buf['data'])
-    if issubclass(testclass, TestSuite):
+    data = pickle.loads(buf["data"])
+    if issubclass(testclass, TestSuiteBase):
         obj = _EmptyClass()
         obj.__class__ = testclass
         obj.loads(data)
         return obj
     else:
         attrs = None
         if isinstance(data, dict) and "__attrs__" in data:
             attrs = data.get("__attrs__")
-        return testclass(data, buf['dname'], attrs)
+        return testclass(data, buf["dname"], attrs)
```

### Comparing `qtaf-5.5.9/testbase/test.py` & `qtaf-5.6.0/testbase/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 from testbase.conf import settings
 
 
 class _NotExistedItem(object):
     pass
 
 
-class modify_settings(object):
-    """temporarily modify settings
-    """
+class modify_settings(object):  # pylint: disable=invalid-name
+    """temporarily modify settings"""
 
     def __init__(self, **kwargs):
         self.new_conf = kwargs
         self.old_conf = {}
 
     def __enter__(self):
         settings._Settings__ensure_loaded()  # ensure loaded
@@ -48,17 +47,16 @@
                 delattr(settings, key)
                 settings._Settings__keys.remove(key)
             else:
                 setattr(settings, key, old_value)
         settings._Settings__sealed = True
 
 
-class modify_environ(object):
-    """temporarily modify envrion
-    """
+class modify_environ(object):  # pylint: disable=invalid-name
+    """temporarily modify envrion"""
 
     def __init__(self, **kwargs):
         self.new_conf = kwargs
         self.old_conf = {}
 
     def __enter__(self):
         for key in self.new_conf:
@@ -70,17 +68,17 @@
             old_value = self.old_conf[key]
             if isinstance(old_value, _NotExistedItem):
                 del os.environ[key]
             else:
                 os.environ[key] = old_value
 
 
-class modify_attributes(object):
-    """temporarily modify attributes
-    """
+class modify_attributes(object):  # pylint: disable=invalid-name
+    """temporarily modify attributes"""
+
     _lock = threading.Lock()
 
     def __init__(self, target, key_values):
         self._target = target
         self._old_values = {}
         self._new_values = key_values
         for key in key_values.keys():
```

### Comparing `qtaf-5.5.9/testbase/testcase.py` & `qtaf-5.6.0/testbase/testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,110 +8,124 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 测试用例基类模块
-'''
+"""
 from __future__ import absolute_import
 
+import inspect
 import os
 import sys
 import json
 import re
 import threading
 import traceback
 import collections
 import types
 import six
 
 from testbase.assertion import AssertionRewriter
-from testbase.util import Singleton, ThreadGroupLocal, ThreadGroupScope, smart_text, get_last_frame_stack, getmembers
+from testbase.util import (
+    Singleton,
+    ThreadGroupLocal,
+    ThreadGroupScope,
+    smart_text,
+    get_last_frame_stack,
+    getmembers,
+)
 from testbase.testresult import EnumLogLevel, TestResultCollection, TestResultType
 from testbase.conf import settings
 from testbase.retry import Retry
 
 
 class BaseTestCaseException(Exception):
     pass
 
 
 # 后续需专门花时间去除TestCaseStatus和TestCasePriority这两个类
 class TestCaseStatus(object):
-    '''测试用例状态
+    """测试用例状态
 
     :attention: 此类将会被移除，请使用TestCase.EnumStatus
-    '''
-    Design, Implement, Review, Ready, Suspend = ('Design', 'Implement', 'Review', 'Ready', 'Suspend')
+    """
+
+    Design, Implement, Review, Ready, Suspend = (
+        "Design",
+        "Implement",
+        "Review",
+        "Ready",
+        "Suspend",
+    )
 
 
 class TestCasePriority(object):
-    '''测试用例优先级
+    """测试用例优先级
 
     :attention: 此类将会被移除，请使用TestCase.EnumPriority
-    '''
-    BVT, High, Normal, Low = ('BVT', 'High', 'Normal', 'Low')
+    """
+
+    BVT, High, Normal, Low = ("BVT", "High", "Normal", "Low")
 
 
 class Environ(six.with_metaclass(Singleton, dict)):
     """测试环境类
 
-用法说明：
-它是一个继承了字典类型的单实例类。使用时，需先实例化该类，如：
-from testbase.testcase import Environ
-env = Environ()
-env保存了用例运行时的一些测试环境变量。
+    用法说明：
+    它是一个继承了字典类型的单实例类。使用时，需先实例化该类，如：
+    from testbase.testcase import Environ
+    env = Environ()
+    env保存了用例运行时的一些测试环境变量。
 
-测试环境变量分为3个部分：
+    测试环境变量分为3个部分：
 
-1、在测试执行时，env则存储了由测试计划定义的用例环境变量，使用方法如下::
+    1、在测试执行时，env则存储了由测试计划定义的用例环境变量，使用方法如下::
 
-    from testbase.testcase import Environ
-    env = Environ()
-    print(env_
-    # 输出
-    env = {
-        'ASSERTTEST':'True',  #注意：这里key是全字母大写
-    }
-
-2、测试用例基类testbase.testcase.TestCase的构造函数中也实例化了Environ类（变量名为environ)，
-并且，保存了当时执行用例类的类名和类说明，使用方法如下::
-
-    #todo: 执行用例中使用evniron，用于打印用例名称和用例说明
-    from testbase.testcase import TestCase
-    class YourTest(TestCase):
-        def runTest(self):
-            print(self.environ['TestName'])
-            print(self.environ['TestDoc'])
+        from testbase.testcase import Environ
+        env = Environ()
+        print(env_
+        # 输出
+        env = {
+            'ASSERTTEST':'True',  #注意：这里key是全字母大写
+        }
 
-3、Environ还可以用于设置自定义的环境变量，使用方法如下::
+    2、测试用例基类testbase.testcase.TestCase的构造函数中也实例化了Environ类（变量名为environ)，
+    并且，保存了当时执行用例类的类名和类说明，使用方法如下::
 
-    from testbase.testcase import Environ
-    env = Environ()
-    env['YourEnvKey'] = "EnvValue"
-    print(env['YourEnvKey'])
+        #todo: 执行用例中使用evniron，用于打印用例名称和用例说明
+        from testbase.testcase import TestCase
+        class YourTest(TestCase):
+            def runTest(self):
+                print(self.environ['TestName'])
+                print(self.environ['TestDoc'])
+
+    3、Environ还可以用于设置自定义的环境变量，使用方法如下::
+
+        from testbase.testcase import Environ
+        env = Environ()
+        env['YourEnvKey'] = "EnvValue"
+        print(env['YourEnvKey'])
 
     """
 
     def __init__(self):
-        """构造函数。判断系统环境变量中是否存在由测试计划中传入的环境变量，有则加载。
-
-        """
+        """构造函数。判断系统环境变量中是否存在由测试计划中传入的环境变量，有则加载。"""
         super(Environ, self).__init__()
         for key in os.environ.keys():
             if key.startswith("QTAF_") and key[5:]:
                 self[key[5:]] = os.environ[key]
 
 
 class TestCaseType(type):
-    '''测试用例元类型
-    '''
+    """测试用例元类型"""
+
     forbid_overload_methods = ["__init__"]
 
     def __new__(cls, name, bases, attrs):
         super_new = super(TestCaseType, cls).__new__
         parents = [b for b in bases if isinstance(b, TestCaseType)]
         # ensure only apply for subclass of TestCase
         if not parents:
@@ -141,69 +155,90 @@
         attrs["tags"] = tags_set
         attrs["base_tags"] = base_tags_set
         return super_new(cls, name, bases, attrs)
 
 
 @six.add_metaclass(TestCaseType)
 class TestCase(object):
-    '''测试用例基类
+    """测试用例基类
+
+     所有测试用例都最终从此基类继承。测试用例的测试脚本主要实现在"runTest()"中，
 
-            所有测试用例都最终从此基类继承。测试用例的测试脚本主要实现在"runTest()"中，
+    而当用例需要初始化和清理测试环境时则分别重写"preTest()"和"postTest()"函数。
+    """
 
-           而当用例需要初始化和清理测试环境时则分别重写"preTest()"和"postTest()"函数。
-    '''
     test_extra_info_def = []  # 自定义字段
 
     class EnumStatus(object):
-        '''测试用例状态枚举类
+        """测试用例状态枚举类
 
         :attention: 如果因为特殊原因需要暂时屏蔽某个用例的任务执行（比如有功能缺陷从而导致执行失败），
                                                      则可以先置为该字段为Suspend,等到可用的时候再将该字段置为Ready
 
-        '''
-        Design, Implement, Review, Ready, Suspend = (TestCaseStatus.Design,
-                                                     TestCaseStatus.Implement,
-                                                     TestCaseStatus.Review,
-                                                     TestCaseStatus.Ready,
-                                                     TestCaseStatus.Suspend)
+        """
+
+        Design, Implement, Review, Ready, Suspend = (
+            TestCaseStatus.Design,
+            TestCaseStatus.Implement,
+            TestCaseStatus.Review,
+            TestCaseStatus.Ready,
+            TestCaseStatus.Suspend,
+        )
 
     class EnumPriority(object):
-        '''测试用例优先级枚举类
-        '''
-        BVT, High, Normal, Low = (TestCasePriority.BVT,
-                                  TestCasePriority.High,
-                                  TestCasePriority.Normal,
-                                  TestCasePriority.Low)
+        """测试用例优先级枚举类"""
+
+        BVT, High, Normal, Low = (
+            TestCasePriority.BVT,
+            TestCasePriority.High,
+            TestCasePriority.Normal,
+            TestCasePriority.Low,
+        )
 
     owner = None
     priority = None
     status = None
     timeout = None
 
-    ATTRIB_OVERWRITE_WHITELIST = ["priority", "status", "owner", "timeout", "tags", "__doc__"]
-    EXTRA_PROPERTY_BLACKLIST = ["start_time", "end_time", "begintime", "endtime", "duration"]
+    ATTRIB_OVERWRITE_WHITELIST = [
+        "priority",
+        "status",
+        "owner",
+        "timeout",
+        "tags",
+        "__doc__",
+    ]
+    EXTRA_PROPERTY_BLACKLIST = [
+        "start_time",
+        "end_time",
+        "begintime",
+        "endtime",
+        "duration",
+        "name",
+    ]
 
     def __init__(self, testdata=None, testdataname=None, attrs=None):
-        '''构造函数
+        """构造函数
 
         :param testdata: 测试数据
         :type testdata: object
         :param testdataname: 测试数据标识
         :type testdataname: str
         :param attrs: 重载的测试用例属性
         :type attrs: dict
-        '''
+        """
         self.__casedata = testdata
         self.__testdataname = testdataname
         self.__environ = Environ()
         self.__testresult = None
         self.__resmgr_session = None
         self.__resmgr = None
         self.__share_data_mgr = None
         self.__test_doc = None
+        self.__current_stage = None
 
         # 参数相关
         self.__params_definitions = {}  # add_params原始的用例参数数据
         self.__params = {}  # key，name的用例参数数据
         self.__dynamic_params = {}  # 外部传入的参数数据
 
         if attrs:
@@ -220,124 +255,120 @@
                 else:
                     self.__dynamic_params[k] = v
 
         self.handle_params()
 
     @property
     def casedata(self):
-        '''测试数据
+        """测试数据
 
         :rtype: list
-        '''
+        """
         return self.__casedata
 
     @property
     def casedataname(self):
-        '''测试数据标识
+        """测试数据标识
 
         :rtype: str
-        '''
+        """
         return self.__testdataname
 
     @property
     def environ(self):
-        '''环境变量
+        """环境变量
 
         :rtype: Environ
-        '''
+        """
         return self.__environ
 
     @property
     def test_result(self):
-        '''对应的测试结果
+        """对应的测试结果
 
         :rtype: TestResult
-        '''
+        """
         return self.__testresult
 
     @property
     def test_dir(self):
-        '''测试用例执行的临时目录
+        """测试用例执行的临时目录
 
         :rtype: str
-        '''
+        """
         return os.path.abspath(os.getcwd())
 
     @property
     def test_class_name(self):
-        '''返回测试用例名字（不同测试用例的名字不同）
+        """返回测试用例名字（不同测试用例的名字不同）
 
         :rtype: str
-        '''
+        """
         cls = type(self)
-        if cls.__module__ == '__main__':
+        if cls.__module__ == "__main__":
             type_name = smart_text(cls.__name__)
         else:
-            type_name = smart_text(cls.__module__ + '.' + cls.__name__)
+            type_name = smart_text(cls.__module__ + "." + cls.__name__)
         return type_name
 
     @property
     def test_name(self):
-        '''返回测试用例实例的名字
+        """返回测试用例实例的名字
 
         :rtype: str
-        '''
+        """
         if self.casedataname is not None:
             casedataname = smart_text(self.casedataname)
-            return '%s/%s' % (self.test_class_name, casedataname)
+            return "%s/%s" % (self.test_class_name, casedataname)
         else:
             return self.test_class_name
 
     @property
     def test_doc(self):
-        '''测试用例说明
+        """测试用例说明
 
         :rtype: str
-        '''
+        """
         if self.__test_doc:
             return self.__test_doc
         desc = self.__class__.__doc__
-#        if desc:
-#            desc = cgi.escape(desc)
+        #        if desc:
+        #            desc = cgi.escape(desc)
         if isinstance(desc, six.text_type):
-            desc = re.sub('^\s*', '', desc)
-            desc = re.sub('\s*$', '', desc)
+            desc = re.sub("^\s*", "", desc)
+            desc = re.sub("\s*$", "", desc)
         return desc
 
     @property
     def test_extra_info(self):
-        '''测试用例额外信息
-        '''
+        """测试用例额外信息"""
         info = {}
         for name, _ in self.test_extra_info_def:
             info[name] = getattr(self, name, None)
         return info
 
     @property
     def test_resmgr(self):
-        '''资源管理器
-        '''
+        """资源管理器"""
         return self.__resmgr
 
     @test_resmgr.setter
     def test_resmgr(self, resmgr):
         self.__resmgr = resmgr
 
     @property
     def test_resources(self):
-        '''资源管理使用接口
-        '''
+        """资源管理使用接口"""
         if not self.__resmgr_session:
             self.__resmgr_session = self.__resmgr.create_session(self)
         return self.__resmgr_session
 
     @property
     def share_data_mgr(self):
-        '''共享数据管理器
-        '''
+        """共享数据管理器"""
         return self.__share_data_mgr
 
     @share_data_mgr.setter
     def share_data_mgr(self, share_data_mgr):
         self.__share_data_mgr = share_data_mgr
 
     @property
@@ -348,173 +379,211 @@
     def qtaf_params(self):
         return self.__params
 
     @property
     def dynamic_params(self):
         return self.__dynamic_params
 
+    @property
+    def current_stage(self):
+        return self.__current_stage
+
+    @current_stage.setter
+    def current_stage(self, current_stage):
+        self.__current_stage = current_stage
+
     def get_test_extra_properties(self):
         var_dicts = {}
         for k, v in getmembers(self):
             if k in self.ATTRIB_OVERWRITE_WHITELIST:
                 continue
             if k in self.EXTRA_PROPERTY_BLACKLIST:
                 continue
-            if not (isinstance(v, bool) or isinstance(v, int) or isinstance(v, float) or isinstance(v, (six.string_types, six.binary_type))):
+            if not (
+                isinstance(v, bool)
+                or isinstance(v, int)
+                or isinstance(v, float)
+                or isinstance(v, (six.string_types, six.binary_type))
+            ):
                 continue
-            if k.islower() and not k.startswith('_') and not k.startswith('test_'):
+            if k.islower() and not k.startswith("_") and not k.startswith("test_"):
                 if isinstance(v, (six.string_types, six.binary_type)):
                     v = smart_text(v)
                 var_dicts[k] = v
         return var_dicts
 
     def add_share_data(self, name, value, level=0):
-        '''添加共享数据
+        """添加共享数据
 
         :type name: string
         :param name: 需要共享的数据名称
         :param value: 需要共享的数据内容
-        '''
+        """
         if self.share_data_mgr:
             self.share_data_mgr.set(name, value, level)
 
     def get_share_data(self, name):
-        '''从内存中获取存储的全局数据，给当前用例使用'''
+        """从内存中获取存储的全局数据，给当前用例使用"""
         if self.share_data_mgr:
             return self.share_data_mgr.get(name)
 
     def remove_share_data(self, name):
-        '''从内存中移除存储的共享数据'''
+        """从内存中移除存储的共享数据"""
         if self.share_data_mgr:
             return self.share_data_mgr.remove(name)
 
     def add_parameters(self):
         # 用例重写或者不重写
         self.add_params()
 
-    def add_parameter(self, name, type=str, optional=False, default=None, description='', validation=None,
-                      rewrite=False, **kwargs):
+    def add_parameter(
+        self,
+        name,
+        type=str,
+        optional=False,
+        default=None,
+        description="",
+        validation=None,
+        rewrite=False,
+        **kwargs
+    ):
         if type not in (bool, list, str, int, float, dict, "json"):
-            raise BaseTestCaseException('Unsupported type of parameter.')
+            raise BaseTestCaseException("Unsupported type of parameter.")
 
         if rewrite is False:  # 如果不能重写，需要判断是否存在
-            assert name not in self.params_definitions, \
-                'Parameters with the same name "{}" were found.'.format(name)
+            assert (
+                name not in self.params_definitions
+            ), 'Parameters with the same name "{}" were found.'.format(name)
 
         if not optional and default is None:
-            raise BaseTestCaseException("Parameter {} must define default value".format(name))
+            raise BaseTestCaseException(
+                "Parameter {} must define default value".format(name)
+            )
 
         self.__params_definitions[name] = {
-            'name': name,
-            'type': type,
-            'optional': optional,
-            'default': default,
-            'description': description,
-            'validation': validation,
-            'kwargs': kwargs
+            "name": name,
+            "type": type,
+            "optional": optional,
+            "default": default,
+            "description": description,
+            "validation": validation,
+            "kwargs": kwargs,
         }
 
     def add_params(self):
         # 用例重写
         pass
 
     add_param = add_parameter
 
     def assert_types(self):
-        '''参数校验并设置self.qtaf_params
-        '''
+        """参数校验并设置self.qtaf_params"""
         errors = []
         for d_name in self.params_definitions:
             default = self.params_definitions[d_name]["default"]
-            define_type = self.params_definitions[d_name]['type']
-            optional = self.params_definitions[d_name]['optional']
+            define_type = self.params_definitions[d_name]["type"]
+            optional = self.params_definitions[d_name]["optional"]
             for c_name in self.dynamic_params:
                 c_name = smart_text(c_name)
                 if c_name == d_name:
                     # 如果有外部传入，直接进行参数类型检查，检查正确设置参数否则记录异常
                     value = self.dynamic_params[c_name]
                     if optional and value is None and default is None:
                         self.__params[c_name] = value
                         break
                     if isinstance(value, six.text_type):
                         value = smart_text(value)
-                    if self.params_definitions[d_name]['type'] == "json":
+                    if self.params_definitions[d_name]["type"] == "json":
                         # json单独处理
                         try:
                             value = json.loads(self.dynamic_params[c_name])
                             self.__params[c_name] = value
-                        except Exception:
-                            errors.append("Parameter:{}, value:{}, is not json type.".format(c_name, value))
+                        except Exception:  # pylint: disable=broad-except
+                            errors.append(
+                                "Parameter:{}, value:{}, is not json type.".format(
+                                    c_name, value
+                                )
+                            )
                     else:
                         if not isinstance(value, define_type):
                             # 如果期望类型是float，int型的数据, 转换为字符串，判断是否是数值型数据，如果是强制转换为数值型数据
                             ret = self.translate2type(define_type, value)
                             if ret is not None:
                                 self.__params[c_name] = ret
                             else:
                                 errors.append(
-                                    "Parameter:{}, value:{}, type {} is not:{} type.".format(c_name,
-                                                                                             value,
-                                                                                             type(value),
-                                                                                             str(define_type)))
+                                    "Parameter:{}, value:{}, type {} is not:{} type.".format(
+                                        c_name, value, type(value), str(define_type)
+                                    )
+                                )
                         else:
                             self.__params[c_name] = value
                     break
             else:
                 # 如果外部未传入使用默认参数
                 if default is not None:
                     if define_type == "json":
                         # json单独处理
                         try:
                             value = json.loads(default)
                             default = value
                         except Exception:
-                            raise BaseTestCaseException("Parameter {}, value {}, is not json type.".format(d_name,
-                                                                                                           default))
+                            raise BaseTestCaseException(
+                                "Parameter {}, value {}, is not json type.".format(
+                                    d_name, default
+                                )
+                            )
                     else:
                         if not isinstance(default, define_type):
                             raise BaseTestCaseException(
-                                "Parameter {}, value {}, is not {} type.".format(d_name, default,
-                                                                                 repr(define_type.__name__)))
+                                "Parameter {}, value {}, is not {} type.".format(
+                                    d_name, default, repr(define_type.__name__)
+                                )
+                            )
                 self.__params[d_name] = default
 
         # validation检查
         for d_name in self.params_definitions:
-            validation = self.params_definitions[d_name]['validation']
-            kwargs = self.params_definitions[d_name]['kwargs']
-            default = self.params_definitions[d_name]['default']
+            validation = self.params_definitions[d_name]["validation"]
+            kwargs = self.params_definitions[d_name]["kwargs"]
+            default = self.params_definitions[d_name]["default"]
             if kwargs is None:
                 kwargs = {}
             if not isinstance(kwargs, dict):
-                errors.append("Parameter:{}, param(kwargs) must be dict.".format(d_name))
+                errors.append(
+                    "Parameter:{}, param(kwargs) must be dict.".format(d_name)
+                )
             if d_name not in self.qtaf_params:
                 value = default
                 # 如果是default就不进行校验
             else:
                 value = self.qtaf_params[d_name]
 
             if value == default:  # 如果值与default相等就不进行校验
                 continue
             # 否则进行校验
             if validation is not None and callable(validation):
                 try:
                     validation(value, self.qtaf_params, **kwargs)
-                except Exception as exe:
+                except Exception as exe:  # pylint: disable=broad-except
                     errors.append(
-                        "Parameter:{}, value:{}, validation error, detail: {}.".format(d_name, value, str(exe)))
+                        "Parameter:{}, value:{}, validation error, detail: {}.".format(
+                            d_name, value, str(exe)
+                        )
+                    )
         if errors:  # 如果参数校验失败抛出异常
             raise BaseTestCaseException("\n".join(errors))
 
     def handle_params(self):
-        '''
+        """
         加载并设置参数,用例中可重写加载方法方式; 并显示的调用以适配不支持参数传递的方式
         正常模式：不设置参数
         设置数据驱动参数：只设置数据驱动参数
         设置全部参数：如果传入参数，以传入参数为准，否则设置数据驱动参数
-        '''
+        """
         # 通过参数控制是否进行参数传递
         param_mode = settings.get("QTAF_PARAM_MODE", False)
         if not param_mode:
             param_mode = settings.get("QC_PARAM_MODE", False)
 
         if not param_mode:  # 正常模式
             return
@@ -535,95 +604,95 @@
             return
         for key, value in temp_data.items():
             if not isinstance(key, six.string_types):
                 continue
             setattr(self, str(key), value)
 
     def init_test(self, testresult):
-        '''初始化测试用例。慎用此函数，尽量将初始化放到preTest里。
+        """初始化测试用例。慎用此函数，尽量将初始化放到preTest里。
 
         :param testresult: 测试结果
         :type testresult: TestResult
-        '''
+        """
         self.__testresult = testresult
 
     def pre_test(self):
-        '''测试环境初始化
-        '''
+        """测试环境初始化"""
         pass
 
     def run_test(self):
-        '''运行测试用例
-        '''
+        """运行测试用例"""
         raise NotImplementedError("请在%s类中实现runTest方法" % type(self))
 
     def post_test(self):
-        '''测试环境清理
-        '''
+        """测试环境清理"""
         pass
 
     def clean_test(self):
-        '''测试用例反初始化。慎用此函数，尽量将清理放到postTest里。
-        '''
+        """测试用例反初始化。慎用此函数，尽量将清理放到postTest里。"""
         if self.__resmgr_session:
             self.test_resources.destroy()
             self.__resmgr_session = None
 
     def start_step(self, stepinfo):
-        '''开始执行一个测试步骤
+        """开始执行一个测试步骤
 
         :param stepinfo: 步骤描述
         :type stepinfo: str
-        '''
+        """
         if not isinstance(stepinfo, six.text_type):
             stepinfo = str(stepinfo)
         self.__testresult.begin_step(stepinfo)
 
     def log_info(self, info):
-        '''Log一条信息
+        """Log一条信息
 
         :type info: string
         :param info: 要Log的信息
-        '''
+        """
         if not isinstance(info, six.text_type):
             info = str(info)
         self.__testresult.info(info)
 
     def fail(self, message):
-        '''测试用例失败
+        """测试用例失败
 
         :type message: string
         :param message: 要Log的信息
-        '''
+        """
         if not isinstance(message, six.text_type):
             message = str(message)
         self.__testresult.error(message)
 
     def __record_assert_failed(self, message, actual, expect):
-        '''记录Assert失败信息
+        """记录Assert失败信息
 
         :param message: 提示信息
         :type message: string
         :param actual: 实际值
         :type actual: string
         :param expect: 期望值
         :type expect: string
-        '''
+        """
         # 得到上一个函数调用帧所在的文件路径，行号，函数名
         stack = get_last_frame_stack(3)
-        msg = "检查点不通过\n%s%s\n期望值：%s%s\n实际值：%s%s" % (smart_text(stack), smart_text(message),
-                                                    expect.__class__, expect,
-                                                    actual.__class__, actual)
+        msg = "检查点不通过\n%s%s\n期望值：%s%s\n实际值：%s%s" % (
+            smart_text(stack),
+            smart_text(message),
+            expect.__class__,
+            expect,
+            actual.__class__,
+            actual,
+        )
         self.__testresult.log_record(EnumLogLevel.ASSERT, msg)
         if not settings.get("QTAF_ASSERT_CONTINUE", True):
             raise RuntimeError("testcase assert failed:%s" % message)
 
     def _log_assert_failed(self, message, back_count=2):
-        """记录断言失败的信息
-        """
+        """记录断言失败的信息"""
         stack = get_last_frame_stack(back_count)
         msg = "检查点不通过\n%s%s\n" % (smart_text(stack), smart_text(message))
         self.__testresult.log_record(EnumLogLevel.ASSERT, msg)
         if not settings.get("QTAF_ASSERT_CONTINUE", True):
             raise RuntimeError("testcase assert failed:%s" % message)
 
     def assert_(self, message, value):
@@ -634,102 +703,105 @@
         :param value:用于判断的值
         :type  value: bool或
         """
         if not value:
             self._log_assert_failed(message, 3)
 
     def assert_equal(self, message, actual, expect=True):
-        '''检查实际值和期望值是否相等，不能则测试用例失败
+        """检查实际值和期望值是否相等，不能则测试用例失败
 
-       :param message: 检查信息
-       :param actual: 实际值
-       :param expect: 期望值(默认：True)
-       :return: True or False
-        '''
+        :param message: 检查信息
+        :param actual: 实际值
+        :param expect: 期望值(默认：True)
+        :return: True or False
+        """
         if isinstance(actual, six.string_types):
             actual = smart_text(actual)
         if isinstance(expect, six.string_types):
             expect = smart_text(expect)
         if expect != actual:
             self.__record_assert_failed(message, actual, expect)
             return False
         else:
             return True
 
     def assert_match(self, message, actual, expect):
-        '''检查actual和expect是否模式匹配，不匹配则记录一个检查失败
+        """检查actual和expect是否模式匹配，不匹配则记录一个检查失败
 
         :type message: string
         :param message: 失败时记录的消息
         :type actual: string
         :param actual: 需要匹配的字符串
         :type expect: string
         :param expect: 要匹配的正则表达式
         :return: 匹配成果
-        '''
+        """
         if isinstance(actual, six.string_types):
             actual = smart_text(actual)
         if isinstance(expect, six.string_types):
             expect = smart_text(expect)
         if re.search(expect, actual):
             return True
         else:
             self.__record_assert_failed(message, actual, expect)
             return False
 
-    def wait_for_equal(self, message, obj, prop_name, expected, timeout=10, interval=0.5):
-        '''每隔interval检查obj.prop_name是否和expected相等，如果在timeout时间内都不相等，则测试用例失败
+    def wait_for_equal(
+        self, message, obj, prop_name, expected, timeout=10, interval=0.5
+    ):
+        """每隔interval检查obj.prop_name是否和expected相等，如果在timeout时间内都不相等，则测试用例失败
 
         :param message: 失败时的输出信息
         :param obj: 需要检查的对象
         :type prop_name: string
         :param prop_name: 需要检查的对象的属性名，支持多层属性
         :param expected: 期望的obj.prop_name值
         :param timeout: 超时秒数
         :param interval: 重试间隔秒数
         :return: True or False
-        '''
+        """
         for _ in Retry(timeout=timeout, interval=interval, raise_error=False):
             actual = getattr(obj, prop_name)
             if actual == expected:
                 return True
         else:
             self.__record_assert_failed(message, getattr(obj, prop_name), expected)
             return False
 
-    def wait_for_match(self, message, obj, prop_name, expected, timeout=10, interval=0.5):
-        '''每隔interval检查obj.prop_name是否和正则表达式expected是否匹配，如果在timeout时间内都不相等，则测试用例失败
+    def wait_for_match(
+        self, message, obj, prop_name, expected, timeout=10, interval=0.5
+    ):
+        """每隔interval检查obj.prop_name是否和正则表达式expected是否匹配，如果在timeout时间内都不相等，则测试用例失败
 
         :param message: 失败时的输出信息
         :param obj: 需要检查的对象
         :type prop_name: string
         :param prop_name: 需要检查的对象的属性名, obj.prop_name返回字符串
         :param expected: 需要匹配的正则表达式
         :param timeout: 超时秒数
         :param interval: 重试间隔秒数
         :return: True or False
-        '''
+        """
         for _ in Retry(timeout=timeout, interval=interval, raise_error=False):
             actual = getattr(obj, prop_name)
             if re.match(expected, actual, re.I):
                 return True
         else:
             self.__record_assert_failed(message, getattr(obj, prop_name), expected)
             return False
 
     def get_extra_fail_record(self):
-        '''当错误发生时，获取需要额外添加的日志记录和附件信息
+        """当错误发生时，获取需要额外添加的日志记录和附件信息
 
         :rtype: dict,dict - 日志记录，附件信息
-        '''
+        """
         return {}, {}
 
     def debug_run(self):
-        '''本地调试测试用例
-        '''
+        """本地调试测试用例"""
         from testbase import datadrive
         from testbase.runner import TestRunner
         from testbase.report import StreamTestReport, EmptyTestReport
         from testbase.testresult import StreamResult
 
         test_cls = type(self)
         if datadrive.is_datadrive(test_cls) or settings.DATA_DRIVE:  # datadrvie
@@ -742,48 +814,53 @@
         else:
             tests = [self]
             report = EmptyTestReport(lambda tc: StreamResult())
         runner = TestRunner(report)
         return runner.run(tests)
 
     def debug_run_one(self, name=None):
-        '''本地调试测试用例，给数据驱动的用例使用，只执行一个用例
+        """本地调试测试用例，给数据驱动的用例使用，只执行一个用例
 
         :param name: 测试数据名称，如果不指定，执行第一个数据的用例
-        '''
+        """
         from testbase import datadrive
         from testbase.runner import TestRunner
         from testbase.report import EmptyTestReport
         from testbase.testresult import StreamResult
 
         test_cls = type(self)
-        if not datadrive.is_datadrive(test_cls) and not settings.DATA_DRIVE:  # non-datadrive
+        if (
+            not datadrive.is_datadrive(test_cls) and not settings.DATA_DRIVE
+        ):  # non-datadrive
             raise RuntimeError("非数据驱动用例，请使用debug_run进行调试")
         if name:
             tests = datadrive.load_datadrive_tests(test_cls, name)
         else:
             tests = datadrive.load_datadrive_tests(test_cls)
             tests = tests[:1]
         runner = TestRunner(EmptyTestReport(lambda tc: StreamResult()))
         return runner.run(tests)
 
-    #----------------------------------------------------
+    # ----------------------------------------------------
     #    以下为兼容老的代码风格的接口，新代码请勿再使用
-    #----------------------------------------------------
+    # ----------------------------------------------------
 
     def run(self):
-        '''本地调试测试用例
-        '''
+        """本地调试测试用例"""
         self.debug_run()
 
-        sys.stderr.write('============================================================\n')
-        sys.stderr.write('注意：TestCase.run接口准备废弃，建议改用为.debug_run接口，例如：\n')
-        sys.stderr.write('if __name__ == \'__main__\'\n')
-        sys.stderr.write('    %s().debug_run()\n' % type(self).__name__)
-        sys.stderr.write('============================================================\n')
+        sys.stderr.write(
+            "============================================================\n"
+        )
+        sys.stderr.write("注意：TestCase.run接口准备废弃，建议改用为.debug_run接口，例如：\n")
+        sys.stderr.write("if __name__ == '__main__'\n")
+        sys.stderr.write("    %s().debug_run()\n" % type(self).__name__)
+        sys.stderr.write(
+            "============================================================\n"
+        )
 
     initTest = init_test
     preTest = pre_test
     runTest = run_test
     postTest = post_test
     cleanTest = clean_test
     startStep = start_step
@@ -797,120 +874,140 @@
     TestName = test_name
     TestDoc = test_doc
 
     logInfo = log_info
 
 
 class ITestCaseRunner(object):
-    '''测试用例执行器接口定义
-    '''
+    """测试用例执行器接口定义"""
 
     def run(self, testcase, testresult_factory):
-        '''执行一个测试用例
+        """执行一个测试用例
 
         :param testcase: 执行的测试用例
         :type testcase: TestCase
         :param testresult_factory: 测试结果工厂
         :type testresult_factory: ITestResultFactory
 
         :return TestResult/TestResultCollection - 测试结果
-        '''
+        """
         raise NotImplementedError()
 
 
 class TestCaseRunner(ITestCaseRunner):
-    '''负责执行一个测试用例
+    """负责执行一个测试用例
 
     如果一个测试用例没有指定case_runner类变量，则默认都使用TestCaseRunner来执行这个用例。
     测试用例可以自定义和TestCaseRunner接口兼容的runner类，并设置case_runner类变量来实现
     自定义一个测试用例的执行逻辑，以下是TestCaseRunner的接口定义
-    '''
+    """
 
     CLEANUP_TIMEOUT = 300
 
     def __init__(self):
-        '''构造函数
-        '''
+        """构造函数"""
         self._lock = threading.Lock()
         self._stop_run = False
         self._error = None
 
     def _rewrite_assert(self, cls):
         if not settings.get("QTAF_REWRITE_ASSERT", True) or cls == TestCase:
             return
         rewriter = AssertionRewriter()
         for key in dir(cls):
             item = getattr(cls, key)
             if isinstance(item, (types.MethodType, types.FunctionType)):
-                rewriter.rewrite(item)
+                item_source_file = inspect.getsourcefile(item)
+                cls_source_file = inspect.getsourcefile(cls)
+                if item_source_file == cls_source_file:
+                    rewriter.rewrite(item)
 
     def _walk_bases(self, test_case):
-        '''遍历所有基类，进行相应的处理
-        '''
+        """遍历所有基类，进行相应的处理"""
         cur_cls = type(test_case)
         self._single_methods_mapping(cur_cls)
         self._rewrite_assert(cur_cls)
         bases = set(cur_cls.__bases__)
         while bases:
             new_bases = set()
             for base_cls in bases:
                 self._single_methods_mapping(base_cls)
-                self._rewrite_assert(cur_cls)
+                self._rewrite_assert(base_cls)
                 new_bases = new_bases.union(set(base_cls.__bases__))
             bases = new_bases
 
     def _single_methods_mapping(self, cls_type):
-        '''针对单个类进行方法映射
-        '''
+        """针对单个类进行方法映射"""
         if object == cls_type:
             return
         case_mothods = [
             ("initTest", "init_test"),
             ("preTest", "pre_test"),
             ("runTest", "run_test"),
             ("postTest", "post_test"),
-            ("cleanTest", "clean_test")
+            ("cleanTest", "clean_test"),
         ]
         cls_dict = cls_type.__dict__
         for pairs in case_mothods:
             if pairs[0] in cls_dict and not pairs[1] in cls_dict:
                 setattr(cls_type, pairs[1], cls_dict[pairs[0]])
-                self._testresult.warning("严重警告：类型%s应当定义方法%s，方法%s已被废弃，请勿使用" % (cls_type.__name__, pairs[1], pairs[0]))
+                self._testresult.warning(
+                    "严重警告：类型%s应当定义方法%s，方法%s已被废弃，请勿使用"
+                    % (cls_type.__name__, pairs[1], pairs[0])
+                )
             elif pairs[0] not in cls_dict and pairs[1] in cls_dict:
                 setattr(cls_type, pairs[0], cls_dict[pairs[1]])
             elif pairs[0] in cls_dict and pairs[1] in cls_dict:
                 if cls_dict[pairs[0]] != cls_dict[pairs[1]]:
-                    raise RuntimeError('类型%s不允许同时独立定义"%s"和"%s"' % (cls_type, pairs[0], pairs[1]))
+                    raise RuntimeError(
+                        '类型%s不允许同时独立定义"%s"和"%s"' % (cls_type, pairs[0], pairs[1])
+                    )
 
     def _check_testcase(self, testcase):
-        '''检查测试用例
+        """检查测试用例
 
         :param testcase: 测试用例
         :type testcase: TestCase
         :returns boolean, string - 检测是否通过，错误消息
-        '''
-        attrnames = ['owner', 'priority', 'status', 'timeout']
+        """
+        attrnames = ["owner", "priority", "status", "timeout"]
         tcattrs = {}
         for attr in attrnames:
             attrvalue = getattr(self._testcase, attr)
             if isinstance(attrvalue, six.text_type):
                 if attrvalue.strip(" ") == "":
                     attrvalue = None
             tcattrs[attr] = attrvalue
-        tcattrs['testname'] = self._testcase.test_name
+        tcattrs["testname"] = self._testcase.test_name
         if None in tcattrs.values():
             raise RuntimeError("测试用例需要设置以下类属性：%s" % attrnames)
         if not self._testcase.test_doc:
             raise RuntimeError("测试用例的描述不能为空，请加上描述！")
 
         self._walk_bases(testcase)
 
+    def _check_valid_customize_result(self, task_result, reason=None):
+        valid_task_result = False
+        for name in TestResultType.__dict__:
+            value = TestResultType.__dict__[name]
+            if task_result == value:
+                valid_task_result = True
+                break
+        if not valid_task_result:
+            self._testresult.warning("指定的自定义状态不支持，用例将继续执行")
+        else:
+            self._testresult.customize_result(task_result, reason)
+            while self._subtasks[0] not in [
+                "post_test",
+                "postTest",
+            ]:
+                self._subtasks.popleft()
+
     def _thread_run(self):
-        '''测试用例线程过程
-        '''
+        """测试用例线程过程"""
         #                     函数时发生了死锁，故注释掉。观察一段时间，看修改是否会影响测试。
         try:
             try:
                 self._check_testcase(self._testcase)
             except RuntimeError as e:
                 self._testresult.error(e.args[0])
                 return
@@ -919,142 +1016,161 @@
                 with self._lock:
                     if len(self._subtasks) == 0 or self._stop_run:
                         break
                     it = self._subtasks.popleft()
 
                 if isinstance(it, str):
                     try:
-                        if it in ['init_test', 'initTest']:
+                        self._testcase.current_stage = it
+                        if it in ["init_test", "initTest"]:
                             getattr(self._testcase, it)(self._testresult)
                         else:
                             task_result = getattr(self._testcase, it)()
-                            if task_result and isinstance(task_result, six.string_types):
-                                valid_task_result = False
-                                for name in TestResultType.__dict__:
-                                    value = TestResultType.__dict__[name]
-                                    if task_result == value:
-                                        valid_task_result = True
-                                        break
-                                if not valid_task_result:
-                                    self._testresult.warning('指定的自定义状态不支持，用例将继续执行')
-                                else:
-                                    self._testresult.customize_result(task_result)
-                                    while self._subtasks[0] not in ['post_test', 'postTest']:
-                                        self._subtasks.popleft()
-                    except:
-                        self._testresult.exception('%s执行失败' % it)
-                        if settings.get("QTAF_FAILED_SKIP_RUNTEST", False) and it in ['pre_test', 'preTest']:
-                            while self._subtasks[0] not in ['post_test', 'postTest']:
+                            if task_result:
+                                if isinstance(
+                                    task_result, six.string_types
+                                ):
+                                    self._check_valid_customize_result(task_result)
+                                elif isinstance(
+                                    task_result, tuple
+                                ) and len(task_result) > 1:
+                                    result, reason = task_result[0], task_result[1]
+                                    self._check_valid_customize_result(result, reason)
+                    except BaseException:  # pylint: disable=broad-except
+                        self._testresult.exception("%s执行失败" % it)
+                        if settings.get("QTAF_FAILED_SKIP_RUNTEST", False) and it in [
+                            "pre_test",
+                            "preTest",
+                        ]:
+                            while self._subtasks[0] not in ["post_test", "postTest"]:
                                 self._subtasks.popleft()
                 else:
                     it()
 
-        except:
+        except BaseException:  # pylint: disable=broad-except
             self._error = traceback.format_exc()
 
     def _thread_cleanup(self):
-        '''清理线程
-        '''
+        """清理线程"""
         try:
             while True:
                 with self._lock:
                     if len(self._subtasks) == 0:
                         break
                     it = self._subtasks.popleft()
-                    if it in ['initTest', 'preTest', 'runTest', 'init_test', 'pre_test', 'run_test']:
+                    if it in [
+                        "initTest",
+                        "preTest",
+                        "runTest",
+                        "init_test",
+                        "pre_test",
+                        "run_test",
+                    ]:
                         continue
 
                 if isinstance(it, str):
                     try:
                         getattr(self._testcase, it)()
-                    except:
-                        self._testresult.exception('用例超时时%s执行失败' % it)
+                    except Exception:  # pylint: disable=broad-except
+                        self._testresult.exception("用例超时时%s执行失败" % it)
                 else:
                     it()
-        except:
+        except Exception:  # pylint: disable=broad-except
             self._error = traceback.format_exc()
 
     def setup(self, testcase, testresult):
-        '''测试执行初始化
+        """测试执行初始化
 
         :param testcase: 执行的测试用例
         :type testcase: TestCase
         :param testresult: 测试用例结果
         :type testresult: TestResult
-        '''
+        """
         pass
 
     def teardown(self, testcase, testresult):
-        '''测试执行清理
+        """测试执行清理
 
         :param testcase: 执行的测试用例
         :type testcase: TestCase
         :param testresult: 测试用例结果
         :type testresult: TestResult
-        '''
+        """
         pass
 
     def run(self, testcase, testresult_factory):
-        '''执行一个测试用例
+        """执行一个测试用例
 
         :param testcase: 执行的测试用例
         :type testcase: TestCase
         :param testresult_factory: 测试结果工厂
         :type testresult_factory: ITestResultFactory
         :rtype: TestResult/TestResultCollection - 测试结果
-        '''
+        """
         #                       临时方案是disable gc后kill掉程序，在enable gc。后续这里
         #                        需要重新考虑已独立进程来执行测试用例。
 
         self._stop_run = False
         self._testcase = testcase
         self._testresult = testresult_factory.create(testcase)
-        self._subtasks = collections.deque(['init_test', 'pre_test', 'run_test', 'post_test', 'clean_test'])
+        self._subtasks = collections.deque(
+            ["init_test", "pre_test", "run_test", "post_test", "clean_test"]
+        )
 
-        with ThreadGroupScope('%s:%s' % (self._testcase.test_name, id(self))):
+        with ThreadGroupScope("%s:%s" % (self._testcase.test_name, id(self))):
 
             ThreadGroupLocal().testcase = self._testcase
             ThreadGroupLocal().testresult = self._testresult
 
             self._testresult.begin_test(self._testcase)
 
             self.setup(self._testcase, self._testresult)
 
-            if isinstance(self._testcase.timeout, int) or isinstance(self._testcase.timeout, float):
+            if isinstance(self._testcase.timeout, int) or isinstance(
+                self._testcase.timeout, float
+            ):
                 timeout = self._testcase.timeout * 60
             else:
                 timeout = 60
 
             test_thread = threading.Thread(target=self._thread_run)
             test_thread.daemon = True
             test_thread.start()
             test_thread.join(timeout)
             if test_thread.is_alive():
                 self._stop_run = True
                 try:
                     thread_traceback = self._get_current_traceback(test_thread)
-                except:
-                    self._testresult.log_record(EnumLogLevel.TESTTIMEOUT, '测试用例执行超时')
+                except Exception:  # pylint: disable=broad-except
+                    self._testresult.log_record(EnumLogLevel.TESTTIMEOUT, "测试用例执行超时")
                 else:
-                    self._testresult.log_record(EnumLogLevel.TESTTIMEOUT, '测试用例执行超时，抓取测试线程当前堆栈',
-                                                dict(traceback=thread_traceback))
+                    self._testresult.log_record(
+                        EnumLogLevel.TESTTIMEOUT,
+                        "测试用例执行超时，抓取测试线程当前堆栈",
+                        dict(traceback=thread_traceback),
+                    )
 
                 # 启动线程执行可能未执行的postTest和cleanTest
                 cleanup_thread = threading.Thread(target=self._thread_cleanup)
                 cleanup_thread.daemon = True
                 cleanup_thread.start()
                 cleanup_thread.join(self.CLEANUP_TIMEOUT)
                 if cleanup_thread.is_alive():
                     try:
                         thread_traceback = self._get_current_traceback(cleanup_thread)
-                    except:
-                        self._testresult.log_record(EnumLogLevel.TESTTIMEOUT, '测试用例执行超时时清理超时')
+                    except Exception:  # pylint: disable=broad-except
+                        self._testresult.log_record(
+                            EnumLogLevel.TESTTIMEOUT, "测试用例执行超时时清理超时"
+                        )
                     else:
-                        self._testresult.log_record(EnumLogLevel.TESTTIMEOUT, '测试用例执行超时时清理超时，抓取清理线程当前堆栈',
-                                                    dict(traceback=thread_traceback))
+                        self._testresult.log_record(
+                            EnumLogLevel.TESTTIMEOUT,
+                            "测试用例执行超时时清理超时，抓取清理线程当前堆栈",
+                            dict(traceback=thread_traceback),
+                        )
                 else:
                     if self._error:
                         raise RuntimeError("用例执行线程异常：\n%s" % smart_text(self._error))
             else:
                 if self._error:
                     raise RuntimeError("用例执行线程异常：\n%s" % smart_text(self._error))
 
@@ -1063,34 +1179,34 @@
             self._testresult.end_test()
 
         # gc.enable()
         # gc.collect()
         return self._testresult
 
     def _get_current_traceback(self, thread):
-        '''获取用例线程的当前的堆栈
+        """获取用例线程的当前的堆栈
 
         :param thread: 要获取堆栈的线程
         :type thread: Thread
-        '''
+        """
         for thread_id, stack in sys._current_frames().items():
             if thread_id != thread.ident:
                 continue
             tb = "Traceback ( thread-%d possibly hold at ):\n" % thread_id
             for filename, lineno, name, line in traceback.extract_stack(stack):
                 tb += '  File: "%s", line %d, in %s\n' % (filename, lineno, name)
                 if line:
                     tb += "    %s\n" % (line.strip())
             return tb
         else:
             raise RuntimeError("thread not found")
 
 
 class RepeatTestCaseRunner(ITestCaseRunner):
-    '''重复执行的用例执行器
+    """重复执行的用例执行器
 
     可以通过设置测试用例的类属性为此runner实例来实现指定测试用例
     执行多次。测试用例执行时可以访问成员变量iteration来判断当前是
     第几次执行。
 
     使用示例如下::
 
@@ -1101,43 +1217,42 @@
             timeout = 1
             status = TestCase.EnumStatus.Ready
             priority = TestCase.EnumPriority.Normal
 
             def run_test(self):
                 self.log_info("第%s次执行测试"%self.iteration)
 
-    '''
+    """
 
     def __init__(self, case_runner_class=None):
-        '''指定执行一个用例的CaseRunner类，不指定则为TestCaseRunner类
-        '''
+        """指定执行一个用例的CaseRunner类，不指定则为TestCaseRunner类"""
         if case_runner_class is None:
             case_runner_class = TestCaseRunner
         self._case_runner_class = case_runner_class
 
     def run(self, testcase, testresult_factory):
-        '''执行一个测试用例
+        """执行一个测试用例
 
         :param testcase: 执行的测试用例
         :type testcase: TestCase
         :param testresult_factory: 测试结果工厂
         :type testresult_factory: ITestResultFactory
 
         :returns : 测试结果
         :rtype TestResult/TestResultCollection - 测试结果
-        '''
+        """
         passed = True
         if not hasattr(testcase, "repeat"):
             passed = False
             err_msg = "使用RepeatTestCaseRunner的测试用例需要设置类属性：repeat"
         elif testcase.repeat <= 0:
             passed = False
             err_msg = "使用RepeatTestCaseRunner的测试用例的类属性'repeat'必须大于0"
         if not passed:
-            with ThreadGroupScope('%s:%s' % (testcase.test_name, id(self))):
+            with ThreadGroupScope("%s:%s" % (testcase.test_name, id(self))):
                 result = testresult_factory.create(testcase)
                 ThreadGroupLocal().testcase = testcase
                 ThreadGroupLocal().testresult = result
                 result.begin_test(testcase)
                 result.error(err_msg)
                 result.end_test()
                 return result
@@ -1150,176 +1265,16 @@
             passed &= case_result.passed
             results.append(case_result)
             if not passed:
                 break
         return TestResultCollection(results, passed)
 
 
-class SeqTestCaseRunner(ITestCaseRunner):
-    '''顺序执行的用例的执行器
-    '''
-
-    def run(self, testsuite, testresult_factory):
-        '''执行一个顺序执行的测试用例套
-
-        :param testsuite: 执行的测试用例套
-        :type testsuite: SeqTestSuite
-        :param testresult_factory: 测试结果工厂
-        :type testresult_factory: ITestResultFactory
-
-        :return TestResult/TestResultCollection - 测试结果
-        '''
-        passed = True
-        results = []
-        for it in testsuite:
-            runner = getattr(it, 'case_runner', TestCaseRunner())
-            case_result = runner.run(it, testresult_factory)
-            passed &= case_result.passed
-            results.append(case_result)
-            if not passed:
-                break
-        return TestResultCollection(results, passed)
-
-
-class TestSuite(object):
-    '''测试用例套
-    '''
-
-    @property
-    def suite_class_name(self):
-        '''测试套类名称
-        '''
-        cls = type(self)
-        if cls.__module__ == '__main__':
-            type_name = cls.__name__
-        else:
-            type_name = (cls.__module__ + '.' + cls.__name__)
-        return type_name
-
-    def dumps(self):
-        '''序列化
-        '''
-        raise NotImplementedError()
-
-    def loads(self, buf):
-        '''反序列化
-        '''
-        raise NotImplementedError()
-
-
-class SeqTestSuite(TestSuite):
-    '''顺序执行的测试用例套
-    '''
-    case_runner = SeqTestCaseRunner()
-
-    def __init__(self, testcases):
-        '''构造函数
-
-        :param testcases: 测试用例列表
-        :type testcases: list
-        :param name: 测试用例名
-        :type name: string
-        '''
-        self._testcases = testcases
-        self._resmgr = None
-        self.__share_data_mgr = None
-
-    def __iter__(self):
-        for it in self._testcases:
-            yield it
-
-    def __len__(self):
-        return len(self._testcases)
-
-    def __repr__(self):
-        return '<SeqTestSuite module:%s>' % self.test_class_name
-
-    @property
-    def test_class_name(self):
-        '''返回测试用例名字（不同测试用例的名字不同）
-
-        :rtype: str
-        '''
-        cls = type(self._testcases[0])
-        return cls.__module__
-
-    @property
-    def test_name(self):
-        '''返回测试用例实例的名字
-
-        :rtype: str
-        '''
-        cls = type(self._testcases[0])
-        return cls.__module__
-
-    @property
-    def test_doc(self):
-        '''测试用例说明
-
-        :rtype: str
-        '''
-        cls = type(self._testcases[0])
-        desc = cls.__module__.__doc__
-        if isinstance(desc, six.text_type):
-            desc = re.sub('^\s*', '', desc)
-            desc = re.sub('\s*$', '', desc)
-        return desc
-
-    @property
-    def test_result(self):
-        '''将最后一个执行的用例结果，作为Suite的结果
-        '''
-        result = None
-        for testcae in self._testcases:
-            if testcae.test_result:
-                result = testcae.test_result
-            else:
-                break
-        return result
-
-    @property
-    def test_resmgr(self):
-        '''资源管理器
-        '''
-        return self._resmgr
-
-    @test_resmgr.setter
-    def test_resmgr(self, resmgr):
-        self._resmgr = resmgr
-        for it in self._testcases:
-            it.test_resmgr = resmgr
-
-
-    @property
-    def share_data_mgr(self):
-        '''共享数据管理器
-        '''
-        return self.__share_data_mgr
-
-    @share_data_mgr.setter
-    def share_data_mgr(self, share_data_mgr):
-        self.__share_data_mgr = share_data_mgr
-        for it in self._testcases:
-            it._share_data_mgr = share_data_mgr
-
-    def dumps(self):
-        '''序列化
-        '''
-        from testbase import serialization
-        return [serialization.dumps(it) for it in self._testcases]
-
-    def loads(self, buf):
-        '''反序列化
-        '''
-        from testbase import serialization
-        self._testcases = [serialization.loads(it) for it in buf]
-
-
 def debug_run_all():
-    '''调试执行当前脚本的全部用例
-    '''
+    """调试执行当前脚本的全部用例"""
     from testbase.loader import TestLoader
     from testbase.runner import TestRunner
     from testbase.report import StreamTestReport
+
     tests = TestLoader().load("__main__")
     runner = TestRunner(StreamTestReport(output_testresult=True, output_summary=True))
     runner.run(tests)
```

### Comparing `qtaf-5.5.9/testbase/testresult.py` & `qtaf-5.6.0/testbase/testresult.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 测试结果模块
 
 参考logging模块的设计，使用示例如下::
 
     result = TestResult()
     result.add_handler(StreamResultHandler())
     result.begin_test()
@@ -27,224 +27,262 @@
 其中result.info接口可以传record扩展信息，比如::
 
     result.error('', '异常发生', traceback=traceback.format_exc())
 
 同logger一样，TestResult对象保证对所有的ITestResultHandler的调用都是线程安全的，可以通过实现
 ITestResultHandler来实现一个新的Handler，详细请参考ITestResultHandler接口
 
-'''
+"""
 
 import json
 import locale
 import os
-import six
-import socket
 import sys
 import time
 import threading
 import traceback
 import xml.dom.minidom as dom
 import xml.parsers.expat as xmlexpat
 import xml.sax.saxutils as saxutils
 
+import six
+
 from testbase import context
-from testbase.util import smart_text, get_thread_traceback, get_method_defined_class, \
-    to_pretty_xml, smart_binary, ensure_binary_stream, codecs_open, get_time_str, \
-    translate_bad_char, file_encoding, path_exists
+from testbase.util import (
+    TimeoutLock,
+    smart_text,
+    get_thread_traceback,
+    get_method_defined_class,
+    to_pretty_xml,
+    smart_binary,
+    ensure_binary_stream,
+    codecs_open,
+    get_time_str,
+    translate_bad_char,
+    path_exists,
+)
 
 
 os_encoding = locale.getdefaultlocale()[1]
 
 
 class EnumLogLevel(object):
-    '''日志级别
-    '''
+    """日志级别"""
+
     DEBUG = 10
     INFO = 20
     Environment = 21  # 测试环境相关信息， device/devices表示使用的设备、machine表示执行的机器
     ENVIRONMENT = Environment
     RESOURCE = 22
 
     WARNING = 30
     ERROR = 40
     ASSERT = 41  # 断言失败，actual/expect/code_location
     CRITICAL = 60
     APPCRASH = 61  # 测试目标Crash
     TESTTIMEOUT = 62  # 测试执行超时
     RESNOTREADY = 69  # 当前资源不能满足测试执行的要求
 
+
 class TestResultType(object):
-    '''扩展用例状态
-    '''
-    FILTERED = 'ignored'
+    """扩展用例状态"""
+
+    FILTERED = "ignored"
 
 
 levelname = {}
 for name in EnumLogLevel.__dict__:
     value = EnumLogLevel.__dict__[name]
     if isinstance(value, int):
         levelname[value] = name
 
-RESULT_TYPES = (
-    (TestResultType.FILTERED, "被忽略"),
-)
-
+RESULT_TYPES = ((TestResultType.FILTERED, "被忽略"),)
 
 
 def _convert_timelength(sec):
     h = int(sec / 3600)
     sec -= h * 3600
     m = int(sec / 60)
     sec -= m * 60
     return (h, m, sec)
 
 
 def smart_text_by_lines(s):
-    '''将任意字符串转换为UTF-8编码
-    '''
+    """将任意字符串转换为UTF-8编码"""
     lines = []
-    for line in s.split('\n'):
+    for line in s.split("\n"):
         lines.append(smart_text(line))
-    return '\n'.join(lines)
+    return "\n".join(lines)
 
 
 class TestResultBase(object):
-    '''测试结果基类
+    """测试结果基类
 
     此类的职责如下：
     1、提供测试结果基本接口
     2、保证线程安全
     2、测试是否通过之逻辑判断
-    '''
+    """
 
     def __init__(self):
-        '''构造函数
-        '''
+        """构造函数"""
         self.__lock = threading.RLock()
+        if sys.version_info[0] >= 3:
+            # Support timeout lock on python3
+            self.__lock = TimeoutLock(30)
         self.__steps_passed = [True]  # 预设置一个，以防用例中没调用startStep
         self.__curr_step = 0
         self.__accept_result = False
         self.__testcase = None
         self.__begin_time = None
         self.__end_time = None
         self.__error_level = 0
         self.__failed_info = ""
         self.__failed_priority = 0
         self._custom_result = None
+        self._custom_reason = None
+        self.__failed_stages = []
 
     @property
     def testcase(self):
-        '''对应的测试用例
+        """对应的测试用例
         :returns: TestCase
-        '''
+        """
         return self.__testcase
 
     @property
     def passed(self):
-        '''测试是否通过
+        """测试是否通过
 
         :returns: True or False
-        '''
+        """
         return all(self.__steps_passed)
 
     @property
     def failed_reason(self):
-        '''用例测试不通过的错误原因
+        """用例测试不通过的错误原因
 
         :returns: str
-        '''
+        """
         if self.__error_level:
-            return levelname.get(self.__error_level, 'unknown')
+            return levelname.get(self.__error_level, "unknown")
         else:
-            return ''
+            return ""
 
     @property
     def failed_info(self):
-        '''测试用例失败时的执行状况
+        """测试用例失败时的执行状况
 
         :returns: str
-        '''
+        """
         return self.__failed_info
 
     @property
     def begin_time(self):
-        '''测试用例开始时间
+        """测试用例开始时间
 
         :returns: float
-        '''
+        """
         return self.__begin_time
 
     @property
     def end_time(self):
-        '''测试用例结束时间
+        """测试用例结束时间
 
         :returns: float
-        '''
+        """
         return self.__end_time
 
+    @property
+    def failed_stages(self):
+        """测试用例失败的阶段
+
+        :returns: str
+        """
+        return self.__failed_stages
+
+    def is_testsuite(self):
+        """是否是测试用例套
+
+        :returns: bool
+        """
+        from testbase.testsuite import TestSuite
+
+        return isinstance(self.testcase, TestSuite)
+
+    def add_failed_stage(self, failed_stage):
+        """增加测试用例失败的阶段
+
+        :param value: 阶段名
+        :type value: str
+        """
+        if isinstance(failed_stage, str):
+            self.failed_stages.append(failed_stage)
+
     def begin_test(self, testcase):
-        '''开始执行测试用例
+        """开始执行测试用例
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
+        """
         with self.__lock:
             if self.__accept_result:
                 raise RuntimeError("此时不可调用begin_test")
             self.__accept_result = True
             self.__begin_time = time.time()
-            self.handle_test_begin(testcase)
             self.__testcase = testcase
+            self.handle_test_begin(testcase)
 
     def end_test(self):
-        '''结束执行测试用例
-        '''
+        """结束执行测试用例"""
         with self.__lock:
             if not self.__accept_result:
                 raise RuntimeError("此时不可调用end_test")
             self.handle_step_end(self.__steps_passed[self.__curr_step])
             self.__end_time = time.time()
             self.handle_test_end(self.passed)  # 防止没有一个步骤
             self.__accept_result = False
 
     def begin_step(self, msg):
-        '''开始一个测试步骤
+        """开始一个测试步骤
 
         :param msg: 测试步骤名称
         :type msg: string
-        '''
+        """
         with self.__lock:
             if not self.__accept_result:
                 raise RuntimeError("此时不可调用begin_step")
             if len(self.__steps_passed) != 1:
                 self.handle_step_end(self.__steps_passed[self.__curr_step])
             self.__steps_passed.append(True)
             self.__curr_step += 1
             self.handle_step_begin(msg)
 
     def log_record(self, level, msg, record=None, attachments=None):
-        '''处理一个日志记录
+        """处理一个日志记录
 
         :param level: 日志级别，参考EnumLogLevel
         :type level: string
         :param msg: 日志消息
         :type msg: string
         :param record: 日志记录
         :type record: dict
         :param attachments: 附件
         :type attachments: dict
-        '''
+        """
         if record is None:
             record = {}
         if attachments is None:
             attachments = {}
         if not isinstance(msg, six.string_types):
             raise ValueError("msg='%r'必须是string类型" % msg)
         msg = smart_text(msg)
         if level >= EnumLogLevel.ERROR:
+            if self.__testcase.current_stage:
+                self.add_failed_stage(self.__testcase.current_stage)
             self.__steps_passed[self.__curr_step] = False
             if level > self.__error_level:
                 self.__error_level = level
             extra_record, extra_attachments = self._get_extra_fail_record_safe()
             record.update(extra_record)
             attachments.update(extra_attachments)
 
@@ -255,355 +293,411 @@
                 self.__failed_info, self.__failed_priority = "用例执行超时", 2
 
             if self.__failed_priority <= 1 and level == EnumLogLevel.ASSERT:
                 self.__failed_info, self.__failed_priority = msg, 1
 
             if self.__failed_priority <= 1 and "traceback" in record:
                 if not self.__failed_info:  # 优先记录第一个异常，第一个异常往往比较大可能是问题的原因
-                    self.__failed_info, self.__failed_priority = record["traceback"].split('\n')[-2], 1
+                    self.__failed_info, self.__failed_priority = (
+                        record["traceback"].split("\n")[-2],
+                        1,
+                    )
 
         with self.__lock:
             if not self.__accept_result:
                 return
             self.handle_log_record(level, msg, record, attachments)
 
     def _get_extra_fail_record_safe(self, timeout=300):
-        '''使用线程调用测试用例的get_extra_fail_record
-        '''
+        """使用线程调用测试用例的get_extra_fail_record"""
 
         def _run(outputs, errors):
             try:
                 outputs.append(context.current_testcase().get_extra_fail_record())
-            except:
+            except Exception:  # pylint: disable=broad-except
                 errors.append(traceback.format_exc())
 
         errors = []
         outputs = []
         t = threading.Thread(target=_run, args=(outputs, errors))
         t.daemon = True
         t.start()
         t.join(timeout)
         extra_record, extra_attachments = {}, {}
         with self.__lock:
             if t.is_alive():
                 stack = get_thread_traceback(t)
-                self.handle_log_record(EnumLogLevel.ERROR, '测试失败时获取其他额外错误信息超过了指定时间：%ds' % timeout,
-                                       {'traceback':stack},
-                                       {})
+                self.handle_log_record(
+                    EnumLogLevel.ERROR,
+                    "测试失败时获取其他额外错误信息超过了指定时间：%ds" % timeout,
+                    {"traceback": stack},
+                    {},
+                )
             else:
                 if errors:
-                    self.handle_log_record(EnumLogLevel.ERROR, '测试失败时获取其他额外错误信息失败',
-                                          {'traceback':errors[0]}, {})
+                    self.handle_log_record(
+                        EnumLogLevel.ERROR,
+                        "测试失败时获取其他额外错误信息失败",
+                        {"traceback": errors[0]},
+                        {},
+                    )
                 else:
                     record_info = outputs[0]
                     if isinstance(record_info, (tuple, list)) and len(record_info) == 2:
                         extra_record, extra_attachments = record_info
                     else:
-                        cls = get_method_defined_class(self.testcase.get_extra_fail_record)
-                        if cls.__module__ == '__main__':
+                        cls = get_method_defined_class(
+                            self.testcase.get_extra_fail_record
+                        )
+                        if cls.__module__ == "__main__":
                             class_path = cls.__name__
                         else:
                             class_path = "%s.%s" % (cls.__module__, cls.__name__)
-                        raise RuntimeError("%s.get_extra_fail_record must return a 2 elements tuple" % class_path)
+                        raise RuntimeError(
+                            "%s.get_extra_fail_record must return a 2 elements tuple"
+                            % class_path
+                        )
         return extra_record, extra_attachments
 
     def debug(self, msg, record=None, attachments=None):
-        '''处理一个DEBUG日志
-        '''
+        """处理一个DEBUG日志"""
         self.log_record(EnumLogLevel.DEBUG, msg, record, attachments)
 
     def info(self, msg, record=None, attachments=None):
-        '''处理一个INFO日志
-        '''
+        """处理一个INFO日志"""
         self.log_record(EnumLogLevel.INFO, msg, record, attachments)
 
     def warning(self, msg, record=None, attachments=None):
-        '''处理一个WARNING日志
-        '''
+        """处理一个WARNING日志"""
         self.log_record(EnumLogLevel.WARNING, msg, record, attachments)
 
     def error(self, msg, record=None, attachments=None):
-        '''处理一个ERROR日志
-        '''
+        """处理一个ERROR日志"""
         self.log_record(EnumLogLevel.ERROR, msg, record, attachments)
 
     def exception(self, msg, record=None, attachments=None):
-        '''处理一个DEBUG日志
-        '''
+        """处理一个DEBUG日志"""
         if record is None:
             record = {}
-        record['traceback'] = traceback.format_exc()
+        record["traceback"] = traceback.format_exc()
         self.log_record(EnumLogLevel.CRITICAL, msg, record, attachments)
 
     def handle_test_begin(self, testcase):
-        '''处理一个测试用例执行的开始
+        """处理一个测试用例执行的开始
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
+        """
         pass
 
     def handle_test_end(self, passed):
-        '''处理一个测试用例执行的结束
+        """处理一个测试用例执行的结束
 
         :param passed: 测试用例是否通过
         :type passed: boolean
-        '''
+        """
         pass
 
     def handle_step_begin(self, msg):
-        '''处理一个测试步骤的开始
+        """处理一个测试步骤的开始
 
         :param msg: 测试步骤名称
         :type msg: string
-        '''
+        """
         pass
 
     def handle_step_end(self, passed):
-        '''处理一个测试步骤的结束
+        """处理一个测试步骤的结束
 
         :param passed: 测试步骤是否通过
         :type passed: boolean
-        '''
+        """
         pass
 
     def handle_log_record(self, level, msg, record, attachments):
-        '''处理一个日志记录
+        """处理一个日志记录
 
         :param level: 日志级别，参考EnumLogLevel
         :type level: string
         :param msg: 日志消息
         :type msg: string
         :param record: 日志记录
         :type record: dict
         :param attachments: 附件
         :type attachments: dict
-        '''
+        """
         pass
 
-    def customize_result(self, result):
+    def customize_result(self, result, reason=None):
         self._custom_result = result
+        if reason:
+            self._custom_reason = reason
+
 
 class EmptyResult(TestResultBase):
-    '''不输出
-    '''
+    """不输出"""
+
     pass
 
 
 class StreamResult(TestResultBase):
-    '''测试用例stream输出
-    '''
+    """测试用例stream输出"""
 
     _seperator1 = "-" * 40 + "\n"
     _seperator2 = "=" * 60 + "\n"
 
     def __init__(self, stream=sys.stdout):
-        '''构造函数
+        """构造函数
 
         :param stream: 流对象
         :type stream: file
-        '''
+        """
         super(StreamResult, self).__init__()
         self._stream, encoding = ensure_binary_stream(stream)
         self._write = lambda x: self._stream.write(smart_binary(x, encoding=encoding))
         self._step_results = []
 
     def handle_test_begin(self, testcase):
-        '''处理一个测试用例执行的开始
+        """处理一个测试用例执行的开始
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
+        """
         self._write(self._seperator2)
-        owner = getattr(testcase, 'owner', None)
-        priority = getattr(testcase, 'priority', None)
-        timeout = getattr(testcase, 'timeout', None)
-        begin_msg = "测试用例:%s 所有者:%s 优先级:%s 超时:%s分钟\n" % (testcase.test_name, owner, priority, timeout)
+        owner = getattr(testcase, "owner", None)
+        priority = getattr(testcase, "priority", None)
+        timeout = getattr(testcase, "timeout", None)
+        begin_msg = "测试%s:%s 所有者:%s 优先级:%s 超时:%s分钟\n" % (
+            "套" if self.is_testsuite() else "用例",
+            testcase.test_name,
+            owner,
+            priority,
+            timeout,
+        )
+
         self._write(begin_msg)
         self._write(self._seperator2)
 
     def handle_test_end(self, passed):
-        '''处理一个测试用例执行的结束
+        """处理一个测试用例执行的结束
 
         :param passed: 测试用例是否通过
         :type passed: boolean
-        '''
+        """
         self._write(self._seperator2)
-        self._write("测试用例开始时间: %s\n" % time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time)))
-        self._write("测试用例结束时间: %s\n" % time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.end_time)))
-        self._write("测试用例执行时间: %02d:%02d:%02.2f\n" % _convert_timelength(self.end_time - self.begin_time))
+        name = "用例"
+        if self.is_testsuite():
+            name = "套"
+
+        self._write(
+            "测试%s开始时间: %s\n"
+            % (
+                name,
+                time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time)),
+            )
+        )
+        self._write(
+            "测试%s结束时间: %s\n"
+            % (name, time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.end_time)))
+        )
+        items = list(_convert_timelength(self.end_time - self.begin_time))
+        items.insert(0, name)
+        self._write("测试%s执行时间: %02d:%02d:%02.2f\n" % tuple(items))
 
-        rsttxts = {True:'通过', False:'失败'}
+        rsttxts = {True: "通过", False: "失败"}
         test_result = rsttxts[passed]
         if self._custom_result:
             test_result = dict(RESULT_TYPES)[self._custom_result]
-        steptxt = ''
+        steptxt = ""
         for i, ipassed in enumerate(self._step_results):
             steptxt += " %s:%s" % (i + 1, rsttxts[ipassed])
-        self._write("测试用例步骤结果: %s\n" % steptxt)
-        self._write("测试用例最终结果: %s\n" % test_result)
+        self._write("测试%s步骤结果: %s\n" % (name, steptxt))
+        self._write("测试%s最终结果: %s\n" % (name, test_result))
         self._write(self._seperator2)
 
     def handle_step_begin(self, msg):
-        '''处理一个测试步骤的开始
+        """处理一个测试步骤的开始
 
         :param msg: 测试步骤名称
         :type msg: string
-        '''
+        """
         if not isinstance(msg, six.string_types):
             raise ValueError("msg='%r'必须是string类型" % msg)
 
         self._write(self._seperator1)
         self._write("步骤%s: %s\n" % (len(self._step_results) + 1, msg))
 
     def handle_step_end(self, passed):
-        '''处理一个测试步骤的结束
+        """处理一个测试步骤的结束
 
         :param passed: 测试步骤是否通过
         :type passed: boolean
-        '''
+        """
         self._step_results.append(passed)
 
     def handle_log_record(self, level, msg, record, attachments):
-        '''处理一个日志记录
+        """处理一个日志记录
 
         :param level: 日志级别，参考EnumLogLevel
         :type level: string
         :param msg: 日志消息
         :type msg: string
         :param record: 日志记录
         :type record: dict
         :param attachments: 附件
         :type attachments: dict
-        '''
+        """
         self._write("%s: %s\n" % (levelname[level], msg))
 
         if level == EnumLogLevel.ASSERT:
             if "actual" in record:
                 actual = record["actual"]
                 self._write("   实际值：%s%s\n" % (actual.__class__, actual))
             if "expect" in record:
                 expect = record["expect"]
                 self._write("   期望值：%s%s\n" % (expect.__class__, expect))
             if "code_location" in record:
-                self._write(smart_text('  File "%s", line %s, in %s\n' % record["code_location"]))
+                self._write(
+                    smart_text(
+                        '  File "%s", line %s, in %s\n' % record["code_location"]
+                    )
+                )
 
         if "traceback" in record:
             self._write(smart_text_by_lines("%s\n" % record["traceback"]))
 
         for name in attachments:
             file_path = smart_text(attachments[name])
             if path_exists(file_path):
                 file_path = os.path.abspath(file_path)
             self._write("   %s:%s\n" % (smart_text(name), file_path))
 
 
 class XmlResult(TestResultBase):
-    '''xml格式的测试用例结果
-    '''
+    """xml格式的测试用例结果"""
 
     def __init__(self, testcase):
-        '''构造函数
+        """构造函数
 
         :param file_path: XML文件路径
         :type file_path: string
-        '''
+        """
         super(XmlResult, self).__init__()
         self._xmldoc = dom.Document()
         translated_name = translate_bad_char(testcase.test_name)
         max_name_len = 200
         if len(translated_name) > max_name_len:
             translated_name = translated_name[:max_name_len]
-        self._file_path = '%s_%s.xml' % (translated_name, get_time_str())
+        self._file_path = "%s_%s.xml" % (translated_name, get_time_str())
 
     @property
     def file_path(self):
-        '''xml文件路径
+        """xml文件路径
 
         :returns: str
-        '''
+        """
         return self._file_path
 
     def handle_test_begin(self, testcase):
-        '''处理一个测试用例执行的开始
+        """处理一个测试用例执行的开始
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
-        self._xmldoc.appendChild(self._xmldoc.createProcessingInstruction("xml-stylesheet", 'type="text/xsl" href="TestResult.xsl"'))
-        owner = getattr(testcase, 'owner', None)
-        priority = getattr(testcase, 'priority', None)
-        timeout = getattr(testcase, 'timeout', None)
-        self._testnode = self._xmldoc.createElement('TEST')
-        self._testnode.setAttribute("name", smart_text(saxutils.escape(testcase.test_name)))
+        """
+        self._xmldoc.appendChild(
+            self._xmldoc.createProcessingInstruction(
+                "xml-stylesheet", 'type="text/xsl" href="TestResult.xsl"'
+            )
+        )
+        owner = getattr(testcase, "owner", None)
+        priority = getattr(testcase, "priority", None)
+        timeout = getattr(testcase, "timeout", None)
+        self._testnode = self._xmldoc.createElement("TEST")
+        self._testnode.setAttribute(
+            "name", smart_text(saxutils.escape(testcase.test_name))
+        )
         self._testnode.setAttribute("owner", smart_text(saxutils.escape(str(owner))))
         self._testnode.setAttribute("priority", str(priority))
         self._testnode.setAttribute("timeout", str(timeout))
-        self._testnode.setAttribute('begintime', time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time)))
+        self._testnode.setAttribute(
+            "begintime",
+            time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time)),
+        )
         extra_properties = testcase.get_test_extra_properties()
         for k, v in extra_properties.items():
             self._testnode.setAttribute(k, str(v))
         if hasattr(testcase, "tags"):
             tag_str = "|".join(testcase.tags)
             if tag_str:
                 tag_str = "|%s|" % tag_str
             self._testnode.setAttribute("tags", smart_text(saxutils.escape(tag_str)))
         self._xmldoc.appendChild(self._testnode)
 
-        self.begin_step('测试用例初始步骤')
+        self.begin_step("测试用例初始步骤")
 
     def handle_test_end(self, passed):
-        '''处理一个测试用例执行的结束
+        """处理一个测试用例执行的结束
 
         :param passed: 测试用例是否通过
         :type passed: boolean
-        '''
+        """
         test_result = str(passed)
         if self._custom_result:
             test_result = str(self._custom_result)
-        self._testnode.setAttribute('result', test_result)
-        self._testnode.setAttribute('endtime', time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.end_time)))
-        self._testnode.setAttribute('duration', "%02d:%02d:%02.2f\n" % _convert_timelength(self.end_time - self.begin_time))
+        self._testnode.setAttribute("result", test_result)
+        if self._custom_reason:
+            self._testnode.setAttribute("reason", self._custom_reason)
+        self._testnode.setAttribute(
+            "endtime", time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.end_time))
+        )
+        self._testnode.setAttribute(
+            "duration",
+            "%02d:%02d:%02.2f\n" % _convert_timelength(self.end_time - self.begin_time),
+        )
+        if self.failed_stages:
+            self._testnode.setAttribute("failed_stages", "|".join(self.failed_stages))
         if self._file_path:
-            with codecs_open(smart_text(self._file_path), 'wb') as fd:
+            with codecs_open(smart_text(self._file_path), "wb") as fd:
                 fd.write(to_pretty_xml(self._xmldoc))
 
     def handle_step_begin(self, msg):
-        '''处理一个测试步骤的开始
+        """处理一个测试步骤的开始
 
         :param msg: 测试步骤名称
         :type msg: string
-        '''
+        """
         if not isinstance(msg, six.string_types):
             raise ValueError("msg='%r'必须是string类型" % msg)
         self._stepnode = self._xmldoc.createElement("STEP")
-        self._stepnode.setAttribute('title', smart_text(msg))
-        self._stepnode.setAttribute('time', time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time())))
+        self._stepnode.setAttribute("title", smart_text(msg))
+        self._stepnode.setAttribute(
+            "time", time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time()))
+        )
         self._testnode.appendChild(self._stepnode)
 
     def handle_step_end(self, passed):
-        '''处理一个测试步骤的结束
+        """处理一个测试步骤的结束
 
         :param passed: 测试步骤是否通过
         :type passed: boolean
-        '''
-        self._stepnode.setAttribute('result', str(passed))
+        """
+        self._stepnode.setAttribute("result", str(passed))
 
     def handle_log_record(self, level, msg, record, attachments):
-        '''处理一个日志记录
+        """处理一个日志记录
 
         :param level: 日志级别，参考EnumLogLevel
         :type level: string
         :param msg: 日志消息
         :type msg: string
         :param record: 日志记录
         :type record: dict
         :param attachments: 附件
         :type attachments: dict
-        '''
+        """
         if not isinstance(msg, six.string_types):
             msg = str(msg)
 
         # 由于目前的报告系统仅支持部分级别的标签，所以这里先做转换
         if level >= EnumLogLevel.ERROR:
             tagname = levelname[EnumLogLevel.ERROR]
         elif level == EnumLogLevel.Environment or level == EnumLogLevel.RESOURCE:
@@ -645,36 +739,37 @@
                     exptxt = "%s%s" % (expect.__class__, repr(expect))
                 except UnicodeEncodeError:
                     exptxt = "%s%s" % (expect.__class__, repr(expect))
                 node.appendChild(self._xmldoc.createTextNode(exptxt))
                 infonode.appendChild(node)
 
         if "traceback" in record:
-            excnode = self._xmldoc.createElement('EXCEPT')
-            excnode.appendChild(self._xmldoc.createTextNode(smart_text(record["traceback"])))
+            excnode = self._xmldoc.createElement("EXCEPT")
+            excnode.appendChild(
+                self._xmldoc.createTextNode(smart_text(record["traceback"]))
+            )
             infonode.appendChild(excnode)
 
         for name in attachments:
             file_path = attachments[name]
-            attnode = self._xmldoc.createElement('ATTACHMENT')
-            attnode.setAttribute('filepath', smart_text(file_path))
+            attnode = self._xmldoc.createElement("ATTACHMENT")
+            attnode.setAttribute("filepath", smart_text(file_path))
             attnode.appendChild(self._xmldoc.createTextNode(smart_text(name)))
             infonode.appendChild(attnode)
 
     def toxml(self):
-        '''返回xml文本
+        """返回xml文本
 
         :returns string - xml文本
-        '''
+        """
         return to_pretty_xml(self._xmldoc)
 
 
 class JSONResult(TestResultBase):
-    '''JSON格式的结果
-    '''
+    """JSON格式的结果"""
 
     def __init__(self, testcase):
         super(JSONResult, self).__init__()
         self._steps = []
         self._data = {
             "testcase": testcase.test_name,
             "steps": self._steps,
@@ -682,121 +777,126 @@
         }
         self._translated_name = translate_bad_char(testcase.test_name)
 
     def get_data(self):
         return self._data
 
     def get_file(self):
-        file_name = '%s_%s.json' % (self._translated_name, get_time_str())
+        file_name = "%s_%s.json" % (self._translated_name, get_time_str())
         if not path_exists(file_name):
             content = json.dumps(self._data)
             with codecs_open(file_name, mode="w", encoding="utf-8") as fd:
                 fd.write(content)
         return file_name
 
     def handle_test_begin(self, testcase):
-        '''处理一个测试用例执行的开始
+        """处理一个测试用例执行的开始
 
         :param testcase: 测试用例
         :type testcase: TestCase
-        '''
+        """
         self.begin_step("测试用例初始化步骤")
 
     def handle_test_end(self, passed):
-        '''处理一个测试用例执行的结束
+        """处理一个测试用例执行的结束
 
         :param passed: 测试用例是否通过
         :type passed: boolean
-        '''
-        rsttxts = {True:'通过', False:'失败'}
+        """
+        rsttxts = {True: "通过", False: "失败"}
         test_result = rsttxts[passed]
         if self._custom_result:
             test_result = dict(RESULT_TYPES)[self._custom_result]
         self._data["result_type"] = test_result
         self._data["succeed"] = passed
-        self._data["start_time"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time))
-        self._data["end_time"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.end_time))
+        self._data["start_time"] = time.strftime(
+            "%Y-%m-%d %H:%M:%S", time.localtime(self.begin_time)
+        )
+        self._data["end_time"] = time.strftime(
+            "%Y-%m-%d %H:%M:%S", time.localtime(self.end_time)
+        )
         self._data["failed_info"] = self.failed_info
 
     def handle_step_begin(self, msg):
-        '''处理一个测试步骤的开始
+        """处理一个测试步骤的开始
 
         :param msg: 测试步骤名称
         :type msg: string
-        '''
-        self._steps.append({
-            "name": msg,
-            "start_time": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
-            "logs": []
-        })
+        """
+        self._steps.append(
+            {
+                "name": msg,
+                "start_time": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
+                "logs": [],
+            }
+        )
 
     def handle_step_end(self, passed):
-        '''处理一个测试步骤的结束
+        """处理一个测试步骤的结束
 
         :param passed: 测试步骤是否通过
         :type passed: boolean
-        '''
+        """
         curr_step = self._steps[-1]
         curr_step["succeed"] = passed
-        curr_step["end_time"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
+        curr_step["end_time"] = (time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),)
 
     def handle_log_record(self, level, msg, record, attachments):
-        '''处理一个日志记录
+        """处理一个日志记录
 
         :param level: 日志级别，参考EnumLogLevel
         :type level: string
         :param msg: 日志消息
         :type msg: string
         :param record: 日志记录
         :type record: dict
         :param attachments: 附件
         :type attachments: dict
-        '''
+        """
         curr_step = self._steps[-1]
-        curr_step["logs"].append({
-            "timestamp": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
-            "level": level,
-            "message": msg,
-            "record": record,
-            "attachments": attachments
-        })
+        curr_step["logs"].append(
+            {
+                "timestamp": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
+                "level": level,
+                "message": msg,
+                "record": record,
+                "attachments": attachments,
+            }
+        )
 
 
 class HtmlResult(JSONResult):
-    """html test result
-    """
+    """html test result"""
 
     def get_file(self):
-        file_name = '%s_%s.js' % (self._translated_name, get_time_str())
+        file_name = "%s_%s.js" % (self._translated_name, get_time_str())
         if not path_exists(file_name):
             var_name = os.path.basename(file_name)
             var_name = os.path.splitext(file_name)[0].replace(".", "_")
             content = "var %s = %s" % (var_name, json.dumps(self._data))
             content = smart_binary(content)
             with codecs_open(file_name, mode="wb") as fd:
                 fd.write(content)
         return file_name
 
 
-
 class TestResultCollection(list):
-    '''测试结果集合
-    '''
+    """测试结果集合"""
 
     def __init__(self, results, passed):
-        '''构造函数
+        """构造函数
 
         :param results: 测试结果列表
         :type results: list
         :param passed: 测试是否通过
         :type passed: boolean
-        '''
+        """
         super(TestResultCollection, self).__init__(results)
         self.__passed = passed
 
     @property
     def passed(self):
-        '''测试是否通过
+        """测试是否通过
 
         :returns: boolean
-        '''
+        """
         return self.__passed
```

### Comparing `qtaf-5.5.9/testbase/types.py` & `qtaf-5.6.0/testbase/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,67 +11,75 @@
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 """qtaf related types
 """
 
-import pkg_resources
 import traceback
 
+import pkg_resources
+
 from testbase import runner, report, resource, logger
 
 RUNNER_ENTRY_POINT = "qtaf.runner"
 REPORT_ENTRY_POINT = "qtaf.report"
 RESMGR_BACKEND_ENTRY_POINT = "qtaf.resmgr_backend"
 
 runner_types = {}
 report_types = {}
 resmgr_backend_types = {}
 
+
 def __init_runner_types():
-    global runner_types
+    global runner_types  # pylint: disable=invalid-name
     if runner_types:
         return
     runner_types["basic"] = runner.TestRunner
     runner_types["multithread"] = runner.ThreadingTestRunner
     runner_types["multiprocess"] = runner.MultiProcessTestRunner
     for ep in pkg_resources.iter_entry_points(RUNNER_ENTRY_POINT):
         if ep.name not in runner_types:
             try:
                 runner_types[ep.name] = ep.load()
-            except:
+            except Exception:  # pylint: disable=broad-except
                 stack = traceback.format_exc()
-                logger.warn("load TestRunner type for %s failed:\n%s" % (ep.name, stack))
+                logger.warn(
+                    "load TestRunner type for %s failed:\n%s" % (ep.name, stack)
+                )
 
 
 def __init_report_types():
-    global report_types
+    global report_types  # pylint: disable=invalid-name
     if report_types:
         return
-    report_types.update({
-        "empty"  : report.EmptyTestReport,
-        "stream" : report.StreamTestReport,
-        "xml"    : report.XMLTestReport,
-        "json"   : report.JSONTestReport,
-        "html"   : report.HtmlTestReport,
-    })
+    report_types.update(
+        {
+            "empty": report.EmptyTestReport,
+            "stream": report.StreamTestReport,
+            "xml": report.XMLTestReport,
+            "json": report.JSONTestReport,
+            "html": report.HtmlTestReport,
+        }
+    )
 
     # Register other `ITestReport` implementations from entry points
     for ep in pkg_resources.iter_entry_points(REPORT_ENTRY_POINT):
         if ep.name not in report_types:
             try:
                 report_types[ep.name] = ep.load()
-            except:
+            except Exception:  # pylint: disable=broad-except
                 stack = traceback.format_exc()
-                logger.warn("load ITestReport entry point for %s failed:\n%s" % (ep.name, stack))
+                logger.warn(
+                    "load ITestReport entry point for %s failed:\n%s" % (ep.name, stack)
+                )
 
 
 def __init_resmgr_backend_types():
-    global resmgr_backend_types
+    global resmgr_backend_types  # pylint: disable=invalid-name
     if resmgr_backend_types:
         return
     resmgr_backend_types["local"] = resource.LocalResourceManagerBackend
     for ep in pkg_resources.iter_entry_points(RESMGR_BACKEND_ENTRY_POINT):
         if ep.name not in resmgr_backend_types:
             resmgr_backend_types[ep.name] = ep.load()
 
@@ -80,8 +88,7 @@
 del __init_runner_types
 
 __init_report_types()
 del __init_report_types
 
 __init_resmgr_backend_types()
 del __init_resmgr_backend_types
-
```

### Comparing `qtaf-5.5.9/testbase/util.py` & `qtaf-5.6.0/testbase/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,73 +8,68 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 共用类模块
-'''
+"""
 
 import binascii
 import codecs
 import importlib
 import inspect
 import io
 import locale
 import os
-import pkg_resources
 import re
-import six
 import sys
 import threading
 import time
 import traceback
 
 from inspect import isclass, getmro, types
 from xml.dom.minidom import Node
 from datetime import datetime
 
+import pkg_resources
+import six
+
 from tuia.exceptions import TimeoutError
 
 default_locale = locale.getdefaultlocale()
 if default_locale:
     default_encoding = default_locale[1] or "utf-8"
 else:
-    default_encoding = "utf-8"
+    default_encoding = "utf-8"  # pylint: disable=invalid-name
 
 file_encoding = sys.getfilesystemencoding()
 file_encoding_lower = file_encoding.lower()
 for special_encoding in ["ansi", "ascii"]:
     if file_encoding_lower.find(special_encoding) >= 0:
-        file_encoding = "utf-8"
+        file_encoding = "utf-8"  # pylint: disable=invalid-name
         break
 file_encoding = file_encoding or "utf-8"
 
 
 class Timeout(object):
-    '''TimeOut类，实现超时重试逻辑
-    '''
+    """TimeOut类，实现超时重试逻辑"""
 
     def __init__(self, timeout=10, interval=0.5):
-        '''Constructor
+        """Constructor
 
         :param timeout: 超时秒数，默认是10
         :param interval: 重试时间间隔秒数，默认是0.5
-        '''
+        """
         self.timeout = float(timeout)
         self.interval = float(interval)
 
-    def retry(self,
-        func,
-        args,
-        exceptions=(),
-        resultmatcher=None,
-        nothrow=False):
+    def retry(self, func, args, exceptions=(), resultmatcher=None, nothrow=False):
         """多次尝试调用函数，成功则并返回调用结果，超时则根据选项决定抛出TimeOutError异常。
 
         :param func: 尝试调用的函数
         :type args: dict或tuple
         :param args: func函数的参数
         :type exceptions: tuple类型，tuple元素是异常类定义，如QPathError, 而不是异常实例，如QPathError()
         :param exceptions: 调用func时抛出这些异常，则重试。
@@ -102,48 +97,50 @@
                 if dict == type(args):
                     ret = func(**args)
                 elif tuple == type(args):
                     ret = func(*args)
                 else:
                     raise TypeError("args type %s is not a dict or tuple" % type(args))
 
-                if resultmatcher == None or resultmatcher(ret) == True:
+                if resultmatcher is None or resultmatcher(ret):
                     return ret
             except exceptions:
                 pass
 
             waited = time.time() - start
             if waited < self.timeout:
                 time.sleep(min(self.interval, self.timeout - waited))
-            elif try_count == 1 :
+            elif try_count == 1:
                 continue
             else:
                 if nothrow:
                     return ret
                 else:
                     raise TimeoutError("在%d秒里尝试了%d次" % (self.timeout, try_count))
 
-    def waitObjectProperty(self, obj, property_name, waited_value, regularMatch=False):
-        '''通过比较obj.property_name和waited_value，等待属性值出现。
+    def waitObjectProperty(
+        self, obj, property_name, waited_value, regularMatch=False
+    ):  # pylint: disable=invalid-name
+        """通过比较obj.property_name和waited_value，等待属性值出现。
                              如果属性值obj.property_name是字符类型则waited_value做为正则表达式进行比较。
                              比较成功则返回，超时则抛出TimeoutError异常。
 
         :param obj: 对象
         :param property_name: 要等待的obj对象的属性名
         :param waited_value: 要比较的的属性值，支持多层属性
         :param regularMatch: 参数 property_name和waited_value是否采用正则表达式的比较。
                                                                             默认为不采用（False）正则，而是采用恒等比较
-        '''
+        """
         start = time.time()
         waited = 0.0
         try_count = 0
         isstr = isinstance(waited_value, six.string_types)
         while True:
             objtmp = obj  # 增加多层属性支持
-            pro_names = property_name.split('.')
+            pro_names = property_name.split(".")
             for i in range(len(pro_names)):
                 propvalue = getattr(objtmp, pro_names[i])
                 objtmp = propvalue
 
             if isstr and regularMatch:  # 简化原逻辑
                 if None != re.search(waited_value, propvalue):
                     return
@@ -151,60 +148,63 @@
                 if waited_value == propvalue:
                     return
             try_count += 1
             waited = time.time() - start
             if waited < self.timeout:
                 time.sleep(min(self.interval, self.timeout - waited))
             else:
-                raise TimeoutError("对象属性值比较超时（%d秒%d次）：期望值:%s，实际值:%s，"
-                                   % (self.timeout, try_count, waited_value, propvalue))
+                raise TimeoutError(
+                    "对象属性值比较超时（%d秒%d次）：期望值:%s，实际值:%s，"
+                    % (self.timeout, try_count, waited_value, propvalue)
+                )
 
     def check(self, func, expect):
-        '''多次检查func的返回值是否符合expect设定的期望值，如果设定时间内满足，则返回True，否则返回False
+        """多次检查func的返回值是否符合expect设定的期望值，如果设定时间内满足，则返回True，否则返回False
 
         :param func: 尝试调用的函数
         :param expect: 设定的期望值
 
         :returns bool - 检查是否符合预期
-        '''
+        """
         start = time.time()
         waited = 0.0
         while True:
             if expect == func():
                 return True
             waited = time.time() - start
             if waited < self.timeout:
                 time.sleep(min(self.interval, self.timeout - waited))
             else:
                 return False
 
 
 class Singleton(type):
     """单实例元类，用于某个类需要实现单例模式。
-            使用方式示例如下::
-          import six
-          class MyClass(with_metaclass(Singleton, object)):
-              def __init__(self, *args, **kwargs):
-                  pass
+      使用方式示例如下::
+    import six
+    class MyClass(with_metaclass(Singleton, object)):
+        def __init__(self, *args, **kwargs):
+            pass
 
     """
+
     _instances = {}
 
     def __init__(cls, name, bases, dic):
         super(Singleton, cls).__init__(name, bases, dic)
         cls._instances = {}
 
     def __call__(self, *args, **kwargs):
         if self not in self._instances:
             self._instances[self] = super(Singleton, self).__call__(*args, **kwargs)
         return self._instances[self]
 
 
 class LazyInit(object):
-    '''实现延迟初始化
+    """实现延迟初始化
 
     使用方式示例::
 
         class _Win32Window(object)
             def click(self):
                 #......
         class Control(object):
@@ -216,66 +216,68 @@
             def click(self):
                 return self._initobj.click()
 
         ctrl = Control("/Name=xxx)
         ctrl.click()  # <-- call _init_window
         ctrl.click()
 
-    '''
+    """
 
     def __init__(self, obj, propname, init_func):
-        '''构造函数
-        '''
+        """构造函数"""
         self.__obj = obj
         self.__propname = propname
         self.__init_func = init_func
 
     def __getattr__(self, attrname):
         obj = self.__init_func()
         setattr(self.__obj, self.__propname, obj)
         attr = getattr(obj, attrname)
         del self.__obj
         del self.__propname
         del self.__init_func
         return attr
 
     def __setattr__(self, attrname, value):
-        if attrname in ['_LazyInit__obj', '_LazyInit__propname', '_LazyInit__init_func']:
+        if attrname in [
+            "_LazyInit__obj",
+            "_LazyInit__propname",
+            "_LazyInit__init_func",
+        ]:
             return super(LazyInit, self).__setattr__(attrname, value)
         obj = self.__init_func()
         setattr(self.__obj, self.__propname, obj)
         setattr(obj, attrname, value)
         del self.__obj
         del self.__propname
         del self.__init_func
 
 
 class ShareDataManager(object):
-    def __init__(self, lock=threading.Lock(), data={}):
+    def __init__(self, lock=threading.Lock(), data=None):
         self._data = data
+        if self._data is None:
+            self._data = {}
         self._lock = lock
 
     @property
     def data(self):
         return self._data
 
     def get(self, key):
         self._lock.acquire()
         data = self._data.get(key)
         self._lock.release()
         if not data:
             raise KeyError("No such key %s exists" % key)
-        return data.get('value', None)
+        return data.get("value", None)
 
     def set(self, key, value, level=0):
         self._lock.acquire()
-        self._data[key] = {
-            "value": value,
-            "level": level
-        }
+        self._data[key] = {"value": value, "level": level}
         self._lock.release()
 
     def pop(self, key):
         try:
             self._lock.acquire()
             data = self._data.pop(key)
         except KeyError:
@@ -291,53 +293,55 @@
         except KeyError:
             raise KeyError("No such key %s exists" % key)
         finally:
             self._lock.release()
 
 
 class ThreadGroupLocal(object):
-    '''使用线程组本地存储的元类
+    """使用线程组本地存储的元类
 
     - 当配合ThreadGroupScope使用，类似threading.local()提供的TLS变种，一个线程和其子孙线程共享一个存储
     详细使用方式请参考ThreadGroupScope类
 
     - 当不在ThreadGroupScope中使用时，行为和threading.local()一致
 
-    '''
+    """
 
     def __init__(self):
         curr_thread = threading.current_thread()
-#         if not hasattr(curr_thread, 'qtaf_group'):
-#             raise RuntimeError("current thread is not in any QTAF thread group scope")
-#         self.__data = curr_thread.qtaf_local
-        if hasattr(curr_thread, 'qtaf_group'):
+        #         if not hasattr(curr_thread, 'qtaf_group'):
+        #             raise RuntimeError("current thread is not in any QTAF thread group scope")
+        #         self.__data = curr_thread.qtaf_local
+        if hasattr(curr_thread, "qtaf_group"):
             self.__data = curr_thread.qtaf_local
         else:
-            if not hasattr(curr_thread, 'qtaf_local_outofscope'):
+            if not hasattr(curr_thread, "qtaf_local_outofscope"):
                 curr_thread.qtaf_local_outofscope = {}
             self.__data = curr_thread.qtaf_local_outofscope
 
     def __setattr__(self, name, value):
-        if name.startswith('_ThreadGroupLocal__'):
+        if name.startswith("_ThreadGroupLocal__"):
             super(ThreadGroupLocal, self).__setattr__(name, value)
         else:
             self.__data[name] = value
 
     def __getattr__(self, name):
-        if name.startswith('_ThreadGroupLocal__'):
+        if name.startswith("_ThreadGroupLocal__"):
             return super(ThreadGroupLocal, self).__getattr__(name)
         else:
             try:
                 return self.__data[name]
             except KeyError:
-                raise AttributeError("'ThreadGroupLocal' object has no attribute '%s'" % (name))
+                raise AttributeError(
+                    "'ThreadGroupLocal' object has no attribute '%s'" % (name)
+                )
 
 
 class ThreadGroupScope(object):
-    '''指定线程组作用域，进入这个作用域的线程，以及在其作用域内创建的线程都同属于一个线程组
+    """指定线程组作用域，进入这个作用域的线程，以及在其作用域内创建的线程都同属于一个线程组
 
     使用示例如下::
 
         def _thread_proc():
             ThreadGroupLocal().counter +=1
 
         with ThreadGroupScope("test_group"):
@@ -346,116 +350,136 @@
             t.start()
             t.join()
             t = threading.Thread(target=_thread_proc)
             t.start()
             t.join()
             assert ThreadGroupLocal().counter == 2
 
-    '''
+    """
 
     def __init__(self, name):
-        '''构造函数
+        """构造函数
 
         :param name: 线程组名称，全局唯一
         :type name: string
-        '''
+        """
         self._name = name
 
     def __enter__(self):
         curr_thread = threading.current_thread()
-        if hasattr(curr_thread, 'qtaf_local'):
+        if hasattr(curr_thread, "qtaf_local"):
             raise RuntimeError("ThreadGroupScope cannot be nested")
         curr_thread.qtaf_local = {}
         curr_thread.qtaf_group = self._name
 
     def __exit__(self, *exc_info):
         del threading.current_thread().qtaf_local
         del threading.current_thread().qtaf_group
 
     @staticmethod
     def current_scope():
-        '''返回当前线程所在的线程组作用域，如果不存在于任务线程组作用域，则返回None
-        '''
+        """返回当前线程所在的线程组作用域，如果不存在于任务线程组作用域，则返回None"""
         curr_thread = threading.current_thread()
-        if hasattr(curr_thread, 'qtaf_group'):
+        if hasattr(curr_thread, "qtaf_group"):
             return curr_thread.qtaf_group
 
 
+class TimeoutLock(object):
+    """Lock with timeout"""
+
+    def __init__(self, timeout=None):
+        self._timeout = timeout
+        self._lock = threading.RLock()
+
+    def acquire(self, blocking=True, timeout=-1):
+        if timeout <= 0:
+            timeout = self._timeout
+        return self._lock.acquire(blocking, timeout)
+
+    def release(self):
+        try:
+            self._lock.release()
+        except RuntimeError:
+            pass
+
+    def __enter__(self):
+        acquired = self.acquire()
+        return acquired
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.release()
+
+
 _origin_thread_start_func = threading.Thread.start
 
 
 def _thread_start_func(self, *args, **kwargs):
-    '''用于劫持threading.Thread.start函数
-    '''
+    """用于劫持threading.Thread.start函数"""
     curr_thread = threading.current_thread()
-    if hasattr(curr_thread, 'qtaf_group'):
+    if hasattr(curr_thread, "qtaf_group"):
         self.qtaf_group = curr_thread.qtaf_group
         self.qtaf_local = curr_thread.qtaf_local
     return _origin_thread_start_func(self, *args, **kwargs)
 
 
 threading.Thread.start = _thread_start_func
 
 
-def ForbidOverloadMethods(func_name_list):
-    '''生成metaclass用于指定基类禁止子类重载函数
-    '''
+def ForbidOverloadMethods(func_name_list):  # pylint: disable=invalid-name
+    """生成metaclass用于指定基类禁止子类重载函数"""
 
     class _metaclass(type):
-
         def __init__(cls, name, bases, dic):
             if len(bases) == 1 and bases[0] == object:
                 super(_metaclass, cls).__init__(name, bases, dic)
             else:
                 for it in func_name_list:
                     if it in dic.keys():
                         raise RuntimeError("不允许%s重载函数: %s" % (cls.__name__, it))
                 super(_metaclass, cls).__init__(name, bases, dic)
 
     return _metaclass
 
 
-class classproperty(object):
-    '''类属性修饰器
-    '''
+class classproperty(object):  # pylint: disable=invalid-name
+    """类属性修饰器"""
 
     def __init__(self, getter):
         self.getter = getter
 
     def __get__(self, instance, owner):
         return self.getter(owner)
 
 
 def smart_text(s, decoding=None):
-    '''convert any text or binary to text
+    """convert any text or binary to text
     py2 text: utf-8 bytes
     py3 text: unicode
-    '''
+    """
     if not isinstance(s, (six.string_types, six.binary_type)):
         raise RuntimeError("string or binary type didn't match with %r" % s)
     if six.PY3:
         if isinstance(s, six.text_type):
             return s
         else:
             try:
-                return s.decode('utf8')
+                return s.decode("utf8")
             except UnicodeDecodeError:  # other encoding
                 try:
                     if decoding is None:
                         decoding = default_encoding
                     return s.decode(decoding)
                 except UnicodeDecodeError:  # mixed encoding
                     return repr(s)
     else:
         return smart_binary(s, decoding=decoding)  # py2
 
 
-def  smart_binary(s, encoding="utf8", decoding=None):
-    '''convert any text or binary to binary of specified encoding
-    '''
+def smart_binary(s, encoding="utf8", decoding=None):
+    """convert any text or binary to binary of specified encoding"""
     if not isinstance(s, (six.string_types, six.binary_type)):
         raise RuntimeError("string or binary type didn't match with %r" % s)
     if isinstance(s, six.text_type):
         try:
             return s.encode(encoding)
         except UnicodeEncodeError:
             if six.PY3:
@@ -496,35 +520,35 @@
 def smart_from_hex(s):
     s = smart_binary(s)
     binary_s = binascii.unhexlify(s)
     return smart_text(binary_s)
 
 
 def smart_bytify(obj, encoding="utf-8", decoding=None):
-    """recursively convert objects from string types to binary
-    """
+    """recursively convert objects from string types to binary"""
     if isinstance(obj, dict):
         dic = {}
         for key, value in obj.items():
-            dic[smart_bytify(key, encoding, decoding)] = smart_bytify(value, encoding, decoding)
+            dic[smart_bytify(key, encoding, decoding)] = smart_bytify(
+                value, encoding, decoding
+            )
         return dic
     elif isinstance(obj, list):
         ls = []
         for element in obj:
             ls.append(smart_bytify(element, encoding, decoding))
         return ls
     elif isinstance(obj, six.string_types):
         return smart_binary(obj, encoding, decoding)
     else:
         return obj
 
 
 def smart_strfy(obj, decoding=None):
-    """recursively convert objects from binary to text
-    """
+    """recursively convert objects from binary to text"""
     if isinstance(obj, dict):
         dic = {}
         for key, value in obj.items():
             dic[smart_strfy(key, decoding)] = smart_strfy(value, decoding)
         return dic
     elif isinstance(obj, list):
         ls = []
@@ -534,19 +558,19 @@
     elif isinstance(obj, six.string_types):
         return smart_text(obj, decoding)
     else:
         return obj
 
 
 def get_thread_traceback(thread):
-    '''获取用例线程的当前的堆栈
+    """获取用例线程的当前的堆栈
 
     :param thread: 要获取堆栈的线程
     :type thread: Thread
-    '''
+    """
     for thread_id, stack in sys._current_frames().items():
         if thread_id != thread.ident:
             continue
         tb = "Traceback ( thread-%d possibly hold at ):\n" % thread_id
         for filename, lineno, name, line in traceback.extract_stack(stack):
             tb += '  File: "%s", line %d, in %s\n' % (filename, lineno, name)
             if line:
@@ -591,20 +615,18 @@
     for _ in range(back_count):
         frame = frame.f_back
     stack = "".join(traceback.format_stack(frame, 1))
     return stack
 
 
 def to_pretty_xml(doc, encoding="utf-8"):
-    """we need to ensure each line to be binary type
-    """
+    """we need to ensure each line to be binary type"""
 
     class _XMLWriter(codecs.StreamWriter):
-        """an inner writer to give writer a chance to handle each line
-        """
+        """an inner writer to give writer a chance to handle each line"""
 
         def write(self, data):
             data = smart_binary(data)
             self.stream.write(data)
 
     buff = io.BytesIO()
     indent = "    "
@@ -636,55 +658,60 @@
                     s = s.encode(encoding)
                 orig_stream_write_func(s)
 
             stream.write = _binary_write
             new_stream = stream
     else:
         if getattr(stream, "encoding", None):
-            if not stream.encoding.lower().startswith('ansi'):  # linux ascii
+            if not stream.encoding.lower().startswith("ansi"):  # linux ascii
                 encoding = stream.encoding
         new_stream = stream
     return new_stream, encoding
 
 
 def codecs_open(filename, mode="rb", encoding=None, errors="strict", buffering=1):
     filename = smart_binary(filename, encoding=file_encoding)
-    return codecs.open(filename, mode=mode, encoding=encoding, errors=errors, buffering=buffering)
+    return codecs.open(
+        filename, mode=mode, encoding=encoding, errors=errors, buffering=buffering
+    )
 
 
 def path_exists(filename):
     filename = smart_binary(filename, encoding=file_encoding)
     return os.path.exists(filename)
 
 
 def get_os_version():
-    if sys.platform == 'win32':
+    if sys.platform == "win32":
         with os.popen("ver") as pipe:
             osver = smart_text(pipe.read())
     else:
         osver = smart_text(str(os.uname()))  # @UndefinedVariable
     return osver
 
 
 if six.PY3:
     maketrans_func = str.maketrans
 else:
     import string
+
     maketrans_func = string.maketrans
 
 BAD_FILE_CHARS = r'\/*?:<>"|~#'
-BAD_VAR_CHAR = BAD_FILE_CHARS + '()[]+-=& '
-TRANS = maketrans_func(BAD_VAR_CHAR, '_' * len(BAD_VAR_CHAR))
+BAD_VAR_CHAR = BAD_FILE_CHARS + "()[]+-=& "
+TRANS = maketrans_func(BAD_VAR_CHAR, "_" * len(BAD_VAR_CHAR))
 BAD_VAR_CHAR_SET = set(BAD_VAR_CHAR)
 
 
 def translate_bad_char(input_string):
     if six.PY2:
         translated_string = smart_binary(input_string).translate(TRANS)
-        translated_string = re.sub(r'[^\x00-\x7f]', '', translated_string) # Replace non-ascii chars
+        translated_string = re.sub(
+            r"[^\x00-\x7f]", "", translated_string
+        )  # Replace non-ascii chars
     else:
         translated_string = smart_text(input_string).translate(TRANS)
     return translated_string
 
 
 def has_bad_char(input_string):
     if set(input_string) & BAD_VAR_CHAR_SET:
@@ -712,25 +739,28 @@
 
 
 def get_attribute_from_string(object_path):
     parts = object_path.split(".")
     parts_len = len(parts)
     mod = None
     for index in range(parts_len):
-        mod_path = ".".join(parts[:index + 1])
+        mod_path = ".".join(parts[: index + 1])
         try:
             mod = importlib.import_module(mod_path)
         except ImportError:
             break
     value = mod
     for new_index in range(index, parts_len):
         try:
             value = getattr(value, parts[new_index])
         except AttributeError:
-            raise AttributeError("%s has no attribute or submodule named \"%s\"" % (value, parts[new_index]))
+            raise AttributeError(
+                '%s has no attribute or submodule named "%s"'
+                % (value, parts[new_index])
+            )
     return value
 
 
 def getmembers(object, predicate=None):
     """Return all members of an object as (name, value) pairs sorted by name.
     Optionally, only return members that satisfy a given predicate."""
     if isclass(object):
@@ -744,15 +774,15 @@
     # this may result in duplicate entries if, for example, a virtual
     # attribute with the same name as a DynamicClassAttribute exists
     try:
         for base in object.__bases__:
             for k, v in base.__dict__.items():
                 if isinstance(v, types.DynamicClassAttribute):
                     names.append(k)
-    except:
+    except Exception:  # pylint: disable=broad-except
         pass
     for key in names:
         # First try to get the value via getattr.  Some descriptors don't
         # like calling their __get__ (see bug #1785), so fall back to
         # looking in the __dict__.
         try:
             value = getattr(object, key)
@@ -764,15 +794,15 @@
                 if key in base.__dict__:
                     value = base.__dict__[key]
                     break
             else:
                 # could be a (currently) missing slot member, or a buggy
                 # __dir__; discard and move on
                 continue
-        except:
+        except Exception:  # pylint: disable=broad-except
             continue
         if not predicate or predicate(value):
             results.append((key, value))
         processed.add(key)
     results.sort(key=lambda pair: pair[0])
     return results
```

### Comparing `qtaf-5.5.9/tuia/__init__.py` & `qtaf-5.6.0/tuia/webcontrols.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''Tuia：Tencent UI Automation Framework
-'''
 
+import warnings
+
+warnings.warn(
+    "`tuia.webcontrols` is depressed, please use `qt4c.webcontrols` instead",
+    DeprecationWarning,
+)
+from qt4c.webcontrols import *  # pylint: disable=wildcard-import
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qtaf-5.5.9/tuia/_tif.py` & `qtaf-5.6.0/tuia/_tif.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia._tif` is depressed, please use `qt4c._tif` instead", DeprecationWarning)
-from qt4c._tif import *
+
+warnings.warn(
+    "`tuia._tif` is depressed, please use `qt4c._tif` instead", DeprecationWarning
+)
+from qt4c._tif import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/accessible.py` & `qtaf-5.6.0/tuia/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# -*- coding: UTF8 -*-
+# -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-
-import warnings
-warnings.warn("`tuia.accessible` is depressed, please use `qt4c.accessible` instead", DeprecationWarning)
-
-from qt4c.accessible import *
+"""Tuia：Tencent UI Automation Framework
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtaf-5.5.9/tuia/app.py` & `qtaf-5.6.0/tuia/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.app` is depressed, please use `qt4c.app` instead", DeprecationWarning)
 
-from qt4c.app import App
+warnings.warn(
+    "`tuia.app` is depressed, please use `qt4c.app` instead", DeprecationWarning
+)
+
+from qt4c.app import App  # pylint: disable=unused-import
```

### Comparing `qtaf-5.5.9/tuia/control.py` & `qtaf-5.6.0/tuia/wincontrols.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.control` is depressed, please use `qt4c.control` instead", DeprecationWarning)
 
-from qt4c.control import Control, ControlContainer
+warnings.warn(
+    "`tuia.wincontrols` is depressed, please use `qt4c.wincontrols` instead",
+    DeprecationWarning,
+)
+from qt4c.wincontrols import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/env.py` & `qtaf-5.6.0/tuia/filedialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
-测试环境模块
-'''
 
 import warnings
 
-warnings.warn("`tuia.env` will be removed in the future", DeprecationWarning)
-
-class EnumEnvType(object):
-    '''测试机运行环境的类型
-    Local代表本机，Lab代表测试任务执行机
-    '''
-    Local, Lab = ('Local', 'Lab')
-
-run_env = EnumEnvType.Local
+warnings.warn(
+    "`tuia.filedialog` is depressed, please use `qt4c.filedialog` instead",
+    DeprecationWarning,
+)
+from qt4c.filedialog import *  # pylint: disable=wildcard-import
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qtaf-5.5.9/tuia/exceptions.py` & `qtaf-5.6.0/tuia/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 异常模块定义
-'''
+"""
+
 
 class ControlNotFoundError(Exception):
-    '''控件没有找到
-    '''
+    """控件没有找到"""
+
     pass
 
+
 class ControlAmbiguousError(Exception):
-    '''找到多个控件
-    '''
+    """找到多个控件"""
+
     pass
 
+
 class ControlExpiredError(Exception):
-    '''控件失效错误
-    '''
+    """控件失效错误"""
+
     pass
 
+
 class TimeoutError(Exception):
-    '''超时异常
-    '''
-    pass
+    """超时异常"""
+
+    pass
```

### Comparing `qtaf-5.5.9/tuia/filedialog.py` & `qtaf-5.6.0/tuia/uiacontrols.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.filedialog` is depressed, please use `qt4c.filedialog` instead", DeprecationWarning)
-from qt4c.filedialog import *
+
+warnings.warn(
+    "`tuia.gfcontrols` is depressed, please use `qt4c.gfcontrols` instead",
+    DeprecationWarning,
+)
+from qt4c.uiacontrols import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/gfcontrols.py` & `qtaf-5.6.0/tuia/control.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.gfcontrols` is depressed, please use `qt4c.gfcontrols` instead", DeprecationWarning)
-from qt4c.gfcontrols import *
+
+warnings.warn(
+    "`tuia.control` is depressed, please use `qt4c.control` instead", DeprecationWarning
+)
+
+from qt4c.control import Control, ControlContainer  # pylint: disable=unused-import
```

### Comparing `qtaf-5.5.9/tuia/keyboard.py` & `qtaf-5.6.0/tuia/keyboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.keyboard` is depressed, please use `qt4c.keyboard` instead", DeprecationWarning)
-from qt4c.keyboard import Key, Keyboard, KeyInputError
+
+warnings.warn(
+    "`tuia.keyboard` is depressed, please use `qt4c.keyboard` instead",
+    DeprecationWarning,
+)
+from qt4c.keyboard import Key, Keyboard, KeyInputError  # pylint: disable=unused-import
```

### Comparing `qtaf-5.5.9/tuia/mouse.py` & `qtaf-5.6.0/tuia/gfcontrols.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.keyboard` is depressed, please use `qt4c.keyboard` instead", DeprecationWarning)
-from qt4c.mouse import Mouse, MouseClickType, MouseCursorType, MouseFlag
+
+warnings.warn(
+    "`tuia.gfcontrols` is depressed, please use `qt4c.gfcontrols` instead",
+    DeprecationWarning,
+)
+from qt4c.gfcontrols import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/qpath.py` & `qtaf-5.6.0/tuia/qpath.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
 
 try:
-    from qt4c.qpath import QPath, QPathError
-    warnings.warn("`tuia.qpath` is depressed, please use `qt4c.qpath` instead", DeprecationWarning)
+    from qt4c.qpath import QPath, QPathError  # pylint: disable=unused-import
+
+    warnings.warn(
+        "`tuia.qpath` is depressed, please use `qt4c.qpath` instead", DeprecationWarning
+    )
 except ImportError:
     try:
-        from qt4a.qpath import QPath, QPathError
-        warnings.warn("`tuia.qpath` is depressed, please use `qt4a.qpath` instead", DeprecationWarning)
+        from qt4a.qpath import QPath, QPathError  # pylint: disable=unused-import
+
+        warnings.warn(
+            "`tuia.qpath` is depressed, please use `qt4a.qpath` instead",
+            DeprecationWarning,
+        )
     except ImportError:
-        pass
+        pass
```

### Comparing `qtaf-5.5.9/tuia/qpathparser.py` & `qtaf-5.6.0/tuia/qpathparser.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 QPath解析器
 
 QPath是一个用于定位各个平台的UI控件（除Web控件）的查询语言。
 
  - QPath语法定义如下::
 
     QPath ::= Seperator QPath Seperator UIObjectLocator
     UIObjectLocator ::= UIObjectProperty PropertyConnector UIObjectLocator
-    UIObjectProperty ::= UIProperty 
-                        | RelationProperty 
+    UIObjectProperty ::= UIProperty
+                        | RelationProperty
                         | IndexProperty
-                        | UITypeProperty 
+                        | UITypeProperty
     UIProperty ::= PropertyName Operator Literal
     RelationProperty ::= MaxDepthIdentifier EqualOperator Literal
     IndexProperty ::= InstanceIdentifier EqualOperator Literal
     UITypeProperty ::= UITypeIdentifier EqualOperator StringLiteral
     MaxDepthIdentifier := "MaxDepth"
     InstanceIdentifier ::= "Instance"
     UITypeIdentifier := "UIType"
@@ -45,303 +45,297 @@
     IntegerLiteral ::= "[0-9]*"
     BooleanLiteral := "True" | "False" | "true" | "false"
 
 
  - 需要注意的是，QPath的属性名都是大小写无关的。
 
  - 简单举例如下::
- 
+
     / ClassName='TxGuiFoundation' && Caption~='QQ\d+' / name='mainpanel'
 
 
-'''
+"""
 from __future__ import absolute_import
 
-import six
 import types
 
+import six
+
 try:
     from .ply import lex, yacc
     from .ply.lex import TOKEN
 except ImportError:
     from ply import lex, yacc
     from ply.lex import TOKEN
 
 
 class QPathSyntaxError(Exception):
-    '''QPath语法错误
-    '''
+    """QPath语法错误"""
 
     def __init__(self, qpath_string, err_msg, lexpos):
-        '''Constructor
-        
+        """Constructor
+
         :param qpath_string: QPath字符串
         :type qpath_string: str
         :parma err_msg: 错误信息
         :type err_msg: str
         :param lexpos: 错误对应的词法位置
         :type lexpos: int
-        '''
+        """
         self.qpath_string = qpath_string
         self.msg = err_msg
         self.lexpos = lexpos
 
     def __str__(self):
-        return '%s\n  %s\n  %s^' % (self.msg, self.qpath_string, ' ' * self.lexpos)
+        return "%s\n  %s\n  %s^" % (self.msg, self.qpath_string, " " * self.lexpos)
 
 
 class QPathLexer(object):
-    '''QPath词法解析器
-    '''
+    """QPath词法解析器"""
 
-    tokens = ['SEPERATOR',
-              'EQUAL',
-              'MATCH',
-              'AND',
-              'BOOL_CONST',
-              'STRING_LITERAL',
-              'INT_CONST_DEC',
-              'INT_CONST_OCT',
-              'INT_CONST_HEX',
-              'PROPERTY',
-              'MINUS']
+    tokens = [
+        "SEPERATOR",
+        "EQUAL",
+        "MATCH",
+        "AND",
+        "BOOL_CONST",
+        "STRING_LITERAL",
+        "INT_CONST_DEC",
+        "INT_CONST_OCT",
+        "INT_CONST_HEX",
+        "PROPERTY",
+        "MINUS",
+    ]
 
     t_ignore = "\t "
-    t_EQUAL = r'='
-    t_MATCH = r'~='
-    t_AND = r'(&&)|(&)'
-    t_MINUS = r'-'
-    t_SEPERATOR = '/'
-
-    bad_match = r'~[^=*]'
-
-    t_PROPERTY = r'[a-zA-Z_][0-9a-zA-Z_]*'
-
-    boolean_constant = '(True)|(False)|(true)|(false)'
-
-    decimal_constant = '(0)|([1-9][0-9]*)'
-    octal_constant = '0[0-7]+'
-    hex_prefix = '0[xX]'
-    hex_digits = '[0-9a-fA-F]+'
+    t_EQUAL = r"="
+    t_MATCH = r"~="
+    t_AND = r"(&&)|(&)"
+    t_MINUS = r"-"
+    t_SEPERATOR = "/"
+
+    bad_match = r"~[^=*]"
+
+    t_PROPERTY = r"[a-zA-Z_][0-9a-zA-Z_]*"
+
+    boolean_constant = "(True)|(False)|(true)|(false)"
+
+    decimal_constant = "(0)|([1-9][0-9]*)"
+    octal_constant = "0[0-7]+"
+    hex_prefix = "0[xX]"
+    hex_digits = "[0-9a-fA-F]+"
     hex_constant = hex_prefix + hex_digits
 
-    bad_octal_constant = '0[0-7]*[89]'
+    bad_octal_constant = "0[0-7]*[89]"
 
     # simple_escape = r"""([a-zA-Z._~!=&\^\-\\?'"])"""
     # decimal_escape = r"""(\d+)"""
     # hex_escape = r"""(x[0-9a-fA-F]+)"""
     # bad_escape = r"""([\\][^a-zA-Z._~^!=&\^\-\\?'"x0-7])"""
     # escape_sequence = r"""(\\("""+simple_escape+'|'+decimal_escape+'|'+hex_escape+'))'
 
     escape_sequence_1 = r'''(?<=\\)"'''
     escape_sequence_2 = r"""(?<=\\)'"""
 
-    string_char_1 = r"""([^"]|""" + escape_sequence_1 + ')'
+    string_char_1 = r"""([^"]|""" + escape_sequence_1 + ")"
     string_literal_1 = '"' + string_char_1 + '*"'
     # bad_string_literal_1 = '"'+string_char_1+'*'+bad_escape+string_char_1+'*"'
 
-    string_char_2 = r"""([^']|""" + escape_sequence_2 + ')'
+    string_char_2 = r"""([^']|""" + escape_sequence_2 + ")"
     string_literal_2 = "'" + string_char_2 + "*'"
     # bad_string_literal_2 = "'"+string_char_2+'*'+bad_escape+string_char_2+"*'"
 
-    string_literal = '(' + string_literal_1 + ')|(' + string_literal_2 + ')'
+    string_literal = "(" + string_literal_1 + ")|(" + string_literal_2 + ")"
     # bad_string_literal = '('+bad_string_literal_1+')|('+bad_string_literal_2+')'
 
     @TOKEN(boolean_constant)
-    def t_BOOL_CONST(self, t):
-        if t.value.lower() == 'true':
+    def t_BOOL_CONST(self, t):  # pylint: disable=invalid-name
+        if t.value.lower() == "true":
             t.value = True
         else:
             t.value = False
         return t
 
     @TOKEN(hex_constant)
-    def t_INT_CONST_HEX(self, t):
+    def t_INT_CONST_HEX(self, t):  # pylint: disable=invalid-name
         t.value = int(t.value, 16)
         return t
 
     @TOKEN(octal_constant)
-    def t_INT_CONST_OCT(self, t):
+    def t_INT_CONST_OCT(self, t):  # pylint: disable=invalid-name
         t.value = int(t.value, 8)
         return t
 
     @TOKEN(decimal_constant)
-    def t_INT_CONST_DEC(self, t):
+    def t_INT_CONST_DEC(self, t):  # pylint: disable=invalid-name
         t.value = int(t.value)
         return t
 
     @TOKEN(string_literal)
-    def t_STRING_LITERAL(self, t):
+    def t_STRING_LITERAL(self, t):  # pylint: disable=invalid-name
         col = t.value[0]
         value = t.value[1:-1].replace("\\%s" % col, col)
         t.value = value
         return t
 
-#     @TOKEN(bad_string_literal)
-#     def t_BAD_STRING_LITERAL(self, t):
-#         self._error("字符串包含非法的转移字符", t)
+    #     @TOKEN(bad_string_literal)
+    #     def t_BAD_STRING_LITERAL(self, t):
+    #         self._error("字符串包含非法的转移字符", t)
 
     @TOKEN(bad_match)
-    def t_BAD_MATCH(self, t):
+    def t_BAD_MATCH(self, t):  # pylint: disable=invalid-name
         self._error("'~'后只能连接'='", t)
 
     def t_error(self, t):
-        msg = '存在非法字符: %s' % repr(t.value[0])
+        msg = "存在非法字符: %s" % repr(t.value[0])
         self._error(msg, t)
 
     def _error(self, msg, t):
-        '''错误通知
-        '''
+        """错误通知"""
         raise QPathSyntaxError(self._qpath_string, msg, t.lexpos)
 
     def input(self, qpath_string):  # @ReservedAssignment
-        '''词法分析输入
-        
+        """词法分析输入
+
         :param qpath_string: QPath字符串
         :type qpath_string: str
-        '''
+        """
         self._qpath_string = qpath_string
         self._lexer = lex.lex(object=self)
         self._lexer.input(qpath_string)
         return self
 
     def token(self):
-        '''解析并返回一个Token
-        '''
+        """解析并返回一个Token"""
         t = self._lexer.token()
         return t
 
 
 class PropertyName(object):
-    '''QPath属性名
-    '''
+    """QPath属性名"""
 
     def __init__(self, value, lexpos):
-        '''Constructor
-        
+        """Constructor
+
         :param value: 属性名字符串
         :type value: str
         :param lexpos: 对应的词法位置
         :type lexpos: int
-        '''
+        """
         self.value = value
         self.lexpos = lexpos
 
     def __str__(self):
-        return '<PropertyName value:%s lexpos:%s>' % (self.value, self.lexpos)
+        return "<PropertyName value:%s lexpos:%s>" % (self.value, self.lexpos)
 
 
 class Literal(object):
-    '''QPath属性常量值
-    '''
+    """QPath属性常量值"""
 
     def __init__(self, value, lexpos):
-        '''Constructor
-        
+        """Constructor
+
         :param value: 属性值常量
         :type value: str/int/bool
         :param lexpos: 对应的词法位置
         :type lexpos: int
-        '''
+        """
         self.value = value
         self.lexpos = lexpos
 
     def __str__(self):
-        return '<Literal value:%s lexpos:%s>' % (repr(self.value), self.lexpos)
+        return "<Literal value:%s lexpos:%s>" % (repr(self.value), self.lexpos)
 
 
 class Operator(object):
-    '''QPath操作符
-    '''
+    """QPath操作符"""
 
     def __init__(self, value, lexpos):
-        '''Constructor
-        
+        """Constructor
+
         :param value: 属性操作符
         :type value: str
         :param lexpos: 对应的词法位置
         :type lexpos: int
-        '''
+        """
         self.value = value
         self.lexpos = lexpos
 
     def __str__(self):
-        return '<Operator value:%s lexpos:%s>' % (repr(self.value), self.lexpos)
+        return "<Operator value:%s lexpos:%s>" % (repr(self.value), self.lexpos)
 
 
 class UIObjectProperty(object):
-    '''QPath属性
-    '''
+    """QPath属性"""
 
     def __init__(self, name, operator, value):
-        '''Constructor
-        
+        """Constructor
+
         :param name: 属性名
         :type name: PropertName
         :param operator: 属性操作符
         :type operator: Operator
         :param value: 属性值
         :type value: Literal
-        '''
+        """
         self.name = name
         self.operator = operator
         self.value = value
         self.lexpos = self.name.lexpos
 
     def __str__(self):
         return "<UIObjectProperty %s>" % (self.format())
 
     def format(self):
-        '''格式化字符串
-        
+        """格式化字符串
+
         :returns: str
-        '''
-        return '%s%s%s' % (self.name.value, self.operator.value, repr(self.value.value))
+        """
+        return "%s%s%s" % (self.name.value, self.operator.value, repr(self.value.value))
 
 
 class UIObjectLocator(object):
-    '''QPath Locator
-    '''
+    """QPath Locator"""
 
     def __init__(self, properties):
-        '''Constructor
-        
+        """Constructor
+
         :param properties: 属性字典
         :type properties: dict
-        '''
+        """
         self._prop_dict = {}
         for it in properties:
             self._prop_dict[it.name.value.upper()] = it
         self.lexpos = properties[0].lexpos
 
     def append(self, prop):
-        '''增加一个属性
-        
+        """增加一个属性
+
         :param prop: 属性
         :type prop: UIObjectProperty
-        '''
+        """
         self._prop_dict[prop.name.value.upper()] = prop
 
     def dumps(self):
-        '''序列化
-        
+        """序列化
+
         :returns: list
-        '''
+        """
         d = {}
         for name in self:
             prop = self[name]
             d[prop.name.value] = [prop.operator.value, prop.value.value]
         return d
 
     def format(self):
-        '''格式化字符串
-        
+        """格式化字符串
+
         :returns: str
-        '''
-        return ' & '.join([it.format() for it in self._prop_dict.values()])
+        """
+        return " & ".join([it.format() for it in self._prop_dict.values()])
 
     def __str__(self):
         return '<UIObjectLocator "%s">' % self.format()
 
     def __getitem__(self, name):
         return self._prop_dict.get(name.upper())
 
@@ -356,197 +350,204 @@
 
     def __iter__(self):
         return self._prop_dict.__iter__()
 
 
 class QPathParser(object):
     '''QPath语法解析器
-    
+
     QPath解析器解析QPath后会生成两个结构:
-    
+
     1. QPath结构列表：每一个UIObjectLocator用一个字典表示
     其中字典的键值为属性名，对应的值为一个长度为2的列表，第一个元素为操作符号，
     目前为字符串'='或'~='，第二个元素为属性值
-    
+
     2. QPath词法位置信息：和解析后的结构对应，每一个UIObjectLocator用一个字典表示
     其中字典的键值为属性名，对应的指为一个长度为3的列表，第一个元素为属性名的
     词法位置，第二个元素为操作符的词法位置，第三个元素为属性值的词法位置
-    
+
     比如以下的QPath::
-    
-        / ClassName="TxGuiFoundation" && Caption1~='QQ\d+' && Instance=-1 / UIType='GF' && name='mainpanel' && MaxDepth=10
-    
+
+        /ClassName="TxGuiFoundation" && Caption1~='QQ\d+' && Instance=-1 /UIType='GF' && name='main' && MaxDepth=10
+
     解析后得到的结构列表为::
-    
+
         [{'Caption1': ['~=', 'QQ\\d+'],
           'ClassName': ['=', 'TxGuiFoundation'],
           'Instance': ['=', -1]},
-         {'MaxDepth': ['=', 10], 
-          'UIType': ['=', 'GF'], 
+         {'MaxDepth': ['=', 10],
+          'UIType': ['=', 'GF'],
           'name': ['=', 'mainpanel']}]
 
     解析后得到的词法位置信息表为::
-    
+
         [{'CAPTION1': [33, 41, 43],
           'CLASSNAME': [2, 11, 12],
           'INSTANCE': [54, 62, 63]},
-         {'MAXDEPTH': [103, 111, 112], 
-          'NAME': [83, 87, 88], 
+         {'MAXDEPTH': [103, 111, 112],
+          'NAME': [83, 87, 88],
           'UITYPE': [68, 74, 75]}]
-    
+
     使用方法示例::
-    
-        qp ="""/ ClassName="TxGuiFoundation" && Caption1~='QQ\d+' && Instance='-1' / UIType='GF' && name='mainpanel' && MaxDepth='10'"""
+
+        qp = """/ClassName="TxGuiFoundation" && Instance='-1' /UIType='GF' && MaxDepth='10'"""
         parser = QPathParser()
         qpath_struct, lex_info = parser.parse(qp)
     '''
 
-    INT_TYPE_PROPNAMES = ['INSTANCE', 'MAXDEPTH']
+    INT_TYPE_PROPNAMES = ["INSTANCE", "MAXDEPTH"]
 
     class _NullStream(object):
-        '''模拟空设备
-        '''
+        """模拟空设备"""
 
         def write(self, *_):
             pass
 
     def __init__(self, verbose=False):
-        '''构造函数
-        
+        """构造函数
+
         :param verbose: 是否有log提示
         :type verbose: boolean
-        '''
+        """
         if verbose:
             self._logger = None
         else:
             self._logger = yacc.PlyLogger(self._NullStream())
 
     def parse(self, qpath_string):
-        '''返回解析后的结果
-        
+        """返回解析后的结果
+
         :param qpath_string: QPath字符串
         :type qpath_string: string
         :returns: list, list - 解析后结构, 词法位置信息
-        '''
+        """
         self._last_locator = None
         qpath_string = qpath_string.strip()
         self._lexer = QPathLexer()
         self.tokens = self._lexer.tokens
-        self._parser = yacc.yacc(module=self, debuglog=self._logger, errorlog=self._logger, write_tables=0)
+        self._parser = yacc.yacc(
+            module=self, debuglog=self._logger, errorlog=self._logger, write_tables=0
+        )
         self._qpath_string = qpath_string
         parsed_structs = []
         lex_structs = []
         for locator in self._parser.parse(qpath_string, self._lexer):
             parsed_structs.append(locator.dumps())
             lex_struct = {}
             for propname in locator:
                 prop = locator[propname]
-                lex_struct[prop.name.value] = [prop.name.lexpos, prop.operator.lexpos, prop.value.lexpos]
+                lex_struct[prop.name.value] = [
+                    prop.name.lexpos,
+                    prop.operator.lexpos,
+                    prop.value.lexpos,
+                ]
             lex_structs.append(lex_struct)
         return parsed_structs, lex_structs
 
     def _error(self, msg, p, pos):
-        '''提示错误
-        '''
+        """提示错误"""
         raise QPathSyntaxError(self._qpath_string, msg, pos)
 
     # 以下为YACC语法构造函数
     def p_qpath(self, p):
-        '''qpath : SEPERATOR qpath_content
-        '''
+        """qpath : SEPERATOR qpath_content"""
         p[0] = p[2]
 
     def p_qpath_content(self, p):
-        '''qpath_content : 
-                         | object_locator
-                         | qpath_content SEPERATOR object_locator
-        '''
+        """qpath_content :
+        | object_locator
+        | qpath_content SEPERATOR object_locator
+        """
         if len(p) == 2:
             p[0] = [p[1]]
         else:
             p[1].append(p[3])
             p[0] = p[1]
 
     def p_object_locator(self, p):
-        '''object_locator : prop
-                          | object_locator AND prop
-        '''
+        """object_locator : prop
+        | object_locator AND prop
+        """
         if len(p) == 2:
             p[0] = UIObjectLocator([p[1]])
         else:
             p[0] = p[1]
             p[0].append(p[3])
 
     def p_prop(self, p):
-        '''prop : prop_name operator prop_value
-        '''
+        """prop : prop_name operator prop_value"""
         if p[1].value.upper() in self.INT_TYPE_PROPNAMES:
-            if p[2].value == '~=':
+            if p[2].value == "~=":
                 self._error('"%s"属性不可以使用"~="操作符' % (p[1].value), p[2], p[2].lexpos)
             if not isinstance(p[3].value, int):
                 try:
                     p[3].value = int(p[3].value)
                 except ValueError:
-                    self._error('"%s"属性值不可为"%s"类型，必须为int类型' % (p[1].value, type(p[3].value)), p[3], p[3].lexpos)
-            if p[1].value.upper() == 'MAXDEPTH':
+                    self._error(
+                        '"%s"属性值不可为"%s"类型，必须为int类型' % (p[1].value, type(p[3].value)),
+                        p[3],
+                        p[3].lexpos,
+                    )
+            if p[1].value.upper() == "MAXDEPTH":
                 if p[3].value <= 0:
                     self._error("MaxDepth属性值必须>0", p[3], p[3].lexpos)
 
-        elif p[2].value == '~=':
+        elif p[2].value == "~=":
             if not isinstance(p[3].value, six.string_types):
-                self._error('操作符"~="不可以连接"%s"类型的属性' % (type(p[3].value)), p[2], p[2].lexpos)
+                self._error(
+                    '操作符"~="不可以连接"%s"类型的属性' % (type(p[3].value)), p[2], p[2].lexpos
+                )
 
         p[0] = UIObjectProperty(p[1], p[2], p[3])
 
     def p_prop_name(self, p):
-        '''prop_name : PROPERTY
-        '''
+        """prop_name : PROPERTY"""
         p[0] = PropertyName(p[1], p.lexpos(1))
 
     def p_operator(self, p):
-        '''operator : EQUAL
-                    | MATCH
-        '''
+        """operator : EQUAL
+        | MATCH
+        """
         p[0] = Operator(p[1], p.lexpos(1))
 
     def p_prop_value(self, p):
-        '''prop_value : STRING_LITERAL
-                      | BOOL_CONST
-                      | int_const
-        '''
-#         if isinstance(p[1], types.StringTypes) and len(p[1]) == 0:
-#             self._error("属性值不可为空", p, p.lexpos(1))
+        """prop_value : STRING_LITERAL
+        | BOOL_CONST
+        | int_const
+        """
+        #         if isinstance(p[1], types.StringTypes) and len(p[1]) == 0:
+        #             self._error("属性值不可为空", p, p.lexpos(1))
         if isinstance(p[1], Literal):
             p[0] = p[1]
         else:
             p[0] = Literal(p[1], p.lexpos(1))
 
     def p_int_const(self, p):
-        '''int_const : INT_CONST_DEC
-                     | INT_CONST_OCT
-                     | INT_CONST_HEX
-                     | MINUS int_const
-        '''
+        """int_const : INT_CONST_DEC
+        | INT_CONST_OCT
+        | INT_CONST_HEX
+        | MINUS int_const
+        """
         if len(p) == 2:
             p[0] = Literal(p[1], p.lexpos(1))
         else:
             p[0] = Literal(-p[2].value, p.lexpos(1))
 
     def p_error(self, p):
-        '''处理错误
-        '''
+        """处理错误"""
         if p is None:
             self._error("不完整的QPath", p, len(self._qpath_string))
         lexpos = p.lexpos
         if not isinstance(lexpos, types.IntType):  # 不是Token
             lexpos = p.lexpos(1)
         self._error("QPath语法错误", p, lexpos)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 
-    q = QPathParser().parse("/classname='UIATableCell' && label~='XXX.*群，\\d，ZZZ.*\:.+，.*\\d\:\\d' && visible=true")
-    x = "/classname='UIATableCell' && label~='XXX.*群，\\d.*\\,' && visible=true"
+    q = QPathParser().parse(
+        "/classname='UIATableCell' && label~='XXX.*群，\\d，ZZZ.*\:.+，.*\\d\:\\d' && visible=true"
+    )
 
     QPathParser().parse('/class="\\d\\""')
 
     QPathParser().parse("/class='\\d\:\"\\'xxx'")
```

### Comparing `qtaf-5.5.9/tuia/remoteprocessing.py` & `qtaf-5.6.0/tuia/remoteprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.remoteprocessing` is depressed, please use `qt4c.remoteprocessing` instead", DeprecationWarning)
-from qt4c.remoteprocessing import *
+
+warnings.warn(
+    "`tuia.remoteprocessing` is depressed, please use `qt4c.remoteprocessing` instead",
+    DeprecationWarning,
+)
+from qt4c.remoteprocessing import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/testcase.py` & `qtaf-5.6.0/tuia/accessible.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-#-*- coding: utf-8 -*
+# -*- coding: UTF8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.testcase` is depressed, please use `qt4c.testcase` instead", DeprecationWarning)
-from qt4c.testcase import *
+
+warnings.warn(
+    "`tuia.accessible` is depressed, please use `qt4c.accessible` instead",
+    DeprecationWarning,
+)
+
+from qt4c.accessible import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/uiacontrols.py` & `qtaf-5.6.0/tuia/mouse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.gfcontrols` is depressed, please use `qt4c.gfcontrols` instead", DeprecationWarning)
-from qt4c.uiacontrols import *
+
+warnings.warn(
+    "`tuia.keyboard` is depressed, please use `qt4c.keyboard` instead",
+    DeprecationWarning,
+)
+
+# pylint: disable=unused-import
+from qt4c.mouse import (
+    Mouse,
+    MouseClickType,
+    MouseCursorType,
+    MouseFlag,
+)
```

### Comparing `qtaf-5.5.9/tuia/webcontrols.py` & `qtaf-5.6.0/tuia/wintypes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
 import warnings
-warnings.warn("`tuia.webcontrols` is depressed, please use `qt4c.webcontrols` instead", DeprecationWarning)
-from qt4c.webcontrols import *
+
+warnings.warn(
+    "`tuia.wintypes` is depressed, please use `qt4c.wintypes` instead",
+    DeprecationWarning,
+)
+from qt4c.wintypes import *  # pylint: disable=wildcard-import
```

### Comparing `qtaf-5.5.9/tuia/wintypes.py` & `qtaf-5.6.0/tuia/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,32 @@
-#-*- coding: utf-8 -*
+# -*- coding: utf-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
+"""
+测试环境模块
+"""
 
 import warnings
-warnings.warn("`tuia.wintypes` is depressed, please use `qt4c.wintypes` instead", DeprecationWarning)
-from qt4c.wintypes import *
+
+warnings.warn("`tuia.env` will be removed in the future", DeprecationWarning)
+
+
+class EnumEnvType(object):
+    """测试机运行环境的类型
+    Local代表本机，Lab代表测试任务执行机
+    """
+
+    Local, Lab = ("Local", "Lab")
+
+
+run_env = EnumEnvType.Local  # pylint: disable=invalid-name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

