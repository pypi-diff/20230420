# Comparing `tmp/snps-2.7.1.tar.gz` & `tmp/snps-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snps-2.7.1.tar", last modified: Mon Feb 13 05:37:48 2023, max compression
+gzip compressed data, was "snps-2.7.2.tar", last modified: Thu Apr 20 06:51:22 2023, max compression
```

## Comparing `snps-2.7.1.tar` & `snps-2.7.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-13 05:37:39.000000 snps-2.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-02-13 05:37:39.000000 snps-2.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-13 05:37:39.000000 snps-2.7.1/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-13 05:37:39.000000 snps-2.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-02-13 05:37:39.000000 snps-2.7.1/LICENSES-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-13 05:37:39.000000 snps-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-02-13 05:37:48.966438 snps-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-02-13 05:37:39.000000 snps-2.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.958438 snps-2.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-13 05:37:39.000000 snps-2.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 05:37:39.000000 snps-2.7.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-02-13 05:37:39.000000 snps-2.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 05:37:39.000000 snps-2.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 05:37:39.000000 snps-2.7.1/docs/contributors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.958438 snps-2.7.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    42629 2023-02-13 05:37:39.000000 snps-2.7.1/docs/images/snps_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-02-13 05:37:39.000000 snps-2.7.1/docs/images/snps_banner.svg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-13 05:37:39.000000 snps-2.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-13 05:37:39.000000 snps-2.7.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-13 05:37:39.000000 snps-2.7.1/docs/output_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-13 05:37:39.000000 snps-2.7.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 05:37:39.000000 snps-2.7.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-13 05:37:39.000000 snps-2.7.1/docs/snps.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-13 05:37:39.000000 snps-2.7.1/docs/snps_banner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-13 05:37:39.000000 snps-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-13 05:37:48.970438 snps-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-02-13 05:37:39.000000 snps-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.954438 snps-2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.970438 snps-2.7.1/src/snps/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-13 05:37:48.970438 snps-2.7.1/src/snps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/ensembl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.962438 snps-2.7.1/src/snps/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48161 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34947 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    71901 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/snps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-02-13 05:37:39.000000 snps-2.7.1/src/snps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.962438 snps-2.7.1/src/snps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-02-13 05:37:48.000000 snps-2.7.1/src/snps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-02-13 05:37:48.000000 snps-2.7.1/src/snps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 05:37:48.000000 snps-2.7.1/src/snps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-13 05:37:48.000000 snps-2.7.1/src/snps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 05:37:48.000000 snps-2.7.1/src/snps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.962438 snps-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-02-13 05:37:39.000000 snps-2.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/tests/input/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/23andme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/23andme_allele.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/23andme_win.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/DNALand.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/GRCh37.csv
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/GRCh37_PAR.csv
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/GRCh38.csv
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/NCBI36.csv
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/ancestry.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/ancestry_mt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/ancestry_multi_sep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/chromosomes.csv
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/circledna.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/codigo46.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/discrepant_snps.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/duplicate_rsids.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/ftdna.csv
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/ftdna_famfinder.csv
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic.csv
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic.fa
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic_extra_column.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic_header_comment.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic_multi_rsid.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic_no_header.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/generic_non_standard_columns.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/genesforgood.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/livingdna.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/mapmygenome.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/mapmygenome_alt_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/myheritage.csv
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/myheritage_extra_quotes.csv
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/sano.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/tellmeGen.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/testvcf.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/testvcf_chr_prefix.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/testvcf_multi_sample.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/testvcf_phased.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-13 05:37:39.000000 snps-2.7.1/tests/input/unannotated_testvcf.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:39.000000 snps-2.7.1/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-02-13 05:37:39.000000 snps-2.7.1/tests/io/test_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12750 2023-02-13 05:37:39.000000 snps-2.7.1/tests/io/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_chrom_prefix_chr.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_generic.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/tests/output/vcf_qc/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_qc/qc_only_F_qc_filter_F.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_qc/qc_only_F_qc_filter_T.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_qc/qc_only_T_qc_filter_F.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-13 05:37:39.000000 snps-2.7.1/tests/output/vcf_qc/qc_only_T_qc_filter_T.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 05:37:48.966438 snps-2.7.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-13 05:37:39.000000 snps-2.7.1/tests/resources/dbsnp_151_37_reverse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-13 05:37:39.000000 snps-2.7.1/tests/resources/gsa_chrpos_map.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-13 05:37:39.000000 snps-2.7.1/tests/resources/gsa_rsid_map.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-02-13 05:37:39.000000 snps-2.7.1/tests/test_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50247 2023-02-13 05:37:39.000000 snps-2.7.1/tests/test_snps.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-02-13 05:37:39.000000 snps-2.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 06:51:09.000000 snps-2.7.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-20 06:51:09.000000 snps-2.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-20 06:51:09.000000 snps-2.7.2/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-20 06:51:09.000000 snps-2.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-04-20 06:51:09.000000 snps-2.7.2/LICENSES-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 06:51:09.000000 snps-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-20 06:51:22.385133 snps-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-04-20 06:51:09.000000 snps-2.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.373133 snps-2.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 06:51:09.000000 snps-2.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 06:51:09.000000 snps-2.7.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-20 06:51:09.000000 snps-2.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 06:51:09.000000 snps-2.7.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 06:51:09.000000 snps-2.7.2/docs/contributors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.373133 snps-2.7.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    42629 2023-04-20 06:51:09.000000 snps-2.7.2/docs/images/snps_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-20 06:51:09.000000 snps-2.7.2/docs/images/snps_banner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-20 06:51:09.000000 snps-2.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-20 06:51:09.000000 snps-2.7.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 06:51:09.000000 snps-2.7.2/docs/output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 06:51:09.000000 snps-2.7.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:51:09.000000 snps-2.7.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-20 06:51:09.000000 snps-2.7.2/docs/snps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-20 06:51:09.000000 snps-2.7.2/docs/snps_banner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 06:51:09.000000 snps-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 06:51:22.385133 snps-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-20 06:51:09.000000 snps-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.369133 snps-2.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/src/snps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 06:51:22.385133 snps-2.7.2/src/snps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/ensembl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.377133 snps-2.7.2/src/snps/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48161 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34947 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71901 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/snps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-20 06:51:09.000000 snps-2.7.2/src/snps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.373133 snps-2.7.2/src/snps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-20 06:51:22.000000 snps-2.7.2/src/snps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-20 06:51:22.000000 snps-2.7.2/src/snps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:51:22.000000 snps-2.7.2/src/snps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 06:51:22.000000 snps-2.7.2/src/snps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 06:51:22.000000 snps-2.7.2/src/snps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.377133 snps-2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-04-20 06:51:09.000000 snps-2.7.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.381133 snps-2.7.2/tests/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/23andme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/23andme_allele.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/23andme_win.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/DNALand.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/GRCh37.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/GRCh37_PAR.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/GRCh38.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/NCBI36.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/ancestry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/ancestry_mt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/ancestry_multi_sep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/chromosomes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/circledna.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/codigo46.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/discrepant_snps.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/duplicate_rsids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/ftdna.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/ftdna_famfinder.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic_extra_column.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic_header_comment.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic_multi_rsid.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic_no_header.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/generic_non_standard_columns.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/genesforgood.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/livingdna.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/mapmygenome.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/mapmygenome_alt_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/myheritage.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/myheritage_extra_quotes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/sano.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/tellmeGen.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/testvcf.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/testvcf_chr_prefix.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/testvcf_multi_sample.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/testvcf_phased.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-20 06:51:09.000000 snps-2.7.2/tests/input/unannotated_testvcf.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:09.000000 snps-2.7.2/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-04-20 06:51:09.000000 snps-2.7.2/tests/io/test_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12750 2023-04-20 06:51:09.000000 snps-2.7.2/tests/io/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_chrom_prefix_chr.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_generic.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/tests/output/vcf_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_qc/qc_only_F_qc_filter_F.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_qc/qc_only_F_qc_filter_T.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_qc/qc_only_T_qc_filter_F.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 06:51:09.000000 snps-2.7.2/tests/output/vcf_qc/qc_only_T_qc_filter_T.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:22.385133 snps-2.7.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 06:51:09.000000 snps-2.7.2/tests/resources/dbsnp_151_37_reverse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 06:51:09.000000 snps-2.7.2/tests/resources/gsa_chrpos_map.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 06:51:09.000000 snps-2.7.2/tests/resources/gsa_rsid_map.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-04-20 06:51:09.000000 snps-2.7.2/tests/test_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50193 2023-04-20 06:51:09.000000 snps-2.7.2/tests/test_snps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-20 06:51:09.000000 snps-2.7.2/versioneer.py
```

### Comparing `snps-2.7.1/CONTRIBUTING.rst` & `snps-2.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/CONTRIBUTORS.rst` & `snps-2.7.2/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/LICENSE.txt` & `snps-2.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/LICENSES-3RD-PARTY.txt` & `snps-2.7.2/LICENSES-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/PKG-INFO` & `snps-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snps
-Version: 2.7.1
+Version: 2.7.2
 Summary: tools for reading, writing, merging, and remapping SNPs
 Home-page: https://github.com/apriha/snps
 Author: Andrew Riha
 Author-email: apriha@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://snps.readthedocs.io/
 Project-URL: Changelog, https://github.com/apriha/snps/releases
