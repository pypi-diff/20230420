# Comparing `tmp/sprint2-0.0.16.tar.gz` & `tmp/sprint2-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint2-0.0.16.tar", last modified: Thu Apr 20 19:09:48 2023, max compression
+gzip compressed data, was "sprint2-0.0.17.tar", last modified: Thu Apr 20 19:34:05 2023, max compression
```

## Comparing `sprint2-0.0.16.tar` & `sprint2-0.0.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.051855 sprint2-0.0.16/
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:53.855872 sprint2-0.0.16/MaskAGref/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-20 19:06:33.000000 sprint2-0.0.16/MaskAGref/MaskAGref.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-20 19:06:33.000000 sprint2-0.0.16/MaskAGref/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:09:54.048856 sprint2-0.0.16/PKG-INFO
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:53.960863 sprint2-0.0.16/getDsRNA/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9597 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step1_transcript_blat.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step2_transcript_dspair.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step3_bedtools_sorted_rmLC.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-20 19:06:25.000000 sprint2-0.0.16/getDsRNA/step4_combine_by_chr.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/step5_merge_dsRNA.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2464 2023-04-20 19:06:26.000000 sprint2-0.0.16/getDsRNA/step6_dsRNA.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.000860 sprint2-0.0.16/getRES/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2034 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    45388 2023-04-20 19:06:32.000000 sprint2-0.0.16/getRES/step1_SNVcalling.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    20538 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/step2_annotation_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    19408 2023-04-20 19:06:33.000000 sprint2-0.0.16/getRES/step3_dsRNA_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-20 19:09:54.052855 sprint2-0.0.16/setup.cfg
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-20 19:09:40.000000 sprint2-0.0.16/setup.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:09:54.041856 sprint2-0.0.16/sprint2.egg-info/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/PKG-INFO
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      565 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/SOURCES.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/dependency_links.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/entry_points.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/requires.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-20 19:09:52.000000 sprint2-0.0.16/sprint2.egg-info/top_level.txt
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.385189 sprint2-0.0.17/
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.250200 sprint2-0.0.17/MaskAGref/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-20 19:33:49.000000 sprint2-0.0.17/MaskAGref/MaskAGref.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-20 19:33:49.000000 sprint2-0.0.17/MaskAGref/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:34:10.383189 sprint2-0.0.17/PKG-INFO
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.296196 sprint2-0.0.17/getDsRNA/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9741 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step1_transcript_blat.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step2_transcript_dspair.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step3_bedtools_sorted_rmLC.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step4_combine_by_chr.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step5_merge_dsRNA.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2464 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step6_dsRNA.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.324194 sprint2-0.0.17/getRES/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2034 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    45388 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step1_SNVcalling.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    20538 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step2_annotation_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    19408 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step3_dsRNA_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-20 19:34:10.386189 sprint2-0.0.17/setup.cfg
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-20 19:33:54.000000 sprint2-0.0.17/setup.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.376189 sprint2-0.0.17/sprint2.egg-info/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      565 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/SOURCES.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/dependency_links.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/entry_points.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/requires.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/top_level.txt
```

### Comparing `sprint2-0.0.16/MaskAGref/MaskAGref.py` & `sprint2-0.0.17/MaskAGref/MaskAGref.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/PKG-INFO` & `sprint2-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.16
+Version: 0.0.17
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.16/getDsRNA/__init__.py` & `sprint2-0.0.17/getDsRNA/__init__.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getDsRNA/step1_transcript_blat.py` & `sprint2-0.0.17/getDsRNA/step1_transcript_blat.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,24 +113,26 @@
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
-    global OUT_DIR,blat_path,trans_path,ref_in_path,CPU,SITE_ADD_AROUND,trans_add,add2
+        
+    global OUT_DIR_BASE,OUT_DIR,blat_path,trans_path,ref_in_path,CPU,SITE_ADD_AROUND,trans_add,add2
     OUT_DIR_BASE=str(args.OUT_DIR)+"/"
     blat_path = str(args.Blat_file)
     trans_path=str(args.Transcript_file)
     ref_in_path = str(args.Reference_file)
     CPU=int(args.cpu)
 
     SITE_ADD_AROUND=40
     trans_add=2
     ##trans_add:...kb
