# Comparing `tmp/sprint2-0.0.15.tar.gz` & `tmp/sprint2-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint2-0.0.15.tar", last modified: Thu Apr  6 17:45:21 2023, max compression
+gzip compressed data, was "sprint2-0.0.16.tar", last modified: Thu Apr 20 19:09:48 2023, max compression
```

## Comparing `sprint2-0.0.15.tar` & `sprint2-0.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-06 17:45:26.719216 sprint2-0.0.15/
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-06 17:45:26.591228 sprint2-0.0.15/MaskAGref/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6734 2023-04-06 17:45:12.000000 sprint2-0.0.15/MaskAGref/MaskAGref.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-06 17:45:12.000000 sprint2-0.0.15/MaskAGref/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-06 17:45:26.716217 sprint2-0.0.15/PKG-INFO
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-06 17:45:26.638224 sprint2-0.0.15/getDsRNA/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1919 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9507 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step1_transcript_blat.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9760 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step2_transcript_dspair.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     3162 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step3_bedtools_sorted_rmLC.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6742 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step4_combine_by_chr.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     5750 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step5_merge_dsRNA.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2408 2023-04-06 17:45:16.000000 sprint2-0.0.15/getDsRNA/step6_dsRNA.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-06 17:45:26.668221 sprint2-0.0.15/getRES/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2034 2023-04-06 17:45:14.000000 sprint2-0.0.15/getRES/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    45388 2023-04-06 17:45:14.000000 sprint2-0.0.15/getRES/step1_SNVcalling.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    20538 2023-04-06 17:45:14.000000 sprint2-0.0.15/getRES/step2_annotation_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    19408 2023-04-06 17:45:14.000000 sprint2-0.0.15/getRES/step3_dsRNA_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-06 17:45:26.720216 sprint2-0.0.15/setup.cfg
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-06 17:45:09.000000 sprint2-0.0.15/setup.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-06 17:45:26.708217 sprint2-0.0.15/sprint2.egg-info/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/PKG-INFO
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      565 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/SOURCES.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/dependency_links.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/entry_points.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/requires.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-06 17:45:26.000000 sprint2-0.0.15/sprint2.egg-info/top_level.txt
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.051855 sprint2-0.0.16/
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:53.855872 sprint2-0.0.16/MaskAGref/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-20 19:06:33.000000 sprint2-0.0.16/MaskAGref/MaskAGref.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-20 19:06:33.000000 sprint2-0.0.16/MaskAGref/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:09:54.048856 sprint2-0.0.16/PKG-INFO
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:53.960863 sprint2-0.0.16/getDsRNA/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9597 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step1_transcript_blat.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step2_transcript_dspair.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step3_bedtools_sorted_rmLC.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step4_combine_by_chr.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/step5_merge_dsRNA.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2464 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/step6_dsRNA.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.000860 sprint2-0.0.16/getRES/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2034 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    45388 2023-04-20 19:06:32.000000 sprint2-0.0.16/getRES/step1_SNVcalling.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    20538 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/step2_annotation_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    19408 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/step3_dsRNA_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-20 19:09:54.052855 sprint2-0.0.16/setup.cfg
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-20 19:09:40.000000 sprint2-0.0.16/setup.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.041856 sprint2-0.0.16/sprint2.egg-info/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      565 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/SOURCES.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/dependency_links.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/entry_points.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/requires.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/top_level.txt
```

### Comparing `sprint2-0.0.15/MaskAGref/MaskAGref.py` & `sprint2-0.0.16/MaskAGref/MaskAGref.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,17 @@
 
     try:
         args = parser.parse_args()
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
 
-    global bwa
+    global bwa,refgenome,CPU, gtf_file
     refgenome=str(args.reference)
-    base_path=str(args.output)
+    base_path=str(args.output)+"/"
     bwa=str(args.bwa)
     CPU=int(args.cpu)
 
     if args.gtf:
         gtf_file=str(args.gtf)
     else:
         gtf_file=False
```

### Comparing `sprint2-0.0.15/PKG-INFO` & `sprint2-0.0.16/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.15
+Version: 0.0.16
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.15/getDsRNA/__init__.py` & `sprint2-0.0.16/getDsRNA/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse
+import argparse,os
 import subprocess
 from .step1_transcript_blat import *
 from .step2_transcript_dspair import *
 from .step3_bedtools_sorted_rmLC import *
 from .step4_combine_by_chr import *
 from .step5_merge_dsRNA import *
 from .step6_dsRNA import *
```

### Comparing `sprint2-0.0.15/getDsRNA/step1_transcript_blat.py` & `sprint2-0.0.16/getDsRNA/step1_transcript_blat.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-
-    OUT_DIR_BASE=str(args.OUT_DIR)
+    global OUT_DIR,blat_path,trans_path,ref_in_path,CPU,SITE_ADD_AROUND,trans_add,add2
+    OUT_DIR_BASE=str(args.OUT_DIR)+"/"
     blat_path = str(args.Blat_file)
     trans_path=str(args.Transcript_file)
     ref_in_path = str(args.Reference_file)
     CPU=int(args.cpu)
 
     SITE_ADD_AROUND=40
     trans_add=2
