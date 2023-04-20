# Comparing `tmp/eQTac-1.0.7.tar.gz` & `tmp/eQTac-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.7.tar", last modified: Thu Apr 20 03:41:28 2023, max compression
+gzip compressed data, was "eQTac-1.0.8.tar", last modified: Thu Apr 20 07:29:19 2023, max compression
```

## Comparing `eQTac-1.0.7.tar` & `eQTac-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.304611 eQTac-1.0.7/
--rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5926 2023-04-20 03:41:28.301618 eQTac-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5429 2023-04-20 02:35:35.000000 eQTac-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.183933 eQTac-1.0.7/eQTac/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.7/eQTac/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.7/eQTac/control_FDR.py
--rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.7/eQTac/eQTac_correlation.py
--rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.7/eQTac/eQTac_permutation.py
--rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.7/eQTac/filter_bkg.py
--rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_PRE.py
--rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_mut_fa.py
--rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_snp_dict.py
--rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.7/eQTac/geno2score.py
--rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.7/eQTac/get_nullseq.py
-drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.284663 eQTac-1.0.7/eQTac.egg-info/
--rw-rw-rw-   0        0        0     5926 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-20 03:41:28.000000 eQTac-1.0.7/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 03:41:28.308600 eQTac-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-04-20 03:41:19.000000 eQTac-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.718642 eQTac-1.0.8/
+-rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5925 2023-04-20 07:29:19.716647 eQTac-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5428 2023-04-20 07:28:59.000000 eQTac-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.590985 eQTac-1.0.8/eQTac/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.8/eQTac/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-04-20 07:27:33.000000 eQTac-1.0.8/eQTac/control_FDR.py
+-rw-rw-rw-   0        0        0     4277 2023-04-20 07:27:36.000000 eQTac-1.0.8/eQTac/eQTac_correlation.py
+-rw-rw-rw-   0        0        0     2195 2023-04-20 07:27:39.000000 eQTac-1.0.8/eQTac/eQTac_permutation.py
+-rw-rw-rw-   0        0        0     2697 2023-04-20 07:27:42.000000 eQTac-1.0.8/eQTac/filter_bkg.py
+-rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_PRE.py
+-rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_mut_fa.py
+-rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_snp_dict.py
+-rw-rw-rw-   0        0        0     3727 2023-04-20 07:27:44.000000 eQTac-1.0.8/eQTac/geno2score.py
+-rw-rw-rw-   0        0        0     2476 2023-04-20 07:27:32.000000 eQTac-1.0.8/eQTac/get_nullseq.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.697697 eQTac-1.0.8/eQTac.egg-info/
+-rw-rw-rw-   0        0        0     5925 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 07:29:19.721634 eQTac-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-04-20 07:28:25.000000 eQTac-1.0.8/setup.py
```

### Comparing `eQTac-1.0.7/LICENSE` & `eQTac-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.7/PKG-INFO` & `eQTac-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.7
+Version: 1.0.8
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
@@ -14,20 +14,20 @@
 # eQTac
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Schematic 
 ![](./imgs/Schematic.png)
 ## Dependence
 ### Python packages
 ```
-numpy >= 1.22.4
-pandas >= 1.4.3
-pybedtools >= 0.8.2
-pysam >= 0.16.0.1
-rpy2 >= 3.4.2
-scipy >= 1.8.1
+numpy >= 1.21.6
+pandas >= 1.2.3
+pybedtools >= 0.8.1
+pysam >= 0.15.3
+rpy2 >= 3.5.11
+scipy >= 1.7.3
 ```
 ### Other software (need manual installation)
 ```
 plink >= v1.90b6.24 (plink should in $PATH)
 bedtools >= v2.30.0 (bedtools should in $PATH)
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
```

### Comparing `eQTac-1.0.7/README.md` & `eQTac-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # eQTac
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Schematic 
 ![](./imgs/Schematic.png)
 ## Dependence
 ### Python packages
 ```
-numpy >= 1.22.4
-pandas >= 1.4.3
-pybedtools >= 0.8.2
-pysam >= 0.16.0.1
-rpy2 >= 3.4.2
-scipy >= 1.8.1
+numpy >= 1.21.6
+pandas >= 1.2.3
+pybedtools >= 0.8.1
+pysam >= 0.15.3
+rpy2 >= 3.5.11
+scipy >= 1.7.3
 ```
 ### Other software (need manual installation)
 ```
 plink >= v1.90b6.24 (plink should in $PATH)
 bedtools >= v2.30.0 (bedtools should in $PATH)
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
```

### Comparing `eQTac-1.0.7/eQTac/control_FDR.py` & `eQTac-1.0.8/eQTac/control_FDR.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,11 +42,11 @@
     observe_data = observe_data.sort_values(by="p")
     # 保存文件
     observe_data.to_csv(output_file, sep="\t", header=True, index=False)
 
 
 if __name__ == "__main__":
     control_FDR(
-        "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result",
-        "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.permutation_plist",
-        "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt"
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result",
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.permutation_plist",
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt"
     )
```

### Comparing `eQTac-1.0.7/eQTac/eQTac_correlation.py` & `eQTac-1.0.8/eQTac/eQTac_correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,10 +88,10 @@
 def eQTac_correlation(PRE_scorefile, exp_file, result_file):
     score_data, exp_data, d_gene_info, d_cis, d_pre_info = extract_data(PRE_scorefile, exp_file)
     with open(result_file, 'w') as ff:
         calculate_correlation(score_data, exp_data, d_gene_info, d_cis, d_pre_info, ff)
 
 
 if __name__ == "__main__":
