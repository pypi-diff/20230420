# Comparing `tmp/hepi-0.2.8.tar.gz` & `tmp/hepi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepi-0.2.8.tar", last modified: Thu Oct 27 11:16:12 2022, max compression
+gzip compressed data, was "hepi-0.2.9.tar", max compression
```

## Comparing `hepi-0.2.8.tar` & `hepi-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,121 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-10-27 11:16:02.000000 hepi-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       50 2022-10-27 11:16:02.000000 hepi-0.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3717 2022-10-27 11:16:12.147714 hepi-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3236 2022-10-27 11:16:02.000000 hepi-0.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/
--rw-r--r--   0 root         (0) root         (0)      524 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60689 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/input.py
--rw-r--r--   0 root         (0) root         (0)     4698 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/madgraph/
--rw-r--r--   0 root         (0) root         (0)      131 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/__init__.py
--rw-r--r--   0 root         (0) root         (0)      112 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/lo.mg
--rw-r--r--   0 root         (0) root         (0)      109 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/nlo.mg
--rw-r--r--   0 root         (0) root         (0)    35804 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/param_card.dat
--rw-r--r--   0 root         (0) root         (0)     2075 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/result.py
--rw-r--r--   0 root         (0) root         (0)     6256 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/run.py
--rw-r--r--   0 root         (0) root         (0)    11548 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/run_card_no_madstr.dat
--rw-r--r--   0 root         (0) root         (0)    12526 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/madgraph/run_card_with_madstr.dat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/nllfast/
--rw-r--r--   0 root         (0) root         (0)      177 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/nllfast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      446 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/nllfast/result.py
--rw-r--r--   0 root         (0) root         (0)     5288 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/nllfast/run.py
--rw-r--r--   0 root         (0) root         (0)    28495 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/output.py
--rw-r--r--   0 root         (0) root         (0)    20429 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/prospino2/
--rw-r--r--   0 root         (0) root         (0)      167 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/prospino2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9108 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/prospino2/prospino_main.f90_template
--rw-r--r--   0 root         (0) root         (0)     6973 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/prospino2/run.py
--rw-r--r--   0 root         (0) root         (0)    14064 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/resummino/
--rw-r--r--   0 root         (0) root         (0)      170 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/resummino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4492 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/resummino/plot_template.in
--rw-r--r--   0 root         (0) root         (0)     6296 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/resummino/result.py
--rw-r--r--   0 root         (0) root         (0)     3641 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/resummino/run.py
--rw-r--r--   0 root         (0) root         (0)    13627 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi/spheno/
--rw-r--r--   0 root         (0) root         (0)      154 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/spheno/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2088 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/spheno/run.py
--rw-r--r--   0 root         (0) root         (0)     6434 2022-10-27 11:16:02.000000 hepi-0.2.8/hepi/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 11:16:12.147714 hepi-0.2.8/hepi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3717 2022-10-27 11:16:12.000000 hepi-0.2.8/hepi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2022-10-27 11:16:12.000000 hepi-0.2.8/hepi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 11:16:12.000000 hepi-0.2.8/hepi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      305 2022-10-27 11:16:12.000000 hepi-0.2.8/hepi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-10-27 11:16:12.000000 hepi-0.2.8/hepi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-27 11:16:12.147714 hepi-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1784 2022-10-27 11:16:02.000000 hepi-0.2.8/setup.py
+-rw-r--r--   0        0        0    35149 2023-03-21 18:27:05.434826 hepi-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3236 2023-03-21 18:27:05.434826 hepi-0.2.9/README.md
+-rw-r--r--   0        0        0      668 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/__init__.py
+-rw-r--r--   0        0        0       20 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/__init__.py
+-rw-r--r--   0        0        0      750 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/data.py
+-rw-r--r--   0        0        0     6272 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_deg_1000022_-1000024_NNLL.json
+-rw-r--r--   0        0        0     6280 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_deg_1000022_1000023_NNLL.json
+-rw-r--r--   0        0        0     6276 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_deg_1000022_1000024_NNLL.json
+-rw-r--r--   0        0        0     6280 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_deg_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0    30690 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_nondeg_1000022_1000023_NNLL.json
+-rw-r--r--   0        0        0    30819 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_nondeg_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0    30678 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_nondeg_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0    30697 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_hino_nondeg_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0     4419 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_sleptons_1000011_-1000011_NNLL.json
+-rw-r--r--   0        0        0     4420 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_sleptons_1000015_-1000015_NNLL.json
+-rw-r--r--   0        0        0     4419 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_sleptons_2000011_-2000011_NNLL.json
+-rw-r--r--   0        0        0     8178 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_wino_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0     8182 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_wino_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0     8177 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13000_wino_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0     6278 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_deg_1000022_-1000024_NNLL.json
+-rw-r--r--   0        0        0     6270 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_deg_1000022_1000023_NNLL.json
+-rw-r--r--   0        0        0     6267 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_deg_1000022_1000024_NNLL.json
+-rw-r--r--   0        0        0     6283 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_deg_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0    30683 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_nondeg_1000022_1000023_NNLL.json
+-rw-r--r--   0        0        0    30790 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_nondeg_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0    30681 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_nondeg_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0    30705 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_hino_nondeg_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0     4417 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_sleptons_1000011_-1000011_NNLL.json
+-rw-r--r--   0        0        0     4426 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_sleptons_1000015_-1000015_NNLL.json
+-rw-r--r--   0        0        0     4413 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_sleptons_2000011_-2000011_NNLL.json
+-rw-r--r--   0        0        0     8195 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_wino_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0     8181 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_wino_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0     8179 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/13600_wino_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0     6900 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_GGxsec_NLO+NLL.json
+-rw-r--r--   0        0        0     6896 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_GGxsec_NNLO+NNLL.json
+-rw-r--r--   0        0        0     9139 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SGxsec_NLO+NLL.json
+-rw-r--r--   0        0        0     9121 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SGxsec_NNLO+NNLL.json
+-rw-r--r--   0        0        0     9073 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SSBxsec_NLO+NLL.json
+-rw-r--r--   0        0        0     9074 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SSBxsec_NNLO+NNLL.json
+-rw-r--r--   0        0        0     9080 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SSxsec_NLO+NLL.json
+-rw-r--r--   0        0        0     9058 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_SGmodel_SSxsec_NNLO+NNLL.json
+-rw-r--r--   0        0        0    35695 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_gluino_NNLO+NNLL.json
+-rw-r--r--   0        0        0    41117 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_gluinosquark_NNLO+NNLL.json
+-rw-r--r--   0        0        0     2952 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_hino_NLO+NLL.json
+-rw-r--r--   0        0        0     8861 2023-03-21 18:27:06.614834 hepi-0.2.9/hepi/data/json/pp13_hinosplit_C1C1_NLO+NLL.json
+-rw-r--r--   0        0        0    11448 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_hinosplit_C1mN2_NLO+NLL.json
+-rw-r--r--   0        0        0    11402 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_hinosplit_C1pN2_NLO+NLL.json
+-rw-r--r--   0        0        0    11410 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_hinosplit_N2N1_NLO+NLL.json
+-rw-r--r--   0        0        0     4516 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_slep_LR_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     2675 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_slep_L_NLO+NLL.json
+-rw-r--r--   0        0        0     4911 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_slep_L_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     2704 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_slep_R_NLO+NLL.json
+-rw-r--r--   0        0        0     4900 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_slep_R_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     4923 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_snu-snu_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     4906 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_snuM-slep_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     4899 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_snuP-slep_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0    40178 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_squark_NNLO+NNLL.json
+-rw-r--r--   0        0        0     4904 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stau_LR_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     2706 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stau_L_NLO+NLL.json
+-rw-r--r--   0        0        0     4464 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stau_L_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0     2735 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stau_R_NLO+NLL.json
+-rw-r--r--   0        0        0     4476 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stau_R_NLO+NLL_PDF4LHC.json
+-rw-r--r--   0        0        0    41909 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_stopsbottom_NNLO+NNLL.json
+-rw-r--r--   0        0        0     6252 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_wino_C1C1_NLO+NLL.json
+-rw-r--r--   0        0        0     6278 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_winom_C1N2_NLO+NLL.json
+-rw-r--r--   0        0        0     6267 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_winop_C1N2_NLO+NLL.json
+-rw-r--r--   0        0        0     6267 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/pp13_winopm_C1N2_NLO+NLL.json
+-rw-r--r--   0        0        0   148241 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_-1000024_LO.json
+-rw-r--r--   0        0        0   163513 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_-1000024_NLO.json
+-rw-r--r--   0        0        0   163479 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0   148297 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_1000024_LO.json
+-rw-r--r--   0        0        0   163449 2023-03-21 18:27:06.618834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_1000024_NLO.json
+-rw-r--r--   0        0        0   163428 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0   147899 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000024_-1000024_LO.json
+-rw-r--r--   0        0        0   163494 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000024_-1000024_NLO.json
+-rw-r--r--   0        0        0   163592 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13000_wino_1000024_-1000024_NNLL.json
+-rw-r--r--   0        0        0   148251 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_-1000024_LO.json
+-rw-r--r--   0        0        0   163444 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_-1000024_NLO.json
+-rw-r--r--   0        0        0   163398 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_-1000024_NNLL.json
+-rw-r--r--   0        0        0   148273 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_1000024_LO.json
+-rw-r--r--   0        0        0   163460 2023-03-21 18:27:06.622834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_1000024_NLO.json
+-rw-r--r--   0        0        0   163456 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000023_1000024_NNLL.json
+-rw-r--r--   0        0        0   148182 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000024_-1000024_LO.json
+-rw-r--r--   0        0        0   163430 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000024_-1000024_NLO.json
+-rw-r--r--   0        0        0   163510 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/data/json/sqsq_13600_wino_1000024_-1000024_NNLL.json
+-rwxr-xr-x   0        0        0     9138 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/fast.py
+-rw-r--r--   0        0        0    60103 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/input.py
+-rw-r--r--   0        0        0     1151 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/interpolate.py
+-rw-r--r--   0        0        0     6634 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/load.py
+-rw-r--r--   0        0        0     1327 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/order.py
+-rw-r--r--   0        0        0    32672 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/output.py
+-rw-r--r--   0        0        0     1512 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/particles.py
+-rw-r--r--   0        0        0       20 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/plot/__init__.py
+-rw-r--r--   0        0        0    18655 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/plot/plot.py
+-rw-r--r--   0        0        0    13796 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/results.py
+-rw-r--r--   0        0        0       19 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/__init__.py
+-rw-r--r--   0        0        0      131 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/__init__.py
+-rw-r--r--   0        0        0      112 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/lo.mg
+-rw-r--r--   0        0        0      109 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/nlo.mg
+-rw-r--r--   0        0        0    35804 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/param_card.dat
+-rw-r--r--   0        0        0     2027 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/result.py
+-rw-r--r--   0        0        0     6237 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/run.py
+-rw-r--r--   0        0        0    11548 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/run_card_no_madstr.dat
+-rw-r--r--   0        0        0    12526 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/madgraph/run_card_with_madstr.dat
+-rw-r--r--   0        0        0      177 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/nllfast/__init__.py
+-rw-r--r--   0        0        0      500 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/nllfast/result.py
+-rw-r--r--   0        0        0     5281 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/nllfast/run.py
+-rw-r--r--   0        0        0      167 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/prospino2/__init__.py
+-rw-r--r--   0        0        0     9106 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/prospino2/prospino_main.f90_template
+-rw-r--r--   0        0        0     7327 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/prospino2/run.py
+-rw-r--r--   0        0        0      171 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/resummino/__init__.py
+-rw-r--r--   0        0        0     4492 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/resummino/plot_template.in
+-rw-r--r--   0        0        0     6507 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/resummino/result.py
+-rw-r--r--   0        0        0     3532 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/resummino/run.py
+-rw-r--r--   0        0        0    13686 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/run.py
+-rw-r--r--   0        0        0      155 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/spheno/__init__.py
+-rw-r--r--   0        0        0     2162 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/run/spheno/run.py
+-rw-r--r--   0        0        0     3703 2023-03-21 18:27:06.626834 hepi-0.2.9/hepi/util.py
+-rw-r--r--   0        0        0     1799 2023-03-21 18:27:09.066851 hepi-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 hepi-0.2.9/setup.py
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 hepi-0.2.9/PKG-INFO
```

### Comparing `hepi-0.2.8/LICENSE` & `hepi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/PKG-INFO` & `hepi-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: hepi
-Version: 0.2.8
-Summary: hepi
-Home-page: https://gitlab.com/APN-Pucky/hepi
-Author: APN
-Author-email: APN-Pucky@no-reply.github.com
+Version: 0.2.9
+Summary: Interface to High Energy Physics tools.
+Home-page: https://github.com/APN-Pucky/HEPi
+Author: Alexander Puck Neuwirth
+Author-email: alexander@neuwirth-informatik.de
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: lhapdf
+Requires-Dist: lhapdf (>=6,<7) ; extra == "lhapdf"
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas (>=1.0.0)
+Requires-Dist: particle
+Requires-Dist: pqdm
+Requires-Dist: pyslha
+Requires-Dist: scipy (>=1.7.0)
+Requires-Dist: smpl (>=0.0.152)
+Requires-Dist: sympy
+Requires-Dist: uncertainties
+Requires-Dist: validators
+Project-URL: Repository, https://github.com/APN-Pucky/HEPi
 Description-Content-Type: text/markdown