```

### Comparing `sprint2-0.0.15/getDsRNA/step2_transcript_dspair.py` & `sprint2-0.0.16/getDsRNA/step2_transcript_dspair.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-
-    OUT_DIR_BASE=str(args.OUT_DIR)
+    global OUT_DIR,trans_path,CPU,SITE_ADD_AROUND,blat,ds_path,rev_path
+    OUT_DIR_BASE=str(args.OUT_DIR)+"/"
     trans_path=str(args.Transcript_file)
     CPU=int(args.cpu)
 
     SITE_ADD_AROUND=40
     blat=OUT_DIR_BASE+"BLAT/"
     ds_path=OUT_DIR_BASE+"ds_files/"
     rev_path=OUT_DIR_BASE+"ds_files_rev/"
```

### Comparing `sprint2-0.0.15/getDsRNA/step3_bedtools_sorted_rmLC.py` & `sprint2-0.0.16/getDsRNA/step3_bedtools_sorted_rmLC.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-
+    global CPU,base_path,bedtools_path,lc_path,rev_path,sort_path,rmlc_path
     CPU=int(int(args.cpu)/10)+1
-    base_path=str(args.OUT_DIR)
+    base_path=str(args.OUT_DIR)+"/"
     bedtools_path=str(args.Bedtools_path)
     lc_path=str(args.lc_path)
 
     rev_path=base_path+"ds_files_rev/"
     sort_path=base_path+"sorted_rev/"
     rmlc_path=base_path+"rmLC_rev/"
```

### Comparing `sprint2-0.0.15/getDsRNA/step4_combine_by_chr.py` & `sprint2-0.0.16/getDsRNA/step4_combine_by_chr.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
 
     try:
         args = parser.parse_args(args.split())
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-
+    global CPU,base_path,trans_path,bedtools_path,path_rev,path_merge
     CPU=int(args.cpu)
-    base_path=str(args.OUT_DIR)
+    base_path=str(args.OUT_DIR)+"/"
     trans_path=str(args.Transcript_file)
     bedtools_path=str(args.Bedtools_path)
 
     path_rev=base_path+"rmLC_rev/"
     path_merge=base_path+"merge_rev/"
 
     if not os.path.isdir(path_merge):
```

### Comparing `sprint2-0.0.15/getDsRNA/step5_merge_dsRNA.py` & `sprint2-0.0.16/getDsRNA/step5_merge_dsRNA.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-
+    global CPU, base_path, bedtools_path, com_path, sort_path
     CPU=int(int(args.cpu)/5)+1
-    base_path=str(args.OUT_DIR)
+    base_path=str(args.OUT_DIR)+"/"
     bedtools_path=str(args.Bedtools_path)
     com_path=base_path+"combine_rev/"
     sort_path=base_path+"sort2_rev/"
 
     if not os.path.isdir(sort_path):
         os.mkdir(sort_path)
```

### Comparing `sprint2-0.0.15/getDsRNA/step6_dsRNA.py` & `sprint2-0.0.16/getDsRNA/step6_dsRNA.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
                 fo.write(this_write + "\n")
 
 def main(args):
     parser = argparse.ArgumentParser(description='python3 step6_dsRNA.py')
     parser.add_argument('-o', '--OUT_DIR', default=os.getcwd(), help='path to Output Directory (default:Working Directory)')
     parser.add_argument('-p', '--cpu', default=1, help='CPU number (default=1)')
     args = parser.parse_args(args.split())
-
+    global CPU,base_path,ds_dir,outdir
     CPU = int(args.cpu)
-    base_path = str(args.OUT_DIR)
+    base_path = str(args.OUT_DIR)+"/"
     ds_dir = base_path + "merge2_rev/"
     outdir = base_path + "dsRNA_file/"
     
     if not os.path.isdir(outdir):
         os.mkdir(outdir)
 
     print("Start step6 get candidate dsRNA...")
@@ -50,18 +50,18 @@
         ds_path = ds_dir + f
         file_out = outdir + f
         ARG = [ds_path, file_out, add_num]
         pool1.apply_async(dspair_add, (ARG,))
 
     pool1.close() 
     pool1.join()     
-
+    '''
     subprocess.Popen("rm -r " + base_path + "*rev/", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "BLAT", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "query", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "reference", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "ds_files/", shell=True).wait()
-
+    '''
     time_end = int(time.perf_counter())
     run_time = str(time_end - time_start)
     print("Processing running time is: " + run_time + " seconds" + "\n")
```

### Comparing `sprint2-0.0.15/getRES/__init__.py` & `sprint2-0.0.16/getRES/__init__.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.15/getRES/step1_SNVcalling.py` & `sprint2-0.0.16/getRES/step1_SNVcalling.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.15/getRES/step2_annotation_based.py` & `sprint2-0.0.16/getRES/step2_annotation_based.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.15/getRES/step3_dsRNA_based.py` & `sprint2-0.0.16/getRES/step3_dsRNA_based.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.15/setup.py` & `sprint2-0.0.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 
 setup(
     name='sprint2',
-    version='0.0.15',
+    version='0.0.16',
     packages=find_packages(),
     install_requires=[
         'argparse',
     ],
     entry_points={
         'console_scripts': [
             'MaskAGref=MaskAGref:main',
```

### Comparing `sprint2-0.0.15/sprint2.egg-info/PKG-INFO` & `sprint2-0.0.16/sprint2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.15
+Version: 0.0.16
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.15/sprint2.egg-info/SOURCES.txt` & `sprint2-0.0.16/sprint2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

