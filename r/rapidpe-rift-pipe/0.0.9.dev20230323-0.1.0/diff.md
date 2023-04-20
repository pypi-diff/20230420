# Comparing `tmp/rapidpe_rift_pipe-0.0.9.dev20230323.tar.gz` & `tmp/rapidpe_rift_pipe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.0.9.dev20230323.tar", last modified: Thu Mar 23 05:16:12 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.1.0.tar", last modified: Thu Apr 20 19:21:14 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.0.9.dev20230323.tar` & `rapidpe_rift_pipe-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.997842 rapidpe_rift_pipe-0.0.9.dev20230323/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-23 05:16:11.997842 rapidpe_rift_pipe-0.0.9.dev20230323/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.991842 rapidpe_rift_pipe-0.0.9.dev20230323/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.993842 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     7599 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)    14833 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/plot_intrinsic_posterior.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-03-23 05:16:11.999842 rapidpe_rift_pipe-0.0.9.dev20230323/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.991842 rapidpe_rift_pipe-0.0.9.dev20230323/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.995842 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35593 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    16803 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.991842 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config_files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.997842 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)     4488 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    30455 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)    10717 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/search_bias_bounds.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-03-23 05:15:48.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 05:16:11.996842 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1059 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 05:16:11.000000 rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.770469 rapidpe_rift_pipe-0.1.0/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.772469 rapidpe_rift_pipe-0.1.0/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)     9851 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-20 19:21:14.778469 rapidpe_rift_pipe-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.770469 rapidpe_rift_pipe-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.775469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-20 18:16:57.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37438 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18220 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.776469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-19 02:10:50.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31369 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-20 16:12:20.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.777469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-07 19:09:31.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-19 04:21:05.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:21:14.776469 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:21:14.000000 rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/COPYING` & `rapidpe_rift_pipe-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/PKG-INFO` & `rapidpe_rift_pipe-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.0.9.dev20230323
+Version: 0.1.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.1.0/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.1.0/bin/postscripts/cprofile_summary.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 """
 Creates cprofile summary page from RapidPE/RIFT results
 """
 
 __author__ = "Vinaya Valsan"
 
 import os
-import sys
 import shutil
 import pstats
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from glob import glob
 from argparse import ArgumentParser
 from rapidpe_rift_pipe.profiling import get_stats_profile
 from rapidpe_rift_pipe.utils import print_output
+
 optp = ArgumentParser()
 optp.add_argument("input_dir", help="path to event run dir")
-optp.add_argument( "--web-dir", default=None, help="path to web dir")
-optp.add_argument( "--output-dir", default=None, help="directory to save plots")
+optp.add_argument("--web-dir", default=None, help="path to web dir")
+optp.add_argument("--output-dir", default=None, help="directory to save plots")
 opts = optp.parse_args()
 
 input_dir = opts.input_dir
 
 if opts.output_dir:
     run_dir = opts.output_dir
 else:
     run_dir = input_dir
 summary_plot_dir = os.path.join(run_dir, "summary_plots")
 