-    eQTac_correlation("../output_eQTac/test.geno.vcf.gz.PRE_score",
-                      "../test_data/test.exp_residual",
-                      "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result")
+    eQTac_correlation("../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score",
+                      "../Utilities_pipeline/test_data/test.exp_residual",
+                      "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result")
```

### Comparing `eQTac-1.0.7/eQTac/eQTac_permutation.py` & `eQTac-1.0.8/eQTac/eQTac_permutation.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,10 +45,10 @@
                     beta, se, p, intercept, r_value = st_linear_reg(exp, score)
                     ff.write("%.5g" % p + "\n")
             print("Permutation", seed + 1, "finished")
 
 
 if __name__ == "__main__":
     eQTac_permutation(
-        "../output_eQTac/test.geno.vcf.gz.PRE_scoree",
-        "../test_data/test.exp_residual", 100,
-        "../output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.permutation_plist")
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_scoree",
+        "../Utilities_pipeline/test_data/test.exp_residual", 100,
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz.PRE_score.eQTac_result.permutation_plist")
```

### Comparing `eQTac-1.0.7/eQTac/filter_bkg.py` & `eQTac-1.0.8/eQTac/filter_bkg.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,9 +66,10 @@
                 if re.sub("^>", "", name) in name_set:
                     ff2.write(">" + name + "\n")
                     ff2.write(seq + "\n")
     return out_neg_fa, out_neg_bed
 
 
 if __name__ == '__main__':
-    filter_bkg("../output_eQTac/test.positive.negraw.bed", "../output_eQTac/test.positive.negraw.fa",
-               "../test_data/test.exclude.bed")
+    filter_bkg("../Utilities_pipeline/example.output_eQTac/test.positive.negraw.bed", 
+               "../Utilities_pipeline/example.output_eQTac/test.positive.negraw.fa",
+               "../Utilities_pipeline/test_data/test.exclude.bed")
```

### Comparing `eQTac-1.0.7/eQTac/generate_PRE.py` & `eQTac-1.0.8/eQTac/generate_PRE.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.7/eQTac/generate_mut_fa.py` & `eQTac-1.0.8/eQTac/generate_mut_fa.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.7/eQTac/generate_snp_dict.py` & `eQTac-1.0.8/eQTac/generate_snp_dict.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.7/eQTac/geno2score.py` & `eQTac-1.0.8/eQTac/geno2score.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,11 +77,11 @@
             snps = ",".join(snp_set)
             ff.write("\t".join([ch, start, end, enhancer, "%d" % snp_count, snps] + score_list) + "\n")
     return PRE_scorefile
 
 
 if __name__ == "__main__":
     geno2score(
-        "../output_eQTac/test.geno.vcf.gz",
-        "../output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.pred_out",
-        "../output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info"
+        "../Utilities_pipeline/example.output_eQTac/test.geno.vcf.gz",
+        "../Utilities_pipeline/example.output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.pred_out",
+        "../Utilities_pipeline/example.output_eQTac/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info"
     )
```

### Comparing `eQTac-1.0.7/eQTac/get_nullseq.py` & `eQTac-1.0.8/eQTac/get_nullseq.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     robjects.r(
         "library(gkmSVM);genNullSeqs('%(pos_bed_newpath)s',nMaxTrials=20,xfold=2.5,GC_match_tol=0.05,repeat_match_tol=0.05,length_match_tol=0.05,batchsize=500000,genomeVersion='hg19', outputPosFastaFN='%(pos_fa)s', outputBedFN='%(negraw_bed)s', outputNegFastaFN='%(negraw_fa)s')"
         % d)
     return pos_fa, pos_bed_newpath, negraw_fa, negraw_bed
 
 
 if __name__ == '__main__':
-    get_nullseq("../test_data/test.positive.bed", ".")
+    get_nullseq("../Utilities_pipeline/test_data/test.positive.bed", ".")
```

### Comparing `eQTac-1.0.7/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.8/eQTac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.7
+Version: 1.0.8
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
@@ -14,20 +14,20 @@
 # eQTac
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Schematic 
 ![](./imgs/Schematic.png)
 ## Dependence
 ### Python packages
 ```
-numpy >= 1.22.4
-pandas >= 1.4.3
-pybedtools >= 0.8.2
-pysam >= 0.16.0.1
-rpy2 >= 3.4.2
-scipy >= 1.8.1
+numpy >= 1.21.6
+pandas >= 1.2.3
+pybedtools >= 0.8.1
+pysam >= 0.15.3
+rpy2 >= 3.5.11
+scipy >= 1.7.3
 ```
 ### Other software (need manual installation)
 ```
 plink >= v1.90b6.24 (plink should in $PATH)
 bedtools >= v2.30.0 (bedtools should in $PATH)
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
```

### Comparing `eQTac-1.0.7/setup.py` & `eQTac-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.7",
+    version="1.0.8",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
@@ -19,10 +19,10 @@
     ],
     python_requires='>=3.7',
     install_requires=[
         'numpy >= 1.21.6',
         'pandas >= 1.2.3',
         'pybedtools >= 0.8.1',
         'pysam >= 0.15.3',
-        'rpy2 >= 3.4.2',
+        'rpy2 >= 3.5.11',
         'scipy >= 1.7.3'],
 )
```

