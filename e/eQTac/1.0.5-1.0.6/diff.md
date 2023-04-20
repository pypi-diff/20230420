# Comparing `tmp/eQTac-1.0.5.tar.gz` & `tmp/eQTac-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.5.tar", last modified: Wed Apr 19 09:10:48 2023, max compression
+gzip compressed data, was "eQTac-1.0.6.tar", last modified: Thu Apr 20 01:54:27 2023, max compression
```

## Comparing `eQTac-1.0.5.tar` & `eQTac-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.926388 eQTac-1.0.5/
--rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3922 2023-04-19 09:10:48.923396 eQTac-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3451 2023-04-19 08:43:06.000000 eQTac-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.815409 eQTac-1.0.5/eQTac/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.5/eQTac/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.5/eQTac/control_FDR.py
--rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.5/eQTac/eQTac_correlation.py
--rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.5/eQTac/eQTac_permutation.py
--rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.5/eQTac/filter_bkg.py
--rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_PRE.py
--rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_mut_fa.py
--rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.5/eQTac/generate_snp_dict.py
--rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.5/eQTac/geno2score.py
--rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.5/eQTac/get_nullseq.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:10:48.906446 eQTac-1.0.5/eQTac.egg-info/
--rw-rw-rw-   0        0        0     3922 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 09:10:48.000000 eQTac-1.0.5/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 09:10:48.928382 eQTac-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-19 09:05:17.000000 eQTac-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:54:27.112834 eQTac-1.0.6/
+-rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5926 2023-04-20 01:54:27.110839 eQTac-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5429 2023-04-20 01:48:21.000000 eQTac-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 01:54:26.996147 eQTac-1.0.6/eQTac/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.6/eQTac/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.6/eQTac/control_FDR.py
+-rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.6/eQTac/eQTac_correlation.py
+-rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.6/eQTac/eQTac_permutation.py
+-rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.6/eQTac/filter_bkg.py
+-rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_PRE.py
+-rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_mut_fa.py
+-rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_snp_dict.py
+-rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.6/eQTac/geno2score.py
+-rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.6/eQTac/get_nullseq.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:54:27.093914 eQTac-1.0.6/eQTac.egg-info/
+-rw-rw-rw-   0        0        0     5926 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 01:54:27.115826 eQTac-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      767 2023-04-20 01:54:17.000000 eQTac-1.0.6/setup.py
```

### Comparing `eQTac-1.0.5/LICENSE` & `eQTac-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/PKG-INFO` & `eQTac-1.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,121 @@
-Metadata-Version: 2.1
-Name: eQTac
-Version: 1.0.5
-Summary: The eQTac method.
-Home-page: https://github.com/JFF1594032292/eQTac
-Author: Jiang Feng
-Author-email: 1594032292@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# eQTac
-EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
-## Dependence
-### Python packages
-```
-numpy >= 1.22.4
-pandas >= 1.4.3
-pybedtools >= 0.8.2
-pysam >= 0.16.0.1
-rpy2 >= 3.4.2
-scipy >= 1.8.1
-```
-### Other software (need manual installation)
-```
-plink >= v1.90b6.24
-bedtools >= v2.30.0
-R >= 3.6.1
-    r-gkmSVM >= 0.8.0
-```
-## Installation
-
-## Input data
-1. Data used in model training:
-    (1) **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See test_data/test.positive.bed
-    (2) **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See test_data/test.exclude.bed.
-    (3) **Fasta file with .fai index.** Usually the human genome sequnce file in fasta format. See test.hg19.chr17.fa.
-2. Data used in eQTac calculation.
-    (1) 
-## Usage pattern
-We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
-### Pipeline level pattern
-For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
-It can be used as follow:
-```
-python Part-All-eQTac_pipeline.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-exp test_data/test.exp_residual \
-	-n 100 \
-	-o output_eQTac \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-```
-### Part level pattern
-For the function level pattern, we provide four scripts:
-```
-python Part-1-Train_model.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-o output_eQTac_part \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-
-python Part-2-Generate_PRE_fa.py \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-o output_eQTac_part
-
-python Part-3-Predict_PRE_score.py \
-	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
-	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
-	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
-	-geno test_data/test.geno \
-	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
-	-T 1 \
-	-o output_eQTac_part
-
-python Part-4-Calculate_eQTac_correlation.py \
-	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
-	-exp test_data/test.exp_residual \
-	-n 50 \
-	-o output_eQTac_part
-```
-### Function level pattern
-For the function level pattern, we provide a series of functions:
-```
-from eQTac.get_nullseq import get_nullseq
-from eQTac.filter_bkg import filter_bkg
-from eQTac.generate_snp_dict import generate_snp_dict
-from eQTac.generate_PRE import generate_PRE
-from eQTac.generate_mut_fa import generate_mut_fa
-from eQTac.geno2score import geno2score
-from eQTac.eQTac_correlation import eQTac_correlation
-from eQTac.eQTac_permutation import eQTac_permutation
-from eQTac.control_FDR import control_FDR
-```
-These functions can be used to construct the whole pipeline. The Part-All-eQTac_pipeline.py file used this
-
-## Notes
+# eQTac
+EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
+## Schematic 
+![](./imgs/Schematic.png)
+## Dependence
+### Python packages
+```
+numpy >= 1.22.4
+pandas >= 1.4.3
+pybedtools >= 0.8.2
+pysam >= 0.16.0.1
+rpy2 >= 3.4.2
+scipy >= 1.8.1
+```
+### Other software (need manual installation)
+```
+plink >= v1.90b6.24 (plink should in $PATH)
+bedtools >= v2.30.0 (bedtools should in $PATH)
+R >= 3.6.1
+    r-gkmSVM >= 0.8.0
+```
+## Installation & test example
+```
+# installation
+pip install eQTac 
+
+# test examples
+git clone https://github.com/JFF1594032292/eQTac.git # just for test
+cd eQTac/Utilities_pipeline
+nohup sh example_All_pipeline.sh &
+```
+Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
+
+## Input data
+1. Data used in model training:
+    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
+2. Data used in eQTac calculation.
+    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
+    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
+    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
+    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
+## Usage pattern
+We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
+### Pipeline-level pattern
+For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
+It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
+```
+python Part-All-eQTac_pipeline.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-exp test_data/test.exp_residual \
+	-n 100 \
+	-o output_eQTac \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+```
+### Part-level pattern
+For the function level pattern, we provide four scripts:
+```
+Part-1-Train_model.py
+Part-2-Generate_PRE_fa.py
+Part-3-Predict_PRE_score.py
+Part-4-Calculate_eQTac_correlation.py
+```
+It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
+```
+python Part-1-Train_model.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-o output_eQTac_part \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+
+python Part-2-Generate_PRE_fa.py \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-o output_eQTac_part
+
+python Part-3-Predict_PRE_score.py \
+	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
+	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
+	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
+	-geno test_data/test.geno \
+	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
+	-T 1 \
+	-o output_eQTac_part
+
+python Part-4-Calculate_eQTac_correlation.py \
+	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
+	-exp test_data/test.exp_residual \
+	-n 50 \
+	-o output_eQTac_part
+```
+### Function-level pattern
+For the function level pattern, we provide a series of functions:
+```
+from eQTac.get_nullseq import get_nullseq
+from eQTac.filter_bkg import filter_bkg
+from eQTac.generate_snp_dict import generate_snp_dict
+from eQTac.generate_PRE import generate_PRE
+from eQTac.generate_mut_fa import generate_mut_fa
+from eQTac.geno2score import geno2score
+from eQTac.eQTac_correlation import eQTac_correlation
+from eQTac.eQTac_permutation import eQTac_permutation
+from eQTac.control_FDR import control_FDR
+```
+These functions can be used to construct the whole pipeline.
+### Recomend
+We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
+
+Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
+
+If you are familiar with this pipeline, you can directly use the `function-level` pattern to construct your own pipeline.
+## Notes
+1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
```

### Comparing `eQTac-1.0.5/eQTac/control_FDR.py` & `eQTac-1.0.6/eQTac/control_FDR.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/eQTac_correlation.py` & `eQTac-1.0.6/eQTac/eQTac_correlation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/eQTac_permutation.py` & `eQTac-1.0.6/eQTac/eQTac_permutation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/filter_bkg.py` & `eQTac-1.0.6/eQTac/filter_bkg.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/generate_PRE.py` & `eQTac-1.0.6/eQTac/generate_PRE.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/generate_mut_fa.py` & `eQTac-1.0.6/eQTac/generate_mut_fa.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/generate_snp_dict.py` & `eQTac-1.0.6/eQTac/generate_snp_dict.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/geno2score.py` & `eQTac-1.0.6/eQTac/geno2score.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac/get_nullseq.py` & `eQTac-1.0.6/eQTac/get_nullseq.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.5/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.5
+Version: 1.0.6
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8.3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # eQTac
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
+## Schematic 
+![](./imgs/Schematic.png)
 ## Dependence
 ### Python packages
 ```
 numpy >= 1.22.4
 pandas >= 1.4.3
 pybedtools >= 0.8.2
 pysam >= 0.16.0.1
 rpy2 >= 3.4.2
 scipy >= 1.8.1
 ```
 ### Other software (need manual installation)
 ```
-plink >= v1.90b6.24
-bedtools >= v2.30.0
+plink >= v1.90b6.24 (plink should in $PATH)
+bedtools >= v2.30.0 (bedtools should in $PATH)
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
 ```