```

### Comparing `snps-2.7.1/README.rst` & `snps-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/Makefile` & `snps-2.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/conf.py` & `snps-2.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/images/snps_banner.png` & `snps-2.7.2/docs/images/snps_banner.png`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/images/snps_banner.svg` & `snps-2.7.2/docs/images/snps_banner.svg`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/index.rst` & `snps-2.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/installation.rst` & `snps-2.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/output_files.rst` & `snps-2.7.2/docs/output_files.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/snps.rst` & `snps-2.7.2/docs/snps.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/docs/snps_banner.rst` & `snps-2.7.2/docs/snps_banner.rst`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/setup.py` & `snps-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/__init__.py` & `snps-2.7.2/src/snps/__init__.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/ensembl.py` & `snps-2.7.2/src/snps/ensembl.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/io/__init__.py` & `snps-2.7.2/src/snps/io/__init__.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/io/reader.py` & `snps-2.7.2/src/snps/io/reader.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/io/writer.py` & `snps-2.7.2/src/snps/io/writer.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/resources.py` & `snps-2.7.2/src/snps/resources.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/snps.py` & `snps-2.7.2/src/snps/snps.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps/utils.py` & `snps-2.7.2/src/snps/utils.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/src/snps.egg-info/PKG-INFO` & `snps-2.7.2/src/snps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snps
-Version: 2.7.1
+Version: 2.7.2
 Summary: tools for reading, writing, merging, and remapping SNPs
 Home-page: https://github.com/apriha/snps
 Author: Andrew Riha
 Author-email: apriha@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://snps.readthedocs.io/
 Project-URL: Changelog, https://github.com/apriha/snps/releases
```