+
     SITE_ADD_AROUND=int(SITE_ADD_AROUND)
     trans_add=int(trans_add)*1000
     add2=2*SITE_ADD_AROUND
 
     ##----------------------------------------------------------------------------------------------------------
     description()
     print("\n\n\nStart step1 BLAT...")
@@ -138,19 +140,19 @@
     OUT_DIR = OUT_DIR_BASE+"/"
     if not os.path.isdir(OUT_DIR):
         os.mkdir(OUT_DIR)
     ##----------------------------------------------------------------------------------------------------------
     ##load reference genome fasta file and compute time
     ##running time is:40 seconds
     print("1.Start load reference genome file...")
-
+    global chrom
     chrom=SeqIO.to_dict(SeqIO.parse(ref_in_path, "fasta"))
     #print(list(chrom.keys())[0:50])
     print("\t\tReference genome file is OK!")
-
+    global all_chroms,all_chroms_new
     ##print number of bases in each chrom
     all_chroms=list(chrom.keys())###640 sequences
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##split each chrom seqence
@@ -177,14 +179,15 @@
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##split reference sequence by chromosome
     ##running time is:4 seconds
     print("3.Start split each transcript sequence...")
+    global ref_out_dir
     ref_out_dir=OUT_DIR+"/reference"
     if not os.path.isdir(ref_out_dir):
         os.mkdir(ref_out_dir)
 
     pool_size = CPU
     pool1 = Pool(pool_size)  
     for this_chr in all_chroms:
@@ -196,14 +199,15 @@
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##find all Query sequences in all hg38 reference file with multiprocessing pool
     ##running time is:334 seconds (5.6 minutes)
     ## all sequence query finder 
     print("4.Start find query sequences....")
+    global fa_out_dir
     fa_out_dir=OUT_DIR+"/query"
     if not os.path.isdir(fa_out_dir):
         os.mkdir(fa_out_dir)
 
     pool_size = int(CPU)
     pool1 = Pool(pool_size)  
 
@@ -216,14 +220,15 @@
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##BLAT by chromosome
     ##running time is : ~ 3 days
     ## all BLAT
+    global blat_out_dir
     blat_out_dir=OUT_DIR+"/BLAT"
     CPU=CPU
     if not os.path.isdir(blat_out_dir):
         os.mkdir(blat_out_dir)
     print("5.Start run BLAT....")     
     time_start = int(time.perf_counter())
```

### Comparing `sprint2-0.0.16/getDsRNA/step2_transcript_dspair.py` & `sprint2-0.0.17/getDsRNA/step2_transcript_dspair.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getDsRNA/step3_bedtools_sorted_rmLC.py` & `sprint2-0.0.17/getDsRNA/step3_bedtools_sorted_rmLC.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getDsRNA/step4_combine_by_chr.py` & `sprint2-0.0.17/getDsRNA/step4_combine_by_chr.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getDsRNA/step5_merge_dsRNA.py` & `sprint2-0.0.17/getDsRNA/step5_merge_dsRNA.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getDsRNA/step6_dsRNA.py` & `sprint2-0.0.17/getDsRNA/step6_dsRNA.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getRES/__init__.py` & `sprint2-0.0.17/getRES/__init__.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getRES/step1_SNVcalling.py` & `sprint2-0.0.17/getRES/step1_SNVcalling.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getRES/step2_annotation_based.py` & `sprint2-0.0.17/getRES/step2_annotation_based.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/getRES/step3_dsRNA_based.py` & `sprint2-0.0.17/getRES/step3_dsRNA_based.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.16/setup.py` & `sprint2-0.0.17/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 
 setup(
     name='sprint2',
-    version='0.0.16',
+    version='0.0.17',
     packages=find_packages(),
     install_requires=[
         'argparse',
     ],
     entry_points={
         'console_scripts': [
             'MaskAGref=MaskAGref:main',
```

### Comparing `sprint2-0.0.16/sprint2.egg-info/PKG-INFO` & `sprint2-0.0.17/sprint2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.16
+Version: 0.0.17
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.16/sprint2.egg-info/SOURCES.txt` & `sprint2-0.0.17/sprint2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