-## Installation
+## Installation & test example
+```
+# installation
+pip install eQTac 
+
+# test examples
+git clone https://github.com/JFF1594032292/eQTac.git # just for test
+cd eQTac/Utilities_pipeline
+nohup sh example_All_pipeline.sh &
+```
+Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
 
 ## Input data
 1. Data used in model training:
-    (1) **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See test_data/test.positive.bed
-    (2) **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See test_data/test.exclude.bed.
-    (3) **Fasta file with .fai index.** Usually the human genome sequnce file in fasta format. See test.hg19.chr17.fa.
+    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
 2. Data used in eQTac calculation.
-    (1) 
+    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
+    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
+    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
+    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
 ## Usage pattern
 We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
-### Pipeline level pattern
+### Pipeline-level pattern
 For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
-It can be used as follow:
+It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
 ```
 python Part-All-eQTac_pipeline.py \
 	-p test_data/test.positive.bed \
 	-ex test_data/test.exclude.bed \
 	-pre test_data/test.pre.bed \
 	--geno test_data/test.geno \
 	--snp test_data/test.geno.snplist \
 	-fa test_data/test.hg19.chr17.fa \
 	-exp test_data/test.exp_residual \
 	-n 100 \
 	-o output_eQTac \
 	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
 ```
-### Part level pattern
+### Part-level pattern
 For the function level pattern, we provide four scripts:
 ```
+Part-1-Train_model.py
+Part-2-Generate_PRE_fa.py
+Part-3-Predict_PRE_score.py
+Part-4-Calculate_eQTac_correlation.py
+```
+It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
+```
 python Part-1-Train_model.py \
 	-p test_data/test.positive.bed \
 	-ex test_data/test.exclude.bed \
 	-o output_eQTac_part \
 	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
 
 python Part-2-Generate_PRE_fa.py \
@@ -84,23 +106,29 @@
 
 python Part-4-Calculate_eQTac_correlation.py \
 	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
 	-exp test_data/test.exp_residual \
 	-n 50 \
 	-o output_eQTac_part
 ```