### Comparing `snps-2.7.1/src/snps.egg-info/SOURCES.txt` & `snps-2.7.2/src/snps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/__init__.py` & `snps-2.7.2/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,21 +541,24 @@
             chrom=["1"] * 8,
             pos=list(range(101, 109)),
             genotype=["AA", "CC", "GG", "TT", np.nan, "GC", "TC", "AT"],
         )
 
     def generic_snps_vcf(self):
         df = self.generic_snps()
-        return df.append(
-            self.create_snp_df(
-                rsid=["rs" + str(i) for i in range(12, 18)],
-                chrom=["1"] * 6,
-                pos=list(range(112, 118)),
-                genotype=[np.nan] * 6,
-            )
+        return pd.concat(
+            [
+                df,
+                self.create_snp_df(
+                    rsid=["rs" + str(i) for i in range(12, 18)],
+                    chrom=["1"] * 6,
+                    pos=list(range(112, 118)),
+                    genotype=[np.nan] * 6,
+                ),
+            ]
         )
 
     def run_parsing_tests(
         self, file, source, phased=False, build=37, build_detected=False, snps_df=None
     ):
         self.make_parsing_assertions(
             self.parse_file(file), source, phased, build, build_detected, snps_df
```

### Comparing `snps-2.7.1/tests/input/discrepant_snps.csv` & `snps-2.7.2/tests/input/discrepant_snps.csv`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/mapmygenome.txt` & `snps-2.7.2/tests/input/mapmygenome.txt`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/mapmygenome_alt_header.txt` & `snps-2.7.2/tests/input/mapmygenome_alt_header.txt`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/testvcf.vcf` & `snps-2.7.2/tests/input/testvcf.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/testvcf_chr_prefix.vcf` & `snps-2.7.2/tests/input/testvcf_chr_prefix.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/testvcf_multi_sample.vcf` & `snps-2.7.2/tests/input/testvcf_multi_sample.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/input/testvcf_phased.vcf` & `snps-2.7.2/tests/input/testvcf_phased.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/io/test_reader.py` & `snps-2.7.2/tests/io/test_reader.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/io/test_writer.py` & `snps-2.7.2/tests/io/test_writer.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/test_resources.py` & `snps-2.7.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `snps-2.7.1/tests/test_snps.py` & `snps-2.7.2/tests/test_snps.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,20 +727,16 @@
                     pd.testing.assert_index_equal(
                         result[key],
                         expected_result[key],
                         check_exact=True,
                         check_names=True,
                     )
                 else:
-                    pd.testing.assert_index_equal(
-                        result[key],
-                        pd.Index([], name="rsid"),
-                        check_exact=True,
-                        check_names=True,
-                    )
+                    self.assertTrue(result[key].empty)
+                    self.assertEqual(result[key].name, "rsid")
 
     def test_source_snps(self):
         with tempfile.TemporaryDirectory() as tmpdir:
             s = SNPs("tests/input/GRCh37.csv", output_dir=tmpdir)
             self.assertEqual(s.source, "generic")
             results = s.merge((SNPs("tests/input/23andme.txt"),))
             self.assertEqual(s.source, "generic, 23andMe")
@@ -1025,21 +1021,24 @@
         )
         pd.testing.assert_frame_equal(
             s.discrepant_vcf_position, get_empty_snps_dataframe(), check_exact=True
         )
 
     def test_merge_chrom(self):
         s1 = SNPs("tests/input/generic.csv")
-        df = s1.snps.append(
-            self.create_snp_df(
-                rsid=["rs100", "rs101", "rs102", "rs103"],
-                chrom=["Y", "Y", "Y", "Y"],
-                pos=[100, 101, 102, 103],
-                genotype=["A", np.nan, "A", "A"],
-            )
+        df = pd.concat(
+            [
+                s1.snps,
+                self.create_snp_df(
+                    rsid=["rs100", "rs101", "rs102", "rs103"],
+                    chrom=["Y", "Y", "Y", "Y"],
+                    pos=[100, 101, 102, 103],
+                    genotype=["A", np.nan, "A", "A"],
+                ),
+            ]
         )
         s1._snps = df.copy()
         s2 = SNPs()
         s2._build = 37
         s2._snps = df.copy()
 
         # set values for chrom that will be ignored (that would otherwise result in
```

### Comparing `snps-2.7.1/versioneer.py` & `snps-2.7.2/versioneer.py`

 * *Files identical despite different names*