-Provides-Extra: opt
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
 
 # HEPi
 
 Python interface for gluing together several HEP programs (e.g. from HEPForge <https://www.hepforge.org/>).
 
 [![PyPI version][pypi image]][pypi link] ![downloads](https://img.shields.io/pypi/dm/hepi.svg) 
 
@@ -76,7 +88,8 @@
 [c t l]: https://coveralls.io/github/APN-Pucky/HEPi?branch=master
 [c t i]: https://coveralls.io/repos/github/APN-Pucky/HEPi/badge.svg?branch=master
 
 [rtd s i]: https://readthedocs.org/projects/hepi/badge/?version=stable
 [rtd s l]: https://hepi.readthedocs.io/en/stable/?badge=stable
 [rtd t i]: https://readthedocs.org/projects/hepi/badge/?version=latest
 [rtd t l]: https://hepi.readthedocs.io/en/latest/?badge=latest
+
```

### Comparing `hepi-0.2.8/README.md` & `hepi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/hepi/input.py` & `hepi-0.2.9/hepi/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from enum import IntEnum
+import copy
 import os
 import shutil
 import warnings
-import copy
-
-import numpy as np
 from typing import Iterable, List
 
+import numpy as np
 import pyslha
-from .util import DictData, get_LR_partner, lhapdf_name_to_id
 
-import lhapdf
+from .order import Order, order_to_string, replace_macros, xsec_to_order
+from .util import DictData, lhapdf_name_to_id
 
 in_dir = "./input/"
 """Input directory."""
 out_dir = "./output/"
 """Output directory."""
 pre = "nice -n 5"
 """Prefix for run commands."""
@@ -66,15 +64,15 @@
 
 def set_output_dir(outd, create: bool = True):
     """
     Sets the output directory.
 
     Args:
         outd (str): new output directory.
-		create (bool): create directory if not existing
+                create (bool): create directory if not existing
     """
     global out_dir
     if create:
         os.makedirs(outd, exist_ok=True)
     out_dir = outd
 
 
@@ -85,65 +83,14 @@
     Args:
         ppre (str): new command prefix.
     """
     global pre
     pre = ppre
 
 
-class Order(IntEnum):
-    """
-    Computation orders.
-    """
-    LO = 0
-    """Leading Order"""
-    NLO = 1
-    """Next-to-Leading Order"""
-    NLO_PLUS_NLL = 2
-    """Next-to-Leading Order plus Next-to-Leading Logarithms"""
-    aNNLO_PLUS_NNLL = 3
-    """Approximate Next-to-next-to-Leading Order plus Next-to-next-to-Leading Logarithms"""
-
-
-def replace_macros(s: str) -> str:
-    return s.replace("_PLUS_", "+").replace(" ", "\\ ")
-
-
-def order_to_string(o: Order, json_style=False, no_macros=False) -> str:
-    ret = ""
-    if o == Order.LO:
-        ret = "LO"
-    elif o == Order.NLO:
-        ret = "NLO"
-    elif o == Order.NLO_PLUS_NLL:
-        ret = "NLO_PLUS_NLL"
-    elif o == Order.aNNLO_PLUS_NNLL:
-        if json_style:
-            ret = "NNLOapprox+NNLL"
-        else:
-            ret = "aNNLO_PLUS_NNLL"
-    else:
-        raise ValueError("Order '" + o + "' not supported by HEPi.")
-    if no_macros:
-        return replace_macros(ret)
-    return ret
-
-
-def xsec_to_order(s: str):
-    if s == "NNLOapprox+NNLL":
-        return Order.aNNLO_PLUS_NNLL
-    elif s == "NLO+NLL":
-        return Order.NLO_PLUS_NLL
-    elif s == "NLO":
-        return Order.NLO
-    elif s == "LO":
-        return Order.LO
-    else:
-        raise ValueError("Unknown Order '" + s + "', not supported by HEPi.")
-
-
 class Input(DictData):
     """
     Input for computation and scans.
 
     Attributes:
         order (:class:`Order`): LO, NLO or NLO+NLL computation.
         energy (int): CMS energy in GeV.
@@ -162,43 +109,45 @@
         mu_f (double): Factorization scale factor.
         mu_r (double): Renormalization scale factor.
         precision (double): Desired numerical relative precision.
         max_iters (int): Upper limit on integration iterations.
         invariant_mass (str): Invariant mass mode 'auto = sqrt((p1+p2)^2)' else value.
         pt (str): Transverse Momentum mode 'auto' or value.
         result (str): Result type 'total'/'pt'/'ptj'/'m'.
-        id (str): Set an id of this run. 
+        id (str): Set an id of this run.
         model (str): Path for MadGraph model.
         update (bool): Update dependent `mu` else set to zero.
     """
 
     # TODO allow unspecified input? Maybe with kwargs + defaults
-    def __init__(self,
-                 order: Order,
-                 energy: float,
-                 particle1: int,
-                 particle2: int,
-                 slha: str,
-                 pdf_lo: str,
-                 pdf_nlo: str,
-                 mu_f=1.0,
-                 mu_r=1.0,
-                 pdfset_lo=0,
-                 pdfset_nlo=0,
-                 precision=0.01,
-                 max_iters=50,
-                 invariant_mass="auto",
-                 result="total",
-                 pt="auto",
-                 id="",
-                 model="",
-                 update=True):
+    def __init__(
+        self,
+        order: Order,
+        energy: float,
+        particle1: int,
+        particle2: int,
+        slha: str,
+        pdf_lo: str,
+        pdf_nlo: str,
+        mu_f=1.0,
+        mu_r=1.0,
+        pdfset_lo=0,
+        pdfset_nlo=0,
+        precision=0.01,
+        max_iters=50,
+        invariant_mass="auto",
+        result="total",
+        pt="auto",
+        id="",
+        model="",
+        update=True,
+    ):
         self.order = order
         self.energy = energy
-        self.energyhalf = energy / 2.
+        self.energyhalf = energy / 2.0
         self.particle1 = particle1
         self.particle2 = particle2
         self.slha = slha
         self.pdf_lo = pdf_lo
         self.pdfset_lo = pdfset_lo
         self.pdf_nlo = pdf_nlo
         self.pdfset_nlo = pdfset_nlo
@@ -209,18 +158,17 @@
         self.precision = precision
         self.max_iters = max_iters
         self.invariant_mass = invariant_mass
         self.pt = pt
         self.result = result
         self.id = id
         self.model = model
-        self.mu = 0.
+        self.mu = 0.0
         if os.path.isfile(get_input_dir() + self.slha):
-            shutil.copy(get_input_dir() + self.slha,
-                        get_output_dir() + self.slha)
+            shutil.copy(get_input_dir() + self.slha, get_output_dir() + self.slha)
         if update:
             update_slha(self)
 
     def has_gluino(self) -> bool:
         return is_gluino(self.particle1) or is_gluino(self.particle2)
 
     def has_neutralino(self) -> bool:
@@ -273,19 +221,23 @@
     """
     Updates dependent parameters in Input `i`.
 
     Mainly concerns the `mu` value used by `madgraph`.
     """
     b = pyslha.read(get_output_dir() + i.slha, ignorenomass=True)
     try:
-        i.mu = (abs(b.blocks["MASS"][abs(i.particle1)]) +
-                abs(b.blocks["MASS"][abs(i.particle2)])) / 2.
+        i.mu = (
+            abs(b.blocks["MASS"][abs(i.particle1)])
+            + abs(b.blocks["MASS"][abs(i.particle2)])
+        ) / 2.0
     except Exception:
-        warnings.warn("Could not set new central scale to average of masses.",
-                      RuntimeWarning)
+        warnings.warn(
+            "Could not set new central scale to average of masses.", RuntimeWarning
+        )
+
 
 def scan(input_list: List[Input], var: str, rrange: Iterable) -> List[Input]:
     """
     Scans a variable `var` over `rrange` in `input_list`.
 
     Note:
         This function does not ensure that dependent vairables are updated (see `energyhalf` in Examples).
@@ -313,15 +265,15 @@
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 10000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
- 
+
     """
     ret = []
     for s in input_list:
         for r in rrange:
             tmp = copy.copy(s)
             setattr(tmp, var, r)
             ret.append(tmp)
@@ -329,15 +281,15 @@
 
 
 def scan_multi(li: List[Input], **kwargs) -> List[Input]:
     """
     Magically scans the variables passed to this function.
 
     Args:
-        **kwargs: 
+        **kwargs:
 
     Examples:
         >>> oli = [Input(Order.LO, 13000,  1000022,1000022, "None", "CT14lo","CT14lo",update=False)]
         >>> li = scan_multi(oli,energy=range(10000,13000,1000))
         >>> for e in li:
         ...     print(e)
         {'order': <Order.LO: 0>, 'energy': 10000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
@@ -350,25 +302,25 @@
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 10000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 11000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO_PLUS_NLL: 2>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
- 
+
     """
     for k, v in kwargs.items():
         li = scan(li, var=k, rrange=v)
     return li
 
 
 multi_scan = scan_multi
 
 
-def scan_scale(l: List[Input], rrange=3, distance=2.):
+def scan_scale(l: List[Input], rrange=3, distance=2.0):
     """
     Scans scale by varying `mu_f` and `mu_r`.
 
     They take `rrange` values from 1/`distance` to `distance` in lograthmic spacing.
     Only points with `mu_f`=`mu_r` or `mu_r/f`=1 or `mu_r/f`=`distance` or `mu_r/f`=1/`distance` are returned.
 
     Examples:
@@ -385,23 +337,34 @@
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 2.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 2.0, 'mu_r': 2.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
     """
     ret = []
     for s in l:
         # not on error pdfs
         if s.pdfset_nlo == 0:
-            tmp = scan([s], "mu_f",
-                       np.logspace(np.log10(1. / distance), np.log10(distance),
-                                   rrange))
             tmp = scan(
-                tmp, "mu_r",
-                np.logspace(np.log10(1. / distance), np.log10(distance),
-                            rrange))
+                [s],
+                "mu_f",
+                np.logspace(np.log10(1.0 / distance), np.log10(distance), rrange),
+            )
+            tmp = scan(
+                tmp,
+                "mu_r",
+                np.logspace(np.log10(1.0 / distance), np.log10(distance), rrange),
+            )
             for t in tmp:
-                if t.mu_f == 1.0 or t.mu_r == 1.0 or t.mu_f == t.mu_r or t.mu_f == distance or t.mu_f == 1. / distance or t.mu_r == distance or t.mu_r == 1. / distance:
+                if (
+                    t.mu_f == 1.0
+                    or t.mu_r == 1.0
+                    or t.mu_f == t.mu_r
+                    or t.mu_f == distance
+                    or t.mu_f == 1.0 / distance
+                    or t.mu_r == distance
+                    or t.mu_r == 1.0 / distance
+                ):
                     ret.append(t)
 
         else:
             ret.append(s)
 
     return ret
 
@@ -422,29 +385,34 @@
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 0.5, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 2.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 2.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.LO: 0>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 2.0, 'mu_r': 2.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
     """
     rrange = 3
-    distance = 2.
+    distance = 2.0
     ret = []
     for s in input_list:
         # not on error pdfs
         if s.pdfset_nlo == 0 and s.mu_f == 1.0 and s.mu_r == 1.0:
-            tmp = scan([s], "mu_f",
-                       np.logspace(np.log10(1. / distance), np.log10(distance),
-                                   rrange))
             tmp = scan(
-                tmp, "mu_r",
-                np.logspace(np.log10(1. / distance), np.log10(distance),
-                            rrange))
+                [s],
+                "mu_f",
+                np.logspace(np.log10(1.0 / distance), np.log10(distance), rrange),
+            )
+            tmp = scan(
+                tmp,
+                "mu_r",
+                np.logspace(np.log10(1.0 / distance), np.log10(distance), rrange),
+            )
             for t in tmp:
-                if not ((t.mu_f == distance and t.mu_r == 1. / distance) or
-                        (t.mu_r == distance and t.mu_f == 1. / distance)):
+                if not (
+                    (t.mu_f == distance and t.mu_r == 1.0 / distance)
+                    or (t.mu_r == distance and t.mu_f == 1.0 / distance)
+                ):
                     ret.append(t)
 
         else:
             ret.append(s)
 
     return ret
 
@@ -469,17 +437,17 @@
 
 def remove_where(input_list: List[Input], condition, **kwargs):
     """
     Remove elements in list which satisfy condition.
 
     Args:
         input_list : List[Input]
-	    The list of inputs to filter.
+            The list of inputs to filter.
         condition : Callable[[Input.__dict__], bool]
-	    The condition to filter on.
+            The condition to filter on.
 
     Examples:
         >>> li = scan_multi([Input(Order.LO, 13000,  1000022,1000022, "None", "CT14lo","CT14lo",update=False)],energy=range(10000,13000,1000))
         >>> for e in remove_where(li,lambda dict : (dict["energy"] == 10000 or dict["energy"] == 11000)):
         ...     print(e)
         {'order': <Order.LO: 0>, 'energy': 12000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14lo', 'pdfset_nlo': 0, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13200, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
     """
@@ -530,46 +498,49 @@
 
 def scan_invariant_mass(input_list: List[Input], diff, points, low=0.001):
     """
     Logarithmic `invariant_mass` scan close to the production threshold.
     """
     ret = []
     for s in input_list:
-        for r in s.mu * 2. + low + (np.logspace(
-                np.log10(low), np.log10(1 + low), points) - low) * diff:
+        for r in (
+            s.mu * 2.0
+            + low
+            + (np.logspace(np.log10(low), np.log10(1 + low), points) - low) * diff
+        ):
             tmp = copy.copy(s)
             setattr(tmp, "invariant_mass", r)
             tmp.result = "m"
             ret.append(tmp)
     return ret
 
 
 def slha_write(newname, d):
     if len(newname) >= 256:
         warnings.warn("probably too long filename")
     f = get_output_dir() + newname
     pyslha.write(f, d)
-    with open(f) as reader, open(f, 'r+') as writer:
+    with open(f) as reader, open(f, "r+") as writer:
         for line in reader:
             if line.strip():
                 writer.write(line)
             else:
                 writer.write("#\n")
         writer.truncate()
 
 
-def masses_scan(input_list: List[Input],
-                varis: List[int],
-                rrange,
-                diff_L_R=None,
-                negate=None) -> List[Input]:
+def masses_scan(
+    input_list: List[Input], varis: List[int], rrange, diff_L_R=None, negate=None
+) -> List[Input]:
     """
     Scans the PDG identified masses in `varis` over `rrange` in the list `input_list`.
     `diff_L_R` allows to set a fixed difference between masses of left- and right-handed particles.
     """
+    from .particles import get_LR_partner
+
     if negate is None:
         negate = []
     ret = []
     for s in input_list:
         for r in rrange:
             d = None
             try:
@@ -604,15 +575,15 @@
     return masses_scan(input_list, [var], rrange, diff_L_R)
 
 
 def slha_scan(input_list: List[Input], block, var, rrange: List) -> List[Input]:
     """
     Scan a generic
     """
-    return slha_scan_rel(input_list, lambda r, : [(block, var, r)], rrange)
+    return slha_scan_rel(input_list, lambda r,: [(block, var, r)], rrange)
 
 
 def slha_scan_rel(input_list: List[Input], lambdas, rrange: List) -> List[Input]:
     """
     Scan a generic slha variable.
     """
     ret = []
@@ -625,17 +596,24 @@
                 d = pyslha.read(s.slha, ignorenomass=True)
             except:
                 d = pyslha.read(get_output_dir() + s.slha, ignorenomass=True)
             ls = lambdas(r)
             for b, v, res in ls:
                 d.blocks[b][v] = res
                 setattr(tmp, b + "_" + str(v), res)
-                newname = newname + "_" + str(b) + "_" + str(v).replace(" ","") + "_" + str(
-                    res)
-            #pyslha.write(get_output_dir()+newname, d)
+                newname = (
+                    newname
+                    + "_"
+                    + str(b)
+                    + "_"
+                    + str(v).replace(" ", "")
+                    + "_"
+                    + str(res)
+                )
+            # pyslha.write(get_output_dir()+newname, d)
             slha_write(newname, d)
 
             setattr(tmp, "slha", newname)
             update_slha(tmp)
             ret.append(tmp)
     return ret
 
@@ -704,14 +682,24 @@
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 51, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 52, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 53, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 54, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 55, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
         {'order': <Order.NLO: 1>, 'energy': 13000, 'energyhalf': 6500.0, 'particle1': 1000022, 'particle2': 1000022, 'slha': 'None', 'pdf_lo': 'CT14lo', 'pdfset_lo': 0, 'pdf_nlo': 'CT14nlo', 'pdfset_nlo': 56, 'pdf_lo_id': 13200, 'pdf_nlo_id': 13100, 'mu_f': 1.0, 'mu_r': 1.0, 'precision': 0.01, 'max_iters': 50, 'invariant_mass': 'auto', 'pt': 'auto', 'result': 'total', 'id': '', 'model': '', 'mu': 0.0}
     """
+    try:
+        import lhapdf
+    except ImportError:
+        raise RuntimeError(
+            "LHAPDF with python bindings needed to compute PDF uncertainties. Make sure you set the PYTHONPATH correctly (i.e. correct python version)."
+        )
+    if not lhapdf.availablePDFSets():
+        raise RuntimeError(
+            "No PDF sets found. Make sure the environment variable LHAPDF_DATA_DIR points to the correct location (.../share/LHAPDF)."
+        )
     ret = []
     for s in input_list:
         # only central scale
         if s.mu_f == 1.0 and s.mu_r == 1.0:
             sset = lhapdf.getPDFSet(s.pdf_nlo)
             for r in range(sset.size):
                 tmp = copy.copy(s)
```

### Comparing `hepi-0.2.8/hepi/madgraph/param_card.dat` & `hepi-0.2.9/hepi/run/madgraph/param_card.dat`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/hepi/madgraph/result.py` & `hepi-0.2.9/hepi/run/madgraph/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import re
 import warnings
+
+from uncertainties import ufloat_fromstr
+
 from hepi.input import Order
+
 from .. import Input, Result
-import re
-from uncertainties import ufloat_fromstr
 
 
 class MadgraphResult(Result):
-    """ MadGraph Result Data."""
+    """MadGraph Result Data."""
 
     def __init__(self, lo, nlo):
         """Sets LO and NLO result. NLO+NLL is set to None."""
         Result.__init__(self, lo, nlo, None)
 
 
 def is_valid(file: str, p: Input, d) -> bool:
@@ -49,23 +52,21 @@
         file (str): File path to be parsed.
 
     Returns:
         :class:`MadGraphResult` : If a value is not found in the file None is used.
 
     """
     # TODO generalize units like RS
-    lo_pattern = re.compile(r'^\s*Total cross section:\s(\S+.*) pb')
+    lo_pattern = re.compile(r"^\s*Total cross section:\s(\S+.*) pb")
 
     lo_result = None
     nlo_result = None
     with open(file) as output:
         for line in output:
             tmp = lo_pattern.search(line)
             if tmp is not None:
                 if lo_result is None:
-                    lo_result = ufloat_fromstr(
-                        tmp.group(1).replace("+-", "+/-"))
+                    lo_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
                 elif nlo_result is None:
-                    nlo_result = ufloat_fromstr(
-                        tmp.group(1).replace("+-", "+/-"))
+                    nlo_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
 
     return MadgraphResult(lo_result, nlo_result)
```

### Comparing `hepi-0.2.8/hepi/madgraph/run.py` & `hepi-0.2.9/hepi/run/madgraph/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Runs MadGraph."""
-from typing import List
+import os
+import pkgutil
 import subprocess
+import time
 from string import Template
+from typing import List
+
 from hepi.input import Order
-from hepi.run import RunParam, Runner
-import pkgutil
+from hepi.run import Runner, RunParam
+
 from .. import Input, Result, get_output_dir
 from .result import is_valid, parse_single
-import time
-import os
 
 
 class MadGraphRunParams(RunParam):
     """Parameters for MadGraph."""
 
     def __init__(self, dic, skip=False, madstr=True):
         super().__init__(skip)
         self.dic = dic
         # self.skip = skip
         self.madstr = madstr
 
 
 class MadGraphRunner(Runner):
-
     def orders(self) -> List[Order]:
         return [Order.LO, Order.NLO]
 
     def _check_path(self) -> bool:
-        if os.path.exists(os.path.expanduser(self.get_path() +
-                                             "/bin/mg5_aMC")):
+        if os.path.exists(os.path.expanduser(self.get_path() + "/bin/mg5_aMC")):
             self.set_path(self.get_path() + "/bin/mg5_aMC")
             return True
         if self.get_path().endswith("mg5_aMC"):
             return True
         return False
 
     def _check_input(self, param: Input, **kwargs) -> bool:
@@ -43,39 +43,44 @@
         if not super()._is_valid(file, p, d):
             return False
         return is_valid(file, p, d)
 
     def _parse_file(self, file: str) -> Result:
         return parse_single(file)
 
-    def _run(self,
-             rps: List[RunParam],
-             wait=True,
-             parallel=True,
-             sleep=0,
-             **kwargs):
+    def _run(self, rps: List[RunParam], wait=True, parallel=True, sleep=0, **kwargs):
         # TODO clean up on exit emergency
         skipall = True
         for rp in rps:
             if not rp.skip:
                 skipall = False
         template = ""
         if not skipall:
-            lo = "&& nice -n 5 {dir}/bin/calculate_xsect LO -f >> {out} " if rps[
-                0].dic["order"] == Order.NLO else ""
-            template =  \
-                'rm -rf {dir} && cp -r ' + rps[0].dic["bdir"] + \
-                ' {dir}  && cp {slha} {dir}/Cards/param_card.dat && cp {run} {dir}/Cards/run_card.dat && echo "nb_core = 1" >> {dir}/Cards/amcatnlo_configuration.txt ' + lo+ '&& nice -n 5 {dir}/bin/calculate_xsect -f >> {out}  && rm -rf {dir}'
+            lo = (
+                "&& nice -n 5 {dir}/bin/calculate_xsect LO -f >> {out} "
+                if rps[0].dic["order"] == Order.NLO
+                else ""
+            )
+            template = (
+                "rm -rf {dir} && cp -r "
+                + rps[0].dic["bdir"]
+                + ' {dir}  && cp {slha} {dir}/Cards/param_card.dat && cp {run} {dir}/Cards/run_card.dat && echo "nb_core = 1" >> {dir}/Cards/amcatnlo_configuration.txt '
+                + lo
+                + "&& nice -n 5 {dir}/bin/calculate_xsect -f >> {out}  && rm -rf {dir}"
+            )
             print(rps[0].dic["out"])
         if not rps[0].skip:
-            mgcom = ''
+            mgcom = ""
             if rps[0].madstr:
                 mgcom = ' --mode="MadSTR"'
-            com = self.get_path() + mgcom + \
-                ' --file {in} >> {out} && cp {slha} {bdir}/Cards/param_card.dat && cp {run} {bdir}/Cards/run_card.dat && sed -i \'s/.*= req_acc_FO/ 1 = req_acc_FO/g\' {bdir}/Cards/run_card.dat && echo "automatic_html_opening = False" >> {bdir}/Cards/amcatnlo_configuration.txt && nice -n 5 {bdir}/bin/calculate_xsect -f'
+            com = (
+                self.get_path()
+                + mgcom
+                + " --file {in} >> {out} && cp {slha} {bdir}/Cards/param_card.dat && cp {run} {bdir}/Cards/run_card.dat && sed -i 's/.*= req_acc_FO/ 1 = req_acc_FO/g' {bdir}/Cards/run_card.dat && echo \"automatic_html_opening = False\" >> {bdir}/Cards/amcatnlo_configuration.txt && nice -n 5 {bdir}/bin/calculate_xsect -f"
+            )
             pp = subprocess.Popen(com.format(**rps[0].dic), shell=True)
             pp.wait()
         # Run commands in parallel
         processes = []
 
         for rp in rps:
             if not rp.skip:
@@ -105,61 +110,58 @@
             if p.order is Order.LO:
                 infile = "lo.mg"
             elif p.order is Order.NLO:
                 infile = "nlo.mg"
             else:
                 raise ValueError("Madgraph only supported for LO/NLO.")
 
-            data = pkgutil.get_data(__name__, infile).decode('utf-8')
+            data = pkgutil.get_data(__name__, infile).decode("utf-8")
             src = Template(data)
             result = src.substitute(d)
             open(get_output_dir() + name + ".mg", "w").write(result)
             if not rp.skip:
-                open(get_output_dir() + name + ".out",
-                     "w").write(result + "\n\n")
+                open(get_output_dir() + name + ".out", "w").write(result + "\n\n")
 
             if p.order == Order.LO:
                 mgfile = "run_card_no_madstr.dat"
             elif p.order == Order.NLO:
                 mgfile = "run_card_with_madstr.dat"
             else:
                 raise ValueError("Order must be one of LO/NLO in MadGraph.")
 
             if "madstr" in kwargs and not kwargs["madstr"]:
                 mgfile = "run_card_no_madstr.dat"
                 rp.madstr = False
             else:
                 rp.madstr = True
-            data = pkgutil.get_data(__name__, mgfile).decode('utf-8')
+            data = pkgutil.get_data(__name__, mgfile).decode("utf-8")
 
             src = Template(data)
             result = src.substitute(d)
             open(get_output_dir() + name + ".dat", "w").write(result)
             if not rp.skip:
-                open(get_output_dir() + name + ".out",
-                     "a").write(result + "\n\n")
+                open(get_output_dir() + name + ".out", "a").write(result + "\n\n")
 
-            sname = d['slha']
-            with open(get_output_dir() + sname, 'r') as f:
-                #src = Template(f.read())
-                #result = src.substitute(d)
-                #open(get_input_dir() + sname + ".in", "w").write(result)
+            sname = d["slha"]
+            with open(get_output_dir() + sname, "r") as f:
+                # src = Template(f.read())
+                # result = src.substitute(d)
+                # open(get_input_dir() + sname + ".in", "w").write(result)
                 if not rp.skip:
-                    open(get_output_dir() + name + ".out",
-                         "a").write(f.read() + "\n\n")
+                    open(get_output_dir() + name + ".out", "a").write(f.read() + "\n\n")
             rp.dic = {
-                'in': get_output_dir() + name + ".mg",
-                'dir': d["dir"],
-                'bdir': d["bdir"],
-                'run': get_output_dir() + name + ".dat",
-                'slha': get_output_dir() + sname,
-                'out': get_output_dir() + name + ".out",
-                'order': p.order
+                "in": get_output_dir() + name + ".mg",
+                "dir": d["dir"],
+                "bdir": d["bdir"],
+                "run": get_output_dir() + name + ".dat",
+                "slha": get_output_dir() + sname,
+                "out": get_output_dir() + name + ".out",
+                "order": p.order,
             }
-            rp.out_file = rp.dic['out']
+            rp.out_file = rp.dic["out"]
         return rp
 
 
 # Legacy
 default_madgraph_runner = MadGraphRunner("/opt/MG5_aMC_v2_7_0/")
 """Default MadGraph Runner to provide backward compatibility"""
 run = default_madgraph_runner.run
```

### Comparing `hepi-0.2.8/hepi/madgraph/run_card_no_madstr.dat` & `hepi-0.2.9/hepi/run/madgraph/run_card_no_madstr.dat`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/hepi/madgraph/run_card_with_madstr.dat` & `hepi-0.2.9/hepi/run/madgraph/run_card_with_madstr.dat`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/hepi/nllfast/run.py` & `hepi-0.2.9/hepi/run/nllfast/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,144 @@
 import os
 import pkgutil
 import stat
+import warnings
 from string import Template
 from typing import List
-import warnings
-from hepi.input import Input, Order, is_gluino, is_squark
-from hepi.results import Result
-from hepi.run import RunParam, Runner
+
 import pyslha
 from uncertainties import ufloat
 
+from hepi.input import Input, Order, is_gluino, is_squark
+from hepi.results import Result
+from hepi.run import Runner, RunParam
+
 
 class NLLfastRunner(Runner):
-    #TODO treat stop sbot separately
-    #TODO separate nll and nnll
+    # TODO treat stop sbot separately
+    # TODO separate nll and nnll
 
     def orders(self) -> List[Order]:
         return [Order.LO, Order.NLO, Order.NLO_PLUS_NLL]
 
     def _get_nf_proc(self, p: Input):
         d = pyslha.read(self.get_output_dir() + p.slha)
         mg = d.blocks["MASS"][1000021]
-        ms = 0.
+        ms = 0.0
         for r in range(1000001, 1000007):
             ms += d.blocks["MASS"][r]
         for r in range(2000001, 2000007):
             ms += d.blocks["MASS"][r]
         ms /= 12
         if p.has_gluino() and p.has_squark():
-            return 'sg', 'cteq', ms, mg
+            return "sg", "cteq", ms, mg
         if is_gluino(p.particle1) and is_gluino(p.particle2):
-            return 'gg', 'cteq', ms, mg
+            return "gg", "cteq", ms, mg
         if is_squark(p.particle1) and is_squark(p.particle2):
             if p.particle1 > 0 and p.particle2 > 0:
-                return 'ss', 'cteq', ms, mg
-            elif (p.particle1 > 0
-                  and p.particle2 < 0) or (p.particle1 < 0
-                                           and p.particle2 > 0):
+                return "ss", "cteq", ms, mg
+            elif (p.particle1 > 0 and p.particle2 < 0) or (
+                p.particle1 < 0 and p.particle2 > 0
+            ):
                 s = p.particle1 if p.particle1 > p.particle2 else p.particle2
                 b = p.particle2 if p.particle1 > p.particle2 else p.particle1
-                return 'sb', 'cteq', s, b
+                return "sb", "cteq", s, b
         return "UNKNOWN_PROCESS_OR_UNIMPLEMENTED_PROCESS"
 
     def _get_nf_input(self, p: Input) -> dict:
         # TODO return masses of squark and gluino
         d = {}
-        #d["ps_inlo"] = int(p.order)
-        d["nf_final_state_in"], d["nf_pdf"], d["nf_squark_mass"], d[
-            "nf_gluino_mass"] = self._get_ps_proc(p)
+        # d["ps_inlo"] = int(p.order)
+        (
+            d["nf_final_state_in"],
+            d["nf_pdf"],
+            d["nf_squark_mass"],
+            d["nf_gluino_mass"],
+        ) = self._get_ps_proc(p)
         return d
 
     def _check_input(self, p: Input, **kwargs) -> bool:
         """Checks input parameter for compatibility with Prospino"""
-        if p.mu_f != 1. or p.mu_r != 1.:
-            warnings.warn(
-                "NLL-fast does not support varying the scales manually.")
+        if p.mu_f != 1.0 or p.mu_r != 1.0:
+            warnings.warn("NLL-fast does not support varying the scales manually.")
             return False
         if p.pdf_lo != "cteq6l1" or p.pdf_nlo != "cteq66":
             warnings.warn(
                 "NLL-fast does not support all pdfs (CTEQ6L1 and CTEQ66 allowed defaults)."
             )
             return False
         return True
 
     def _is_valid(self, file: str, p: Input, d) -> bool:
         return super()._is_valid(file, p, d)
 
     def _parse_file(self, file: str) -> Result:
-        #TODO parse result
+        # TODO parse result
         ret = []
         with open(file) as output:
             for line in output:
-                if line.startswith("nn") or line.startswith(
-                        "ng") or line.startswith("ns") or line.startswith(
-                            "sg") or line.startswith("ll") or line.startswith(
-                                "gg") or line.startswith(
-                                    "ss") or line.startswith(
-                                        "sb"):  # TODO generalize
+                if (
+                    line.startswith("nn")
+                    or line.startswith("ng")
+                    or line.startswith("ns")
+                    or line.startswith("sg")
+                    or line.startswith("ll")
+                    or line.startswith("gg")
+                    or line.startswith("ss")
+                    or line.startswith("sb")
+                ):  # TODO generalize
                     for s in line[2:].split():
                         ret.append(float(s))
         return Result(
             ufloat(ret[8], ret[8] * ret[9]),
-            ufloat(ret[10], ret[10] * ret[11]) if ret[10] != 0. else None,
-            None)
+            ufloat(ret[10], ret[10] * ret[11]) if ret[10] != 0.0 else None,
+            None,
+        )
 
     def _prepare(self, p: Input, **kwargs) -> RunParam:
         rp = super()._prepare(p, **kwargs)
         if not rp.skip:
             d = p.__dict__
-            data = pkgutil.get_data(
-                __name__, "prospino_main.f90_template").decode('utf-8')
+            data = pkgutil.get_data(__name__, "prospino_main.f90_template").decode(
+                "utf-8"
+            )
             src = Template(data)
-            #compute dependent pieces for template
+            # compute dependent pieces for template
             for k, v in self._get_nf_input(p).items():
                 d[k] = v
             result = src.substitute(d)
-            #open(rp.in_file, "w").write(result)
+            # open(rp.in_file, "w").write(result)
             open(rp.out_file, "w").write(result + "\n\n")
-            #rdir = self.get_output_dir() + rp.name + ".rdir"
-            #if os.path.exists(rdir) and os.path.isdir(rdir):
-            #	shutil.rmtree(rdir)
-            #shutil.copytree(self.get_path(),rdir)
-            #open(rdir  +"/prospino_main.f90", "w").write(result)
+            # rdir = self.get_output_dir() + rp.name + ".rdir"
+            # if os.path.exists(rdir) and os.path.isdir(rdir):
+            # 	shutil.rmtree(rdir)
+            # shutil.copytree(self.get_path(),rdir)
+            # open(rdir  +"/prospino_main.f90", "w").write(result)
             ## compile
-            #subprocess.Popen("cd " + rdir + " && make", shell=True,stdout=subprocess.DEVNULL).wait()
+            # subprocess.Popen("cd " + rdir + " && make", shell=True,stdout=subprocess.DEVNULL).wait()
 
-            open(rp.execute,
-                 "w").write("#!/bin/sh\n" +
-                            "{path}/nll-fast {proc} {pdf} {sq} {gl}> {out}".
-                            format(path=self.get_path(),
-                                   out=rp.out_file,
-                                   proc=d["nf_final_state_in"],
-                                   sq=d["nf_squark_mass"],
-                                   gl=d["nf_gluino_mass"],
-                                   pdf=d["nf_pdf"]))
+            open(rp.execute, "w").write(
+                "#!/bin/sh\n"
+                + "{path}/nll-fast {proc} {pdf} {sq} {gl}> {out}".format(
+                    path=self.get_path(),
+                    out=rp.out_file,
+                    proc=d["nf_final_state_in"],
+                    sq=d["nf_squark_mass"],
+                    gl=d["nf_gluino_mass"],
+                    pdf=d["nf_pdf"],
+                )
+            )
             st = os.stat(rp.execute)
             os.chmod(rp.execute, st.st_mode | stat.S_IEXEC)
 
-            sname = d['slha']
-            with open(self.get_output_dir() + sname, 'r') as f:
+            sname = d["slha"]
+            with open(self.get_output_dir() + sname, "r") as f:
                 open(rp.out_file, "a").write(f.read() + "\n\n")
         return rp
 
 
 # Legacy
 default_nllfast_runner = NLLfastRunner("~/git/nll-fast/")
 """Default Prospino Runner to provide backward compatibility"""
 run = default_nllfast_runner.run
 set_path = default_nllfast_runner.set_path
-get_path = default_nllfast_runner.get_path
+get_path = default_nllfast_runner.get_path
```

### Comparing `hepi-0.2.8/hepi/output.py` & `hepi-0.2.9/hepi/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,229 +1,291 @@
 import json
-from smpl import plot
-import numpy as np
-import pkg_resources as pkg
 
-from .input import Order, order_to_string
-from .util import DL2DF, get_name
+# from smpl import plot
+import numpy as np
+import uncertainties.unumpy as unp
 from smpl import io
 
-splot = plot
+import hepi
+
+from .order import Order, order_to_string
+from .util import DL2DF
+
+# splot = plot
 
 
-def write_latex_table_transposed_header(dict_list, t, fname, key, yscale=1.):
+unv = unp.nominal_values
+usd = unp.std_devs
+
+
+def write_latex_table_transposed_header(dict_list, t, fname, key, yscale=1.0):
     dl = dict_list
     mask = dl[t + "_SCALE"].notnull()
-    #lo = splot.unv(dl["LO"][mask])
-    #nlo = splot.unv(dl["NLO"][mask])
-    #nlo_plus_nll = splot.unv(dl["NLO_PLUS_NLL"][mask])
+    # lo = unv(dl["LO"][mask])
+    # nlo = unv(dl["NLO"][mask])
+    # nlo_plus_nll = unv(dl["NLO_PLUS_NLL"][mask])
     s = ""
     mdl = dl[key][mask]
     for i in range(len(dl[t][mask])):
         s = s + "$" + io.gf(4).format(mdl.iloc[i] * yscale) + "$ \t&\t "
 
     if s not in io.read(fname):
-        io.write(fname, s + "\\\\\n", mode='a+')
+        io.write(fname, s + "\\\\\n", mode="a+")
 
 
 # TODO fix PDF scale brackets here for output
-def write_latex_table_transposed(dict_list,
-                                 t,
-                                 fname,
-                                 scale=True,
-                                 pdf=True,
-                                 yscale=1.):
+def write_latex_table_transposed(
+    dict_list, t, fname, scale=True, pdf=True, yscale=1.0, max_rows=None
+):
     dl = dict_list
     mask = dl[t + "_SCALE"].notnull()
     # NLO is a relict misnomer
-    nlo = splot.unv(dl[t][mask])
-    with open(fname, 'a') as f:
-        for i in range(len(dl[t][mask])):
-            f.write("${:.4g}".format(nlo[i] * yscale) + "^{+" +
-                    ("{:.1f}".format(dl[t + "_SCALE_ERRPLUS"][mask].iloc[i] /
-                                     nlo[i] * 100.) if scale else "") +
-                    ("\\%+" +
-                     "{:.1f}".format(dl[t + "_PDF_ERRPLUS"][mask].iloc[i] /
-                                     nlo[i] * 100.) if pdf else "") +
-                    ("\\%}_{" +
-                     "{:.1f}".format(dl[t + "_SCALE_ERRMINUS"][mask].iloc[i] /
-                                     nlo[i] * 100.) if scale else "") +
-                    ("\\%" +
-                     "{:.1f}".format(dl[t + "_PDF_ERRMINUS"][mask].iloc[i] /
-                                     nlo[i] * 100.) if pdf else "") +
-                    "\\%}$ \t&\t ")
+    nlo = unv(dl[t][mask])
+    with open(fname, "a") as f:
+        for i in range(
+            0,
+            len(dl[t][mask]),
+            1 if max_rows is None else int(len(dl[t][mask]) / max_rows),
+        ):
+            f.write(
+                "${:.4g}".format(nlo[i] * yscale)
+                + "^{+"
+                + (
+                    "{:.1f}".format(
+                        dl[t + "_SCALE_ERRPLUS"][mask].iloc[i] / nlo[i] * 100.0
+                    )
+                    if scale
+                    else ""
+                )
+                + (
+                    "\\%+"
+                    + "{:.1f}".format(
+                        dl[t + "_PDF_ERRPLUS"][mask].iloc[i] / nlo[i] * 100.0
+                    )
+                    if pdf
+                    else ""
+                )
+                + (
+                    "\\%}_{"
+                    + "{:.1f}".format(
+                        dl[t + "_SCALE_ERRMINUS"][mask].iloc[i] / nlo[i] * 100.0
+                    )
+                    if scale
+                    else ""
+                )
+                + (
+                    "\\%"
+                    + "{:.1f}".format(
+                        dl[t + "_PDF_ERRMINUS"][mask].iloc[i] / nlo[i] * 100.0
+                    )
+                    if pdf
+                    else ""
+                )
+                + "\\%}$ \t&\t "
+            )
         f.write("\\\\\n")
 
 
-def write_latex(dict_list, t, key, fname, scale=True, pdf=True, yscale=1.):
+def write_latex(dict_list, t, key, fname, scale=True, pdf=True, yscale=1.0):
     """
     Saves a `dict` of `list`s to `filename` as latex table.
     """
     dl = dict_list
     mask = dl[t + "_SCALE"].notnull()
-    #lo = splot.unv(dl["LO"][mask])
-    #nlo = splot.unv(dl["NLO"][mask])
-    #nlo_plus_nll = splot.unv(dl["NLO_PLUS_NLL"][mask])
-    with open(fname, 'w+') as f:
+    lo = unv(dl["LO"][mask])
+    nlo = unv(dl["NLO"][mask])
+    nlo_plus_nll = unv(dl["NLO_PLUS_NLL"][mask])
+    with open(fname, "w+") as f:
         for i in range(len(dl[t][mask])):
             f.write(
-                "$" + io.gf(4).format(dl[key][mask][i]) + "$ \t&\t $" +
-                "{:.3f}".format(lo[i] * yscale) + "^{+" +
-                "{:.1f}".format(dl["LO_SCALE_ERRPLUS"][mask][i] / lo[i] *
-                                100.) + "\\%}_{" +
-                "{:.1f}".format(dl["LO_SCALE_ERRMINUS"][mask][i] / lo[i] *
-                                100.) + "\\%}$ \t&\t $" +
-                "{:.3f}".format(nlo[i] * yscale) + "^{+" +
-                "{:.1f}".format(dl["NLO_SCALE_ERRPLUS"][mask][i] / nlo[i] *
-                                100.) +
-                ("\\%+" + "{:.1f}".format(dl["NLO_PDF_ERRPLUS"][mask][i] /
-                                          nlo[i] * 100.) if pdf else "") +
-                "\\%}_{" + "{:.1f}".format(dl["NLO_SCALE_ERRMINUS"][mask][i] /
-                                           nlo[i] * 100.) +
-                ("\\%" + "{:.1f}".format(dl["NLO_PDF_ERRMINUS"][mask][i] /
-                                         nlo[i] * 100.) if pdf else "") +
-                "\\%}$ \t&\t $" + "{:.3f}".format(nlo_plus_nll[i] * yscale) +
-                "^{+" +
-                "{:.1f}".format(dl["NLO_PLUS_NLL_SCALE_ERRPLUS"][mask][i] /
-                                nlo_plus_nll[i] * 100.) +
-                ("\\%+" +
-                 "{:.1f}".format(dl["NLO_PLUS_NLL_PDF_ERRPLUS"][mask][i] /
-                                 nlo_plus_nll[i] * 100.) if pdf else "") +
-                "\\%}_{" +
-                "{:.1f}".format(dl["NLO_PLUS_NLL_SCALE_ERRMINUS"][mask][i] /
-                                nlo_plus_nll[i] * 100.) +
-                ("\\%" +
-                 "{:.1f}".format(dl["NLO_PLUS_NLL_PDF_ERRMINUS"][mask][i] /
-                                 nlo_plus_nll[i] * 100.) if pdf else "") +
-                "\\%}$ " + "\\\\\n")
+                "$"
+                + io.gf(4).format(dl[key][mask][i])
+                + "$ \t&\t $"
+                + "{:.3f}".format(lo[i] * yscale)
+                + "^{+"
+                + "{:.1f}".format(dl["LO_SCALE_ERRPLUS"][mask][i] / lo[i] * 100.0)
+                + "\\%}_{"
+                + "{:.1f}".format(dl["LO_SCALE_ERRMINUS"][mask][i] / lo[i] * 100.0)
+                + "\\%}$ \t&\t $"
+                + "{:.3f}".format(nlo[i] * yscale)
+                + "^{+"
+                + "{:.1f}".format(dl["NLO_SCALE_ERRPLUS"][mask][i] / nlo[i] * 100.0)
+                + (
+                    "\\%+"
+                    + "{:.1f}".format(dl["NLO_PDF_ERRPLUS"][mask][i] / nlo[i] * 100.0)
+                    if pdf
+                    else ""
+                )
+                + "\\%}_{"
+                + "{:.1f}".format(dl["NLO_SCALE_ERRMINUS"][mask][i] / nlo[i] * 100.0)
+                + (
+                    "\\%"
+                    + "{:.1f}".format(dl["NLO_PDF_ERRMINUS"][mask][i] / nlo[i] * 100.0)
+                    if pdf
+                    else ""
+                )
+                + "\\%}$ \t&\t $"
+                + "{:.3f}".format(nlo_plus_nll[i] * yscale)
+                + "^{+"
+                + "{:.1f}".format(
+                    dl["NLO_PLUS_NLL_SCALE_ERRPLUS"][mask][i] / nlo_plus_nll[i] * 100.0
+                )
+                + (
+                    "\\%+"
+                    + "{:.1f}".format(
+                        dl["NLO_PLUS_NLL_PDF_ERRPLUS"][mask][i]
+                        / nlo_plus_nll[i]
+                        * 100.0
+                    )
+                    if pdf
+                    else ""
+                )
+                + "\\%}_{"
+                + "{:.1f}".format(
+                    dl["NLO_PLUS_NLL_SCALE_ERRMINUS"][mask][i] / nlo_plus_nll[i] * 100.0
+                )
+                + (
+                    "\\%"
+                    + "{:.1f}".format(
+                        dl["NLO_PLUS_NLL_PDF_ERRMINUS"][mask][i]
+                        / nlo_plus_nll[i]
+                        * 100.0
+                    )
+                    if pdf
+                    else ""
+                )
+                + "\\%}$ "
+                + "\\\\\n"
+            )
 
 
 tex_table = write_latex
 
 
 def write_csv(dict_list: list, filename: str):
     """
- Saves a `dict` of `list`s to `filename` as csv table.
+    Saves a `dict` of `list`s to `filename` as csv table.
 
- Examples:
-    >>> import hepi 
-    >>> import urllib.request
-    >>> dl = hepi.load(urllib.request.urlopen(
-    ... "https://raw.githubusercontent.com/fuenfundachtzig/xsec/master/json/pp13_hinosplit_N2N1_NLO%2BNLL.json"
-    ... ),dimensions=2)
-    >>> hepi.write_csv(dl, open("test.csv", 'w'))
-    >>> with open('test.csv', 'r') as f:
-    ...     print(f.read())
-    order,energy,energyhalf,particle1,particle2,slha,pdf_lo,pdfset_lo,pdf_nlo,pdfset_nlo,pdf_lo_id,pdf_nlo_id,mu_f,mu_r,precision,max_iters,invariant_mass,pt,result,id,model,mu,runner,N2,N1,NLO_PLUS_NLL
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,81.5,80.0,7.746+/-0.023
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,82.0,80.0,7.646+/-0.024
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,83.0,80.0,7.451+/-0.024
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,85.0,80.0,7.080+/-0.024
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,90.0,80.0,6.249+/-0.025
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,95.0,80.0,5.537+/-0.025
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,100.0,60.0,7.613+/-0.024
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,100.0,80.0,4.925+/-0.025
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,101.5,100.0,3.201+/-0.026
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,102.0,100.0,3.170+/-0.027
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,103.0,100.0,3.110+/-0.027
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,105.0,100.0,2.994+/-0.027
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,110.0,100.0,2.726+/-0.027
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,110.0,80.0,3.934+/-0.026
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,115.0,100.0,2.486+/-0.028
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,100.0,2.271+/-0.028
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,60.0,4.505+/-0.025
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,80.0,3.180+/-0.027
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,126.5,125.0,1.384+/-0.030
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,127.0,125.0,1.373+/-0.030
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,128.0,125.0,1.352+/-0.031
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,130.0,100.0,1.905+/-0.029
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,130.0,125.0,1.313+/-0.031
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,135.0,125.0,1.220+/-0.031
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,100.0,1.608+/-0.029
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,125.0,1.135+/-0.031
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,80.0,2.142+/-0.028
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,145.0,125.0,1.056+/-0.032
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,152.0,150.0,0.700+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,153.0,150.0,0.691+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,155.0,125.0,0.918+/-0.032
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,155.0,150.0,0.674+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,160.0,100.0,1.166+/-0.031
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,160.0,150.0,0.634+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,165.0,125.0,0.800+/-0.033
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,165.0,150.0,0.597+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,170.0,150.0,0.562+/-0.035
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,178.0,175.0,0.39+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,180.0,150.0,0.500+/-0.035
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,180.0,175.0,0.38+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,185.0,125.0,0.615+/-0.034
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,185.0,175.0,0.36+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,190.0,150.0,0.44+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,190.0,175.0,0.35+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,195.0,175.0,0.33+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,202.0,200.0,0.24+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,203.0,200.0,0.24+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,205.0,200.0,0.23+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,210.0,150.0,0.35+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,210.0,200.0,0.22+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,215.0,200.0,0.21+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,220.0,200.0,0.20+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,230.0,200.0,0.19+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,230.0,225.0,0.15+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,235.0,225.0,0.14+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,240.0,200.0,0.17+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,240.0,225.0,0.14+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,252.0,250.0,0.10+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,253.0,250.0,0.10+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,255.0,250.0,0.10+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,260.0,200.0,0.14+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,260.0,250.0,0.10+/-0.04
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,265.0,250.0,0.09+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,270.0,250.0,0.09+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,280.0,250.0,0.08+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,290.0,250.0,0.08+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,302.0,300.0,0.05+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,303.0,300.0,0.05+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,305.0,300.0,0.05+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,310.0,250.0,0.07+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,310.0,300.0,0.05+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,315.0,300.0,0.05+/-0.05
-    2,13000.0,6500.0,-1,-1,$\\tilde\\chi_2^0\\tilde\\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,320.0,300.0,0.04+/-0.05
-    <BLANKLINE>
- """
+    Examples:
+       >>> import hepi
+       >>> import urllib.request
+       >>> dl = hepi.load(urllib.request.urlopen(
+       ... "https://raw.githubusercontent.com/fuenfundachtzig/xsec/master/json/pp13_hinosplit_N2N1_NLO%2BNLL.json"
+       ... ),dimensions=2)
+       >>> hepi.write_csv(dl, open("test.csv", 'w'))
+       >>> with open('test.csv', 'r') as f:
+       ...     print(f.read())
+       order,energy,energyhalf,particle1,particle2,slha,pdf_lo,pdfset_lo,pdf_nlo,pdfset_nlo,pdf_lo_id,pdf_nlo_id,mu_f,mu_r,precision,max_iters,invariant_mass,pt,result,id,model,mu,runner,N2,N1,NLO_PLUS_NLL_NOERR,NLO_PLUS_NLL_COMBINED
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,81.5,80.0,7.746232,7.746+/-0.023
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,82.0,80.0,7.646339,7.646+/-0.024
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,83.0,80.0,7.450843,7.451+/-0.024
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,85.0,80.0,7.079679,7.080+/-0.024
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,90.0,80.0,6.248933,6.249+/-0.025
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,95.0,80.0,5.53691,5.537+/-0.025
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,100.0,60.0,7.613015,7.613+/-0.024
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,100.0,80.0,4.924686,4.925+/-0.025
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,101.5,100.0,3.201246,3.201+/-0.026
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,102.0,100.0,3.169948,3.170+/-0.027
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,103.0,100.0,3.109625,3.110+/-0.027
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,105.0,100.0,2.993584,2.994+/-0.027
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,110.0,100.0,2.725548,2.726+/-0.027
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,110.0,80.0,3.933723,3.934+/-0.026
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,115.0,100.0,2.485705,2.486+/-0.028
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,100.0,2.271269,2.271+/-0.028
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,60.0,4.504708,4.505+/-0.025
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,120.0,80.0,3.180276,3.180+/-0.027
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,126.5,125.0,1.383578,1.384+/-0.030
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,127.0,125.0,1.373155,1.373+/-0.030
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,128.0,125.0,1.352257,1.352+/-0.031
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,130.0,100.0,1.905211,1.905+/-0.029
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,130.0,125.0,1.3128,1.313+/-0.031
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,135.0,125.0,1.219904,1.220+/-0.031
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,100.0,1.608394,1.608+/-0.029
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,125.0,1.134614,1.135+/-0.031
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,140.0,80.0,2.142151,2.142+/-0.028
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,145.0,125.0,1.056242,1.056+/-0.032
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,152.0,150.0,0.699925,0.700+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,153.0,150.0,0.691281,0.691+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,155.0,125.0,0.917808,0.918+/-0.032
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,155.0,150.0,0.674484,0.674+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,160.0,100.0,1.165897,1.166+/-0.031
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,160.0,150.0,0.6345,0.634+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,165.0,125.0,0.800281,0.800+/-0.033
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,165.0,150.0,0.597167,0.597+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,170.0,150.0,0.562441,0.562+/-0.035
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,178.0,175.0,0.391649,0.39+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,180.0,150.0,0.499633,0.500+/-0.035
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,180.0,175.0,0.383418,0.38+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,185.0,125.0,0.614697,0.615+/-0.034
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,185.0,175.0,0.363707,0.36+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,190.0,150.0,0.444892,0.44+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,190.0,175.0,0.345126,0.35+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,195.0,175.0,0.327625,0.33+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,202.0,200.0,0.2403,0.24+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,203.0,200.0,0.238047,0.24+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,205.0,200.0,0.233619,0.23+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,210.0,150.0,0.354984,0.35+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,210.0,200.0,0.222947,0.22+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,215.0,200.0,0.212818,0.21+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,220.0,200.0,0.203209,0.20+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,230.0,200.0,0.18536,0.19+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,230.0,225.0,0.150189,0.15+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,235.0,225.0,0.14399,0.14+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,240.0,200.0,0.169381,0.17+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,240.0,225.0,0.138083,0.14+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,252.0,250.0,0.102807,0.10+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,253.0,250.0,0.102017,0.10+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,255.0,250.0,0.100453,0.10+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,260.0,200.0,0.141817,0.14+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,260.0,250.0,0.096658,0.10+/-0.04
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,265.0,250.0,0.092955,0.09+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,270.0,250.0,0.089536,0.09+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,280.0,250.0,0.082931,0.08+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,290.0,250.0,0.076979,0.08+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,302.0,300.0,0.050316,0.05+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,303.0,300.0,0.049985,0.05+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,305.0,300.0,0.049326,0.05+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,310.0,250.0,0.066363,0.07+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,310.0,300.0,0.047719,0.05+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,315.0,300.0,0.046111,0.05+/-0.05
+       2,13000.0,6500.0,-1,-1,$\\tilde\chi_2^0\\tilde\chi_1^0$ (higgsino),CTEQ6.6 and MSTW2008nlo90cl,0,CTEQ6.6 and MSTW2008nlo90cl,0,0,0,1.0,1.0,0.01,50,auto,auto,total,,,0.0,Resummino,320.0,300.0,0.044674,0.04+/-0.05
+       <BLANKLINE>
+    """
     df = DL2DF(dict_list)
     df.to_csv(filename, index=False)
 
 
-def write_json(dict_list: list,
-               o: Order,
-               parameters: str,
-               output,
-               error_sym=False,
-               error_asym=False,
-               scale=True,
-               pdf=True,
-               ):
+def write_json(
+    dict_list: list,
+    o: Order,
+    parameters: str,
+    output,
+    error=True,
+    error_sym=None,
+    scale=True,
+    pdf=True,
+):
     """
     Saves a `dict` of `list`s to `filename` as json.
 
 
     Cf. https://github.com/fuenfundachtzig/xsec
 
 
     Args:
        output (writeable or file name str) : Should support a function `.write()`.
 
     Examples:
-       >>> import hepi 
+       >>> import hepi
        >>> import urllib.request
        >>> dl = hepi.load(urllib.request.urlopen(
        ... "https://raw.githubusercontent.com/fuenfundachtzig/xsec/master/json/pp13_hinosplit_N2N1_NLO%2BNLL.json"
        ... ),dimensions=2)
        >>> with open("test.json", "w") as f:
-       ...     hepi.write_json(dl, Order.NLO_PLUS_NLL,["N1"],f)
+       ...     hepi.write_json(dl, Order.NLO_PLUS_NLL,["N1"],f,error=False)
        >>> with open('test.json', 'r') as f:
        ...     print(f.read())
        {
            "initial state": "pp",
            "order": "NLO+NLL",
            "source": "hepi-...",
            "contact": "...",
@@ -269,113 +331,218 @@
                },
                "300.0": {
                    "xsec_pb": 0.044674
                }
            }
        }
     """
+    from .particles import get_name
 
     jd = {}
     jd["initial state"] = "pp"  # TODO add more such cases + filters, also in resummino
     if o == Order.LO:
         jd["order"] = "LO"
     elif o == Order.NLO:
         jd["order"] = "NLO"
     elif o == Order.NLO_PLUS_NLL:
         jd["order"] = "NLO+NLL"
     elif o == Order.aNNLO_PLUS_NNLL:
         jd["order"] = "NNLOapprox+NNLL"
     else:
         raise ValueError("Order not supported by write_json.")
-    so =  order_to_string(o)
+    so = order_to_string(o)
     package = "hepi"
     try:
-        version = pkg.require(package)[0].version
-    except pkg.DistributionNotFound:
+        version = hepi.__version__
+    except Exception:
         version = "dirty"
     jd["source"] = package + "-" + version
 
     jd["contact"] = "Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"
     jd["tool"] = dict_list["runner"].iloc[0].replace("Runner", "")
-    jd["process_latex"] = "$" + get_name(dict_list["particle1"].iloc[0]) + get_name(
-        dict_list["particle2"].iloc[0]) + "$"
+    jd["process_latex"] = (
+        "$"
+        + get_name(dict_list["particle1"].iloc[0])
+        + get_name(dict_list["particle2"].iloc[0])
+        + "$"
+    )
     jd["comment"] = dict_list["id"].iloc[0]
     jd["reference"] = "?"
     jd["Ecom [GeV]"] = str(dict_list["energy"].iloc[0])
-    jd["process_id"] = "pp_" + str(dict_list["energy"].iloc[0]) + "_" + str(
-        dict_list["particle1"].iloc[0]) + "_" + str(dict_list["particle2"].iloc[0])
+    jd["process_id"] = (
+        "pp_"
+        + str(dict_list["energy"].iloc[0])
+        + "_"
+        + str(dict_list["particle1"].iloc[0])
+        + "_"
+        + str(dict_list["particle2"].iloc[0])
+    )
     jd["PDF set"] = dict_list["pdf_nlo"].iloc[0]
     dat = {}
+
+    # Here we determine if the errors are asymmetric, that is NOERR and COMBINED have a different mean value
+    if error and error_sym is None:
+        if len(parameters) == 2:
+            tp = parameters[0]
+        elif len(parameters) == 1:
+            tp = parameters[0]
+        error_sym = True
+        for j in range(len(dict_list[tp])):
+            if not np.isclose(
+                float(unv(dict_list[so + "_NOERR"].iloc[j])),
+                float(unv(dict_list[so + "_COMBINED"].iloc[j])),
+                rtol=1e-05,
+                atol=1e-08,
+                equal_nan=False,
+            ):
+                error_sym = False
+                break
+        error_asym = not error_sym
+    if not error:
+        error_asym = False
+        error_sym = False
+
     if len(parameters) == 2:
         parameterj = parameters[0]
         parameteri = parameters[1]
         for j in range(len(dict_list[parameterj])):
             dati = {}
             if error_asym:
                 td = {
-                    "xsec_pb": float(plot.unv(dict_list[so + "_NOERR"].iloc[j])),
-                    "unc_up_pb": float(plot.unv(dict_list[so+ "_COMBINED"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_COMBINED"].iloc[j])),
-                    "unc_down_pb": float(plot.unv(dict_list[so+ "_COMBINED"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_COMBINED"].iloc[j])),
-
+                    "xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j])),
+                    "unc_up_pb": float(
+                        unv(dict_list[so + "_COMBINED"].iloc[j])
+                        - unv(dict_list[so + "_NOERR"].iloc[j])
+                        + usd(dict_list[so + "_COMBINED"].iloc[j])
+                    ),
+                    "unc_down_pb": float(
+                        unv(dict_list[so + "_COMBINED"].iloc[j])
+                        - unv(dict_list[so + "_NOERR"].iloc[j])
+                        - usd(dict_list[so + "_COMBINED"].iloc[j])
+                    ),
                 }
                 if scale:
-                    td = {**td,"unc_scale_up_pb": float(plot.unv(dict_list[so+ "_SCALE"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_SCALE"].iloc[j])),
-                    "unc_scale_down_pb": float(plot.unv(dict_list[so+ "_SCALE"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_SCALE"].iloc[j])),
+                    td = {
+                        **td,
+                        "unc_scale_up_pb": float(
+                            unv(dict_list[so + "_SCALE"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            + usd(dict_list[so + "_SCALE"].iloc[j])
+                        ),
+                        "unc_scale_down_pb": float(
+                            unv(dict_list[so + "_SCALE"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            - usd(dict_list[so + "_SCALE"].iloc[j])
+                        ),
                     }
                 if pdf:
-                    td = {**td,"unc_pdf_up_pb": float(plot.unv(dict_list[so+ "_PDF"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_PDF"].iloc[j])),
-                    "unc_pdf_down_pb": float(plot.unv(dict_list[so+ "_PDF"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_PDF"].iloc[j])),
+                    td = {
+                        **td,
+                        "unc_pdf_up_pb": float(
+                            unv(dict_list[so + "_PDF"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            + usd(dict_list[so + "_PDF"].iloc[j])
+                        ),
+                        "unc_pdf_down_pb": float(
+                            unv(dict_list[so + "_PDF"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            - usd(dict_list[so + "_PDF"].iloc[j])
+                        ),
                     }
             elif error_sym:
-                td= {
-                    "xsec_pb": float(plot.unv(dict_list[so].iloc[j])),
-                    "unc_pb": float(plot.usd(dict_list[so].iloc[j]))
+
+                # COMBINED and NOERR are the same mean for sym errors
+                td = {
+                    "xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j])),
+                    "unc_pb": float(usd(dict_list[so + "_COMBINED"].iloc[j])),
                 }
                 if scale:
-                    td = {**td,"unc_scale_pb": float(plot.usd(dict_list[so+ "_SCALE"].iloc[j]))}
+                    td = {
+                        **td,
+                        "unc_scale_pb": float(usd(dict_list[so + "_SCALE"].iloc[j])),
+                    }
                 if pdf:
-                    td = {**td,"unc_pdf_pb": float(plot.usd(dict_list[so+ "_PDF"].iloc[j]))}
+                    td = {
+                        **td,
+                        "unc_pdf_pb": float(usd(dict_list[so + "_PDF"].iloc[j])),
+                    }
             else:
-                 td= {
-                    "xsec_pb": float(plot.unv(dict_list[so].iloc[j]))
-                }
+                td = {"xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j]))}
             if str(dict_list[parameterj].iloc[j]) in dat:
-                dat[str(dict_list[parameterj].iloc[j])]={**dat[str(dict_list[parameterj].iloc[j])],str(dict_list[parameteri].iloc[j]):td}
+                dat[str(dict_list[parameterj].iloc[j])] = {
+                    **dat[str(dict_list[parameterj].iloc[j])],
+                    str(dict_list[parameteri].iloc[j]): td,
+                }
             else:
-                dat[str(dict_list[parameterj].iloc[j])]={str(dict_list[parameteri].iloc[j]):td}
+                dat[str(dict_list[parameterj].iloc[j])] = {
+                    str(dict_list[parameteri].iloc[j]): td
+                }
 
-        jd["parameters"] = [[parameterj],[parameteri]]
+        jd["parameters"] = [[parameterj], [parameteri]]
     if len(parameters) == 1:
         parameter = parameters[0]
         for j in range(len(dict_list[parameter])):
             if error_asym:
-                td= {
-                    "xsec_pb": float(plot.unv(dict_list[so + "_NOERR"].iloc[j])),
-                    "unc_up_pb": float(plot.unv(dict_list[so+ "_COMBINED"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_COMBINED"].iloc[j])),
-                    "unc_down_pb": float(plot.unv(dict_list[so+ "_COMBINED"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_COMBINED"].iloc[j])),
+                td = {
+                    "xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j])),
+                    "unc_up_pb": float(
+                        unv(dict_list[so + "_COMBINED"].iloc[j])
+                        - unv(dict_list[so + "_NOERR"].iloc[j])
+                        + usd(dict_list[so + "_COMBINED"].iloc[j])
+                    ),
+                    "unc_down_pb": float(
+                        unv(dict_list[so + "_COMBINED"].iloc[j])
+                        - unv(dict_list[so + "_NOERR"].iloc[j])
+                        - usd(dict_list[so + "_COMBINED"].iloc[j])
+                    ),
                 }
                 if scale:
-                    td = {**td,"unc_scale_up_pb": float(plot.unv(dict_list[so+ "_SCALE"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_SCALE"].iloc[j])),
-                    "unc_scale_down_pb": float(plot.unv(dict_list[so+ "_SCALE"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_SCALE"].iloc[j])),
+                    td = {
+                        **td,
+                        "unc_scale_up_pb": float(
+                            unv(dict_list[so + "_SCALE"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            + usd(dict_list[so + "_SCALE"].iloc[j])
+                        ),
+                        "unc_scale_down_pb": float(
+                            unv(dict_list[so + "_SCALE"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            - usd(dict_list[so + "_SCALE"].iloc[j])
+                        ),
                     }
                 if pdf:
-                    td = {**td,"unc_pdf_up_pb": float(plot.unv(dict_list[so+ "_PDF"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) + plot.usd(dict_list[so+ "_PDF"].iloc[j])),
-                    "unc_pdf_down_pb": float(plot.unv(dict_list[so+ "_PDF"].iloc[j])-plot.unv(dict_list[so + "_NOERR"].iloc[j]) - plot.usd(dict_list[so+ "_PDF"].iloc[j])),
+                    td = {
+                        **td,
+                        "unc_pdf_up_pb": float(
+                            unv(dict_list[so + "_PDF"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            + usd(dict_list[so + "_PDF"].iloc[j])
+                        ),
+                        "unc_pdf_down_pb": float(
+                            unv(dict_list[so + "_PDF"].iloc[j])
+                            - unv(dict_list[so + "_NOERR"].iloc[j])
+                            - usd(dict_list[so + "_PDF"].iloc[j])
+                        ),
                     }
             elif error_sym:
+                # COMBINED and NOERR are the same mean for sym errors
                 td = {
-                    "xsec_pb": float(plot.unv(dict_list[so].iloc[j])),
-                    "unc_pb": float(plot.usd(dict_list[so].iloc[j]))
+                    "xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j])),
+                    "unc_pb": float(usd(dict_list[so + "_COMBINED"].iloc[j])),
                 }
                 if scale:
-                    td = {**td,"unc_scale_pb": float(plot.usd(dict_list[so+ "_SCALE"].iloc[j]))}
+                    td = {
+                        **td,
+                        "unc_scale_pb": float(usd(dict_list[so + "_SCALE"].iloc[j])),
+                    }
                 if pdf:
-                    td = {**td,"unc_pdf_pb": float(plot.usd(dict_list[so+ "_PDF"].iloc[j]))}
+                    td = {
+                        **td,
+                        "unc_pdf_pb": float(usd(dict_list[so + "_PDF"].iloc[j])),
+                    }
             else:
-                 td= {
-                    "xsec_pb": float(plot.unv(dict_list[so].iloc[j]))
-                }
-            dat[str(dict_list[parameter].iloc[j])]=td
+                td = {"xsec_pb": float(unv(dict_list[so + "_NOERR"].iloc[j]))}
+            dat[str(dict_list[parameter].iloc[j])] = td
         jd["parameters"] = [[parameter]]
 
     jd["data"] = dat
     io.write(output, json.dumps(jd, indent=4))
```

### Comparing `hepi-0.2.8/hepi/plot.py` & `hepi-0.2.9/hepi/plot/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,247 @@
-from matplotlib.image import NonUniformImage
 from collections.abc import Iterable
-import matplotlib as mpl
-from smpl import plot as splot
-import numpy as np
-from scipy.interpolate import make_interp_spline, BSpline
 
+import matplotlib as mpl
+import matplotlib.cm as cm
 import matplotlib.pyplot as plt
-
+import numpy as np
 import pyslha
-
-import matplotlib.cm as cm
 from matplotlib import colors
-
-from .input import Input, get_output_dir, replace_macros
-from .util import get_name
+from matplotlib.image import NonUniformImage
 from matplotlib.ticker import NullFormatter
 from scipy import integrate as auc
+from scipy.interpolate import BSpline, make_interp_spline
+from smpl import plot as splot
 
+from ..input import Input, get_output_dir, replace_macros
+from ..particles import get_name
 
-def title(i: Input,
-          axe=None,
-          scenario=None,
-          diff_L_R=None,
-          extra="",
-          cms_energy=True,
-          pdf_info=True,
-          id=False,
-          **kwargs):
+
+def title(
+    i: Input,
+    axe=None,
+    scenario=None,
+    diff_L_R=None,
+    extra="",
+    cms_energy=True,
+    pdf_info=True,
+    id=False,
+    **kwargs
+):
     """Sets the title on axis `axe`."""
     if axe is None:
         axe = plt.gca()
-    axe.set_title("$pp\\to" + get_name(i.particle1) + get_name(i.particle2) +
-                  "$" + (" at $\\sqrt{S} = " + str(i.energy / 1000) +
-                         "$ TeV" if cms_energy else "") +
-                  ((" for " +
-                    i.slha.split(".")[0]) if scenario is None else scenario) +
-                  (" with " + i.pdf_nlo if pdf_info else "") + " " + extra +
-                  ((" [" + i.id + "]") if id else ""))
-
-
-def energy_plot(dict_list,
-                y,
-                yscale=1.,
-                xaxis="E [GeV]",
-                yaxis="$\\sigma$ [pb]",
-                label=None,
-                **kwargs):
+    axe.set_title(
+        "$pp\\to"
+        + get_name(i.particle1)
+        + get_name(i.particle2)
+        + "$"
+        + (" at $\\sqrt{S} = " + str(i.energy / 1000) + "$ TeV" if cms_energy else "")
+        + ((" for " + i.slha.split(".")[0]) if scenario is None else scenario)
+        + (" with " + i.pdf_nlo if pdf_info else "")
+        + " "
+        + extra
+        + ((" [" + i.id + "]") if id else "")
+    )
+
+
+def energy_plot(
+    dict_list,
+    y,
+    yscale=1.0,
+    xaxis="E [GeV]",
+    yaxis="$\\sigma$ [pb]",
+    label=None,
+    **kwargs
+):
     """Plot energy on the x-axis."""
-    plot(dict_list,
-         "energy",
-         y,
-         label=label,
-         xaxis=xaxis,
-         yaxis=yaxis,
-         logy=True,
-         yscale=yscale,
-         **kwargs)
-
-def combined_mass_plot(dict_list,
-                          y,
-                            part,
-                            label=None,
-                            **kwargs):
+    plot(
+        dict_list,
+        "energy",
+        y,
+        label=label,
+        xaxis=xaxis,
+        yaxis=yaxis,
+        logy=True,
+        yscale=yscale,
+        **kwargs
+    )
+
+
+def combined_mass_plot(dict_list, y, part, label=None, **kwargs):
     if label == "":
         kwargs["label"] = ""
-    mass_plot(dict_list, y +"_NOERR",part,next_color=False,fmt=" ",fill=False,interpolate_label=label,  **kwargs)
-    if 'label' in kwargs:
+    mass_plot(
+        dict_list,
+        y + "_NOERR",
+        part,
+        next_color=False,
+        fmt=" ",
+        fill=False,
+        interpolate_label=label,
+        **kwargs
+    )
+    if "label" in kwargs:
         del kwargs["label"]
-    mass_plot(dict_list, y +"_COMBINED",part,next_color=True,fit_fmt=" ",fill=True, label="",interpolate_lower_uncertainty=False, **kwargs)
+    mass_plot(
+        dict_list,
+        y + "_COMBINED",
+        part,
+        next_color=True,
+        fit_fmt=" ",
+        fill=True,
+        label="",
+        interpolate_lower_uncertainty=False,
+        **kwargs
+    )
 
-def combined_plot(dict_list,
-x,
-                          y,
-                            label=None,
-                            **kwargs):
+
+def combined_plot(dict_list, x, y, label=None, **kwargs):
     if label == "":
         kwargs["label"] = ""
-    plot(dict_list, x,y +"_NOERR",next_color=False,fmt=" ",fill=False,interpolate_label=label,  **kwargs)
-    if 'label' in kwargs:
+    plot(
+        dict_list,
+        x,
+        y + "_NOERR",
+        next_color=False,
+        fmt=" ",
+        fill=False,
+        interpolate_label=label,
+        **kwargs
+    )
+    if "label" in kwargs:
         del kwargs["label"]
-    plot(dict_list, x,y +"_COMBINED",next_color=True,fit_fmt=" ",fill=True, label="",interpolate_lower_uncertainty=False, **kwargs)
-
-
-
-def mass_plot(dict_list,
-              y,
-              part,
-              logy=True,
-              yaxis="$\\sigma$ [pb]",
-              yscale=1.,
-              label=None,
-              xaxis = None,
-              **kwargs):
+    plot(
+        dict_list,
+        x,
+        y + "_COMBINED",
+        next_color=True,
+        fit_fmt=" ",
+        fill=True,
+        label="",
+        interpolate_lower_uncertainty=False,
+        **kwargs
+    )
+
+
+def mass_plot(
+    dict_list,
+    y,
+    part,
+    logy=True,
+    yaxis="$\\sigma$ [pb]",
+    yscale=1.0,
+    label=None,
+    xaxis=None,
+    **kwargs
+):
     if not "mass_" + str(part) in dict_list:
         dict_list["mass_" + str(part)] = get_mass(dict_list, abs(part))
     if xaxis is None:
         xaxis = "$m_{" + get_name(part) + "}$ [GeV]"
-    plot(dict_list,
-         "mass_" + str(part),
-         y,
-         label=label,
-         yaxis=yaxis,
-         xaxis=xaxis,
-         logy=logy,
-         yscale=yscale,
-         **kwargs)
-
-
-def mass_vplot(dict_list,
-               y,
-               part,
-               logy=True,
-               yaxis="$\\sigma$ [pb]",
-               yscale=1.,
-               label=None,
-               mask=None,
-               **kwargs):
-    vplot(get_mass(dict_list, part)[mask],
-          y[mask],
-          label=label,
-          xaxis="$m_{" + get_name(part) + "}$ [GeV]",
-          yaxis=yaxis,
-          logy=logy,
-          yscale=yscale,
-          mask=mask,
-          **kwargs)
+    plot(
+        dict_list,
+        "mass_" + str(part),
+        y,
+        label=label,
+        yaxis=yaxis,
+        xaxis=xaxis,
+        logy=logy,
+        yscale=yscale,
+        **kwargs
+    )
+
+
+def mass_vplot(
+    dict_list,
+    y,
+    part,
+    logy=True,
+    yaxis="$\\sigma$ [pb]",
+    yscale=1.0,
+    label=None,
+    mask=None,
+    **kwargs
+):
+    vplot(
+        get_mass(dict_list, part)[mask],
+        y[mask],
+        label=label,
+        xaxis="$m_{" + get_name(part) + "}$ [GeV]",
+        yaxis=yaxis,
+        logy=logy,
+        yscale=yscale,
+        mask=mask,
+        **kwargs
+    )
 
 
 def get_mass(l: dict, iid: int):
     """
     Get the mass of particle with id `iid` out of the list in the "slha" element in the dict.
 
     Returns
         :obj:`list` of float : masses of particles in each element of the dict list.
 
     """
     ret = []
     for s in l["slha"]:
         d = pyslha.read(get_output_dir() + s)
         ret.append(d.blocks["MASS"][abs(iid)])
-        
+
     return np.array(ret)
 
 
-def plot(dict_list,
-         x,
-         y,
-         label=None,
-         xaxis="E [GeV]",
-         yaxis="$\\sigma$ [pb]",
-         ratio=False,
-         K=False,
-         K_plus_1=False,
-         logy=True,
-         yscale=1.,
-         mask=None,
-         **kwargs) -> None:
+def plot(
+    dict_list,
+    x,
+    y,
+    label=None,
+    xaxis="M [GeV]",
+    yaxis="$\\sigma$ [pb]",
+    ratio=False,
+    K=False,
+    K_plus_1=False,
+    logy=True,
+    yscale=1.0,
+    mask=None,
+    **kwargs
+) -> None:
     """
     Creates a plot based on the entries `x`and `y` in `dict_list`.
-    
+
     Examples
 
     .. plot::
         :include-source:
 
         >>> import urllib.request
-        >>> import hepi 
+        >>> import hepi
         >>> dl = hepi.load(urllib.request.urlopen(
         ... "https://raw.githubusercontent.com/fuenfundachtzig/xsec/master/json/pp13_hino_NLO%2BNLL.json"
         ... ))
-        >>> hepi.plot(dl,"N1","NLO_PLUS_NLL",xaxis="$m_{\\\\tilde{\\\\chi}_1^0}$ [GeV]")
+        >>> hepi.plot(dl,"N1","NLO_PLUS_NLL_COMBINED",xaxis="$m_{\\\\tilde{\\\\chi}_1^0}$ [GeV]")
     """
     if isinstance(y, Iterable) and not isinstance(y, str):
         for yi in y:
-            plot(dict_list, x, yi, label, xaxis, yaxis, ratio, K, K_plus_1,
-                 logy, yscale, mask, **kwargs)
+            plot(
+                dict_list,
+                x,
+                yi,
+                label,
+                xaxis,
+                yaxis,
+                ratio,
+                K,
+                K_plus_1,
+                logy,
+                yscale,
+                mask,
+                **kwargs
+            )
         return
     # TODO use kwargs
     if label is None:
         label = y.replace("_PLUS_", "+").replace("_OVER_", "/")
     if label == "":
         label = None
 
@@ -216,390 +279,376 @@
 def slha_plot(li, x, y, **kwargs):
     vx = slha_data(li, x)
     vy = slha_data(li, y)
 
     vplot(np.array(vx), np.array(vy), **kwargs)
 
 
-def vplot(x,
-          y,
-          label=None,
-          xaxis="E [GeV]",
-          yaxis="$\\sigma$ [pb]",
-          logy=True,
-          yscale=1.,
-          interpolate=True,
-          plot_data=True,
-          data_color=None,
-          mask=-1,
-          fill=False,
-          data_fmt=".",
-          fmt="-",
-          print_area=False,
-          sort=True,
-          **kwargs):
+def vplot(
+    x,
+    y,
+    label=None,
+    xaxis="E [GeV]",
+    yaxis="$\\sigma$ [pb]",
+    logy=True,
+    yscale=1.0,
+    interpolate=True,
+    plot_data=True,
+    data_color=None,
+    mask=-1,
+    fill=False,
+    data_fmt=".",
+    fmt="-",
+    print_area=False,
+    sort=True,
+    **kwargs
+):
     """
     Creates a plot based on the values in `x`and `y`.
-    
+
     """
     color = data_color
     if label is None:
-        #label = "??"
+        # label = "??"
         pass
     if mask is None:
         x = x[0]
         y = y[0]
     if sort:
-        permute = x.argsort(kind='stable')
+        permute = x.argsort(kind="stable")
         vx = x[permute]
         vy = y[permute]
     else:
         vx = x
         vy = y
 
-    if data_color is None and 'next_color' not in kwargs:
-        if 'axes' in kwargs and kwargs['axes'] is not None:
-            bl, = kwargs['axes'].plot([], [])
+    if data_color is None and "next_color" not in kwargs:
+        if "axes" in kwargs and kwargs["axes"] is not None:
+            (bl,) = kwargs["axes"].plot([], [])
         else:
-            bl, = plt.gca().plot([], [])
+            (bl,) = plt.gca().plot([], [])
         color = bl.get_color()
-    iii = splot.data(vx,
-                     vy * yscale,
-                     label=label,
-                     xaxis=xaxis,
-                     yaxis=yaxis,
-                     logy=logy,
-                     data_color=color,
-                     fit_color=color,
-                     also_data=plot_data,
-                     interpolate=interpolate,
-                     fmt=data_fmt,
-                     sigmas=0 if not fill else 1,
-                     **kwargs)
+    iii = splot.data(
+        vx,
+        vy * yscale,
+        label=label,
+        xaxis=xaxis,
+        yaxis=yaxis,
+        logy=logy,
+        data_color=color,
+        fit_color=color,
+        also_data=plot_data,
+        interpolate=interpolate,
+        fmt=data_fmt,
+        sigmas=0 if not fill else 1,
+        **kwargs
+    )
     if iii is not None:
-        #ii = iii[0]
+        # ii = iii[0]
         ix = iii[1]
         iy = iii[2]
     if print_area:
-        print('computed AUC using scipy.integrate.simpson: {}'.format(auc.simpson(iy, ix)))
-    if ((np.any(np.less(vy, 0)) or (interpolate and np.any(np.less(iy, 0))))
-            and logy):
-        splot.data(vx,
-                   -vy * yscale,
-                   label="-" + label,
-                   xaxis=xaxis,
-                   yaxis=yaxis,
-                   logy=logy,
-                   data_color=color,
-                   fit_color=color,
-                   also_data=plot_data,
-                   interpolate=interpolate,
-                   interpolate_fmt=(0, (3, 1, 3, 1, 1, 1)),
-                   fmt=data_fmt,
-                   sigmas=0 if not fill else 1,
-                   **kwargs)
-
-
-def mass_mapplot(dict_list,
-                 part1,
-                 part2,
-                 z,
-                 logz=True,
-                 zaxis="$\\sigma$ [pb]",
-                 zscale=1.,
-                 label=None):
-    mapplot(dict_list,
-            "mass_" + str(part1),
-            "mass_" + str(part2),
-            z,
-            xaxis="$M_{" + get_name(part1) + "}$ [GeV]",
-            yaxis="$M_{" + get_name(part2) + "}$ [GeV]",
-            zaxis=zaxis,
-            logz=logz,
-            zscale=zscale)
+        print(
+            "computed AUC using scipy.integrate.simpson: {}".format(auc.simpson(iy, ix))
+        )
+    if (np.any(np.less(vy, 0)) or (interpolate and np.any(np.less(iy, 0)))) and logy:
+        splot.data(
+            vx,
+            -vy * yscale,
+            label="-" + label,
+            xaxis=xaxis,
+            yaxis=yaxis,
+            logy=logy,
+            data_color=color,
+            fit_color=color,
+            also_data=plot_data,
+            interpolate=interpolate,
+            interpolate_fmt=(0, (3, 1, 3, 1, 1, 1)),
+            fmt=data_fmt,
+            sigmas=0 if not fill else 1,
+            **kwargs
+        )
+
+
+def mass_mapplot(
+    dict_list,
+    part1,
+    part2,
+    z,
+    logz=True,
+    zaxis="$\\sigma$ [pb]",
+    zscale=1.0,
+    label=None,
+):
+    mapplot(
+        dict_list,
+        "mass_" + str(part1),
+        "mass_" + str(part2),
+        z,
+        xaxis="$M_{" + get_name(part1) + "}$ [GeV]",
+        yaxis="$M_{" + get_name(part2) + "}$ [GeV]",
+        zaxis=zaxis,
+        logz=logz,
+        zscale=zscale,
+    )
 
 
 def mapplot(dict_list, x, y, z, xaxis=None, yaxis=None, zaxis=None, **kwargs):
     """
 
     Examples
 
     .. plot::
         :include-source:
 
         >>> import urllib.request
-        >>> import hepi 
+        >>> import hepi
 
         >>> dl = hepi.load(urllib.request.urlopen(
         ... "https://raw.githubusercontent.com/APN-Pucky/xsec/master/json/pp13_SGmodel_GGxsec_NLO%2BNLL.json"
         ... ),dimensions=2)
-        >>> hepi.mapplot(dl,"gl","sq","NLO_PLUS_NLL",xaxis="$m_{\\\\tilde{g}}$ [GeV]",yaxis="$m_{\\\\tilde{q}}$ [GeV]" , zaxis="$\\\\sigma_{\\\\mathrm{NLO+NLL}}$ [pb]")
+        >>> hepi.mapplot(dl,"gl","sq","NLO_PLUS_NLL_COMBINED",xaxis="$m_{\\\\tilde{g}}$ [GeV]",yaxis="$m_{\\\\tilde{q}}$ [GeV]" , zaxis="$\\\\sigma_{\\\\mathrm{NLO+NLL}}$ [pb]")
     """
     if xaxis is None:
         xaxis = x
     if yaxis is None:
         yaxis = y
     if zaxis is None:
         zaxis = replace_macros(z)
     vx = dict_list[x]
     vy = dict_list[y]
     vz = dict_list[z]
-    splot.plot2d(vx,
-                 vy,
-                 vz,
-                 style="pcolormesh",
-                 xaxis=xaxis,
-                 yaxis=yaxis,
-                 zaxis=zaxis,
-                 **kwargs)
+    splot.plot2d(
+        vx, vy, vz, style="pcolormesh", xaxis=xaxis, yaxis=yaxis, zaxis=zaxis, **kwargs
+    )
 
 
 map_vplot = lambda *a, **da: splot.plot2d(*a, style="pcolormesh", **da)
 scatter_vplot = lambda *a, **da: splot.plot2d(*a, style="scatter", **da)
 
 
-def scatterplot(dict_list,
-                x,
-                y,
-                z,
-                xaxis=None,
-                yaxis=None,
-                zaxis=None,
-                **kwargs):
+def scatterplot(dict_list, x, y, z, xaxis=None, yaxis=None, zaxis=None, **kwargs):
     """
     Scatter map 2d.
     Central color is the central value, while the inner and outer ring are lower and upper bounds of the uncertainty interval.
 
     Examples
 
     .. plot::
         :include-source:
 
         >>> import urllib.request
-        >>> import hepi 
+        >>> import hepi
         >>> dl = hepi.load(urllib.request.urlopen(
         ... "https://raw.githubusercontent.com/APN-Pucky/xsec/master/json/pp13_hinosplit_N2N1_NLO%2BNLL.json"
         ... ),dimensions=2)
-        >>> hepi.scatterplot(dl,"N1","N2","NLO_PLUS_NLL",xaxis="$m_{\\\\tilde{\\\\chi}_1^0}$ [GeV]",yaxis="$m_{\\\\tilde{\\\\chi}_2^0}$ [GeV]" , zaxis="$\\\\sigma_{\\\\mathrm{NLO+NLL}}$ [pb]")
+        >>> hepi.scatterplot(dl,"N1","N2","NLO_PLUS_NLL_COMBINED",xaxis="$m_{\\\\tilde{\\\\chi}_1^0}$ [GeV]",yaxis="$m_{\\\\tilde{\\\\chi}_2^0}$ [GeV]" , zaxis="$\\\\sigma_{\\\\mathrm{NLO+NLL}}$ [pb]")
 
     """
     if xaxis is None:
         xaxis = x
     if yaxis is None:
         yaxis = y
     if zaxis is None:
         zaxis = replace_macros(z)
     vx = dict_list[x]
     vy = dict_list[y]
     vz = dict_list[z]
-    splot.plot2d(vx,
-                 vy,
-                 vz,
-                 style="scatter",
-                 xaxis=xaxis,
-                 yaxis=yaxis,
-                 zaxis=zaxis,
-                 **kwargs)
+    splot.plot2d(
+        vx, vy, vz, style="scatter", xaxis=xaxis, yaxis=yaxis, zaxis=zaxis, **kwargs
+    )
 
 
 fig = None
 axs = None
 lines = []
 labels = []
 
 
 def err_plt(axes, x, y, label=None, error=False):
     v = label
-    ind = np.argsort(splot.unv(x), kind='stable')
+    ind = np.argsort(splot.unv(x), kind="stable")
     if error:
-        l, _, _ = axes.errorbar(x.to_numpy()[ind],
-                                splot.unv(y)[ind],
-                                yerr=splot.usd(y),
-                                capsize=5,
-                                label=v)
+        l, _, _ = axes.errorbar(
+            x.to_numpy()[ind], splot.unv(y)[ind], yerr=splot.usd(y), capsize=5, label=v
+        )
         return l
     else:
         l = axes.plot(x.to_numpy()[ind], splot.unv(y)[ind], label=v)
         return l[0]
 
 
-def scale_plot(dict_list,
-               vl,
-               seven_point_band=False,
-               cont=False,
-               error=True,
-               li=None,
-               plehn_color=False,
-               yscale=1.,
-               unit="pb",
-               yaxis=None,
-               **kwargs):
+def scale_plot(
+    dict_list,
+    vl,
+    seven_point_band=False,
+    cont=False,
+    error=True,
+    li=None,
+    plehn_color=False,
+    yscale=1.0,
+    unit="pb",
+    yaxis=None,
+    **kwargs
+):
     """Creates a scale variance plot with 5 panels (xline)."""
     global fig, axs, lines, labels
-    cycle_safe = mpl.rcParams['axes.prop_cycle']
+    cycle_safe = mpl.rcParams["axes.prop_cycle"]
     if plehn_color:
-        mpl.rcParams['axes.prop_cycle'] = mpl.cycler(color=["b", "r", "g"])
+        mpl.rcParams["axes.prop_cycle"] = mpl.cycler(color=["b", "r", "g"])
     if not cont:
         fig, axs = plt.subplots(1, 5, figsize=(12, 3), sharey=True)
         # Remove horizontal space between axes
         fig.subplots_adjust(wspace=0)
         if li is not None:
             title(axs[2], li[0], **kwargs)
 
     mr = dict_list["mu_r"]
     mf = dict_list["mu_f"]
 
     if not cont:
         lines = []
         labels = []
-        axs[0].plot([], [], ' ', color='k', label="$\\mu_R=" + "\\mu_F$")
-        axs[1].plot([], [],
-                    ' ',
-                    color='k',
-                    label="$\\mu_R=" + str(np.max(mr)) + "\\mu_0$")
-        axs[2].plot([], [],
-                    ' ',
-                    color='k',
-                    label="$\\mu_F=" + str(np.min(mf)) + "\\mu_0$")
-        axs[3].plot([], [],
-                    ' ',
-                    color='k',
-                    label="$\\mu_R=" + str(np.min(mr)) + "\\mu_0$")
-        axs[4].plot([], [],
-                    ' ',
-                    color='k',
-                    label="$\\mu_F=" + str(np.max(mf)) + "\\mu_0$")
+        axs[0].plot([], [], " ", color="k", label="$\\mu_R=" + "\\mu_F$")
+        axs[1].plot(
+            [], [], " ", color="k", label="$\\mu_R=" + str(np.max(mr)) + "\\mu_0$"
+        )
+        axs[2].plot(
+            [], [], " ", color="k", label="$\\mu_F=" + str(np.min(mf)) + "\\mu_0$"
+        )
+        axs[3].plot(
+            [], [], " ", color="k", label="$\\mu_R=" + str(np.min(mr)) + "\\mu_0$"
+        )
+        axs[4].plot(
+            [], [], " ", color="k", label="$\\mu_F=" + str(np.max(mf)) + "\\mu_0$"
+        )
 
     for v in vl:
         mv = dict_list[v] * yscale
         if seven_point_band:
-            #mask = (mf/mr < 4.) & (mf/mr > 1./4.) & (mf <= 2) & (mf >= 1./2.) & (mr <= 2) & (mr >= 1./2.)
-            mask = (((mf == 2.) & (mr == 2.)) | ((mf == 2.) & (mr == 1.)) |
-                    ((mf == 1.) & (mr == 1.)) | ((mf == 1.) & (mr == 2.)) |
-                    ((mf == 1 / 2.) & (mr == 1 / 2.)) |
-                    ((mf == 1 / 2.) & (mr == 1.)) | ((mf == 1.) &
-                                                     (mr == 1 / 2.)))
+            # mask = (mf/mr < 4.) & (mf/mr > 1./4.) & (mf <= 2) & (mf >= 1./2.) & (mr <= 2) & (mr >= 1./2.)
+            mask = (
+                ((mf == 2.0) & (mr == 2.0))
+                | ((mf == 2.0) & (mr == 1.0))
+                | ((mf == 1.0) & (mr == 1.0))
+                | ((mf == 1.0) & (mr == 2.0))
+                | ((mf == 1 / 2.0) & (mr == 1 / 2.0))
+                | ((mf == 1 / 2.0) & (mr == 1.0))
+                | ((mf == 1.0) & (mr == 1 / 2.0))
+            )
             mvmax = np.max(splot.unv(mv[mask]))
             mvmin = np.min(splot.unv(mv[mask]))
 
         mask = mf == mr
         l = err_plt(axs[0], mf[mask], mv[mask], error=error)
-        #l, _, _ = axs[0].errorbar(mf[mask], splot.unv(mv[mask]),
+        # l, _, _ = axs[0].errorbar(mf[mask], splot.unv(mv[mask]),
         #                          yerr=splot.usd(mv[mask]), capsize=5, label=v)
         if seven_point_band:
-            axs[0].fill_between(mf[mask],
-                                mvmax,
-                                mvmin,
-                                facecolor=l.get_color(),
-                                alpha=0.3)
+            axs[0].fill_between(
+                mf[mask], mvmax, mvmin, facecolor=l.get_color(), alpha=0.3
+            )
 
         mask = mr == np.max(mr)
         l = err_plt(axs[1], mf[mask], mv[mask], error=error)
         lines.append(l)
-        labels.append("$\\sigma_{\\mathrm{" +
-                      v.replace("_PLUS_", "+").replace(" ", "\\ ") + "} }$")
-        #l, _, _ = axs[1].errorbar(mf[mask], splot.unv(mv[mask]),
+        labels.append(
+            "$\\sigma_{\\mathrm{"
+            + v.replace("_PLUS_", "+").replace(" ", "\\ ")
+            + "} }$"
+        )
+        # l, _, _ = axs[1].errorbar(mf[mask], splot.unv(mv[mask]),
         #                          yerr=splot.usd(mv[mask]), capsize=5)
         if seven_point_band:
-            axs[1].fill_between(mf[mask],
-                                mvmax,
-                                mvmin,
-                                facecolor=l.get_color(),
-                                alpha=0.3)
+            axs[1].fill_between(
+                mf[mask], mvmax, mvmin, facecolor=l.get_color(), alpha=0.3
+            )
 
         mask = mf == np.min(mf)
         l = err_plt(axs[2], mr[mask], mv[mask], error=error)
-        #l, _, _ = axs[2].errorbar(mr[mask], splot.unv(mv[mask]),
+        # l, _, _ = axs[2].errorbar(mr[mask], splot.unv(mv[mask]),
         #                          yerr=splot.usd(mv[mask]), capsize=5)
         if seven_point_band:
-            axs[2].fill_between(mr[mask],
-                                mvmax,
-                                mvmin,
-                                facecolor=l.get_color(),
-                                alpha=0.3)
+            axs[2].fill_between(
+                mr[mask], mvmax, mvmin, facecolor=l.get_color(), alpha=0.3
+            )
 
         mask = mr == np.min(mr)
         l = err_plt(axs[3], mf[mask], mv[mask], error=error)
-        #l, _, _ = axs[3].errorbar(mf[mask], splot.unv(mv[mask]),
+        # l, _, _ = axs[3].errorbar(mf[mask], splot.unv(mv[mask]),
         #                          yerr=splot.usd(mv[mask]), capsize=5)
         if seven_point_band:
-            axs[3].fill_between(mf[mask],
-                                mvmax,
-                                mvmin,
-                                facecolor=l.get_color(),
-                                alpha=0.3)
+            axs[3].fill_between(
+                mf[mask], mvmax, mvmin, facecolor=l.get_color(), alpha=0.3
+            )
 
         mask = mf == np.max(mf)
         l = err_plt(axs[4], mr[mask], mv[mask], error=error)
-        #l, _, _ = axs[4].errorbar(mr[mask], splot.unv(mv[mask]),
+        # l, _, _ = axs[4].errorbar(mr[mask], splot.unv(mv[mask]),
         #                          yerr=splot.usd(mv[mask]), capsize=5)
         if seven_point_band:
-            f = axs[4].fill_between(mr[mask],
-                                    mvmax,
-                                    mvmin,
-                                    facecolor=l.get_color(),
-                                    alpha=0.3)
+            f = axs[4].fill_between(
+                mr[mask], mvmax, mvmin, facecolor=l.get_color(), alpha=0.3
+            )
             lines.append(f)
-            labels.append("$\\Delta \\sigma_{\\mathrm{" + v.replace(
-                "NLO_PLUS_NLL", "NLO+NLL").replace(" ", "\\<space>") + "} }$")
+            labels.append(
+                "$\\Delta \\sigma_{\\mathrm{"
+                + v.replace("NLO_PLUS_NLL", "NLO+NLL").replace(" ", "\\<space>")
+                + "} }$"
+            )
 
     axs[0].set_ylabel("$\\sigma$ [" + unit + "]" if yaxis is None else yaxis)
 
     axs[0].set_xscale("log")
     axs[0].set_xlim(np.min(mf), np.max(mf))
     axs[0].set_xlabel("$\\mu_{R,F}/\\mu_0$")
 
     # axs[1].plot(t, s2)
     axs[1].set_xscale("log")
     axs[1].set_xlim(np.max(mf), np.min(mf))
-    axs[1].set_xticks([1.])
+    axs[1].set_xticks([1.0])
     axs[1].xaxis.set_minor_formatter(NullFormatter())
     axs[1].set_xlabel("$\\mu_{F}/\\mu_0$")
 
     # axs[2].plot(t, s3)
     axs[2].set_xscale("log")
     axs[2].set_xlim(np.max(mf), np.min(mf))
-    axs[2].set_xticks([1.])
+    axs[2].set_xticks([1.0])
     axs[2].xaxis.set_minor_formatter(NullFormatter())
     axs[2].set_xlabel("$\\mu_{R}/\\mu_0$")
 
     # axs[3].plot(t, s3)
     axs[3].set_xscale("log")
     axs[3].set_xlim(np.min(mf), np.max(mf))
-    axs[3].set_xticks([1.])
+    axs[3].set_xticks([1.0])
     axs[3].xaxis.set_minor_formatter(NullFormatter())
     axs[3].set_xlabel("$\\mu_{F}/\\mu_0$")
 
     # axs[4].plot(t, s3)
     axs[4].set_xscale("log")
     axs[4].set_xlim(np.min(mf), np.max(mf))
-    axs[4].set_xticks([1.])
+    axs[4].set_xticks([1.0])
     axs[4].xaxis.set_minor_formatter(NullFormatter())
     axs[4].set_xlabel("$\\mu_{R}/\\mu_0$")
 
     axs[0].legend(handletextpad=-0.0, handlelength=0, fancybox=False)
     axs[1].legend(handletextpad=-0.0, handlelength=0, fancybox=False)
     axs[2].legend(handletextpad=-0.0, handlelength=0, fancybox=False)
     axs[3].legend(handletextpad=-0.0, handlelength=0, fancybox=False)
     axs[4].legend(handletextpad=-0.0, handlelength=0, fancybox=False)
     fig.legend()
     fig.legends = []
     fig.legend(handles=lines, labels=labels, loc="center right")
     plt.subplots_adjust(right=0.84)
     # plt.show()
-    mpl.rcParams['axes.prop_cycle'] = cycle_safe
+    mpl.rcParams["axes.prop_cycle"] = cycle_safe
 
 
-def central_scale_plot(dict_list,
-                       vl,
-                       cont=False,
-                       error=True,
-                       yscale=1.,
-                       unit="pb",
-                       yaxis=None):
+def central_scale_plot(
+    dict_list, vl, cont=False, error=True, yscale=1.0, unit="pb", yaxis=None
+):
     """Creates a scale variance plot with 3 panels (ystacked)."""
     global fig, axs
     if not cont:
         fig, axs = plt.subplots(3, 1, figsize=(12, 8), sharex=True)
         # Remove horizontal space between axes
         fig.subplots_adjust(hspace=0)
 
@@ -615,37 +664,33 @@
         mask = mf == 1.0
         l = err_plt(axs[1], mr[mask], mv[mask], error=error)
 
         mask = mr == 1.0
         l = err_plt(axs[2], mf[mask], mv[mask], error=error)
 
     if not cont:
-        axs[0].plot([], [], ' ', label="$\\mu_R=\\mu_F=\\mu$")
-        axs[1].plot([], [], ' ', label="$\\mu_F=\\mu_0$, $\\mu_R=\\mu$")
-        axs[2].plot([], [], ' ', label="$\\mu_R=\\mu_0$, $\\mu_F=\\mu$")
+        axs[0].plot([], [], " ", label="$\\mu_R=\\mu_F=\\mu$")
+        axs[1].plot([], [], " ", label="$\\mu_F=\\mu_0$, $\\mu_R=\\mu$")
+        axs[2].plot([], [], " ", label="$\\mu_R=\\mu_0$, $\\mu_F=\\mu$")
 
     axs[1].set_ylabel("$\\sigma$ [" + unit + "]" if yaxis is None else yaxis)
 
     axs[0].set_xscale("log")
-    #axs[0].set_xlim(np.min(mf), np.max(mf))
+    # axs[0].set_xlim(np.min(mf), np.max(mf))
     axs[2].set_xlabel("$\\mu/\\mu_0$")
 
     axs[0].legend()
     axs[1].legend()
     axs[2].legend()
     # plt.show()
 
 
-def init_double_plot(figsize=(6, 8),
-                     sharex=True,
-                     sharey=False,
-                     gridspec_kw={'height_ratios': [3, 1]}):
+def init_double_plot(
+    figsize=(6, 8), sharex=True, sharey=False, gridspec_kw={"height_ratios": [3, 1]}
+):
     """Initialze subplot for Ratio/K plots with another figure below."""
-    fig, axs = plt.subplots(2,
-                            1,
-                            figsize=figsize,
-                            sharex=sharex,
-                            sharey=sharey,
-                            gridspec_kw=gridspec_kw)
+    fig, axs = plt.subplots(
+        2, 1, figsize=figsize, sharex=sharex, sharey=sharey, gridspec_kw=gridspec_kw
+    )
     # Remove horizontal space between axes
     fig.subplots_adjust(hspace=0)
     return fig, axs
```

### Comparing `hepi-0.2.8/hepi/prospino2/prospino_main.f90_template` & `hepi-0.2.9/hepi/run/prospino2/prospino_main.f90_template`

 * *Files 0% similar despite different names*

```diff
@@ -125,9 +125,7 @@
 !  output file: prospino.dat   for compact output format                    !
 !               prospino.dat2  for long output including subchannels        !
 !               prospino.dat3  lo file for masses, flags, etc               !
 !----------------------------------------------------------------------------
   call PROSPINO_OPEN_CLOSE(1)                                                            ! close all input/output files 
 
 end program main
-
-
```

### Comparing `hepi-0.2.8/hepi/prospino2/run.py` & `hepi-0.2.9/hepi/run/prospino2/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import pkgutil
 import shutil
 import stat
-from string import Template
 import subprocess
 import warnings
+from string import Template
+
+from uncertainties import ufloat
+
 from hepi.input import Input, Order, is_gluino, is_slepton, is_squark, is_weakino
 from hepi.results import Result
-from hepi.run import RunParam, Runner
-from uncertainties import ufloat
+from hepi.run import Runner, RunParam
 
 
 class ProspinoResult(Result):
     """
     Prospino Result Data.
     """
 
@@ -57,58 +59,83 @@
         (2000015, 1000016): 13,
     }
 
     def _get_ps_proc(self, p: Input):
         if p.has_squark() and p.has_weakino():
             sq = p.particle1 if is_squark(p.particle1) else p.particle2
             weakino = p.particle2 if is_squark(p.particle1) else p.particle1
-            return 'ns', self.weakino_map[weakino], 1, self.squark_map[abs(
-                sq)], 1
+            return "ns", self.weakino_map[weakino], 1, self.squark_map[abs(sq)], 1
         if p.has_gluino() and p.has_weakino():
-            return 'ng', self.weakino_map[p.particle1 if is_gluino(p.particle2
-                                                                   ) else p.
-                                          particle2], 1, 1, 1
+            return (
+                "ng",
+                self.weakino_map[
+                    p.particle1 if is_gluino(p.particle2) else p.particle2
+                ],
+                1,
+                1,
+                1,
+            )
         if p.has_gluino() and p.has_squark():
-            return 'sg', 1, 1, self.squark_map[abs(
-                p.particle1 if is_gluino(p.particle2) else p.particle2)], 1
+            return (
+                "sg",
+                1,
+                1,
+                self.squark_map[
+                    abs(p.particle1 if is_gluino(p.particle2) else p.particle2)
+                ],
+                1,
+            )
         if is_weakino(p.particle1) and is_weakino(p.particle2):
-            return 'nn', self.weakino_map[p.particle1], self.weakino_map[
-                p.particle2], 1, 1
+            return (
+                "nn",
+                self.weakino_map[p.particle1],
+                self.weakino_map[p.particle2],
+                1,
+                1,
+            )
         if is_slepton(p.particle1) and is_slepton(p.particle2):
-            return 'll', self.slepton_map[(p.particle1, p.particle2)], 1, 1, 1
+            return "ll", self.slepton_map[(p.particle1, p.particle2)], 1, 1, 1
         if is_gluino(p.particle1) and is_gluino(p.particle2):
-            return 'gg', 1, 1, 1, 1
+            return "gg", 1, 1, 1, 1
         if is_squark(p.particle1) and is_squark(p.particle2):
             if p.particle1 > 0 and p.particle2 > 0:
-                return 'ss', 1, 1, self.squark_map[abs(
-                    p.particle1)], self.squark_map[abs(p.particle2)]
-            elif (p.particle1 > 0
-                  and p.particle2 < 0) or (p.particle1 < 0
-                                           and p.particle2 > 0):
+                return (
+                    "ss",
+                    1,
+                    1,
+                    self.squark_map[abs(p.particle1)],
+                    self.squark_map[abs(p.particle2)],
+                )
+            elif (p.particle1 > 0 and p.particle2 < 0) or (
+                p.particle1 < 0 and p.particle2 > 0
+            ):
                 s = p.particle1 if p.particle1 > p.particle2 else p.particle2
                 b = p.particle2 if p.particle1 > p.particle2 else p.particle1
-                return 'sb', 1, 1, self.squark_map[abs(s)], self.squark_map[
-                    abs(b)]
+                return "sb", 1, 1, self.squark_map[abs(s)], self.squark_map[abs(b)]
         return "UNKNOWN_PROCESS_OR_UNIMPLEMENTED_PROCESS"
 
     def _get_ps_input(self, p: Input) -> dict:
         d = {}
         d["ps_inlo"] = int(p.order)
-        d["ps_final_state_in"], d["ps_ipart1_in"], d["ps_ipart2_in"], d[
-            "ps_isquark1_in"], d["ps_isquark2_in"] = self._get_ps_proc(p)
+        (
+            d["ps_final_state_in"],
+            d["ps_ipart1_in"],
+            d["ps_ipart2_in"],
+            d["ps_isquark1_in"],
+            d["ps_isquark2_in"],
+        ) = self._get_ps_proc(p)
         return d
 
     def orders(self) -> Order:
         return [Order.LO, Order.NLO]
 
     def _check_input(self, p: Input, **kwargs) -> bool:
         """Checks input parameter for compatibility with Prospino"""
-        if p.mu_f != 1. or p.mu_r != 1.:
-            warnings.warn(
-                "Prospino2 does not support varying the scales manually.")
+        if p.mu_f != 1.0 or p.mu_r != 1.0:
+            warnings.warn("Prospino2 does not support varying the scales manually.")
             return False
         if p.pdf_lo != "cteq6l1" or p.pdf_nlo != "cteq66":
             warnings.warn(
                 "Prospino2 does not support all pdfs (CTEQ6L1 and CTEQ66 allowed defaults)."
             )
             return False
         return True
@@ -116,65 +143,74 @@
     def _is_valid(self, file: str, p: Input, d) -> bool:
         return super()._is_valid(file, p, d)
 
     def _parse_file(self, file: str) -> Result:
         ret = []
         with open(file) as output:
             for line in output:
-                if line.startswith("nn") or line.startswith(
-                        "ng") or line.startswith("ns") or line.startswith(
-                            "sg") or line.startswith("ll") or line.startswith(
-                                "gg") or line.startswith(
-                                    "ss") or line.startswith(
-                                        "sb"):  # TODO generalize
+                if (
+                    line.startswith("nn")
+                    or line.startswith("ng")
+                    or line.startswith("ns")
+                    or line.startswith("sg")
+                    or line.startswith("ll")
+                    or line.startswith("gg")
+                    or line.startswith("ss")
+                    or line.startswith("sb")
+                ):  # TODO generalize
                     for s in line[2:].split():
                         ret.append(float(s))
         return ProspinoResult(
             ufloat(ret[8], ret[8] * ret[9]),
-            ufloat(ret[10], ret[10] * ret[11]) if ret[10] != 0. else None,
-            None)
+            ufloat(ret[10], ret[10] * ret[11]) if ret[10] != 0.0 else None,
+            None,
+        )
 
     def _prepare(self, p: Input, **kwargs) -> RunParam:
         rp = super()._prepare(p, **kwargs)
         if not rp.skip:
             d = p.__dict__
-            data = pkgutil.get_data(
-                __name__, "prospino_main.f90_template").decode('utf-8')
+            data = pkgutil.get_data(__name__, "prospino_main.f90_template").decode(
+                "utf-8"
+            )
             src = Template(data)
-            #compute dependent pieces for template
+            # compute dependent pieces for template
             d["ps_inlo"] = int(p.order)
             for k, v in self._get_ps_input(p).items():
                 d[k] = v
             result = src.substitute(d)
-            #open(rp.in_file, "w").write(result)
+            # open(rp.in_file, "w").write(result)
             open(rp.out_file, "w").write(result + "\n\n")
             rdir = self.get_output_dir() + rp.name + ".rdir"
             if os.path.exists(rdir) and os.path.isdir(rdir):
                 shutil.rmtree(rdir)
             shutil.copytree(self.get_path(), rdir)
             open(rdir + "/prospino_main.f90", "w").write(result)
             # compile
-            subprocess.Popen("cd " + rdir + " && make",
-                             shell=True,
-                             stdout=subprocess.DEVNULL).wait()
+            subprocess.Popen(
+                "cd " + rdir + " && make", shell=True, stdout=subprocess.DEVNULL
+            ).wait()
 
             open(rp.execute, "w").write(
-                "#!/bin/sh\n" +
-                "H=$PWD && cd {rdir}&& ./prospino_2.run > tmp.out && cd $H  && cat {rdir}/tmp.out  >> {out} && cat {rdir}/prospino.dat>> {out} && rm -rf {rdir}"
-                .format(rdir=rdir, out=rp.out_file))
+                "#!/bin/sh\n"
+                + "H=$PWD && cd {rdir}&& ./prospino_2.run > tmp.out && cd $H  && cat {rdir}/tmp.out  >> {out} && cat {rdir}/prospino.dat>> {out} && rm -rf {rdir}".format(
+                    rdir=rdir, out=rp.out_file
+                )
+            )
             st = os.stat(rp.execute)
             os.chmod(rp.execute, st.st_mode | stat.S_IEXEC)
 
-            sname = d['slha']
-            shutil.copy(self.get_output_dir() + sname,
-                        rdir + "/prospino.in.les_houches")
-            with open(self.get_output_dir() + sname, 'r') as f:
+            sname = d["slha"]
+            shutil.copy(
+                self.get_output_dir() + sname, rdir + "/prospino.in.les_houches"
+            )
+            with open(self.get_output_dir() + sname, "r") as f:
                 open(rp.out_file, "a").write(f.read() + "\n\n")
         return rp
 
 
 # Legacy
 default_prospino_runner = ProspinoRunner("~/git/Prospino2/")
 """Default Prospino Runner to provide backward compatibility"""
 run = default_prospino_runner.run
 set_path = default_prospino_runner.set_path
-get_path = default_prospino_runner.get_path
+get_path = default_prospino_runner.get_path
```

### Comparing `hepi-0.2.8/hepi/results.py` & `hepi-0.2.9/hepi/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 """Results and postprocessing for the :mod:`hepi` package."""
-from .util import DictData
-import numpy as np
-from uncertainties import unumpy
-from smpl import plot
+import multiprocessing as mp
 import warnings
-import tqdm
-#from pqdm.processes import pqdm as ppqdm
+
+import numpy as np
+import uncertainties.unumpy as unp
+
+# from pqdm.processes import pqdm as ppqdm
 from pqdm.threads import pqdm as tpqdm
-import multiprocessing as mp
-from smpl.parallel import par
 
-#If the numerical uncertainty times :attr:`required_numerical_uncertainty_factor` is higher than the scale or pdf uncertainty a warning is shown.
-required_numerical_uncertainty_factor = 5
+from .util import DictData
 
+# If the numerical uncertainty times :attr:`required_numerical_uncertainty_factor` is higher than the scale or pdf uncertainty a warning is shown.
+required_numerical_uncertainty_factor = 5
 
-def my_parallel(arr, f, n_jobs=None, desc=None):
-    """
-    Parallel execution of f on each element of args
-    """
-    n_jobs = n_jobs or mp.cpu_count()
-    sa = np.array_split(np.array(arr), len(arr) / n_jobs)
-    res = []
-    for i in tqdm.tqdm(range(len(sa)), desc=desc):
-        res += par(f, sa[i])
-    return res
+unv = unp.nominal_values
+usd = unp.std_devs
 
 
 class Result(DictData):
     """
-    General result class.
+    General result class. All uncertainties are of numerical origin.
 
     Attributes:
         LO (:obj:`double`): Leading Order result. Defaults to None.
         NLO (:obj:`double`): Next-to-Leading Order result. Defaults to None.
         NLO_PLUS_NLL (:obj:`double`): Next-to-Leading Order plus Next-to-Leading Logarithm result. Defaults to None.
         K_LO (:obj:`double`): LO divided by LO.
         K_NLO (:obj:`double`): NLO divided by LO result.
         K_NLO_PLUS_NLL (:obj:`double`): NLO+NLL divided by LO.
         K_aNNLO_PLUS_NNLL (:obj:`double`): aNNLO+NNLL divided by LO.
         NLO_PLUS_NLL_OVER_NLO (:obj:`double`): NLO+NLL divided by NLO.
         aNNLO_PLUS_NNLL_OVER_NLO (:obj:`double`): aNNLO+NNLL divided by NLO.
     """
 
-    def __init__(self,
-                 lo=None,
-                 nlo=None,
-                 nlo_plus_nll=None,
-                 annlo_plus_nnll=None):
+    def __init__(self, lo=None, nlo=None, nlo_plus_nll=None, annlo_plus_nnll=None):
         """
         Sets given and computes dependent ``Attributes``.
 
         Args:
             lo (:obj:`double`): corresponds to :attr:`LO`.
             nlo (:obj:`double`): corresponds to :attr:`NLO`.
             nlo_plus_nll (:obj:`double`): corresponds to :attr:`NLO_PLUS_NLL`.
@@ -86,60 +73,60 @@
         if annlo_plus_nnll is not None and nlo != 0:
             self.aNNLO_PLUS_NNLL_OVER_NLO = annlo_plus_nnll / nlo
         else:
             self.aNNLO_PLUS_NNLL_OVER_NLO = None
 
 
 # TODO detect which errors also for scales
-def pdf_errors(li,
-               dl,
-               ordernames=None,
-               confidence_level=90,n_jobs=None):
+def pdf_errors(li, dl, ordernames=None, confidence_level=90, n_jobs=None):
     """
     Just like `pdf_error` but over a list of ordernames.
     """
     if ordernames is None:
         ordernames = ["LO", "NLO", "aNNLO_PLUS_NNLL"]
     r_dl = dl
     for o in ordernames:
-        r_dl = pdf_error(li, r_dl, o, confidence_level=confidence_level,n_jobs=n_jobs)
+        r_dl = pdf_error(li, r_dl, o, confidence_level=confidence_level, n_jobs=n_jobs)
 
     return r_dl
 
 
-def _pdf_error_single(members, i, dl, ordername, confidence_level=90):  
+def _pdf_error_single(members, i, dl, ordername, confidence_level=90):
     try:
         import lhapdf
     except ImportError:
-        raise RuntimeError("LHAPDF with python bindings needed to compute PDF uncertainties. Make sure you set the PYTHONPATH correctly (i.e. correct python version).")
+        raise RuntimeError(
+            "LHAPDF with python bindings needed to compute PDF uncertainties. Make sure you set the PYTHONPATH correctly (i.e. correct python version)."
+        )
     if not lhapdf.availablePDFSets():
-        raise RuntimeError("No PDF sets found. Make sure the environment variable LHAPDF_DATA_DIR points to the correct location (.../share/LHAPDF).")
-    if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][
-            i] == 1.0:
+        raise RuntimeError(
+            "No PDF sets found. Make sure the environment variable LHAPDF_DATA_DIR points to the correct location (.../share/LHAPDF)."
+        )
+    if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0:
         pdfset = lhapdf.getPDFSet(dl["pdf_nlo"][i])
         pdfs = [0.0] * pdfset.size
-        ddl = dl[members].drop(columns=["pdfset_nlo", "precision","max_iters"])
-        bol = ddl.eq(ddl.iloc[i]).all(axis='columns')
+        ddl = dl[members].drop(columns=["pdfset_nlo", "precision", "max_iters"])
+        bol = ddl.eq(ddl.iloc[i]).all(axis="columns")
         for j in range(len(dl["pdfset_nlo"])):
             if bol[j]:
                 pdfs[dl["pdfset_nlo"][j]] = j
 
-    # lo_unc = pdfset.uncertainty(
-    #    [plot.unv(dl["LO"][k]) for k in pdfs], -1)
-    #if ordername == "LO":
-    #    dl.loc[i, "LO_PDF_CENTRAL"] = plot.unv(dl["LO"][i])
-    #    dl.loc[i, "LO_PDF_ERRPLUS"] = 0.0
-    #    dl.loc[i, "LO_PDF_ERRMINUS"] = 0.0
-    #    dl.loc[i, "LO_PDF_ERRSYM"] = 0.0
-    #else:
-    #print([float(plot.unv(dl[ordername][k])) for k in pdfs])
+        # lo_unc = pdfset.uncertainty(
+        #    [unv(dl["LO"][k]) for k in pdfs], -1)
+        # if ordername == "LO":
+        #    dl.loc[i, "LO_PDF_CENTRAL"] = unv(dl["LO"][i])
+        #    dl.loc[i, "LO_PDF_ERRPLUS"] = 0.0
+        #    dl.loc[i, "LO_PDF_ERRMINUS"] = 0.0
+        #    dl.loc[i, "LO_PDF_ERRSYM"] = 0.0
+        # else:
+        # print([float(unv(dl[ordername][k])) for k in pdfs])
         nlo_unc = pdfset.uncertainty(
-            [float(plot.unv(dl[ordername][k])) for k in pdfs],
-            confidence_level)
-    return (i,nlo_unc)
+            [float(unv(dl[ordername][k])) for k in pdfs], confidence_level
+        )
+    return (i, nlo_unc)
 
 
 def pdf_error(li, dl, ordername="LO", confidence_level=90, n_jobs=None):
     """
     Computes Parton Density Function (PDF) uncertainties through :func:`lhapdf.set.uncertainty`.
 
     Args:
@@ -152,157 +139,183 @@
         :obj:`dict`: Modified `dl` with new `ordername_{PDF,PDF_CENTRAL,PDF_ERRPLUS,PDF_ERRMINUS,PDF_ERRSYM}` entries.
             - (`ordername`)_`PDF` contains a symmetrized :mod:`uncertainties` object.
     """
     global required_numerical_uncertainty_factor
 
     example = li[0]
     members = [
-        attr for attr in dir(example)
+        attr
+        for attr in dir(example)
         if not callable(getattr(example, attr)) and not attr.startswith("__")
     ]
 
     dl[ordername + "_PDF"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_PDF_CENTRAL"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_PDF_ERRPLUS"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_PDF_ERRMINUS"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_PDF_ERRSYM"] = np.array([None] * len(dl["pdfset_nlo"]))
 
-    args = [{
-        "members": members,
-        "i": i,
-        "dl": dl,
-        "ordername": ordername,
-        "confidence_level": confidence_level
-    } for i in range(len(dl["pdfset_nlo"])) if dl["pdfset_nlo"][i] == 0
-            and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0]
-    ret = tpqdm(args,
-                _pdf_error_single,
-                n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                argument_type='kwargs',
-                desc="PDF uncertainty @ " + ordername)
+    args = [
+        {
+            "members": members,
+            "i": i,
+            "dl": dl,
+            "ordername": ordername,
+            "confidence_level": confidence_level,
+        }
+        for i in range(len(dl["pdfset_nlo"]))
+        if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0
+    ]
+    ret = tpqdm(
+        args,
+        _pdf_error_single,
+        n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+        argument_type="kwargs",
+        desc="PDF uncertainty @ " + ordername,
+    )
     for i, nlo_unc in ret:
         dl.loc[i, ordername + "_PDF_CENTRAL"] = nlo_unc.central
         dl.loc[i, ordername + "_PDF_ERRPLUS"] = nlo_unc.errplus
         dl.loc[i, ordername + "_PDF_ERRMINUS"] = -nlo_unc.errminus
         dl.loc[i, ordername + "_PDF_ERRSYM"] = nlo_unc.errsymm
-        #TODO error sym to minus and plus
-        #if :
-        if (ordername != "LO" and
-            (plot.usd(dl[ordername][i]) * required_numerical_uncertainty_factor
-             > dl[ordername + "_PDF_ERRPLUS"][i]-dl[ordername + "_PDF_ERRMINUS"][i]  )):
-            rel = plot.unv(dl[ordername][i])
+        # TODO error sym to minus and plus
+        # if :
+        if ordername != "LO" and (
+            usd(dl[ordername][i]) * required_numerical_uncertainty_factor
+            > dl[ordername + "_PDF_ERRPLUS"][i] - dl[ordername + "_PDF_ERRMINUS"][i]
+        ):
+            rel = unv(dl[ordername][i])
             warnings.warn(
-                "too bad numerical precision vs pdf @ " + ordername +
-                " num: " + str(plot.usd(dl[ordername][i]) / rel * 100.) +
-                "% vs " + str(dl[ordername + "_PDF_ERRPLUS"][i] / rel * 100.) +
-                "% to pdf: " +
-                str(dl[ordername + "_PDF_ERRMINUS"][i] / rel * 100.) + "%",
-                RuntimeWarning)
+                "too bad numerical precision vs pdf @ "
+                + ordername
+                + " num: "
+                + str(usd(dl[ordername][i]) / rel * 100.0)
+                + "% vs "
+                + str(dl[ordername + "_PDF_ERRPLUS"][i] / rel * 100.0)
+                + "% to pdf: "
+                + str(dl[ordername + "_PDF_ERRMINUS"][i] / rel * 100.0)
+                + "%",
+                RuntimeWarning,
+            )
 
     mask = dl[ordername + "_PDF_CENTRAL"].notnull()
-    dl.loc[mask, ordername + "_PDF"] = unumpy.uarray(
-        plot.unv(dl[ordername + "_PDF_CENTRAL"][mask]) +
-        dl[ordername + "_PDF_ERRPLUS"][mask] / 2. +
-        dl[ordername + "_PDF_ERRMINUS"][mask] / 2.,
-        (dl[ordername + "_PDF_ERRPLUS"][mask] -
-         dl[ordername + "_PDF_ERRMINUS"][mask]) / 2.)
+    dl.loc[mask, ordername + "_PDF"] = unp.uarray(
+        unv(dl[ordername + "_PDF_CENTRAL"][mask])
+        + dl[ordername + "_PDF_ERRPLUS"][mask] / 2.0
+        + dl[ordername + "_PDF_ERRMINUS"][mask] / 2.0,
+        (dl[ordername + "_PDF_ERRPLUS"][mask] - dl[ordername + "_PDF_ERRMINUS"][mask])
+        / 2.0,
+    )
 
     return dl
 
 
-def scale_errors(li, dl, ordernames=None,n_jobs=None):
+def scale_errors(li, dl, ordernames=None, n_jobs=None):
     """
     Just like `scale_error` but over a list of ordernames.
     """
     if ordernames is None:
         ordernames = ["LO", "NLO", "aNNLO_PLUS_NNLL"]
     r_dl = dl
     for o in ordernames:
         r_dl = scale_error(li, r_dl, o, n_jobs=n_jobs)
 
     return r_dl
 
-def _scale_error_single(members,i,dl,ordername="LO"):
-    if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][
-        i] == 1.0:
+
+def _scale_error_single(members, i, dl, ordername="LO"):
+    if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0:
         scales = []
-        ddl = dl[members].drop(columns=["mu_f","mu_r", "precision","max_iters"])
-        bol = ddl.eq(ddl.iloc[i]).all(axis='columns')
+        ddl = dl[members].drop(columns=["mu_f", "mu_r", "precision", "max_iters"])
+        bol = ddl.eq(ddl.iloc[i]).all(axis="columns")
         for j in range(len(dl["pdfset_nlo"])):
             if bol[j]:
                 scales.append(j)
     # index, errplus,errminus
     return (
         i,
-        np.max( [plot.unv(dl[ordername][k]) for k in scales]) - plot.unv(dl[ordername][i]),
-        np.min( [plot.unv(dl[ordername][k]) for k in scales]) - plot.unv(dl[ordername][i])
+        np.max([unv(dl[ordername][k]) for k in scales]) - unv(dl[ordername][i]),
+        np.min([unv(dl[ordername][k]) for k in scales]) - unv(dl[ordername][i]),
     )
 
-def scale_error(li, dl, ordername="LO",n_jobs=None):
+
+def scale_error(li, dl, ordername="LO", n_jobs=None):
     """
     Computes seven-point scale uncertainties from the results where the renormalization and factorization scales are varied by factors of 2 and  relative factors of four are excluded (cf. :meth:`seven_point_scan`).
 
     Args:
         li (:obj:`list` of :class:`Input`): Input list.
         dl (:obj:`dict`): :class:`Result` dictionary with lists per entry.
 
     Returns:
         :obj:`dict`: Modified `dl` with new `ordername_{SCALE,SCALE_ERRPLUS,SCALE_ERRMINUS}` entries.
             - `ordername_SCALE` contains a symmetrized :mod:`uncertainties` object.
     """
     global required_numerical_uncertainty_factor
     example = li[0]
     members = [
-        attr for attr in dir(example)
+        attr
+        for attr in dir(example)
         if not callable(getattr(example, attr)) and not attr.startswith("__")
     ]
     dl[ordername + "_SCALE"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_SCALE_ERRPLUS"] = np.array([None] * len(dl["pdfset_nlo"]))
-    dl[ordername + "_SCALE_ERRMINUS"] = np.array([None] *
-                                                 len(dl["pdfset_nlo"]))
-
+    dl[ordername + "_SCALE_ERRMINUS"] = np.array([None] * len(dl["pdfset_nlo"]))
 
-    args = [{
-        "members": members,
-        "i": i,
-        "dl": dl,
-        "ordername": ordername,
-    } for i in range(len(dl["pdfset_nlo"])) if dl["pdfset_nlo"][i] == 0
-            and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0]
-    ret = tpqdm(args,
-                _scale_error_single,
-                n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                argument_type='kwargs',
-                desc="Scale uncertainty @ " + ordername)
-    for i,errplus,errminus in ret:
+    args = [
+        {
+            "members": members,
+            "i": i,
+            "dl": dl,
+            "ordername": ordername,
+        }
+        for i in range(len(dl["pdfset_nlo"]))
+        if dl["pdfset_nlo"][i] == 0 and dl["mu_f"][i] == 1.0 and dl["mu_r"][i] == 1.0
+    ]
+    ret = tpqdm(
+        args,
+        _scale_error_single,
+        n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+        argument_type="kwargs",
+        desc="Scale uncertainty @ " + ordername,
+    )
+    for i, errplus, errminus in ret:
         # lo_unc = pdfset.uncertainty(
-        #    [plot.unv(dl["LO"][k]) for k in pdfs], -1)
+        #    [unv(dl["LO"][k]) for k in pdfs], -1)
         dl.loc[i, ordername + "_SCALE_ERRPLUS"] = errplus
         dl.loc[i, ordername + "_SCALE_ERRMINUS"] = errminus
-        if (plot.usd(dl[ordername][i]) *
-                required_numerical_uncertainty_factor >
-                dl[ordername + "_SCALE_ERRPLUS"][i]-dl[ordername + "_SCALE_ERRMINUS"][i]
-                ):
-            rel = plot.unv(dl[ordername][i])
+        if (
+            usd(dl[ordername][i]) * required_numerical_uncertainty_factor
+            > dl[ordername + "_SCALE_ERRPLUS"][i] - dl[ordername + "_SCALE_ERRMINUS"][i]
+        ):
+            rel = unv(dl[ordername][i])
             warnings.warn(
-                "too bad numerical precision vs scale @ num:" + ordername +
-                " " + str(plot.usd(dl[ordername][i]) / rel * 100.) +
-                "% vs scale:" +
-                str(dl[ordername + "_SCALE_ERRPLUS"][i] / rel * 100.) +
-                "% to " +
-                str(dl[ordername + "_SCALE_ERRMINUS"][i] / rel * 100.) +
-                "%", RuntimeWarning)
+                "too bad numerical precision vs scale @ num:"
+                + ordername
+                + " "
+                + str(usd(dl[ordername][i]) / rel * 100.0)
+                + "% vs scale:"
+                + str(dl[ordername + "_SCALE_ERRPLUS"][i] / rel * 100.0)
+                + "% to "
+                + str(dl[ordername + "_SCALE_ERRMINUS"][i] / rel * 100.0)
+                + "%",
+                RuntimeWarning,
+            )
 
     mask = dl[ordername + "_SCALE_ERRPLUS"].notnull()
-    dl.loc[mask, ordername + "_SCALE"] = unumpy.uarray(
-        plot.unv(dl[ordername][mask]) +
-        dl[ordername + "_SCALE_ERRPLUS"][mask] / 2. +
-        dl[ordername + "_SCALE_ERRMINUS"][mask] / 2.,
-        (+dl[ordername + "_SCALE_ERRPLUS"][mask] -
-         dl[ordername + "_SCALE_ERRMINUS"][mask]) / 2.)
+    dl.loc[mask, ordername + "_SCALE"] = unp.uarray(
+        unv(dl[ordername][mask])
+        + dl[ordername + "_SCALE_ERRPLUS"][mask] / 2.0
+        + dl[ordername + "_SCALE_ERRMINUS"][mask] / 2.0,
+        (
+            +dl[ordername + "_SCALE_ERRPLUS"][mask]
+            - dl[ordername + "_SCALE_ERRMINUS"][mask]
+        )
+        / 2.0,
+    )
 
     return dl
 
 
 def combine_errors(dl, ordernames=None):
     """
     Just like `combine_error` but over a list of ordernames.
@@ -332,23 +345,24 @@
     """
     dl[ordername + "_NOERR"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_ERRPLUS"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_ERRMINUS"] = np.array([None] * len(dl["pdfset_nlo"]))
     dl[ordername + "_COMBINED"] = np.array([None] * len(dl["pdfset_nlo"]))
 
     mask = dl[ordername + "_PDF_CENTRAL"].notnull()
-    dl.loc[mask, ordername + "_NOERR"] = plot.unv(dl[ordername +
-                                                     ""][mask]).astype(float)
+    dl.loc[mask, ordername + "_NOERR"] = unv(dl[ordername + ""][mask]).astype(float)
     dl.loc[mask, ordername + "_ERRPLUS"] = np.sqrt(
-        dl[ordername + "_PDF_ERRPLUS"][mask].astype(float)**2 +
-        dl[ordername + "_SCALE_ERRPLUS"][mask].astype(float)**2)
+        dl[ordername + "_PDF_ERRPLUS"][mask].astype(float) ** 2
+        + dl[ordername + "_SCALE_ERRPLUS"][mask].astype(float) ** 2
+    )
     dl.loc[mask, ordername + "_ERRMINUS"] = -np.sqrt(
-        dl[ordername + "_PDF_ERRMINUS"][mask].astype(float)**2 +
-        dl[ordername + "_SCALE_ERRMINUS"][mask].astype(float)**2)
-    dl.loc[mask, ordername + "_COMBINED"] = unumpy.uarray(
-        plot.unv(dl[ordername + ""][mask]) +
-        dl[ordername + "_ERRPLUS"][mask] / 2. +
-        dl[ordername + "_ERRMINUS"][mask] / 2.,
-        (+dl[ordername + "_ERRPLUS"][mask] - dl[ordername + "_ERRMINUS"][mask])
-        / 2.)
+        dl[ordername + "_PDF_ERRMINUS"][mask].astype(float) ** 2
+        + dl[ordername + "_SCALE_ERRMINUS"][mask].astype(float) ** 2
+    )
+    dl.loc[mask, ordername + "_COMBINED"] = unp.uarray(
+        unv(dl[ordername + ""][mask])
+        + dl[ordername + "_ERRPLUS"][mask] / 2.0
+        + dl[ordername + "_ERRMINUS"][mask] / 2.0,
+        (+dl[ordername + "_ERRPLUS"][mask] - dl[ordername + "_ERRMINUS"][mask]) / 2.0,
+    )
 
     return dl
```

### Comparing `hepi-0.2.8/hepi/resummino/plot_template.in` & `hepi-0.2.9/hepi/run/resummino/plot_template.in`

 * *Files identical despite different names*

### Comparing `hepi-0.2.8/hepi/resummino/result.py` & `hepi-0.2.9/hepi/run/resummino/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import os
+import pkgutil
+import re
+import shutil
 import warnings
+from string import Template
+
+from uncertainties import ufloat_fromstr
+
 from hepi.input import Order
+
 from .. import Input, Result, get_output_dir
-import re
-from uncertainties import ufloat_fromstr
-from string import Template
-import pkgutil
-import os
-import shutil
 
 
 class ResumminoResult(Result):
     """
     Resummino Result Data.
 
     Attributes:
@@ -19,16 +22,17 @@
         P_PLUS_K (double): collineare remainders P+K NLO result.
         RNLOG (double): real NLO gluon result.
         RNLOQ (double): real NLO quark result.
         VNLO_PLUS_P_PLUS_K (double): VNLO+P+K result.
         RNLO_PLUS_VNLO_PLUS_P_PLUS_K (double): RNLO+VNLO+P+K result.
     """
 
-    def __init__(self, lo, nlo, nlo_plus_nll, annlo_plus_nnll, vnlo, p_plus_k,
-                 rnlog, rnloq):
+    def __init__(
+        self, lo, nlo, nlo_plus_nll, annlo_plus_nnll, vnlo, p_plus_k, rnlog, rnloq
+    ):
         """
         Sets given and computes dependent ``Attributes``.
 
         Args:
             lo (:obj:`double`): corresponds to :attr:`LO`.
             nlo (:obj:`double`): corresponds to :attr:`NLO`.
             nlo_plus_nll (:obj:`double`): corresponds to :attr:`NLO_PLUS_NLL`.
@@ -52,47 +56,64 @@
             self.RNLO = None
         if not (self.RNLO is None or self.VNLO_PLUS_P_PLUS_K is None):
             self.RNLO_PLUS_VNLO_PLUS_P_PLUS_K = self.RNLO + self.VNLO_PLUS_P_PLUS_K
         else:
             self.RNLO_PLUS_VNLO_PLUS_P_PLUS_K = None
 
 
-def is_valid(file: str, p: Input, d,**kwargs) -> bool:
+def is_valid(file: str, p: Input, d, **kwargs) -> bool:
     """
     Verifies that an file is a complete output.
 
     Args:
         file (str): File path to be parsed.
         p (:class:`hepi.Input`): Onput parameters.
         d (:obj:`dict`): Param dictionary.
 
     Returns:
         bool : True if `file` could be parsed.
     """
     order = p.order
-    data = pkgutil.get_data(__name__, "plot_template.in").decode('utf-8')
+    data = pkgutil.get_data(__name__, "plot_template.in").decode("utf-8")
     src = Template(data)
     result = src.substitute(d)
-    sname = d['slha']
-    with open(file, mode='r') as f:
-        with open(get_output_dir() + sname, 'r') as sf:
-            if not kwargs['ignore_error'] and not f.read().startswith(result + "\n\n" + sf.read()):
+    sname = d["slha"]
+    with open(file, mode="r") as f:
+        with open(get_output_dir() + sname, "r") as sf:
+            if not kwargs["ignore_error"] and not f.read().startswith(
+                result + "\n\n" + sf.read()
+            ):
                 warnings.warn(
-                    "Possible hash collision in " + file + " -> moved to " +
-                    file + ".old", RuntimeWarning)
+                    "Possible hash collision in "
+                    + file
+                    + " -> moved to "
+                    + file
+                    + ".old",
+                    RuntimeWarning,
+                )
                 shutil.move(file, file + ".old")
                 return False
     res = parse_single(file)
     if res.LO is not None and order is Order.LO:
         return True
     if res.LO is not None and res.NLO is not None and order is Order.NLO:
         return True
-    if res.LO is not None and res.NLO is not None and res.NLO_PLUS_NLL is not None and order is Order.NLO_PLUS_NLL:
+    if (
+        res.LO is not None
+        and res.NLO is not None
+        and res.NLO_PLUS_NLL is not None
+        and order is Order.NLO_PLUS_NLL
+    ):
         return True
-    if res.LO is not None and res.NLO is not None and res.aNNLO_PLUS_NNLL is not None and order is Order.aNNLO_PLUS_NNLL:
+    if (
+        res.LO is not None
+        and res.NLO is not None
+        and res.aNNLO_PLUS_NNLL is not None
+        and order is Order.aNNLO_PLUS_NNLL
+    ):
         return True
     print("RESTART", res.LO, res.NLO, res.NLO_PLUS_NLL, file)
     return False
 
 
 def parse_single(file: str) -> ResumminoResult:
     """
@@ -102,23 +123,23 @@
         file (str): File path to be parsed.
 
     Returns:
         :class:`ResumminoResult` : If a value is not found in the file None is used.
 
     """
     # TODO generalize units like RS
-    lo_pattern = re.compile(r'^LO = \((.*)\) pb')
-    nlo_pattern = re.compile(r'^NLO = \((.*)\) pb')
-    nll_pattern = re.compile(r'^NLO\+NLL = \((.*)\) pb')
-    nnll_pattern = re.compile(r'^aNNLO\+NNLL = \((.*)\) pb')
-
-    vnlo_pattern = re.compile(r'^vNLO = \((.*)\) pb')
-    ppk_pattern = re.compile(r'^P\+K = \((.*)\) pb')
-    rnlog_pattern = re.compile(r'^rNLOg = \((.*)\) pb')
-    rnloq_pattern = re.compile(r'^rNLOq = \((.*)\) pb')
+    lo_pattern = re.compile(r"^LO = \((.*)\) pb")
+    nlo_pattern = re.compile(r"^NLO = \((.*)\) pb")
+    nll_pattern = re.compile(r"^NLO\+NLL = \((.*)\) pb")
+    nnll_pattern = re.compile(r"^aNNLO\+NNLL = \((.*)\) pb")
+
+    vnlo_pattern = re.compile(r"^vNLO = \((.*)\) pb")
+    ppk_pattern = re.compile(r"^P\+K = \((.*)\) pb")
+    rnlog_pattern = re.compile(r"^rNLOg = \((.*)\) pb")
+    rnloq_pattern = re.compile(r"^rNLOq = \((.*)\) pb")
 
     lo_result = None
     nlo_result = None
     nll_result = None
     nnll_result = None
 
     vnlo_result = None
@@ -143,23 +164,29 @@
             if tmp is not None:
                 vnlo_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
             tmp = ppk_pattern.search(line)
             if tmp is not None:
                 ppk_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
             tmp = rnlog_pattern.search(line)
             if tmp is not None:
-                rnlog_result = ufloat_fromstr(
-                    tmp.group(1).replace("+-", "+/-"))
+                rnlog_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
             tmp = rnloq_pattern.search(line)
             if tmp is not None:
-                rnloq_result = ufloat_fromstr(
-                    tmp.group(1).replace("+-", "+/-"))
+                rnloq_result = ufloat_fromstr(tmp.group(1).replace("+-", "+/-"))
     if lo_result is not None and lo_result < 0:
         warnings.warn("LO < 0")
     if nlo_result is not None and nlo_result < 0:
         warnings.warn("NLO < 0")
     if nll_result is not None and nll_result < 0:
         warnings.warn("NLL < 0")
     if nnll_result is not None and nnll_result < 0:
         warnings.warn("NNLL < 0")
-    return ResumminoResult(lo_result, nlo_result, nll_result, nnll_result,
-                           vnlo_result, ppk_result, rnlog_result, rnloq_result)
+    return ResumminoResult(
+        lo_result,
+        nlo_result,
+        nll_result,
+        nnll_result,
+        vnlo_result,
+        ppk_result,
+        rnlog_result,
+        rnloq_result,
+    )
```

### Comparing `hepi-0.2.8/hepi/resummino/run.py` & `hepi-0.2.9/hepi/run/resummino/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 """Runs Resummino"""
-from typing import List
-from string import Template
+import os
+import os.path
+import pkgutil
+import stat
 import warnings
+from string import Template
+from typing import List
+
 from hepi.input import Order
 from hepi.results import Result
-from hepi.run import RunParam, Runner
-import pkgutil
+from hepi.run import Runner, RunParam
 
 from .. import Input
-import os.path
 from .result import is_valid, parse_single
-import os
-import stat
 
 
 class ResumminoRunner(Runner):
-
     def orders(self) -> List[Order]:
         return [Order.LO, Order.NLO, Order.NLO_PLUS_NLL, Order.aNNLO_PLUS_NNLL]
 
     def get_version(self) -> str:
         p = os.path.expanduser(self.get_path())
         ret = self._sub_run([p, "--version"])
         return ret.split("\n")[-2]
 
     def _check_path(self) -> bool:
-        if os.path.exists(
-                os.path.expanduser(self.get_path() + "/build/bin/resummino")):
+        if os.path.exists(os.path.expanduser(self.get_path() + "/build/bin/resummino")):
             self.set_path(self.get_path() + "/build/bin/resummino")
             return True
-        if os.path.exists(
-                os.path.expanduser(self.get_path() + "/bin/resummino")):
+        if os.path.exists(os.path.expanduser(self.get_path() + "/bin/resummino")):
             self.set_path(self.get_path() + "/bin/resummino")
             return True
         if self.get_path().endswith("resummino"):
             return True
         return False
 
     def _check_input(self, p: Input, **kwargs) -> bool:
 
         if p.order == Order.aNNLO_PLUS_NNLL and (
-            (p.has_gluino() and p.has_weakino()) or
-            (p.has_squark() and p.has_weakino())):
-            warnings.warn(
-                "Resummino does not support stong-weak mixed aNNLO+NNLL.")
+            (p.has_gluino() and p.has_weakino()) or (p.has_squark() and p.has_weakino())
+        ):
+            warnings.warn("Resummino does not support stong-weak mixed aNNLO+NNLL.")
             return False
         return True
 
     def _is_valid(self, file: str, p: Input, d, **kwargs) -> bool:
         if not super()._is_valid(file, p, d):
             return False
         return is_valid(file, p, d, **kwargs)
 
     def _parse_file(self, file: str) -> Result:
         return parse_single(file)
 
     def _prepare(self, p: Input, **kwargs) -> RunParam:
         rp = super()._prepare(p, **kwargs)
         if not rp.skip:
-            data = pkgutil.get_data(__name__,
-                                    "plot_template.in").decode('utf-8')
+            data = pkgutil.get_data(__name__, "plot_template.in").decode("utf-8")
             flags = ""
             if p.order == Order.LO:
                 flags = flags + "--lo"
             elif p.order == Order.NLO:
                 flags = flags + "--nlo"
             elif p.order == Order.NLO_PLUS_NLL:
                 flags = flags + "--nll"
@@ -74,28 +70,28 @@
                     "Order not supported by resummino. Must be one of LO/NLO/NLO+NLL/aNNLO+NNLL."
                 )
 
             src = Template(data)
             result = src.substitute(p.__dict__)
             od = self.get_output_dir()
             open(od + rp.name + ".in", "w").write(result)
-            open(od + rp.name + ".sh",
-                 "w").write("#!/bin/sh\n" + get_path() + ' {} {} >> {}'.format(
-                     od + rp.name + ".in", flags,
-                     od + rp.name + ".out"))
+            open(od + rp.name + ".sh", "w").write(
+                "#!/bin/sh\n"
+                + get_path()
+                + " {} {} >> {}".format(
+                    od + rp.name + ".in", flags, od + rp.name + ".out"
+                )
+            )
             st = os.stat(od + rp.name + ".sh")
-            os.chmod(od + rp.name + ".sh",
-                     st.st_mode | stat.S_IEXEC)
-            open(od + rp.name + ".out",
-                 "w").write(result + "\n\n")
+            os.chmod(od + rp.name + ".sh", st.st_mode | stat.S_IEXEC)
+            open(od + rp.name + ".out", "w").write(result + "\n\n")
 
             sname = p.slha
-            with open(od + sname, 'r') as f:
-                open(od + rp.name + ".out",
-                     "a").write(f.read() + "\n\n")
+            with open(od + sname, "r") as f:
+                open(od + rp.name + ".out", "a").write(f.read() + "\n\n")
         return rp
 
 
 # Legacy
 default_resummino_runner = ResumminoRunner("~/resummino/")
 """Default Resummino Runner to provide backward compatibility"""
 run = default_resummino_runner.run
```

### Comparing `hepi-0.2.8/hepi/run.py` & `hepi-0.2.9/hepi/run/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-from concurrent.futures import ThreadPoolExecutor
-from logging import warning
+import multiprocessing as mp
 import os
 import subprocess
-from subprocess import Popen, PIPE
-from typing import List
+import time
 import warnings
+from concurrent.futures import ThreadPoolExecutor
+from logging import warning
+from subprocess import PIPE, Popen
+from typing import List
 
 import numpy as np
+import tqdm
+from pqdm.processes import pqdm as ppqdm
+from pqdm.threads import pqdm as tpqdm
+
 from hepi.input import Input, Order, get_input_dir, get_output_dir, get_pre
 from hepi.results import Result
 from hepi.util import DL2DF, LD2DL, DictData, namehash
-from smpl.parallel import par
-import time
-import tqdm
-from pqdm.threads import pqdm as tpqdm
-from pqdm.processes import pqdm as ppqdm
-import multiprocessing as mp
-#from pqdm.processes import pqdm
+
+# from pqdm.processes import pqdm
+
 
 class RunParam(DictData):
     """Abstract class that is similar to a dictionary but with fixed keys."""
 
-    def __init__(self,
-                 skip: bool = False,
-                 in_file: str = None,
-                 out_file: str = None,
-                 execute: str = None,
-                 name: str = None):
+    def __init__(
+        self,
+        skip: bool = False,
+        in_file: str = None,
+        out_file: str = None,
+        execute: str = None,
+        name: str = None,
+    ):
         self.name = name
         self.skip = skip
         self.in_file = in_file
         self.out_file = out_file
         self.execute = execute
 
 
 class Runner:
-
-    def __init__(self,
-                 path: str,
-                 in_dir: str = None,
-                 out_dir: str = None,
-                 pre=None):
+    def __init__(self, path: str, in_dir: str = None, out_dir: str = None, pre=None):
         self.path = path
         if in_dir is None:
             self.in_dir = get_input_dir()
         else:
             self.in_dir = in_dir
         if out_dir is None:
             self.out_dir = get_output_dir()
@@ -75,197 +74,214 @@
         else:
             return output.decode()
 
     def _check_path(self) -> bool:
         """Checks if the passed path is valid."""
         return True
 
-    def _prepare(self, p: Input, skip=False, assume_valid = False, **kwargs) -> RunParam:
+    def _prepare(self, p: Input, skip=False, assume_valid=False, **kwargs) -> RunParam:
         skip_ = skip
-        #p.runner = str(type(self).__name__) + "-" + self.get_version()
+        # p.runner = str(type(self).__name__) + "-" + self.get_version()
 
         d = p.__dict__
-        #d["runner"] = str(type(self).__name__) + "-" + self.get_version(
-        #)  # TODO re add version, but removed for reusable hashing!
-        name = namehash("_".join("".join(str(_[0]) + "_" + str(_[1]))
-                                 for _ in d.items()).replace("/", "-"))
-        #print(name)
+        # d["runner"] = str(type(self).__name__) + "-" + self.get_version(
+        # )  # TODO re add version, but removed for reusable hashing!
+        name = namehash(
+            "_".join("".join(str(_[0]) + "_" + str(_[1])) for _ in d.items()).replace(
+                "/", "-"
+            )
+        )
+        # print(name)
         skip = False
-        if skip_ and os.path.isfile(self.get_output_dir() + name + ".out") and (assume_valid or self._is_valid(
-                                        self.get_output_dir() + name + ".out",
-                                        p,
-                                        d,
-                                        skip=skip_,
-                                        **kwargs)):
-            #print(".", end='')
+        if (
+            skip_
+            and os.path.isfile(self.get_output_dir() + name + ".out")
+            and (
+                assume_valid
+                or self._is_valid(
+                    self.get_output_dir() + name + ".out", p, d, skip=skip_, **kwargs
+                )
+            )
+        ):
+            # print(".", end='')
             skip = True
         else:
-            #print(str(self.get_output_dir()  + name + ".out")) 
-            #print('|', end='')
+            # print(str(self.get_output_dir()  + name + ".out"))
+            # print('|', end='')
             skip = False
-        return RunParam(execute=self.get_output_dir() + name + ".sh",
-                        in_file=self.get_output_dir() + name + ".in",
-                        out_file=self.get_output_dir() + name + ".out",
-                        skip=skip,
-                        name=name)
+        return RunParam(
+            execute=self.get_output_dir() + name + ".sh",
+            in_file=self.get_output_dir() + name + ".in",
+            out_file=self.get_output_dir() + name + ".out",
+            skip=skip,
+            name=name,
+        )
 
     def _check_input(self, param: Input, **kwargs) -> bool:
         if param.order not in self.orders():
-            warnings.warn("Order " + str(param.order) + " not supported in " +
-                          type(self).__name__)
+            warnings.warn(
+                "Order " + str(param.order) + " not supported in " + type(self).__name__
+            )
             return False
         return True
 
-    def _prepare_all(self,
-                     params: List[Input],
-                     skip=True,
-                     n_jobs = None,
-                     **kwargs) -> List[RunParam]:
+    def _prepare_all(
+        self, params: List[Input], skip=True, n_jobs=None, **kwargs
+    ) -> List[RunParam]:
         """
         Prepares all parameters for execution.
 
         Args:
             params (List[:class:`hepi.Input`]): List of input parameters.
             skip (bool, optional): If True, the runner will check if the output file already exists and skip the execution if it does. Defaults to True.
             n_jobs (int): Number of parallel jobs. If None, use all available cores.
         """
         ret = []
 
-        #ret = my_parallel(self._check_input,params,desc="Checking input")
-        ret = tpqdm(params,
-                    self._check_input,
-                    n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                    desc="Checking input")
+        # ret = my_parallel(self._check_input,params,desc="Checking input")
+        ret = tpqdm(
+            params,
+            self._check_input,
+            n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+            desc="Checking input",
+        )
         if not np.alltrue(ret):
             warnings.warn("Check input failed.")
             return []
-        #ret = my_parallel(
+        # ret = my_parallel(
         #    lambda p: self._prepare(p, skip=skip, **kwargs),
         #    params,
         #    #n_jobs=mp.cpu_count(),
         #    desc="Preparing")
         runnername = str(type(self).__name__) + "-" + self.get_version()
-        for p in params: p.runner = runnername
-        args = [{'p': p, 'skip': skip, **kwargs} for p in params]
-        ret = ppqdm(args,
-                    self._prepare,
-                    n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                    argument_type='kwargs',
-                    desc="Preparing")
+        for p in params:
+            p.runner = runnername
+        args = [{"p": p, "skip": skip, **kwargs} for p in params]
+        ret = ppqdm(
+            args,
+            self._prepare,
+            n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+            argument_type="kwargs",
+            desc="Preparing",
+        )
         skipped = 0
         not_skipped = 0
         for r in ret:
             if r.skip:
                 skipped += 1
             else:
                 not_skipped += 1
         print("Skipped: " + str(skipped) + " Not skipped: " + str(not_skipped))
-        #for p in params:
+        # for p in params:
         #    if not self._check_input(p):
         #        warnings.warn("Check input failed.")
         #        return []
         #    ret.append(self._prepare(p, skip=skip, **kwargs))
         return ret
 
-    def run(self,
-            params: List[Input],
-            skip=True,
-            parse=True,
-            parallel=True,
-            sleep=0,
-            run=True,
-            ignore_error=False,
-            n_jobs = None,
-            **kwargs):
-        """
-		Run the passed list of parameters.
-
-		Args:
-		    params (:obj:`list` of :class:`hepi.Input`): All parameters that should be executed/queued.
-		    skip (bool): True means stored runs will be skipped. Else the are overwritten.
-		    parse (bool): Parse the results. 
-		        This is not the prefered cluster/parallel mode, as there the function only queues the job.
-		    parallel (bool): Run jobs in parallel.
-		    sleep (int): Sleep seconds after starting job.
-            run (bool): Actually start/queue runner.
-            ignore_error (bool): Continue instead of raising Exceptions. Also ignores hash collisions.
-            n_jobs (int): Number of parallel jobs. If None, use all available cores.
+    def run(
+        self,
+        params: List[Input],
+        skip=True,
+        parse=True,
+        parallel=True,
+        sleep=0,
+        run=True,
+        ignore_error=False,
+        n_jobs=None,
+        **kwargs
+    ):
+        """
+            Run the passed list of parameters.
+
+            Args:
+                params (:obj:`list` of :class:`hepi.Input`): All parameters that should be executed/queued.
+                skip (bool): True means stored runs will be skipped. Else the are overwritten.
+                parse (bool): Parse the results.
+                    This is not the prefered cluster/parallel mode, as there the function only queues the job.
+                parallel (bool): Run jobs in parallel.
+                sleep (int): Sleep seconds after starting job.
+        run (bool): Actually start/queue runner.
+        ignore_error (bool): Continue instead of raising Exceptions. Also ignores hash collisions.
+        n_jobs (int): Number of parallel jobs. If None, use all available cores.
 
-		Returns:
-		    :obj:`pd.DataFrame` : combined dataframe of results and parameters. The dataframe is empty if `parse` is set to False.
+            Returns:
+                :obj:`pd.DataFrame` : combined dataframe of results and parameters. The dataframe is empty if `parse` is set to False.
 
-		"""
+        """
         if not self._check_path():
             warnings.warn("The path is not valid for " + self.get_name())
             if not ignore_error:
-                raise RuntimeError("The path is not valid for " +
-                                   self.get_name())
-        rps = self._prepare_all(params,
-                                parse=parse,
-                                skip=skip,
-                                ignore_error=ignore_error,
-                                n_jobs=n_jobs,
-                                **kwargs)
-        #print("= " + str(len(params)) + " jobs")
+                raise RuntimeError("The path is not valid for " + self.get_name())
+        rps = self._prepare_all(
+            params,
+            parse=parse,
+            skip=skip,
+            ignore_error=ignore_error,
+            n_jobs=n_jobs,
+            **kwargs
+        )
+        # print("= " + str(len(params)) + " jobs")
         if sleep is None:
             sleep = 0 if parse else 5
         if run:
-            self._run(rps,
-                      wait=parse,
-                      parallel=parallel,
-                      sleep=sleep,
-                      n_jobs = n_jobs,
-                      **kwargs)
+            self._run(
+                rps, wait=parse, parallel=parallel, sleep=sleep, n_jobs=n_jobs, **kwargs
+            )
         if parse:
             outs = LD2DL(rps)["out_file"]
-            results = self.parse(outs,n_jobs=n_jobs)
+            results = self.parse(outs, n_jobs=n_jobs)
             rdl = LD2DL(results)
             pdl = LD2DL(params)
             return DL2DF({**rdl, **pdl})
         return DL2DF({})
 
-    def _run(self,
-             rps: List[RunParam],
-             wait=True,
-             parallel=True,
-             sleep=0,
-             n_jobs = None,
-             **kwargs):
-        """
-		Runs Runner per :class:`RunParams`.
-	
-		Args:
-		    rps (:obj:`list` of :class:`RunParams`): Extended run parameters.
-		    bar (bool): Enable info bar.
-		    wait (bool): Wait for parallel runs to finish.
-		    sleep (int): Sleep seconds after starting subprocess.
-		    parallel (bool): Run jobs in parallel.
-            n_jobs (int): Number of parallel jobs. If None, use all available cores.
-	
-		Returns:
-		    :obj:`list` of int: return codes from jobs if `no_parse` is False.
-		"""
+    def _run(
+        self,
+        rps: List[RunParam],
+        wait=True,
+        parallel=True,
+        sleep=0,
+        n_jobs=None,
+        **kwargs
+    ):
+        """
+            Runs Runner per :class:`RunParams`.
+
+            Args:
+                rps (:obj:`list` of :class:`RunParams`): Extended run parameters.
+                bar (bool): Enable info bar.
+                wait (bool): Wait for parallel runs to finish.
+                sleep (int): Sleep seconds after starting subprocess.
+                parallel (bool): Run jobs in parallel.
+        n_jobs (int): Number of parallel jobs. If None, use all available cores.
+
+            Returns:
+                :obj:`list` of int: return codes from jobs if `no_parse` is False.
+        """
         # get cluster or niceness prefix
         template = self.get_pre() + " " + "{}"
 
         # Run commands in parallel
         processes = []
         cmds = []
 
         for rp in rps:
             if not rp.skip:
                 command = template.format(rp.execute)
                 cmds.append(command)
 
         if wait and parallel:
-            return tpqdm(cmds,
-                  lambda c: subprocess.call(c,shell=True),
-                  n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                  desc="Running")
-            #with ThreadPoolExecutor(max_workers=n_jobs if n_jobs is not None else mp.cpu_count()) as executor:
+            return tpqdm(
+                cmds,
+                lambda c: subprocess.call(c, shell=True),
+                n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+                desc="Running",
+            )
+            # with ThreadPoolExecutor(max_workers=n_jobs if n_jobs is not None else mp.cpu_count()) as executor:
             #    for cmd in cmds:
             #        processes.append(executor.submit(subprocess.call, cmd, shell=True))
             #        time.sleep(sleep)
             #    return [p.result() for p in processes]
 
         for command in cmds:
             command = template.format(rp.execute)
@@ -280,144 +296,146 @@
             # Collect statuses
             output = [p.wait() for p in processes]
             return output
         return []
 
     def _is_valid(self, file: str, p: Input, d, **kwargs) -> bool:
         """
-		Verifies that a file is a complete output.
-	
-		Args:
-		    file (str): File path to be parsed.
-		    p (:class:`hepi.Input`): Onput parameters.
-		    d (:obj:`dict`): Param dictionary.
-	
-		Returns:
-		    bool : True if `file` could be parsed.
-		"""
+        Verifies that a file is a complete output.
+
+        Args:
+            file (str): File path to be parsed.
+            p (:class:`hepi.Input`): Onput parameters.
+            d (:obj:`dict`): Param dictionary.
+
+        Returns:
+            bool : True if `file` could be parsed.
+        """
         res = self._parse_file(file)
         if res.LO is None and p.order is Order.LO:
             return False
         if res.NLO is None and p.order is Order.NLO:
             return False
         if res.NLO_PLUS_NLL is None and p.order is Order.NLO_PLUS_NLL:
             return False
         if res.aNNLO_PLUS_NNLL is None and p.order is Order.aNNLO_PLUS_NNLL:
             return False
         return True
 
-    def parse(self, outputs: List[str],n_jobs=None) -> List[Result]:
+    def parse(self, outputs: List[str], n_jobs=None) -> List[Result]:
+        """
+            Parses Resummino output files and returns List of Results.
+
+            Args:
+                outputs (:obj:`list` of `str`): List of the filenames to be parsed.
+        n_jobs (int): Number of parallel jobs. If None, use all available cores.
+
+            Returns:
+                :obj:`list` of :class:`hepi.resummino.result.ResumminoResult`
+
         """
-		Parses Resummino output files and returns List of Results.
-	
-		Args:
-		    outputs (:obj:`list` of `str`): List of the filenames to be parsed.
-            n_jobs (int): Number of parallel jobs. If None, use all available cores.
-	
-		Returns:
-		    :obj:`list` of :class:`hepi.resummino.result.ResumminoResult`
-	
-		"""
         rsl = []
-        #for r in parallel(self._parse_file, outputs):
+        # for r in parallel(self._parse_file, outputs):
         #    rsl.append(r)
 
         # parallelized opens to many files at times
-        #rsl = my_parallel(self._parse_file, outputs, desc="Parsing")
-        rsl = tpqdm(outputs,
-                   self._parse_file,
-                   n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
-                   desc="Parsing")
+        # rsl = my_parallel(self._parse_file, outputs, desc="Parsing")
+        rsl = tpqdm(
+            outputs,
+            self._parse_file,
+            n_jobs=n_jobs if n_jobs is not None else mp.cpu_count(),
+            desc="Parsing",
+        )
         return rsl
-        #for o in tqdm.tqdm(outputs):
+        # for o in tqdm.tqdm(outputs):
         #    rsl.append(self._parse_file(o))
-        #return rsl
+        # return rsl
 
     def _parse_file(self, file: str) -> Result:
         """
-		Extracts results from an output file.
+        Extracts results from an output file.
 
-		Args:
-		    file (str): File path to be parsed.
+        Args:
+            file (str): File path to be parsed.
 
-		Returns:
-		    :class:`Result` : If a value is not found in the file None is used.
+        Returns:
+            :class:`Result` : If a value is not found in the file None is used.
 
-		"""
+        """
         return None
 
     def get_path(self) -> str:
         """
-		Get the Runner path.
+        Get the Runner path.
 
-		Returns:
-		    str: current Runner path.
-		"""
+        Returns:
+            str: current Runner path.
+        """
         return self.path
 
     def get_input_dir(self) -> str:
         """
-		Get the input directory.
+        Get the input directory.
 
-		Returns:
-		    str: :attr:`in_dir`
-		"""
+        Returns:
+            str: :attr:`in_dir`
+        """
         return self.in_dir
 
     def get_output_dir(self) -> str:
         """
-		Get the input directory.
+        Get the input directory.
 
-		Returns:
-		    str: :attr:`out_dir`
-		"""
+        Returns:
+            str: :attr:`out_dir`
+        """
         return self.out_dir
 
     def get_pre(self) -> str:
         """
-		Gets the command prefix.
+        Gets the command prefix.
 
-		Returns:
-		    str: :attr:`pre`
-		"""
+        Returns:
+            str: :attr:`pre`
+        """
         return self.pre
 
     def set_path(self, p: str):
         """
-		Set the path to the Runner folder containing the binary in './bin' or './build/bin'.
+        Set the path to the Runner folder containing the binary in './bin' or './build/bin'.
 
-		Args:
-		    p (str): new path.
-		"""
+        Args:
+            p (str): new path.
+        """
         if os.path.isdir(p):
             self.path = p + ("/" if p[-1] != "/" else "")
         self.path = p
 
     def set_input_dir(self, indir: str):
         """
-		Sets the input directory.
+        Sets the input directory.
 
-		Args:
-		    indir (str): new input directory.
-		"""
+        Args:
+            indir (str): new input directory.
+        """
         self.in_dir = indir
 
     def set_output_dir(self, outdir: str, create: bool = True):
         """
-		Sets the output directory.
+        Sets the output directory.
 
-		Args:
-		    outdir (str): new output directory.
-			create (bool): create directory if not existing.
-		"""
+        Args:
+            outdir (str): new output directory.
+                create (bool): create directory if not existing.
+        """
         if create:
             os.makedirs(outdir, exist_ok=True)
         self.out_dir = outdir
 
     def set_pre(self, ppre: str):
         """
-		Sets the command prefix.
+        Sets the command prefix.
 
-		Args:
-		    ppre (str): new command prefix.
-		"""
+        Args:
+            ppre (str): new command prefix.
+        """
         self.pre = ppre
```

### Comparing `hepi-0.2.8/hepi/spheno/run.py` & `hepi-0.2.9/hepi/run/spheno/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,61 @@
-from typing import List
-import warnings
-import subprocess
 import os
+import subprocess
+import warnings
+from typing import List
+
 from hepi.input import Input, update_slha
 from hepi.run import Runner
 
 
 class SPhenoRunner(Runner):
-
     def _check_path(self) -> bool:
         if os.path.exists(os.path.expanduser(self.get_path() + "/bin/SPheno")):
             self.set_path(self.get_path() + "/bin/SPheno")
             return True
         if self.get_path().endswith("SPheno"):
             return True
         return False
 
     def run(self, slhas: List[Input], **kwargs) -> List[Input]:
         """
         Run the passed list of parameters for SPheno.
-    
+
         Args:
             slhas (:obj:`list` of :class:`Input`): Input parameters with a SLHA file that can be processed by SPheno.
         Returns:
             :obj:`list` of :class:`Input`
         """
         if not self._check_path():
             warnings.warn("The path is not valid for " + self.get_name())
         if os.path.exists("Messages.out"):
             os.remove("Messages.out")
         for s in slhas:
             # Remove Creation time for hash-/caching
-            comm = "cp " + self.get_output_dir(
-            ) + s.slha + " spheno_tmp.in && " + get_path(
-            ) + " spheno_tmp.in && mv " + "SPheno.spc " + self.get_output_dir(
-            ) + s.slha + " && sed -i '/Created/d' " + self.get_output_dir(
-            ) + s.slha
-            proc = subprocess.Popen(comm,
-                                    shell=True,
-                                    stdout=subprocess.PIPE,
-                                    stderr=subprocess.PIPE)
+            comm = (
+                "cp "
+                + self.get_output_dir()
+                + s.slha
+                + " spheno_tmp.in && "
+                + get_path()
+                + " spheno_tmp.in && mv "
+                + "SPheno.spc "
+                + self.get_output_dir()
+                + s.slha
+                + " && sed -i '/Created/d' "
+                + self.get_output_dir()
+                + s.slha
+            )
+            proc = subprocess.Popen(
+                comm, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+            )
             proc.wait()
             update_slha(s)
         if os.path.exists("Messages.out"):
-            with open("Messages.out", 'r') as r:
+            with open("Messages.out", "r") as r:
                 t = r.read()
                 if t != "":
                     warnings.warn(r.read())
         return slhas
 
 
 # Backward compatibility
```

