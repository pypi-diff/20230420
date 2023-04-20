# Comparing `tmp/pymCADRE-1.2.4.tar.gz` & `tmp/pymCADRE-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymCADRE-1.2.4.tar", last modified: Wed Apr 19 11:40:30 2023, max compression
+gzip compressed data, was "dist/pymCADRE-1.2.5.tar", last modified: Thu Apr 20 06:13:25 2023, max compression
```

## Comparing `pymCADRE-1.2.4.tar` & `pymCADRE-1.2.5.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.359646 pymCADRE-1.2.4/
--rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 11:40:30.358168 pymCADRE-1.2.4/PKG-INFO
--rw-rw-r--   0 leonidou   (501) staff       (20)     4648 2023-04-19 09:38:15.000000 pymCADRE-1.2.4/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.342632 pymCADRE-1.2.4/pymCADRE.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)     1511 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       28 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       14 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/top_level.txt
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.339295 pymCADRE-1.2.4/pymCADRE_code/
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.343194 pymCADRE-1.2.4/pymCADRE_code/code/
--rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/__init__.py
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.346224 pymCADRE-1.2.4/pymCADRE_code/code/check/
--rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/__init__.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     5053 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/check_model_function.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3429 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/check_rxn_flux.py
--rw-rw-r--   0 leonidou   (501) staff       (20)      636 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_ex_reactions.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2066 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_organic_ex_rxns.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3035 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_required_rxns.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     1361 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/set_metabolite_bounds.py
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.348511 pymCADRE-1.2.4/pymCADRE_code/code/prune/
--rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/__init__.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3773 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_core_deadends.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3915 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_model_consistency.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     4021 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_salvage_path.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3084 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/find_inactive_rxns.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     7430 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/prune_model.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2473 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/pymcadre.py
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.352217 pymCADRE-1.2.4/pymCADRE_code/code/rank/
--rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/__init__.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2148 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_conn_evidence.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2078 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_expr_evidence.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2886 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/initialize_generic_model.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2159 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/map_gene_scores_to_rxns.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3235 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/map_high_conf_to_rxns.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3096 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/parse_gprs.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     4504 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/rank_reactions.py
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.356791 pymCADRE-1.2.4/pymCADRE_code/pre_processing/
--rw-rw-r--   0 leonidou   (501) staff       (20)      948 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/consistent_conf_scores.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     4931 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/data_preprocessing.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     2298 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/entrez_ids.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     1433 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/format_model_matlab.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     3703 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/get_conf_scores.py
--rw-rw-r--   0 leonidou   (501) staff       (20)     1151 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/ubiquity_scores.py
--rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 11:40:30.360093 pymCADRE-1.2.4/setup.cfg
--rw-rw-r--   0 leonidou   (501) staff       (20)     1311 2023-04-19 11:40:14.000000 pymCADRE-1.2.4/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.120866 pymCADRE-1.2.5/
+-rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.5/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-20 06:13:25.120285 pymCADRE-1.2.5/PKG-INFO
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4648 2023-04-19 09:38:15.000000 pymCADRE-1.2.5/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.103283 pymCADRE-1.2.5/pre_processing_scripts/
+-rw-rw-r--   0 leonidou   (501) staff       (20)      948 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/consistent_conf_scores.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4931 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/data_preprocessing.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2298 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/entrez_ids.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1433 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/format_model_matlab.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3703 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/get_conf_scores.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1151 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pre_processing_scripts/ubiquity_scores.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.097693 pymCADRE-1.2.5/pymCADRE/
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.109397 pymCADRE-1.2.5/pymCADRE/check/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     5053 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/check_model_function.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3429 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/check_rxn_flux.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)      636 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/find_ex_reactions.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2066 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/find_organic_ex_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3035 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/find_required_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1361 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/check/set_metabolite_bounds.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.115759 pymCADRE-1.2.5/pymCADRE/prune/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3773 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/check_core_deadends.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3915 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/check_model_consistency.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4021 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/check_salvage_path.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3084 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/find_inactive_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     7430 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/prune/prune_model.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.119718 pymCADRE-1.2.5/pymCADRE/rank/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2148 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/calc_conn_evidence.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2078 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/calc_expr_evidence.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2886 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/initialize_generic_model.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2159 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/map_gene_scores_to_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3235 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/map_high_conf_to_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3096 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/parse_gprs.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4504 2023-04-19 09:43:04.000000 pymCADRE-1.2.5/pymCADRE/rank/rank_reactions.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-20 06:13:25.105856 pymCADRE-1.2.5/pymCADRE.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-20 06:13:24.000000 pymCADRE-1.2.5/pymCADRE.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)     1203 2023-04-20 06:13:25.000000 pymCADRE-1.2.5/pymCADRE.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-20 06:13:24.000000 pymCADRE-1.2.5/pymCADRE.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       28 2023-04-20 06:13:24.000000 pymCADRE-1.2.5/pymCADRE.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       45 2023-04-20 06:13:24.000000 pymCADRE-1.2.5/pymCADRE.egg-info/top_level.txt
+-rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.5/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-20 06:13:25.121015 pymCADRE-1.2.5/setup.cfg
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1253 2023-04-20 06:13:03.000000 pymCADRE-1.2.5/setup.py
```

### Comparing `pymCADRE-1.2.4/LICENSE` & `pymCADRE-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/PKG-INFO` & `pymCADRE-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.4
+Version: 1.2.5
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
```

### Comparing `pymCADRE-1.2.4/README.md` & `pymCADRE-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE.egg-info/PKG-INFO` & `pymCADRE-1.2.5/pymCADRE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.4
+Version: 1.2.5
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
```

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/check_model_function.py` & `pymCADRE-1.2.5/pymCADRE/check/check_model_function.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/check_rxn_flux.py` & `pymCADRE-1.2.5/pymCADRE/check/check_rxn_flux.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/find_ex_reactions.py` & `pymCADRE-1.2.5/pymCADRE/check/find_ex_reactions.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/find_organic_ex_rxns.py` & `pymCADRE-1.2.5/pymCADRE/check/find_organic_ex_rxns.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/find_required_rxns.py` & `pymCADRE-1.2.5/pymCADRE/check/find_required_rxns.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/check/set_metabolite_bounds.py` & `pymCADRE-1.2.5/pymCADRE/check/set_metabolite_bounds.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/prune/check_core_deadends.py` & `pymCADRE-1.2.5/pymCADRE/prune/check_core_deadends.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/prune/check_model_consistency.py` & `pymCADRE-1.2.5/pymCADRE/prune/check_model_consistency.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/prune/check_salvage_path.py` & `pymCADRE-1.2.5/pymCADRE/prune/check_salvage_path.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/prune/find_inactive_rxns.py` & `pymCADRE-1.2.5/pymCADRE/prune/find_inactive_rxns.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/prune/prune_model.py` & `pymCADRE-1.2.5/pymCADRE/prune/prune_model.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_conn_evidence.py` & `pymCADRE-1.2.5/pymCADRE/rank/calc_conn_evidence.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_expr_evidence.py` & `pymCADRE-1.2.5/pymCADRE/rank/calc_expr_evidence.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/initialize_generic_model.py` & `pymCADRE-1.2.5/pymCADRE/rank/initialize_generic_model.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/map_gene_scores_to_rxns.py` & `pymCADRE-1.2.5/pymCADRE/rank/map_gene_scores_to_rxns.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/map_high_conf_to_rxns.py` & `pymCADRE-1.2.5/pymCADRE/rank/map_high_conf_to_rxns.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/parse_gprs.py` & `pymCADRE-1.2.5/pymCADRE/rank/parse_gprs.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/code/rank/rank_reactions.py` & `pymCADRE-1.2.5/pymCADRE/rank/rank_reactions.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/consistent_conf_scores.py` & `pymCADRE-1.2.5/pre_processing_scripts/consistent_conf_scores.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/data_preprocessing.py` & `pymCADRE-1.2.5/pre_processing_scripts/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/entrez_ids.py` & `pymCADRE-1.2.5/pre_processing_scripts/entrez_ids.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/format_model_matlab.py` & `pymCADRE-1.2.5/pre_processing_scripts/format_model_matlab.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/get_conf_scores.py` & `pymCADRE-1.2.5/pre_processing_scripts/get_conf_scores.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/pymCADRE_code/pre_processing/ubiquity_scores.py` & `pymCADRE-1.2.5/pre_processing_scripts/ubiquity_scores.py`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.4/setup.py` & `pymCADRE-1.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymCADRE',
-    version='1.2.4',
+    version='1.2.5',
     description='The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/pymCADRE',
     author='Nantia Leonidou',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
     keywords=['pymCADRE', 'systems biology', 'tissue-specific metabolic models'],
     #packages=find_packages(include=['pymCADRE_code']),
     #py_modules=['SBOannotator', 'main'],
     #packages=find_packages(),
-    packages=['pymCADRE_code','pymCADRE_code.code','pymCADRE_code.pre_processing',
-        'pymCADRE_code.code.check','pymCADRE_code.code.prune','pymCADRE_code.code.rank'],
+    packages=['test_dataset','pre_processing_scripts',
+        'pymCADRE.check','pymCADRE.prune','pymCADRE.rank'],
     include_package_data=True,
     install_requires=['pandas',
                       'numpy',
                       'cobra',
                       'requests']
 )
```