-cprofile_html_file = open(summary_plot_dir + "/cprofile.html", "w")
+cprofile_html_file = open(os.path.join(summary_plot_dir, "cprofile.html"), "w")
 print_output(
     cprofile_html_file,
     """
 <html>
 <head>
 <link rel="stylesheet" href="stylesheet.css">
 <script src="https://www.kryogenix.org/code/browser/sorttable/sorttable.js"></script>
@@ -89,109 +89,116 @@
 Iter_level = []
 PRECOMPUTE_TIME = []
 LIKELIHOOD_EVALUATION_TIME = []
 PRESET_TIME = []
 ANALYZE_EVENT = []
 
 for n, ff in enumerate(file_list):
-    file_name = ff.split("/")[-1]
-    File_name.append(file_name)
-    ps = pstats.Stats(ff)
-    ps.strip_dirs()
-    timestamped_stats_profiles = []
-    iter_level = ff[ff.find("ILE_iteration") + len("ILE_iteration_") : -4]
-    stats_profile = get_stats_profile(ps)
-    all_func_profiles = stats_profile.func_profiles
-    all_keys = list(all_func_profiles.keys())
-    ILE_SCRIPT_RUNTIME.append(stats_profile.total_tt)
-    Iter_level.append(iter_level)
-    PRECOMPUTE_TIME.append(
-        all_func_profiles["PrecomputeLikelihoodTerms"].cumtime
-    )
-
-    # all_line_numbers = [all_func_profiles[k].line_number for k in all_keys]
-    # analyze_event_line = all_func_profiles['analyze_event'].line_number
-    # ind_lines_before_analyze_event = np.where(np.array(all_line_numbers)<analyze_event_line)[0]
-    # pre_func = np.array(all_keys)[ind_lines_before_analyze_event]
-    # preset_time = sum([all_func_profiles[k].tottime for k in pre_func])
-    # PRESET_TIME.append(preset_time)
-    LIKELIHOOD_EVALUATION_TIME.append(
-        all_func_profiles["likelihood_function"].cumtime
-    )
-    ANALYZE_EVENT.append(
-        all_func_profiles["analyze_event"].cumtime
-    )
-    if n == 0:
-        shutil.copyfile(ff,os.path.join(summary_plot_dir,file_name))
-        print_output(
-            cprofile_html_file, f"<details><summary>{file_name}</summary>"
-        )
-
-        print_output(cprofile_html_file, '<table class="sortable">')
-        print_output(cprofile_html_file,
-            f"""<caption>
-            Download cprofile stats file <a href='./{file_name}' download>here</a>
-            </caption>""")
-        print_output(cprofile_html_file, table_thread)
+    try:
+        file_name = ff.split("/")[-1]
+        ps = pstats.Stats(ff)
+        ps.strip_dirs()
+        timestamped_stats_profiles = []
+        iter_level = ff[ff.find("ILE_iteration") + len("ILE_iteration_") : -4]
+        stats_profile = get_stats_profile(ps)
+        all_func_profiles = stats_profile.func_profiles
+        all_keys = list(all_func_profiles.keys())
+        precompute_time = all_func_profiles[
+            "PrecomputeLikelihoodTerms"
+        ].cumtime
+
+        # all_line_numbers = [all_func_profiles[k].line_number for k in all_keys]
+        # analyze_event_line = all_func_profiles['analyze_event'].line_number
+        # ind_lines_before_analyze_event = np.where(np.array(all_line_numbers)<analyze_event_line)[0]
+        # pre_func = np.array(all_keys)[ind_lines_before_analyze_event]
+        # preset_time = sum([all_func_profiles[k].tottime for k in pre_func])
+        # PRESET_TIME.append(preset_time)
+        likelihood_evaluation_time = all_func_profiles[
+            "likelihood_function"
+        ].cumtime
+
+        analyze_event = all_func_profiles["analyze_event"].cumtime
+
+        ile_script_runtime = stats_profile.total_tt
+        if n == 0:
+            shutil.copyfile(ff, os.path.join(summary_plot_dir, file_name))
+            print_output(
+                cprofile_html_file, f"<details><summary>{file_name}</summary>"
+            )
 
-        print_output(cprofile_html_file, "<tbody>")
-        for func_key in all_keys:
+            print_output(cprofile_html_file, '<table class="sortable">')
             print_output(
                 cprofile_html_file,
-                f"""<tr>
-            <td>{all_func_profiles[func_key].ncalls}</td>
-            <td>{all_func_profiles[func_key].cumtime}</td>
-            <td>{all_func_profiles[func_key].percall_cumtime}</td>
-            <td>{all_func_profiles[func_key].line_number}</td>
-            <td>{all_func_profiles[func_key].file_name}</td>
-            <td>{all_func_profiles[func_key].func_name}</td>
-            </tr>""",
+                f"""<caption>
+                Download cprofile stats file <a href='./{file_name}' download>here</a>
+                </caption>""",
             )
-        print_output(cprofile_html_file, "</tbody></table></details>")
-
-
-save_data = np.column_stack(
-    [
-        File_name,
-        Iter_level,
-        ILE_SCRIPT_RUNTIME,
-        PRECOMPUTE_TIME,
-        LIKELIHOOD_EVALUATION_TIME,
-        ANALYZE_EVENT,
-    ]
-)
-np.savetxt(
-    f"{summary_plot_dir}/cprofile_summary.txt",
-    save_data,
-    header="FILENAME ITER_LEVEL ILE_SCRIPT_RUNTIME PRECOMPUTE_TIME LIKELIHOOD_EVALUATION_TIME ANALYZE_EVENT",
-    fmt="%s",
-)
+            print_output(cprofile_html_file, table_thread)
 
+            print_output(cprofile_html_file, "<tbody>")
+            for func_key in all_keys:
+                print_output(
+                    cprofile_html_file,
+                    f"""<tr>
+                <td>{all_func_profiles[func_key].ncalls}</td>
+                <td>{all_func_profiles[func_key].cumtime}</td>
+                <td>{all_func_profiles[func_key].percall_cumtime}</td>
+                <td>{all_func_profiles[func_key].line_number}</td>
+                <td>{all_func_profiles[func_key].file_name}</td>
+                <td>{all_func_profiles[func_key].func_name}</td>
+                </tr>""",
+                )
+            print_output(cprofile_html_file, "</tbody></table></details>")
+    except KeyError:
+        continue
+    File_name.append(file_name)
+    Iter_level.append(iter_level)
+    ILE_SCRIPT_RUNTIME.append(ile_script_runtime)
+    PRECOMPUTE_TIME.append(precompute_time)
+    LIKELIHOOD_EVALUATION_TIME.append(likelihood_evaluation_time)
+    ANALYZE_EVENT.append(analyze_event)
+
+if File_name != []:
+    save_data = np.column_stack(
+        [
+            File_name,
+            Iter_level,
+            ILE_SCRIPT_RUNTIME,
+            PRECOMPUTE_TIME,
+            LIKELIHOOD_EVALUATION_TIME,
+            ANALYZE_EVENT,
+        ]
+    )
+    np.savetxt(
+        f"{summary_plot_dir}/cprofile_summary.txt",
+        save_data,
+        header="FILENAME ITER_LEVEL ILE_SCRIPT_RUNTIME PRECOMPUTE_TIME LIKELIHOOD_EVALUATION_TIME ANALYZE_EVENT",
+        fmt="%s",
+    )
 
-unique_iter_levels = np.unique(Iter_level)
-
-
-plt.figure()
-plt.hist(PRECOMPUTE_TIME, bins=int(len(PRECOMPUTE_TIME) / 5))
-plt.xlabel("PRECOMPUTE_TIME(s)")
-plt.savefig(summary_plot_dir + "/cprofile_PRECOMPUTE_TIME_hist.png")
-
-
-plt.figure()
-plt.hist(ILE_SCRIPT_RUNTIME, bins=int(len(PRECOMPUTE_TIME) / 5))
-plt.xlabel("ILE_SCRIPT_RUNTIME(s)")
-plt.savefig(summary_plot_dir + "/cprofile_ILE_SCRIPT_RUNTIME_hist.png")
-
-
-plt.figure()
-plt.hist(ANALYZE_EVENT, bins=int(len(PRECOMPUTE_TIME) / 5))
-plt.xlabel("ANALYZE_EVENT(s)")
-plt.savefig(summary_plot_dir + "/cprofile_ANALYZE_EVENT_hist.png")
-
+    unique_iter_levels = np.unique(Iter_level)
 
-plt.figure()
-plt.hist(np.array(ILE_SCRIPT_RUNTIME)-np.array(ANALYZE_EVENT), bins=int(len(PRECOMPUTE_TIME) / 5))
-plt.xlabel("ILE_SCRIPT_RUNTIME-ANALYZE_EVENT (s)")
-plt.savefig(summary_plot_dir + "/cprofile_PRESET_TIME_hist.png")
+    plt.figure()
+    plt.hist(PRECOMPUTE_TIME, bins=int(len(PRECOMPUTE_TIME) / 5))
+    plt.xlabel("PRECOMPUTE_TIME(s)")
+    plt.savefig(summary_plot_dir + "/cprofile_PRECOMPUTE_TIME_hist.png")
+
+    plt.figure()
+    plt.hist(ILE_SCRIPT_RUNTIME, bins=int(len(PRECOMPUTE_TIME) / 5))
+    plt.xlabel("ILE_SCRIPT_RUNTIME(s)")
+    plt.savefig(summary_plot_dir + "/cprofile_ILE_SCRIPT_RUNTIME_hist.png")
+
+    plt.figure()
+    plt.hist(ANALYZE_EVENT, bins=int(len(PRECOMPUTE_TIME) / 5))
+    plt.xlabel("ANALYZE_EVENT(s)")
+    plt.savefig(summary_plot_dir + "/cprofile_ANALYZE_EVENT_hist.png")
+
+    plt.figure()
+    plt.hist(
+        np.array(ILE_SCRIPT_RUNTIME) - np.array(ANALYZE_EVENT),
+        bins=int(len(PRECOMPUTE_TIME) / 5),
+    )
+    plt.xlabel("ILE_SCRIPT_RUNTIME-ANALYZE_EVENT (s)")
+    plt.savefig(summary_plot_dir + "/cprofile_PRESET_TIME_hist.png")
 
 
 print_output(cprofile_html_file, "</body></html>")
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.1.0/bin/postscripts/create_summarypage.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 """
 Creates summary page from RapidPE/RIFT results
 """
 
 __author__ = "Vinaya Valsan"
 
 import os
-import sys
-import ast
 
 import subprocess as sp
 import numpy as np
 
 from tabulate import tabulate
 from glob import glob
 from argparse import ArgumentParser
 from urllib.parse import urlparse
+
+import rapidpe_rift_pipe.postscript_utils as postutils
+
 from rapidpe_rift_pipe.config import Config
 from rapidpe_rift_pipe.profiling import write_css_file
 from rapidpe_rift_pipe.utils import print_output
 
-
 optp = ArgumentParser()
 optp.add_argument("input_dir", help="path to event run dir")
 optp.add_argument("--web-dir", default=None, help="path to web dir")
 optp.add_argument("--output-dir", default=None, help="directory to save plots")
 opts = optp.parse_args()
 print("-----------Creating summary page--------------")
 input_dir = opts.input_dir
@@ -40,19 +40,19 @@
 os.makedirs(output_dir, exist_ok=True)
 write_css_file(output_dir, "stylesheet.css")
 
 if opts.output_dir:
     run_dir = opts.output_dir
 else:
     run_dir = input_dir
-summary_plot_dir = run_dir + "/summary_plots/"
+summary_plot_dir = os.path.join(run_dir, "summary_plots")
 
-os.system(f"cp {summary_plot_dir}* {output_dir}/")
+os.system(f"cp {summary_plot_dir}/* {output_dir}/")
 print(f"Summary page will be saved in {output_dir}")
-index_html_file = output_dir + "/summarypage.html"
+index_html_file = os.path.join(output_dir, "summarypage.html")
 
 html_file = open(index_html_file, "w")
 
 
 print_output(
     html_file,
     """
@@ -62,31 +62,30 @@
 <script src="https://www.kryogenix.org/code/browser/sorttable/sorttable.js"></script>
 </head>
 """,
 )
 
 print_output(html_file, "<body>")
 print_output(html_file, f"<h2>rundir = {run_dir}</h2>")
-event_info_file = input_dir + "/event_info_dict.txt"
-with open(event_info_file) as f:
-    contents = f.read()
-    dictionary = ast.literal_eval(contents)
+
+event_info = postutils.event_info(input_dir)
+
+event_info_dict = event_info.load_event_info()
 
 print_output(html_file, "<h1> Event Info  </h1>")
 print_output(
     html_file,
     f"""
-snr = {dictionary["snr"]} <br>
-approximant = {dictionary["approximant"]} <br>
-intrinsic_param = {dictionary["intrinsic_param"]} <br>
-event_time = {dictionary["event_time"]} <br>
+snr = {event_info_dict["snr"]} <br>
+approximant = {event_info_dict["approximant"]} <br>
+gstlal_recovered_param = {event_info_dict["intrinsic_param"]} <br>
+event_time = {event_info_dict["event_time"]} <br>
 """,
 )
-
-config = Config.load(input_dir + "/Config.ini")
+config = Config.load(os.path.join(input_dir, "Config.ini"))
 is_event = config.event.mode in {"sid", "gid"}
 if is_event:
     gracedb_url = urlparse(config.gracedb_url)
     if config.event.mode == "sid":
         event_id = config.event.superevent_id
         event_path = f"/superevents/{event_id}/view/"
     else:
@@ -96,49 +95,54 @@
     print_output(
         html_file, f'GraceDB url : <a href="{event_url}">{event_id}</a> <br>'
     )
 
 filelist = glob(output_dir + "/grid*png")
 print_output(html_file, "<h1> Grid Plots </h1>")
 for fname_full in sorted(filelist):
-    fname_split = fname_full.split("/")
-    fname = fname_split[-1]
+    fname = os.path.basename(fname_full)
     print_output(html_file, f'<img src="{fname}">')
 
 print_output(html_file, "<h1> Posterior Plots </h1>")
 
 
-filelist = glob(output_dir + f"/posterior*.png")
+filelist = glob(output_dir + "/posterior*.png")
 for fname_full in sorted(filelist):
-    fname_split = fname_full.split("/")
-    fname = fname_split[-1]
+    fname = os.path.basename(fname_full)
     print_output(html_file, f'<img src="{fname}">')
 
+filelist = glob(output_dir + "/p_astro*png")
+if filelist != []:
+    print_output(html_file, "<h1> Pastro </h1>")
+    for fname_full in sorted(filelist):
+        fname = os.path.basename(fname_full)
+        print_output(html_file, f"<br>{fname}")
+        print_output(html_file, f'<img src="{fname}">')
+
+
 print_output(html_file, "<h1> Skymaps </h1>")
 filelist = glob(output_dir + "/skymap*png")
 for fname_full in sorted(filelist):
-    fname_split = fname_full.split("/")
-    fname = fname_split[-1]
+    fname = os.path.basename(fname_full)
     print_output(html_file, f"<br>{fname}")
     print_output(html_file, f'<img src="{fname}">')
 
 
 print_output(html_file, """<h1> Timing </h1> """)
 
-if os.path.exists(f"{summary_plot_dir}/cprofile.html") == True:
+if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
     filelist = np.sort(glob(output_dir + "/cprofile*hist*png"))
     for fname_full in sorted(filelist):
-        fname_split = fname_full.split("/")
-        fname = fname_split[-1]
+        fname = os.path.basename(fname_full)
         print_output(html_file, f'<img src="{fname}">')
 
 
 # Total job time:
-condor_submit_time = int(dictionary["condor_submit_time"])
-job_timing_file = input_dir + "/job_timing.txt"
+condor_submit_time = int(event_info_dict["condor_submit_time"])
+job_timing_file = os.path.join(input_dir, "job_timing.txt")
 iteration_completion_time = []
 with open(job_timing_file) as f:
     lines = f.readlines()
     for line_id, line in enumerate(lines):
         line_split = line.split(" ")
         level_complete_time = float(line_split[1])
         iteration_completion_time.append(level_complete_time)
@@ -152,22 +156,22 @@
             print_output(
                 html_file,
                 f'<br> <font size="+2"> iteration level {line_split[0]} took '
                 f"{level_complete_time-iteration_completion_time[line_id-1]} s </font>",
             )
 
 
-if os.path.exists(f"{summary_plot_dir}/cprofile.html") == True:
+if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
     print_output(
         html_file,
         "<br><a href='cprofile.html'>Detailed cProfile info for a single ILE job</a>",
     )
 print_output(html_file, "<h1> Config.ini </h1>")
 
-with open(input_dir + "/Config.ini") as config_f:
+with open(os.path.join(input_dir, "Config.ini")) as config_f:
     for line in config_f:
         if line[0] != "#" and len(line.strip()) > 0:
             if line[0] == "[":
                 print_output(html_file, f"<br> <b> {line} </b>")
             else:
                 print_output(html_file, f"<br> {line}")
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.1.0/bin/postscripts/plot_skymap.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 
 import numpy as np
 import healpy as hp
 import matplotlib.pyplot as plt
 
 from argparse import ArgumentParser
 from matplotlib import rcParams
+from astropy.coordinates import SkyCoord
 from glob import glob
 from ligo.skymap import plot
 from ligo.skymap import postprocess
 
+import rapidpe_rift_pipe.postscript_utils as postutils
+
 optp = ArgumentParser()
 optp.add_argument("input_dir", help="path to event run dir")
-optp.add_argument( "--ratio-to-include", type=str, default=None, help="if specified, considers outputfile tagged by this from convert_result_to_txt.py ")
-optp.add_argument( "--output-dir", default=None, help="directory to save plots")
+optp.add_argument(
+    "--ratio-to-include",
+    type=str,
+    default=None,
+    help="if specified, considers outputfile tagged by this from convert_result_to_txt.py ",
+)
+optp.add_argument("--output-dir", default=None, help="directory to save plots")
 opts = optp.parse_args()
 
 
-print('---------------------Creating skymap---------------------')
+print("---------------------Creating skymap---------------------")
 input_dir = opts.input_dir
 
 ratio_to_include = opts.ratio_to_include
 
 if opts.output_dir:
     output_dir = opts.output_dir
 else:
@@ -110,8 +118,23 @@
 text = []
 pp = np.round((50, 90)).astype(int)
 ii = np.round(np.searchsorted(np.sort(cls), (50, 90)) * deg2perpix).astype(int)
 for i, p in zip(ii, pp):
     text.append("{:d}% area: {:d} deg²".format(p, i, grouping=True))
 ax.text(1, 1, "\n".join(text), transform=ax.transAxes, ha="right")
 
+
+event_info = postutils.event_info(input_dir)
+injection_info = event_info.load_injection_info()
+if injection_info is not None:
+    ax.plot_coord(
+        SkyCoord(
+            injection_info["longitude"], injection_info["latitude"], unit="rad"
+        ),
+        "*",
+        markerfacecolor="white",
+        markeredgecolor="black",
+        markersize=10,
+    )
+
+
 plt.savefig(f"{output_dir}/summary_plots/skymap_{namestr}.png")
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/setup.cfg` & `rapidpe_rift_pipe-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rapidpe_rift_pipe
-version = 0.0.9
+version = attr: rapidpe_rift_pipe.__version__
 description = Pipeline for running RapidPE and RIFT parameter estimation codes
 long_description = file: README.md
 keywords = parameter estimation, gravitational waves
 license = GPL-2+
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
@@ -17,38 +17,42 @@
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = True
 include_package_data = True
-packages = 
-	rapidpe_rift_pipe
+packages = find:
 package_dir = 
 	= src
 install_requires = 
 	numpy
 	matplotlib
 	h5py
 	tabulate
+	astropy
 	lalsuite
-	rift==0.0.15.7
-	rapid_pe==0.0.4
+	rift>=0.0.15.7,<0.0.15.9
+	rapid_pe>=0.1.0,<0.2.0
 scripts = 
 	bin/postscripts/convert_result_to_txt.py
 	bin/postscripts/create_summarypage.py
-	bin/postscripts/plot_intrinsic_posterior.py
+	bin/postscripts/compute_posterior.py
 	bin/postscripts/plot_skymap.py
 	bin/postscripts/cprofile_summary.py
 
+[options.packages.find]
+where = src
+
 [options.package_data]
 * = *.txt, *.rst
-rapidpe_rift_pipe.static = *.html, *.css, *.js
+rapidpe_rift_pipe.static = *
+rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230323
+tag_build = 
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         n_submitted = 0
         params_all = {}
         n_events = len(injections)
     else:
         n_events = 1
 
     for event_index in range(n_events):
-        os.chdir(init_directory)
+        #os.chdir(init_directory)
         if is_event:
             fmin_template = float(
                 config.integrate_likelihood_cmds_dict["fmin-template"]
             )
 
             # lvalert submission script workflow
             client = GraceDb(config.gracedb_url)
@@ -127,14 +127,18 @@
             if config.event.mode == 'sid':
                 sevent = client.superevent(config.event.superevent_id).json()
                 gracedb_id = sevent['preferred_event']
             elif config.event.mode == 'gid':
                 gracedb_id = config.event.gracedb_id
             else:
                 raise RuntimeError(f'Unknown mode {config.event.mode}')
+            mdc_event_injection_file = config.event.mdc_event_injection_file
+            is_mdc = mdc_event_injection_file is not None
+            if is_mdc:
+                mdc_time_offset = int(config.event.mdc_time_offset)
             gracedb_id = get_graceid_after_superevent_check(
                 gracedb_id, client,
                 output_parent_directory,
                 email_address_for_job_complete_notice,
             )
 
             event = client.event(gracedb_id).json()
@@ -151,14 +155,35 @@
             params = insp_type["SingleInspiral"][0]
             event_info = {}
             event_info["gracedb_id"] = gracedb_id
             event_info["event_time"] = construct_event_time_string(
                 params["end_time"], params["end_time_ns"],
             )
             event_info["snr"] = coinc["snr"]
+            event_info["likelihood"] = event["likelihood"]
+
+            if is_mdc:
+                mdc_xml_doc = ligolw_utils.load_filename(
+                        mdc_event_injection_file,
+                        contenthandler=ligolw.LIGOLWContentHandler,
+                        )
+                mdc_sim_inspiral_tbl = lsctables.SimInspiralTable.get_table(mdc_xml_doc)
+                list_of_keys = ["gpstime","mass1","mass2","spin1z","spin2z","distance","latitude","longitude"]
+                mdc_data_dict = {k: [] for k in list_of_keys}
+                for row in mdc_sim_inspiral_tbl:
+                    for key in list_of_keys:
+                        if key== 'gpstime':
+                           mdc_data_dict[key].append(row.geocent_end_time + 1e-9 * row.geocent_end_time_ns)
+                        else:
+                            mdc_data_dict[key].append(getattr(row,key))
+                time_diff_from_injections = np.absolute(np.array(mdc_data_dict['gpstime'])-float(event_info['event_time'])+mdc_time_offset)
+                nearest_inj_index = np.argmin(time_diff_from_injections)
+                mdc_injection_info = {k:0 for k in list_of_keys}
+                for k in list_of_keys:
+                    mdc_injection_info[k] = mdc_data_dict[k][nearest_inj_index]
         else:
             inj = injections[event_index]
             event_info = {}
             # TODO: double check this is still used
             if read_inj_index:
                 # Note: this is only true for the inj files I generated with
                 # generate_injections.
@@ -190,19 +215,20 @@
             if not os.path.isfile(event_info["cache_file"]):
                 sys.exit(
                     "ERROR: cache file doesn't exist: "
                     + event_info["cache_file"]
                 )
             event_info["output_event_ID"] = f"inj_{inj_index}"
             output_event_directory = event_info["output_event_ID"]
-            output_dir = os.path.join(
-                init_directory,
-                config.output_parent_directory, output_event_directory,
-                "",  # NOTE: trailing '/' might not be needed
-            )
+            output_dir = os.path.abspath(
+                    os.path.join(
+                        config.output_parent_directory, 
+                        output_event_directory,
+                        ),
+                    )
             event_all_iterations_fname = os.path.join(
                 output_dir, "event_all_iterations.dag",
             )
             if not os.path.isdir(output_dir):
                 os.makedirs(output_dir, exist_ok=True)
             elif os.path.isfile(event_all_iterations_fname):
                 # Skip this inejction if it has already been submitted
@@ -268,19 +294,15 @@
                     if use_event_spin or "spin1z" in intrinsic_param_to_search:
                         # SpinTaylorT4 is the fastest for spinning searches.
                         event_info["approximant"] = "SpinTaylorT4"
                     else:
                         # TaylorT2 is the fastest in general.
                         event_info["approximant"] = "TaylorT2"
 
-            output_dir = os.path.join(
-                init_directory,
-                config.output_parent_directory,
-                ""  # TODO: confirm trailing '/' is needed
-            )
+            output_dir = os.path.abspath(config.output_parent_directory)
             if not os.path.isdir(output_dir):
                 os.makedirs(output_dir, exist_ok=True)
 
             if packet != "":
                 packet_fname = os.path.join(output_dir, "lvalert_packet.txt")
                 with open(packet_fname, "w") as packet_file:
                     print(packet, file=packet_file)
@@ -292,15 +314,15 @@
                 if (float(params["mass1"]) +
                         float(params["mass2"])) > 10.0:
                     # Note: pp-plots injections used SEOBNRv4, NOT SEOBNRv4_ROM
                     event_info["approximant"] = "SEOBNRv4"
                 else:
                     # all approximants checked with BNS
                     event_info["approximant"] = "TaylorF2"
-        os.chdir(output_dir)
+        event_info["output_dir"] = output_dir
         if is_event:
             coinc_xml_filename = os.path.join(output_dir, "coinc.xml")
             # The PSD file name is set here, but it's written later because
             # sometimes it takes a while for the file to upload
             psd_filename = os.path.join(output_dir, "psd.xml.gz")
             skymap_filename = os.path.join(output_dir, "bayestar.fits")
 
@@ -338,42 +360,44 @@
                 # TODO: double-check these parentheses are intentionally placed
                 data_start_time = int(t_event - int(t_before))
                 data_end_time = int(t_event + 500)
 
                 data_type = config.event.frame_data_types[ifo]
                 # TODO: We should import gwdatafind and call the underlying
                 #       functions directly.
+                raw_cache_file_path = os.path.join(output_dir,f"{ifo[0]}_raw.cache")
                 dcmd = (
                     "python -m gwdatafind -u file "
                     f"-o {ifo[0]} -t {data_type} -s {data_start_time} "
-                    f"-e {data_end_time} > {ifo[0]}_raw.cache"
+                    f"-e {data_end_time} > {raw_cache_file_path}"
                 )
                 logging.info(dcmd)
                 exit_status = os.system(dcmd)
                 if exit_status != 0:
                     logging.error(dcmd)
                     sys.exit(f"ERROR: non zero exit status {exit_status}")
 
             # path2cache always assumes data is in output_dir, so that path
             # needs to be removed before passing output to data.cache
-            text_for_sed_removal = "localhost{}file:\\/".format(
-                output_dir.replace('/', '\\/')
+            text_for_sed_removal = "localhost{}\/file:\\/".format(
+                init_directory.replace('/', '\\/')
             )
             if shutil.which('lal_path2cache') is not None:
                 path2cache = 'lal_path2cache'
             else:
                 path2cache = 'lalapps_path2cache'
+            data_cache_file_path = os.path.join(output_dir,'data.cache')
             os.system(
-                "cat *_raw.cache "
+                f"cat {output_dir}/*_raw.cache "
                 f"| {path2cache} "
-                f"| sed 's/{text_for_sed_removal}//g' > data.cache"
+                f"| sed 's/{text_for_sed_removal}//g' > {data_cache_file_path}"
             )
 
             # Check if the data.cache file is empty
-            if os.stat("data.cache").st_size == 0:
+            if os.stat(data_cache_file_path).st_size == 0:
                 if lvalert and email_address_for_job_complete_notice != "":
                     email_cmd = (
                         f"Failed Lvalert, no data at trigger time "
                         f"{gracedb_id} | mail -s {output_parent_directory} "
                         f"          {email_address_for_job_complete_notice}"
                     )
                     # TODO: Instead of system call, should use Python's
@@ -381,15 +405,15 @@
                     os.system(email_cmd)
 
                 sys.exit(
                     "ERROR: There is no data at the time when this triggered, "
                     "how can that happen?"
                 )
             # Put together cache file
-            event_info["cache_file"] = os.path.join(output_dir, "data.cache")
+            event_info["cache_file"] = data_cache_file_path
             event_info["psd_file"] = psd_file_str[:-1] + "]"
             event_info["channel_name"] = channel_str[:-1] + "]"
             event_info["coinc_xml_file"] = coinc_xml_filename
 
         from . import create_submit_dag_one_event
         if config.submit_only_at_exact_signal_position:
             # Only submit one integrate job at the exact signal position
@@ -403,15 +427,15 @@
         else:
             # Create the initial grid for this event
             intrinsic_param = convert_list_string_to_dict(
                 event_info["intrinsic_param"]
             )
             exe = config.exe_grid_refine
 
-            intrinsic_grid_name_base = "intrinsic_grid"
+            intrinsic_grid_name_base = os.path.join(output_dir,"intrinsic_grid")
             initial_grid_xml = intrinsic_grid_name_base+"_iteration_0.xml.gz"
             initial_grid_hdf = intrinsic_grid_name_base+"_all_iterations.hdf"
             # now fill in the rest
             cmd = (
                 f"{exe} --verbose --no-exact-match --setup "
                 f"{initial_grid_hdf} --output-xml-file-name {initial_grid_xml}"
             )
@@ -685,15 +709,15 @@
                 sys.exit("ERROR: non zero exit status"+str(exit_status))
 
             print(
                 f"[initial_grid_xml={initial_grid_xml},"
                 f"initial_grid_hdf={initial_grid_hdf}]"
             )
 
-        intrinsic_grid_name_base = "intrinsic_grid"
+        intrinsic_grid_name_base = os.path.join(output_dir,"intrinsic_grid")
         event_info["initial_grid_xml"] = (
             f"{intrinsic_grid_name_base}_iteration_0.xml.gz"
         )
         event_info["initial_grid_hdf"] = (
             f"{intrinsic_grid_name_base}_all_iterations.hdf"
         )
 
@@ -736,14 +760,19 @@
                         r = client.files(
                             gracedb_id, 'bayestar.multiorder.fits'
                         )
                     for line in r:
                         skymapfileobj.write(line)
 
                 event_info["skymap_file"] = skymap_filename
+            if is_mdc:
+                with open(os.path.join(output_dir, "injection_info.txt"),'w') as injectionobj:
+                    json.dump(mdc_injection_info, injectionobj)
+
+
         # Run create_submit_dag
         event_info_list_strings_reformatted = {
             key : correct_list_string_formatting_if_list_string(val)
             for key, val in event_info.items()
         }
         create_submit_dag_one_event.main(
             config, event_info_list_strings_reformatted,
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import warnings
 from ast import literal_eval
 from typing import List, Optional
 from dataclasses import dataclass
 import json
 import shutil
+import getpass
 from rapidpe_rift_pipe.modules import *
 
 
 # Directory containing default config files
 DEFAULT_CONFIG_DIR = os.path.join(os.path.dirname(__file__), "config_files")
 
 
@@ -25,14 +26,15 @@
     # Path to the config file itself
     config_fname: Optional[str]
 
     # GraceDB settings
     gracedb_url: Optional[str]
     # Condor info
     accounting_group: str
+    accounting_group_user: str
     email_address_for_job_complete_notice: Optional[str]
     # Paths
     output_parent_directory: str
     injections_filename: str
     web_dir: Optional[str]
     # Sampling settings
     n_iterations_per_job: int
@@ -41,15 +43,16 @@
     # Flags
     # TODO: should convert from ints to bool (only have values 0 and 1 currently)
     event_params_in_cfg: bool
     overwrite_existing_event_dag: int
     submit_only_at_exact_signal_position: int
     submit_dag: int
     use_skymap: int
-    use_event_spin: Optional[bool]
+    use_event_spin: bool
+    cProfile: bool
 
     # Grid refinement options
     distance_coordinates: str
 
     # Executable paths
     exe_create_event_dag: str
 #    exe_compute_intrinsic_grid: str
@@ -64,27 +67,26 @@
     create_event_dag_condor_commands: dict
     grid_refine_info: dict
     grid_refine_condor_commands: dict
 
     # Mutually exclusive groups
     event: "EventConfig"
     initial_grid_setup: "InitialGridSetupConfig"
+    pastro: "Pastro"
 
     # Entire sections parsed as command line args
     initial_grid_only_cli_args: str
 
     @staticmethod
     def load(fname) -> "Config":
         from configparser import ConfigParser
 
         cfg = ConfigParser()
         cfg.optionxform = str
         cfg.read(fname)
-        if cfg.getint("General","event_parameters_in_config_file") == 1:
-            sys.exit("ERROR: this cfg file expects the event params to by in the cfg file, instead of passed from here")
 
         attrs = {}
 
         attrs["config_fname"] = fname
 
         ###########
         # General #
@@ -93,14 +95,18 @@
         attrs["gracedb_url"] = cfg.get(
             "General", "gracedb_url",
             fallback="https://gracedb.ligo.org/api/",
         )
 
         # Condor info
         attrs["accounting_group"] = cfg.get("General","accounting_group")
+        attrs["accounting_group_user"] = cfg.get(
+                "General","accounting_group_user",
+                fallback=getpass.getuser()
+                )
         attrs["email_address_for_job_complete_notice"] = cfg.get(
             "General", "email_address_for_job_complete_notice",
             fallback="",
         )
         attrs["web_dir"] = cfg.get(
             "General", "web_dir",
             fallback="",
@@ -115,26 +121,33 @@
         attrs["intrinsic_param_to_search"] = literal_eval(correct_list_string_formatting(
             cfg.get("General","intrinsic_param_to_search", fallback="[mass1,mass2]")
         ))
 
         # Flags
         attrs["event_params_in_cfg"] = cfg.getboolean(
             "General", "event_parameters_in_config_file",
+            fallback=False,
         )
+        if attrs["event_params_in_cfg"]:
+            raise ValueError(
+                "event_parameters_in_config_file=True is currently unsupported"
+            )
+
         attrs["overwrite_existing_event_dag"] = cfg.getint(
             "General", "overwrite_existing_event_dag",
             fallback=0,
         )
         attrs["submit_only_at_exact_signal_position"] = cfg.getint(
             "General", "submit_only_at_exact_signal_position",
             fallback=0,
         )
         attrs["submit_dag"] = cfg.getint("General", "submit_dag")
         attrs["use_skymap"] = cfg.getint("General", "use_skymap")
         attrs["use_event_spin"] = cfg.getboolean("General", "use_event_spin", fallback=False)
+        attrs["cProfile"] = cfg.getboolean("General", "cProfile", fallback=False)
         # Executables
         attrs["exe_create_event_dag"] = os.path.abspath(shutil.which(
             cfg.get(
                 "General", "exe_create_event_dag",
                 fallback="rapidpe_create_event_dag",
             )
         ))
@@ -180,14 +193,19 @@
         attrs["event"] = EventConfig(cfg)
 
         ####################
         # InitialGridSetup #
         ####################
         attrs["initial_grid_setup"] = InitialGridSetupConfig(cfg)
 
+        ##########
+        # Pastro #
+        ##########
+        attrs["pastro"] = PastroConfig(cfg)
+
         #####################
         # Sections as Dicts #
         #####################
         attrs["common_event_info"] = convert_section_args_to_dict(cfg, "Event")
         attrs["integrate_likelihood_cmds_dict"] = (
             convert_section_args_to_dict(cfg, "LikelihoodIntegration")
         )
@@ -238,14 +256,17 @@
 
 def parse_str(cfg, section, option, fallback=None):
     return cfg.get(section, option, fallback=fallback)
 
 def parse_int(cfg, section, option, fallback=None):
     return cfg.getint(section, option, fallback=fallback)
 
+def parse_float(cfg, section, option, fallback=None):
+    return cfg.getfloat(section, option, fallback=fallback)
+
 def parse_bool(cfg, section, option, fallback=None):
     return cfg.getboolean(section, option, fallback=fallback)
 
 def parse_list(cfg, section, option, fallback=None):
     if not cfg.has_option(section, option):
         return fallback
 
@@ -405,19 +426,35 @@
 
 
 _event_group_spec = {
     "gid" : {
         "gracedb_id" : {
             "parser" : parse_str,
         },
+        "mdc_event_injection_file" : {
+            "parser": parse_str,
+            "fallback": None
+        },
+        "mdc_time_offset" : {
+            "parser" : parse_str,
+            "fallback" : None
+        },
     },
     "sid" : {
         "superevent_id" : {
             "parser" : parse_str,
         },
+        "mdc_event_injection_file" : {
+            "parser": parse_str,
+            "fallback": None
+        },
+        "mdc_time_offset" : {
+            "parser" : parse_str,
+            "fallback" : None
+        },
     },
     "injections" : {
         "injections_file" : {
             "parser" : parse_str,
             "fallback" : "/home/caitlin.rose/my_rapidPE_work/f2y2016data/subset_f2y2016inj/exact_inj/f2y2016_HLV_100shuffled_exactmasses.txt",
         },
         "cache_file" : {
@@ -512,7 +549,28 @@
     },
 }
 
 InitialGridSetupConfig = _make_config_group(
     "InitialGridSetupConfig", "InitialGridSetup",
     _initial_grid_setup_spec,
 )
+
+
+_pastro_group_spec = {
+    "enabled" : {
+        "category_rates": {
+            "parser": parse_dict,
+        },
+        "prior_boundary": {
+            "parser": parse_dict,
+        },
+        "rankstat_pdf_file": {
+            "parser": parse_str,
+        },
+        "far_threshold": {
+            "parser": parse_float,
+        }
+    },
+    "disabled" : {}
+}
+
+PastroConfig = _make_config_group("PastroConfig", "Pastro", _pastro_group_spec)
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {'0': "{'limits': {1: {'lower': {'formula': 'v1', 'settings': {'const': -0.851577514511174}}}}}",*

 * * '2': "{'limits': {1: {'lower': {'formula': 'v1', 'settings': {'const': -0.851577514511174}}}}}",*

 * * '3': "{'limits': {1: {'lower': {'formula': 'v1', 'settings': {'const': -0.851577514511174}}}}}",*

 * * '5': "{'limits': {1: {'lower': {'formula': 'v1', 'settings': {'const': -0.851577514511174}}}}}"}*

```diff
@@ -18,17 +18,17 @@
                         "param_power": 0.6666666666667,
                         "reciprocal": true
                     }
                 }
             },
             {
                 "lower": {
-                    "formula": "const",
+                    "formula": "v1",
                     "settings": {
-                        "const": 0.4
+                        "const": -0.851577514511174
                     }
                 },
                 "param": "q",
                 "upper": {
                     "formula": "const",
                     "settings": {
                         "const": 1.0
@@ -102,17 +102,17 @@
                     "settings": {
                         "const": -0.0066063
                     }
                 }
             },
             {
                 "lower": {
-                    "formula": "const",
+                    "formula": "v1",
                     "settings": {
-                        "const": 0.5
+                        "const": -0.851577514511174
                     }
                 },
                 "param": "q",
                 "upper": {
                     "formula": "const",
                     "settings": {
                         "const": 1.0
@@ -150,17 +150,17 @@
                         "reciprocal": true,
                         "snr_power": -1.0
                     }
                 }
             },
             {
                 "lower": {
-                    "formula": "const",
+                    "formula": "v1",
                     "settings": {
-                        "const": 0.4
+                        "const": -0.851577514511174
                     }
                 },
                 "param": "q",
                 "upper": {
                     "formula": "const",
                     "settings": {
                         "const": 1.0
@@ -238,17 +238,17 @@
                         "const": -0.011057,
                         "snr_power": -0.2
                     }
                 }
             },
             {
                 "lower": {
-                    "formula": "const",
+                    "formula": "v1",
                     "settings": {
-                        "const": 0.5
+                        "const": -0.851577514511174
                     }
                 },
                 "param": "q",
                 "upper": {
                     "formula": "const",
                     "settings": {
                         "const": 1.0
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,39 +62,41 @@
     elif event_info is None:
         raise ValueError(
             "Need to pass dict of event args if event not in config."
         )
 
     event_info["dag_script_start_time"] = time.time()
 
-    output_dir =  os.getcwd()
+    output_dir =  event_info['output_dir']
+
 
 
     #
     # Create new working directory for the event
     #
     print(("The directory for this event is",output_dir))
     print ("The working dir will change to the above after initial grid generation, if generating the initial grid")
 #    if not os.path.isdir(init_directory+"/"+config.output_parent_directory):
 #        os.system("mkdir "+init_directory+"/"+config.output_parent_directory)
     if not os.path.isdir(output_dir):
         os.system("mkdir -p "+output_dir)
     elif not config.overwrite_existing_event_dag:
         sys.exit("ERROR: event directory already exists")
-    if not os.path.isdir(output_dir+"/logs"):
-        os.mkdir(output_dir+"/logs")
-        os.mkdir(output_dir+"/results")
-        os.mkdir(output_dir+"/summary_plots")
+    log_dir = os.path.join(output_dir,"logs","")
+    if not os.path.isdir(log_dir):
+        os.mkdir(log_dir)
+        os.mkdir(os.path.join(output_dir,"results"))
+        os.mkdir(os.path.join(output_dir,"summary_plots"))
     if config.web_dir:
         summarypage_dir = config.web_dir
     else:
         summarypage_dir = os.path.join(os.getenv("HOME"),"public_html/RapidPE/"+output_dir[output_dir.rfind("output/")+7:])
     os.makedirs(summarypage_dir, exist_ok=True)
-    os.system("cp "+cfgname+" "+output_dir+"/Config.ini")
-    os.system('echo "\n#Original config name: '+cfgname+'" >> '+output_dir+'/Config.ini')
+    os.system("cp "+cfgname+" "+os.path.join(output_dir,"Config.ini"))
+    os.system('echo "\n#Original config name: '+cfgname+'" >> '+os.path.join(output_dir,'Config.ini'))
 
     integrate_likelihood_cmds_dict = config.integrate_likelihood_cmds_dict.copy()
     if 'manual-logarithm-offset' in integrate_likelihood_cmds_dict:
         integrate_likelihood_cmds_dict["manual-logarithm-offset"] = 0.5*event_info["snr"]**2.
     if "event-time" in integrate_likelihood_cmds_dict or "psd-file" in integrate_likelihood_cmds_dict or "channel-name" in integrate_likelihood_cmds_dict:
         sys.exit("ERROR: event specific info specified in LikelihoodIntegration of config and in command line or Event section of config. event_time, psd_file,cache_file and channel_name must be specified in the [Event] section or in the input event dictionary ")
     else:
@@ -104,49 +106,49 @@
         integrate_likelihood_cmds_dict["cache-file"] = event_info["cache_file"]
         integrate_likelihood_cmds_dict["approximant"] = event_info["approximant"]
         if "skymap_file" in event_info:
             integrate_likelihood_cmds_dict["skymap-file"] = event_info["skymap_file"]
 
     if config.submit_only_at_exact_signal_position:
         #This is the filename for the output at each intrinsic grid point
-        integration_output_file_name = "results/ILE_iteration_exact_intrinsic"
+        integration_output_file_name = os.path.join(output_dir,"results/ILE_iteration_exact_intrinsic")
         if 'injection_param' in event_info:
             inj_param = convert_list_string_to_dict(event_info["injection_param"])
         else:
             inj_param = convert_list_string_to_dict(event_info["intrinsic_param"])
 
         newlines = "universe = vanilla\n"
         newlines += "executable = "+sys.executable+"\n"
         #newlines += "executable = "+config.exe_integration_extrinsic_likelihood+"\n"
        # newlines += 'arguments = " '
-        if 'cProfile' in integrate_likelihood_cmds_dict:
-            newlines += "arguments = \" -m cProfile -o logs/cprofile_integrate.out " + config.exe_integration_extrinsic_likelihood
-            del integrate_likelihood_cmds_dict['cProfile']
+        if config.cProfile:
+            newlines += f"arguments = \" -m cProfile -o {log_dir}/cprofile_integrate.out " + config.exe_integration_extrinsic_likelihood
         else:
             newlines += "arguments = \" "+ config.exe_integration_extrinsic_likelihood
         newlines += " --output-file="+integration_output_file_name
         newlines += " --mass1 "+str(inj_param["mass1"])+" --mass2 "+str(inj_param["mass2"])
         if 'spin1z' in inj_param:
             newlines += " --spin1z "+str(inj_param["spin1z"])+" --spin2z "+str(inj_param["spin2z"])
         newlines += " "+convert_dict_to_cmd_line(integrate_likelihood_cmds_dict)
         newlines += ' "\n'
-        newlines += "request_memory = 2048\naccounting_group = "+config.accounting_group+"\ngetenv = True\n"
+        newlines += "request_memory = 2048\n"
+        newlines += "accounting_group = "+config.accounting_group+"\n"
+        newlines += "accounting_group_user = "+config.accounting_group_user+"\n"
+        newlines += "getenv = True\n"
         newlines += "request_disk = 512\n"
-        newlines += "log = logs/integrate.log\nerror = logs/integrate.err\noutput = logs/integrate.out\n"
+        newlines += f"log = {log_dir}/integrate.log\nerror = {log_dir}/integrate.err\noutput = {log_dir}/integrate.out\n"
         newlines += "notification = never\nqueue 1\n"
 
-        sub_file_path = output_dir+"/integrate.sub"
+        sub_file_path = os.path.join(output_dir,"integrate.sub")
         with open(sub_file_path,"w") as fo:
             fo.write(newlines)
 
-        #make the output directory your working directory
-        os.chdir(output_dir)
         event_info["condor_submit_time"] = time.time()
         #Write the event_info dictionary to the output dir
-        with open(output_dir+"/event_info_dict.txt","w") as ef:
+        with open(os.path.join(output_dir,"event_info_dict.txt"),"w") as ef:
             ef.write(json.dumps(event_info))
 
         print("Job ready for submission",sub_file_path)
         if config.submit_dag:
             os.system("condor_submit "+sub_file_path)
         return
     else:
@@ -158,49 +160,49 @@
                 sys.exit("ERROR: grid generator must return output xml filename in format [initial_grid_xml=filename]")
 
             stdout_dict = convert_list_string_to_dict(stdout_grid_gen)
             event_info["initial_grid_xml"] = stdout_dict["initial_grid_xml"]
             if "initial_grid_hdf" in stdout_dict:
                 event_info["initial_grid_hdf"] = stdout_dict["initial_grid_hdf"]
 
-        #make the output directory your working directory
-        os.chdir(output_dir)
 
         #if initial grid isn't local, or doesn't hvae the iteration_0 identifier, copy to event dir and append iteration_0
         intrinsic_grid_xml = (event_info["initial_grid_xml"][event_info["initial_grid_xml"].rfind("/")+1:])
         if not "iteration_0" in intrinsic_grid_xml:
             #FIXME: want to remove path info from event_info["initial_grid_xml"] before this copy
             intrinsic_grid_xml = intrinsic_grid_xml[intrinsic_grid_xml.rfine("/")+1:] if "/" in intrinsic_grid_xml else intrinsic_grid_xml
             intrinsic_grid_xml = intrinsic_grid_xml.replace(".xml.gz","iteration_0.xml.gz")
-            os.system("cp "+event_info["initial_grid_xml"]+" "+output_dir+"/"+intrinsic_grid_xml)
+            os.system("cp "+event_info["initial_grid_xml"]+" "+os.path.join(output_dir,intrinsic_grid_xml))
         else:
-            os.system("cp "+event_info["initial_grid_xml"]+" "+output_dir+"/")
+            os.system("cp "+event_info["initial_grid_xml"]+" "+os.path.join(output_dir,""))
 
         print(("Intrinsic grid for iteration 0",intrinsic_grid_xml))
 
         ###
         ### With the inital grid generated, you have all the information you need to run iteration 0. You set up the dag for that here, using rapidpe_create_event_dag in lalsuite. FIXME: this only works for m1 m2. It needs to be adapted for any dimension by taking 
         ### The output .dag file has a few lines for every m1 m2 etc point with the values of the point. The output .sh file has the values filled into the common command line arguements for integrate extrinsic likelihood. The only variable that remains to be filled in the integarte commands is the name of the output file, which includes the cluster and process id. Why are these neeed? I don't know, but it's probably for debugging
         ###
         ### output-name is the name of the dag files for iteration 0. output-file is the name of the file output per intrinsic grid point. The latter will have the massID, cluster and process appended to it.
         ###
         ### FIXME: What doesn the output xml.gz file contain. output name and output file are independent
  
         #event specific commands which need to be lassed to the integration exe are added to the dict here
         #This is the filename for the output at each intrinsic grid point
-        integration_output_file_base = "results/ILE_iteration_"
+        integration_output_file_base = os.path.join(output_dir,"results/ILE_iteration_")
 #        integrate_likelihood_cmds_dict["output-file"] = integration_output_file_base+"0.xml.gz"
-        iteration_dag_name = "marginalize_extrinsic_parameters_iteration_0"
+        iteration_dag_name = os.path.join(output_dir,"marginalize_extrinsic_parameters_iteration_0")
 
         print ("Constructing iteration 0 event dag with command lines for each intrinsic grid point")
         #FIXME: the condor-command option is the condor_commands for the integration. should be possible to pass via LikelihoodIntegration cmd. 
         #accounting_group is passed by default because it's required for all jobs.
-        it_0_dag_cmd = config.exe_create_event_dag + " --condor-command accounting_group="+config.accounting_group+" --exe-integrate-likelihood "+config.exe_integration_extrinsic_likelihood+" --log-directory logs/ --integration-args-dict='"+json.dumps(integrate_likelihood_cmds_dict, sort_keys=True)+"' --write-script"
+        it_0_dag_cmd = config.exe_create_event_dag + " --condor-command accounting_group="+config.accounting_group+" --accounting-group-user "+config.accounting_group_user+" --exe-integrate-likelihood "+config.exe_integration_extrinsic_likelihood+" --working-directory "+ output_dir+ " --log-directory "+log_dir+" --integration-args-dict='"+json.dumps(integrate_likelihood_cmds_dict, sort_keys=True)+"' --write-script "
+        if config.cProfile:
+            it_0_dag_cmd += " --cProfile"
         #Variables which change per iteration are difined below 
-        it_0_dag_cmd +=" --output-name "+iteration_dag_name+" --template-bank-xml "+intrinsic_grid_xml
+        it_0_dag_cmd +=" --output-name "+iteration_dag_name+" --template-bank-xml "+os.path.join(output_dir,intrinsic_grid_xml)
         #event time is within the integrate_likelihood_cmds_dict but it's also defined here because it's used within create_event_dag, not just passed to the integrate exe
         it_0_dag_cmd +=" --event-time="+event_info["event_time"]
         #This is only used by the likelihood itegration exe, but it changes per iteration so it is defined here, which means that any exe used has to 
         #take --output-file as an argumnet
         it_0_dag_cmd +=" --output-file "+integration_output_file_base+"0.xml.gz"
         it_0_dag_cmd += " --iteration-level 0"
         #You can pass extra create_event_dag options by creating a section called CreateEventDag and adding them there.
@@ -218,22 +220,22 @@
         ###
         ### DAG generation
         ### I don't see the benefit of using the dagutils or dag_utils functions which then use the glue.pipeline functions to write the dag. So I write the dag here instead
         ###
 
         print ("Constructing uberdag")
         #this is a hold-all container for all subdags, doesn't appear to correspond to and specific file
-        uberdag = pipeline.CondorDAG(log=os.getcwd())
-        event_dag_name = "event_all_iterations"
+        uberdag = pipeline.CondorDAG(log=output_dir)
+        event_dag_name = os.path.join(output_dir,"event_all_iterations")
         uberdag.set_dag_file(event_dag_name)
 
         # This is meant to ensure that the DAG continues even if some of the integrator jobs fail                                        
         # It also prints the time that the job completed
-        passthrough_filename = "passthrough_%ITER%.sh"
-        passthrough_str = "#!/bin/bash\necho %ITER% `date +%s` >> job_timing.txt\n/bin/true"
+        passthrough_filename = os.path.join(output_dir,"passthrough_%ITER%.sh")
+        passthrough_str = f"#!/bin/bash\necho %ITER% `date +%s` >> {output_dir}/job_timing.txt\n/bin/true"
         indx = 0
         iter_pt_filename = passthrough_filename.replace("%ITER%",str(int(indx)))
         iter_pt_str =passthrough_str.replace("%ITER%",str(int(indx)))
         with open(iter_pt_filename, "w") as fout:
             print(iter_pt_str, file=fout)
         os.chmod(iter_pt_filename, 0o744)
 
@@ -246,47 +248,51 @@
         print ("Passthrough script added")
 
         print ("Generating gridding sub file")
         #After iteration 0, you need to run rapidpe_compute_intrinsic_grid to get the intrinsic grid for the next stage.
         grid_refine_kwargs = config.grid_refine_info
         if config.use_event_spin:
             event_spin = event_info["event_spin"]
-            grid_refine_kwargs['pin-params'] = [f"spin1z={event_spin['spin1z']}",f"spin2z={event_spin['spin2z']}"]
-        grid_job = write_generic_dag_job(config.exe_grid_refine, "GridRefine", config.accounting_group, grid_refine_kwargs, config.grid_refine_condor_commands)
+            grid_refine_kwargs['pin-param'] = [f"spin1z={event_spin['spin1z']}",f"spin2z={event_spin['spin2z']}"]
+        grid_job = write_generic_dag_job(config.exe_grid_refine, "GridRefine", output_dir, config.accounting_group,config.accounting_group_user, grid_refine_kwargs, config.grid_refine_condor_commands)
         #### These options may only apply for the lalsuite rapidpe_compute_intrinsic_grid. If we want to use a different grid refinement scheme we'll need to add a switch here.
         #It requires a .hdf file, which has the grid information for each preceding level. This file is generated by rapidpe_compute_intrinsic_grid when generating the initial grid.
         grid_job.add_opt("refine",event_info["initial_grid_hdf"])
-        grid_job.add_opt("output-xml-file-name","$(macrooutputxmlfilename)")
+        grid_job.add_opt("output-xml-file-name",os.path.join(output_dir,"$(macrooutputxmlfilename)"))
         #take the output from all previous iterations to calculate the confidence region. Since this ready *.xml.gz, it is reading the results from all previous stages. So the command line doesn't change per iteration but the input will be different as it is run after each iteration.
         grid_job.add_opt("result-file","'"+integration_output_file_base+"*.xml.gz'")
         grid_job.write_sub_file()
         print ("Gridding sub file complete")
 
         #This is the dag for rapidpe_create_event_dag. This creates the  marginalize_extrinsic_parameters_iteration_N.dag in the same way as done for iteration 0 above.
-        iteration_job = write_generic_dag_job(config.exe_create_event_dag, "CreateEventDag", config.accounting_group, config.create_event_dag_info, config.create_event_dag_condor_commands)
+        iteration_job = write_generic_dag_job(config.exe_create_event_dag, "CreateEventDag",output_dir, config.accounting_group, config.accounting_group_user,config.create_event_dag_info, config.create_event_dag_condor_commands)
         #Option added to create_event_dag to use integration.sub file which was generated for iteration 0, regenerating it is unnecessary.
         #FIXME: add this option to rapidpe_create_event_dag
         iteration_job.add_opt("condor-command","accounting_group="+config.accounting_group)
+        iteration_job.add_opt("accounting-group-user",config.accounting_group_user)
+        iteration_job.add_opt("working-directory",output_dir)
         # Name / tag for the output of the per intrinsic grid point integration
         iteration_job.add_opt("output-file", "$(macrooutputfile)")
         iteration_job.add_opt("iteration-level", "$(iterlevel)")
         # Name / tag for DAG itself, which runs the integration for all intrinsic grid points
         iteration_job.add_opt("output-name", "$(macrooutputname)")
         # Input grid points to generate the margianlization jobs
-        iteration_job.add_opt("template-bank-xml", "$(macroinputname)")
+        iteration_job.add_opt("template-bank-xml", os.path.join(output_dir,"$(macroinputname)"))
         #same as for iteration 0, this is the stuff needed to run the integration per intrinsic grid point. and some default stuff 
         iteration_job.add_opt("exe-integrate-likelihood", config.exe_integration_extrinsic_likelihood)
-        iteration_job.add_opt("log-directory", "logs/")
+        iteration_job.add_opt("log-directory", log_dir)
 #        iteration_job.add_opt("integration-args-dict", "'"+json.dumps(integrate_likelihood_cmds_dict, sort_keys=True).replace('"','\\"')+"'")
         #Condor dag jobs require a very strange very specific format for string submission. see http://research.cs.wisc.edu/htcondor/manual/v7.6/2_10DAGMan_Applications.html. In short the dict string needs to be passed as '{""a"": ""0"",""b"": ""[\""var1\""]""}'
         iteration_job.add_opt("integration-args-dict", "'"+(json.dumps(integrate_likelihood_cmds_dict, sort_keys=True).replace('"','""'))+"'")
 #        tmp_test = "\"\"{\'n-max\': \'10000\'}\"\""
 #        iteration_job.add_opt("integration-args-dict", tmp_test)
         iteration_job.add_opt("event-time", event_info["event_time"])
         iteration_job.add_opt("write-script", "")
+        if config.cProfile:
+            iteration_job.add_opt("cProfile", "")
         iteration_job.write_sub_file()
         print ("Create event dag subfile complete")
 
         #This assignment is for naming consistency
         #FIXME: currently disabled option to begin iterating at an input iteraton. Should reimplement this, make sure overwite_dag=1 if start iteration is set. check results from previous step exist, read in those
         for indx in np.arange(1,config.n_iterations_per_job):
 #            iteration_dir = output_dir+"/iteration_"+str(indx)
@@ -334,23 +340,23 @@
             iter_pt_filename = passthrough_filename.replace("%ITER%",str(int(indx)))
             #If it's the last command, it should launch the plotting script
             #FIXME: should this be optional?
             iter_pt_str = passthrough_str.replace("%ITER%",str(int(indx)))
             web_dir_str = ""
             if config.web_dir:
                 web_dir_str = f"--web-dir {config.web_dir}"
-            summary_plots_outfile = f"{output_dir}/summary_plots/summary_plots.out"
+            summary_plots_outfile = os.path.join(output_dir,"summary_plots/summary_plots.out")
             if indx == (config.n_iterations_per_job-1):
-                iter_pt_str = f"#!/bin/bash\necho {str(int(indx))} `date +%s` >> job_timing.txt\n"
-                iter_pt_str += "echo 'job_complete' >> JOB_COMPLETE\n"
+                iter_pt_str = f"#!/bin/bash\necho {str(int(indx))} `date +%s` >> {output_dir}/job_timing.txt\n"
+                iter_pt_str += f"echo 'job_complete' >> {output_dir}/JOB_COMPLETE\n"
                 #iter_pt_str += "ligolw_no_ilwdchar "+output_dir+"/results/* &>> "+output_dir+"/summary_plots/summary_plots.out\n"
                 iter_pt_str += f"convert_result_to_txt.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"plot_skymap.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
-                iter_pt_str += f"plot_intrinsic_posterior.py {output_dir} --distance-coordinates {config.distance_coordinates } &>> {summary_plots_outfile}\n"
-                if 'cProfile' in integrate_likelihood_cmds_dict:
+                iter_pt_str += f"compute_posterior.py {output_dir} --distance-coordinates {config.distance_coordinates } &>> {summary_plots_outfile}\n"
+                if config.cProfile:
                     iter_pt_str += f"cprofile_summary.py {output_dir} &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"create_summarypage.py {output_dir} {web_dir_str}  &>> {summary_plots_outfile}\n"
                 #automatically plot the posteriors when the job is done. FIXME: change 0.99 to whatever
                 #iter_pt_str += "python "+init_directory+"/plot_all_posteriors.py "+output_dir+" 0.99\n"
                 #iter_pt_str += "python "+init_directory+"/plot_all_posteriors.py "+output_dir+" 0.9\n"
                 #iter_pt_str += "python "+init_directory+"/plot_all_posteriors_vinaya.py "+output_dir+" 0\n"
                 if config.email_address_for_job_complete_notice != "":
@@ -366,15 +372,15 @@
 
 
         uberdag.write_concrete_dag()
         uberdag.write_script()
 
         event_info["condor_submit_time"] = time.time()
         #Write the event_info dictionary to the output dir
-        with open(output_dir+"/event_info_dict.txt","w") as ef:
+        with open(os.path.join(output_dir,"event_info_dict.txt"),"w") as ef:
             ef.write(json.dumps(event_info, sort_keys=True))
     
         if config.submit_dag:
             print(("Submitting dag job",event_dag_name))
             os.system("condor_submit_dag "+event_dag_name+".dag")
     
         return        
@@ -407,28 +413,29 @@
 ##%cip_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_cip/logs/cip-$(cluster)-$(process).log")
 ##%cip_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_cip/logs/cip-$(cluster)-$(process).err")
 ##%cip_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_cip/logs/cip-$(cluster)-$(process).out")
 ##%cip_job.write_sub_file()
 
 
 
-def write_generic_dag_job(exe, job_name, accounting_group, dict_of_kwargs,dict_of_condor_commands={},log_dir="logs/",log_files_uniq_str = "$(cluster)-$(process)"):
+def write_generic_dag_job(exe, job_name,output_dir, accounting_group,accounting_group_user, dict_of_kwargs,dict_of_condor_commands={},log_dir="logs/",log_files_uniq_str = "$(cluster)-$(process)"):
     ###
     ### Utility function to construct a generic condor job for the top level hierarchy of the DAG.
     ### given an executable, and a config section with command line arguments which can be read directly and do not change from dag node to node, create a generic dag job
     ### This returns the dag job object, so variable arguments can be added later
     ### the job_name is used for the sub file and to identify log files
     ###
 
     dag_job = pipeline.CondorDAGJob(universe="vanilla", executable=exe)
-    dag_job.set_sub_file(job_name+".sub")
+    dag_job.set_sub_file(os.path.join(output_dir,f"{job_name}.sub"))
 
     #
     # Logging options
     #
+    log_dir = os.path.join(output_dir,log_dir)
     dag_job.set_log_file("%s%s-%s.log" % (log_dir, job_name, log_files_uniq_str))
     dag_job.set_stderr_file("%s%s-%s.err" % (log_dir, job_name, log_files_uniq_str))
     dag_job.set_stdout_file("%s%s-%s.out" % (log_dir, job_name, log_files_uniq_str))
 
     new_kwargs = {}
     for opt, param in dict_of_kwargs.items():
         if len(param) > 1 and param[0] == "[" and param[-1] == "]":
@@ -454,14 +461,15 @@
     if 'request_memory' not in dict_of_condor_commands:
         # Memory request is 2 GB by default
         dag_job.add_condor_cmd('request_memory', '2048')
     if 'request_disk' not in dict_of_condor_commands:
         # Disk request is 512 MB by default
         dag_job.add_condor_cmd('request_disk', '512')
     dag_job.add_condor_cmd('accounting_group', accounting_group)
+    dag_job.add_condor_cmd('accounting_group_user', accounting_group_user)
 
     # Typically used to add things like accounting information.
     for cmd, value in dict_of_condor_commands.items():
         dag_job.add_condor_cmd(cmd, value)
 
     # This is a hack since CondorDAGJob hides the queue property 
     dag_job._CondorJob__queue = 1
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.0.9.dev20230323
+Version: 0.1.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.0.9.dev20230323/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.1.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 COPYING
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+bin/postscripts/compute_posterior.py
 bin/postscripts/convert_result_to_txt.py
 bin/postscripts/cprofile_summary.py
 bin/postscripts/create_summarypage.py
-bin/postscripts/plot_intrinsic_posterior.py
 bin/postscripts/plot_skymap.py
 src/rapidpe_rift_pipe/__init__.py
 src/rapidpe_rift_pipe/cli.py
 src/rapidpe_rift_pipe/config.py
 src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+src/rapidpe_rift_pipe/jacobians.py
 src/rapidpe_rift_pipe/modules.py
+src/rapidpe_rift_pipe/pastro.py
 src/rapidpe_rift_pipe/postscript_utils.py
 src/rapidpe_rift_pipe/profiling.py
 src/rapidpe_rift_pipe/search_bias_bounds.py
 src/rapidpe_rift_pipe/test_cli.py
 src/rapidpe_rift_pipe/test_config.py
 src/rapidpe_rift_pipe/test_modules.py
 src/rapidpe_rift_pipe/utils.py
 src/rapidpe_rift_pipe.egg-info/PKG-INFO
 src/rapidpe_rift_pipe.egg-info/SOURCES.txt
 src/rapidpe_rift_pipe.egg-info/dependency_links.txt
 src/rapidpe_rift_pipe.egg-info/entry_points.txt
 src/rapidpe_rift_pipe.egg-info/requires.txt
 src/rapidpe_rift_pipe.egg-info/top_level.txt
 src/rapidpe_rift_pipe.egg-info/zip-safe
-src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+src/rapidpe_rift_pipe/config_files/__init__.py
+src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+src/rapidpe_rift_pipe/static/__init__.py
+src/rapidpe_rift_pipe/static/stylesheet.css
```