-### Function level pattern
+### Function-level pattern
 For the function level pattern, we provide a series of functions:
 ```
 from eQTac.get_nullseq import get_nullseq
 from eQTac.filter_bkg import filter_bkg
 from eQTac.generate_snp_dict import generate_snp_dict
 from eQTac.generate_PRE import generate_PRE
 from eQTac.generate_mut_fa import generate_mut_fa
 from eQTac.geno2score import geno2score
 from eQTac.eQTac_correlation import eQTac_correlation
 from eQTac.eQTac_permutation import eQTac_permutation
 from eQTac.control_FDR import control_FDR
 ```
-These functions can be used to construct the whole pipeline. The Part-All-eQTac_pipeline.py file used this
+These functions can be used to construct the whole pipeline.
+### Recomend
+We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
+
+Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
 
+If you are familiar with this pipeline, you can directly use the `function-level` pattern to construct your own pipeline.
 ## Notes
+1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
```

### Comparing `eQTac-1.0.5/setup.py` & `eQTac-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.5",
+    version="1.0.6",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
     ],
-    python_requires='>=3.8.3',
+    python_requires='>=3.7',
     install_requires=[
         'numpy >= 1.22.4',
         'pandas >= 1.4.3',
         'pybedtools >= 0.8.2',
         'pysam >= 0.16.0.1',
         'rpy2 >= 3.4.2',
         'scipy >= 1.8.1'],
```

