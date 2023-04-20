# Comparing `tmp/slurmui-0.2.9.3-py3-none-any.whl.zip` & `tmp/slurmui-0.3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6323 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       27 b- defN 23-Jan-03 17:17 slurmui/__init__.py
+Zip file size: 6546 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       27 b- defN 23-Apr-20 12:40 slurmui/__init__.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 12:39 slurmui/_version.py
 -rw-rw-r--  2.0 unx     9278 b- defN 23-Jan-13 19:20 slurmui/debug_strings.py
--rw-rw-r--  2.0 unx    11180 b- defN 23-Apr-03 11:53 slurmui/slurmui.py
+-rw-rw-r--  2.0 unx    11249 b- defN 23-Apr-20 12:47 slurmui/slurmui.py
 -rw-rw-r--  2.0 unx      269 b- defN 23-Jan-03 17:14 slurmui/slurmui_cli.py
--rw-rw-r--  2.0 unx      836 b- defN 23-Apr-03 11:55 slurmui-0.2.9.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-03 11:55 slurmui-0.2.9.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 23-Apr-03 11:55 slurmui-0.2.9.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-03 11:55 slurmui-0.2.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      710 b- defN 23-Apr-03 11:55 slurmui-0.2.9.3.dist-info/RECORD
-9 files, 22460 bytes uncompressed, 5095 bytes compressed:  77.3%
+-rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/RECORD
+10 files, 22626 bytes uncompressed, 5204 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: slurmui/__init__.py
 Comment: 
 
+Filename: slurmui/_version.py
+Comment: 
+
 Filename: slurmui/debug_strings.py
 Comment: 
 
 Filename: slurmui/slurmui.py
 Comment: 
 
 Filename: slurmui/slurmui_cli.py
 Comment: 
 
-Filename: slurmui-0.2.9.3.dist-info/METADATA
+Filename: slurmui-0.3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: slurmui-0.2.9.3.dist-info/WHEEL
+Filename: slurmui-0.3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: slurmui-0.2.9.3.dist-info/entry_points.txt
+Filename: slurmui-0.3.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: slurmui-0.2.9.3.dist-info/top_level.txt
+Filename: slurmui-0.3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: slurmui-0.2.9.3.dist-info/RECORD
+Filename: slurmui-0.3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slurmui/slurmui.py

```diff
@@ -5,14 +5,15 @@
 from textual.containers import Container, Vertical 
 from textual.containers import Grid
 from textual.screen import Screen
 import subprocess
 import pandas as pd
 import re
 import os
+from ._version import __version__
 
 DEBUG = False
 if DEBUG:
     from slurmui.debug_strings import SINFO_DEBUG, SQUEUE_DEBUG
 
 class SlurmUI(App):
 
@@ -52,15 +53,15 @@
     def update_squeue_table(self, sort_column=None, sort_ascending=True):
         self.table.clear()
         squeue_df = self.query_squeue(sort_column=sort_column, sort_ascending=sort_ascending)
         # add device information
         squeue_df["GPU_IDS"] = "N/A"
         real_session_mask = squeue_df["PA"]!="in"
         if real_session_mask.any():
-            squeue_df["GPU_IDS"][real_session_mask] = squeue_df[real_session_mask]["JOBID"].apply(lambda x: get_job_gpu_ids(x))
+            squeue_df["GPU_IDS"][real_session_mask] =squeue_df[real_session_mask]["JOBID"].apply(lambda x: get_job_gpu_ids(x))
         self.table.columns = []
         self.table.add_columns(*squeue_df.columns)
         for row in squeue_df.iterrows():
             table_row = [str(x) for x in row[1].values]
             self.table.add_row(*table_row)
         self.table.focus()
 
@@ -131,15 +132,15 @@
         if sort_column is not None:
             overview_df = overview_df.sort_values(overview_df.columns[sort_column],ascending=sort_ascending)
         
         self.gpu_overview_df = overview_df
         # also change the title to include GPU information
         total_num_gpus = overview_df["#Total"].sum()
         total_available = overview_df["#Avail"].sum()
-        self.title = f"SlurmUI --- GPU STATS: {total_available}/{total_num_gpus}"
+        self.title = f"SlurmUI --- GPU STATS: {total_available}/{total_num_gpus} -- Version: {__version__}"
         return overview_df
 
 
     def update_gpu_table(self, sort_column=None, sort_ascending=True):
         self.table.clear()
         self.table.columns = []
         overview_df = self.query_gpus(sort_column=sort_column, sort_ascending=sort_ascending)
@@ -282,17 +283,17 @@
     data = io.StringIO(formatted_string)
     df = pd.read_csv(data, sep=sep)
     df.columns = [x.strip() for x in df.columns]
     return df 
 
 def get_job_gpu_ids(job_id):
     try:
-        response_string = subprocess.check_output(f"""srun --jobid {job_id} '/bin/env' | grep SLURM_STEP_GPUS""", shell=True).decode("utf-8")
+        response_string = subprocess.check_output(f"""srun --jobid {job_id} '/bin/env' | grep SLURM_STEP_GPUS""", shell=True,stderr=subprocess.STDOUT).decode("utf-8")
         formatted_string = response_string.split("=")[-1].strip()
-    except Exception as e:
+    except:
         return "N/A"
     return formatted_string
 
 
 def get_log_fn(job_id):
     response_string = subprocess.check_output(f"""scontrol show job {job_id} | grep StdOut""", shell=True).decode("utf-8")
     formatted_string = response_string.split("=")[-1].strip()
```

## Comparing `slurmui-0.2.9.3.dist-info/METADATA` & `slurmui-0.3.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmui
-Version: 0.2.9.3
+Version: 0.3.0.0
 Summary: Terminal UI for Slurm
 Home-page: https://github.com/SirWyver/slurmui
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

