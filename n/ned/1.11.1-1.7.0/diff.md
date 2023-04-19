# Comparing `tmp/ned-1.11.1.tar.gz` & `tmp/ned-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ned-1.11.1.tar", max compression
+gzip compressed data, was "ned-1.7.0.tar", max compression
```

## Comparing `ned-1.11.1.tar` & `ned-1.7.0.tar`

### file list

```diff
@@ -1,81 +1,64 @@
--rw-r--r--   0        0        0     1064 2022-10-28 21:58:46.138094 ned-1.11.1/LICENSE
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.138158 ned-1.11.1/ned/__init__.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.138226 ned-1.11.1/ned/actors/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-03 05:40:08.536543 ned-1.11.1/ned/actors/__main__.py
--rw-r--r--   0        0        0    10005 2023-04-03 05:40:08.536921 ned-1.11.1/ned/actors/candidate_generation.py
--rw-r--r--   0        0        0    16371 2023-04-03 05:40:08.537211 ned-1.11.1/ned/actors/candidate_ranking.py
--rw-r--r--   0        0        0        0 2023-04-03 05:40:08.537323 ned-1.11.1/ned/actors/dataset/__init__.py
--rw-r--r--   0        0        0     8772 2023-04-03 05:40:08.537520 ned-1.11.1/ned/actors/dataset/auto_dataset.py
--rw-r--r--   0        0        0    10215 2023-04-03 05:40:08.537709 ned-1.11.1/ned/actors/dataset/dataset.py
--rw-r--r--   0        0        0      243 2023-04-03 05:40:08.537800 ned-1.11.1/ned/actors/dataset/prelude.py
--rw-r--r--   0        0        0     4157 2023-04-03 05:40:08.537938 ned-1.11.1/ned/actors/dataset/utils.py
--rw-r--r--   0        0        0     1069 2023-04-03 05:40:08.538049 ned-1.11.1/ned/actors/db.py
--rw-r--r--   0        0        0     8641 2023-04-03 05:40:08.538259 ned-1.11.1/ned/actors/entity_recognition.py
--rw-r--r--   0        0        0    15448 2023-04-03 05:40:08.538509 ned-1.11.1/ned/actors/evaluate_helper.py
--rw-r--r--   0        0        0        0 2023-04-03 05:40:08.538623 ned-1.11.1/ned/autodata/__init__.py
--rw-r--r--   0        0        0     1159 2023-04-03 05:40:08.538742 ned-1.11.1/ned/autodata/erv1.py
--rw-r--r--   0        0        0     2262 2023-04-03 05:40:08.538879 ned-1.11.1/ned/autodata/fbhct.py
--rw-r--r--   0        0        0     2028 2023-04-03 05:40:08.539011 ned-1.11.1/ned/autodata/fbt.py
--rw-r--r--   0        0        0     1132 2023-04-03 05:40:08.539119 ned-1.11.1/ned/autodata/fcom.py
--rw-r--r--   0        0        0     1144 2023-04-03 05:40:08.539249 ned-1.11.1/ned/autodata/freg.py
--rw-r--r--   0        0        0     3143 2023-04-03 05:40:08.539419 ned-1.11.1/ned/autodata/fv1.py
--rw-r--r--   0        0        0     3480 2023-04-03 05:40:08.539564 ned-1.11.1/ned/autodata/lv1.py
--rw-r--r--   0        0        0     9355 2023-04-03 05:40:08.539722 ned-1.11.1/ned/autodata/mv1.py
--rw-r--r--   0        0        0      796 2023-04-03 05:40:08.539840 ned-1.11.1/ned/autodata/prelude.py
--rw-r--r--   0        0        0     1081 2023-04-03 05:40:08.539961 ned-1.11.1/ned/autodata/utils.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.139006 ned-1.11.1/ned/candidate_generation/__init__.py
--rw-r--r--   0        0        0     7004 2023-04-03 05:40:08.540212 ned-1.11.1/ned/candidate_generation/common.py
--rw-r--r--   0        0        0     9900 2023-04-03 05:40:08.540379 ned-1.11.1/ned/candidate_generation/localsearch.py
--rw-r--r--   0        0        0    10890 2023-04-03 05:40:08.540558 ned-1.11.1/ned/candidate_generation/mtab_wrapper.py
--rw-r--r--   0        0        0     7398 2023-04-03 05:40:08.540819 ned-1.11.1/ned/candidate_generation/oracle_semtyper.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.139169 ned-1.11.1/ned/candidate_generation/pyserini/__init__.py
--rw-r--r--   0        0        0     1375 2022-10-28 21:58:46.139248 ned-1.11.1/ned/candidate_generation/pyserini/analyzer.py
--rw-r--r--   0        0        0     1712 2022-10-28 21:58:46.139319 ned-1.11.1/ned/candidate_generation/pyserini/configuration.py
--rw-r--r--   0        0        0     3642 2023-04-03 05:40:08.541041 ned-1.11.1/ned/candidate_generation/pyserini/document.py
--rw-r--r--   0        0        0    15844 2023-04-03 05:40:08.541304 ned-1.11.1/ned/candidate_generation/pyserini/indexing.py
--rw-r--r--   0        0        0     5607 2023-04-03 05:40:08.541539 ned-1.11.1/ned/candidate_generation/pyserini/search.py
--rw-r--r--   0        0        0     4028 2023-04-03 05:40:08.541743 ned-1.11.1/ned/candidate_generation/pyserini_wrapper.py
--rw-r--r--   0        0        0    23422 2022-10-28 21:58:46.139812 ned-1.11.1/ned/candidate_generation/table_linker.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.139866 ned-1.11.1/ned/candidate_generation/table_linker_wrapper.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.139949 ned-1.11.1/ned/candidate_ranking/__init__.py
--rw-r--r--   0        0        0    13158 2022-12-15 15:16:53.773079 ned-1.11.1/ned/candidate_ranking/columnwise_model.py
--rw-r--r--   0        0        0     3484 2022-12-15 15:16:53.773922 ned-1.11.1/ned/candidate_ranking/contrastive_pairwise_model.py
--rw-r--r--   0        0        0    21381 2023-04-03 05:40:08.542052 ned-1.11.1/ned/candidate_ranking/cr_dataset.py
--rw-r--r--   0        0        0     4472 2023-04-03 05:40:08.542294 ned-1.11.1/ned/candidate_ranking/cr_method.py
--rw-r--r--   0        0        0     2850 2023-02-03 20:33:41.023513 ned-1.11.1/ned/candidate_ranking/cr_searchscore.py
--rw-r--r--   0        0        0     4768 2023-02-03 20:33:41.023597 ned-1.11.1/ned/candidate_ranking/cr_string_similarity.py
--rw-r--r--   0        0        0    14149 2023-04-03 05:40:08.542569 ned-1.11.1/ned/candidate_ranking/cr_training.py
--rw-r--r--   0        0        0        0 2022-12-15 15:16:53.775307 ned-1.11.1/ned/candidate_ranking/dataset/__init__.py
--rw-r--r--   0        0        0     7643 2023-04-03 05:40:08.542773 ned-1.11.1/ned/candidate_ranking/dataset/base.py
--rw-r--r--   0        0        0     7185 2023-04-04 04:26:52.465438 ned-1.11.1/ned/candidate_ranking/dataset/basic_features.py
--rw-r--r--   0        0        0     4691 2023-02-03 20:33:41.024138 ned-1.11.1/ned/candidate_ranking/dataset/matched_prop_feature.py
--rw-r--r--   0        0        0    12216 2023-02-03 20:33:41.024283 ned-1.11.1/ned/candidate_ranking/dataset/types.py
--rw-r--r--   0        0        0       82 2022-11-09 06:50:59.994461 ned-1.11.1/ned/candidate_ranking/helpers/__init__.py
--rw-r--r--   0        0        0     3491 2023-04-03 05:40:08.543114 ned-1.11.1/ned/candidate_ranking/helpers/dataset.py
--rw-r--r--   0        0        0     1181 2022-12-15 15:16:53.776552 ned-1.11.1/ned/candidate_ranking/helpers/db_helper.py
--rw-r--r--   0        0        0    23690 2022-10-28 21:58:46.140615 ned-1.11.1/ned/candidate_ranking/helpers/debug_helper.py
--rw-r--r--   0        0        0     9511 2023-04-03 05:40:08.543297 ned-1.11.1/ned/candidate_ranking/helpers/training_helper.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.140951 ned-1.11.1/ned/candidate_ranking/metrics/__init__.py
--rw-r--r--   0        0        0     4222 2023-04-03 05:40:08.543484 ned-1.11.1/ned/candidate_ranking/metrics/ned_metric.py
--rw-r--r--   0        0        0     5569 2023-02-03 20:33:41.024804 ned-1.11.1/ned/candidate_ranking/pairwise_model.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.141190 ned-1.11.1/ned/data_models/__init__.py
--rw-r--r--   0        0        0    11558 2022-10-28 21:58:46.141319 ned-1.11.1/ned/data_models/deprecated/np_candidate_arrays.py
--rw-r--r--   0        0        0     1769 2022-10-28 21:58:46.141572 ned-1.11.1/ned/data_models/deprecated/py_candidate_arrays.py
--rw-r--r--   0        0        0    25293 2023-04-03 05:40:08.543724 ned-1.11.1/ned/data_models/npmodels.py
--rw-r--r--   0        0        0      757 2023-04-03 05:40:08.543889 ned-1.11.1/ned/data_models/prelude.py
--rw-r--r--   0        0        0     7123 2023-04-03 05:40:08.544077 ned-1.11.1/ned/data_models/pymodels.py
--rw-r--r--   0        0        0        0 2023-02-03 20:33:41.025365 ned-1.11.1/ned/entity_recognition/__init__.py
--rw-r--r--   0        0        0     4569 2023-02-03 20:33:41.025506 ned-1.11.1/ned/entity_recognition/ensemble_model.py
--rw-r--r--   0        0        0      789 2023-02-03 20:33:41.025609 ned-1.11.1/ned/entity_recognition/er_model_interface.py
--rw-r--r--   0        0        0        0 2023-02-03 20:33:41.025703 ned-1.11.1/ned/entity_recognition/model_data/__init__.py
--rw-r--r--   0        0        0     3028 2023-02-03 20:33:41.025818 ned-1.11.1/ned/entity_recognition/model_data/feature_store.py
--rw-r--r--   0        0        0      793 2023-02-03 20:33:41.025910 ned-1.11.1/ned/entity_recognition/model_data/main.py
--rw-r--r--   0        0        0     1956 2023-04-03 05:40:08.544249 ned-1.11.1/ned/entity_recognition/oracle_model.py
--rw-r--r--   0        0        0     1950 2023-02-03 20:33:41.026331 ned-1.11.1/ned/entity_recognition/training.py
--rw-r--r--   0        0        0     6383 2023-04-03 05:40:08.544423 ned-1.11.1/ned/metrics.py
--rw-r--r--   0        0        0        0 2023-04-03 05:40:08.544508 ned-1.11.1/ned/models_and_training/__init__.py
--rw-r--r--   0        0        0     3238 2023-04-03 05:40:08.544635 ned-1.11.1/ned/models_and_training/ensemble_classifier.py
--rw-r--r--   0        0        0     2876 2023-04-03 05:40:08.544742 ned-1.11.1/ned/models_and_training/sklearn_classifier.py
--rw-r--r--   0        0        0      583 2023-04-03 05:40:08.544892 ned-1.11.1/pyproject.toml
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 ned-1.11.1/setup.py
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 ned-1.11.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-06-27 06:54:17.413574 ned-1.7.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-06-27 06:54:17.414574 ned-1.7.0/ned/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.476973 ned-1.7.0/ned/actors/__init__.py
+-rw-r--r--   0        0        0     2313 2022-12-27 20:30:47.331693 ned-1.7.0/ned/actors/__main__.py
+-rw-r--r--   0        0        0     7830 2022-12-31 20:57:16.660906 ned-1.7.0/ned/actors/candidate_generation.py
+-rw-r--r--   0        0        0    15510 2023-01-10 07:14:28.055301 ned-1.7.0/ned/actors/candidate_ranking.py
+-rw-r--r--   0        0        0    12564 2023-01-11 06:57:43.902902 ned-1.7.0/ned/actors/dataset.py
+-rw-r--r--   0        0        0     7910 2022-12-31 21:45:59.245419 ned-1.7.0/ned/actors/entity_recognition.py
+-rw-r--r--   0        0        0     9655 2022-12-26 07:11:54.889372 ned-1.7.0/ned/actors/evaluate_helper.py
+-rw-r--r--   0        0        0        0 2022-06-27 06:54:17.414574 ned-1.7.0/ned/candidate_generation/__init__.py
+-rw-r--r--   0        0        0     2965 2022-12-27 07:30:46.180920 ned-1.7.0/ned/candidate_generation/common.py
+-rw-r--r--   0        0        0     7362 2023-01-11 06:58:38.672862 ned-1.7.0/ned/candidate_generation/oracle_semtyper.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.478973 ned-1.7.0/ned/candidate_generation/pyserini/__init__.py
+-rw-r--r--   0        0        0     1375 2022-11-09 03:09:51.478973 ned-1.7.0/ned/candidate_generation/pyserini/analyzer.py
+-rw-r--r--   0        0        0     1712 2022-11-09 03:09:51.479973 ned-1.7.0/ned/candidate_generation/pyserini/configuration.py
+-rw-r--r--   0        0        0     1214 2022-11-09 03:09:51.479973 ned-1.7.0/ned/candidate_generation/pyserini/document.py
+-rw-r--r--   0        0        0     5000 2022-12-22 04:02:16.176160 ned-1.7.0/ned/candidate_generation/pyserini/indexing.py
+-rw-r--r--   0        0        0     5552 2022-11-09 03:09:51.479973 ned-1.7.0/ned/candidate_generation/pyserini/search.py
+-rw-r--r--   0        0        0     3265 2022-12-22 04:02:46.597144 ned-1.7.0/ned/candidate_generation/pyserini_wrapper.py
+-rw-r--r--   0        0        0    23422 2022-06-27 06:54:17.414574 ned-1.7.0/ned/candidate_generation/table_linker.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.480973 ned-1.7.0/ned/candidate_generation/table_linker_wrapper.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.480973 ned-1.7.0/ned/candidate_ranking/__init__.py
+-rw-r--r--   0        0        0    13158 2022-12-08 09:43:29.391396 ned-1.7.0/ned/candidate_ranking/columnwise_model.py
+-rw-r--r--   0        0        0     8472 2022-12-01 19:09:05.805290 ned-1.7.0/ned/candidate_ranking/columnwise_model.v1
+-rw-r--r--   0        0        0    11440 2022-12-06 23:36:27.001155 ned-1.7.0/ned/candidate_ranking/columnwise_model.v2
+-rw-r--r--   0        0        0     3484 2022-12-06 06:33:13.583975 ned-1.7.0/ned/candidate_ranking/contrastive_pairwise_model.py
+-rw-r--r--   0        0        0    21030 2023-01-11 22:48:04.644488 ned-1.7.0/ned/candidate_ranking/cr_dataset.py
+-rw-r--r--   0        0        0    44939 2022-12-06 04:19:33.743647 ned-1.7.0/ned/candidate_ranking/cr_dataset.py.tmp
+-rw-r--r--   0        0        0     4353 2022-12-26 08:37:33.475624 ned-1.7.0/ned/candidate_ranking/cr_method.py
+-rw-r--r--   0        0        0     2850 2023-01-05 21:53:21.809868 ned-1.7.0/ned/candidate_ranking/cr_searchscore.py
+-rw-r--r--   0        0        0     4768 2023-01-10 07:38:01.680880 ned-1.7.0/ned/candidate_ranking/cr_string_similarity.py
+-rw-r--r--   0        0        0    13128 2022-12-27 20:18:46.367156 ned-1.7.0/ned/candidate_ranking/cr_training.py
+-rw-r--r--   0        0        0        0 2022-12-06 00:00:47.475427 ned-1.7.0/ned/candidate_ranking/dataset/__init__.py
+-rw-r--r--   0        0        0     6731 2022-12-23 09:09:56.099531 ned-1.7.0/ned/candidate_ranking/dataset/base.py
+-rw-r--r--   0        0        0     7136 2023-01-10 07:14:16.037306 ned-1.7.0/ned/candidate_ranking/dataset/basic_features.py
+-rw-r--r--   0        0        0     4691 2023-01-11 06:57:56.402892 ned-1.7.0/ned/candidate_ranking/dataset/matched_prop_feature.py
+-rw-r--r--   0        0        0    12216 2023-01-11 06:58:04.786886 ned-1.7.0/ned/candidate_ranking/dataset/types.py
+-rw-r--r--   0        0        0       82 2022-11-09 03:09:51.481973 ned-1.7.0/ned/candidate_ranking/helpers/__init__.py
+-rw-r--r--   0        0        0     2028 2022-12-26 21:03:44.070983 ned-1.7.0/ned/candidate_ranking/helpers/dataset.py
+-rw-r--r--   0        0        0     1181 2022-12-03 08:27:09.665067 ned-1.7.0/ned/candidate_ranking/helpers/db_helper.py
+-rw-r--r--   0        0        0    23690 2022-11-09 03:09:51.482973 ned-1.7.0/ned/candidate_ranking/helpers/debug_helper.py
+-rw-r--r--   0        0        0     8943 2022-12-25 20:52:30.791920 ned-1.7.0/ned/candidate_ranking/helpers/training_helper.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.482973 ned-1.7.0/ned/candidate_ranking/metrics/__init__.py
+-rw-r--r--   0        0        0     4197 2022-12-24 06:48:51.855052 ned-1.7.0/ned/candidate_ranking/metrics/ned_metric.py
+-rw-r--r--   0        0        0     5569 2023-01-10 06:39:54.898162 ned-1.7.0/ned/candidate_ranking/pairwise_model.py
+-rw-r--r--   0        0        0        0 2022-11-09 03:09:51.483973 ned-1.7.0/ned/data_models/__init__.py
+-rw-r--r--   0        0        0    11558 2022-11-09 03:09:51.483973 ned-1.7.0/ned/data_models/deprecated/np_candidate_arrays.py
+-rw-r--r--   0        0        0     1769 2022-11-09 03:09:51.484973 ned-1.7.0/ned/data_models/deprecated/py_candidate_arrays.py
+-rw-r--r--   0        0        0    19866 2022-12-31 05:44:01.099448 ned-1.7.0/ned/data_models/npmodels.py
+-rw-r--r--   0        0        0      655 2022-12-26 06:59:38.654796 ned-1.7.0/ned/data_models/prelude.py
+-rw-r--r--   0        0        0     6952 2023-01-10 20:07:56.670500 ned-1.7.0/ned/data_models/pymodels.py
+-rw-r--r--   0        0        0        0 2022-12-24 21:29:06.395329 ned-1.7.0/ned/entity_recognition/__init__.py
+-rw-r--r--   0        0        0     4569 2022-12-26 21:45:17.051036 ned-1.7.0/ned/entity_recognition/ensemble_model.py
+-rw-r--r--   0        0        0      789 2022-12-26 21:45:02.353026 ned-1.7.0/ned/entity_recognition/er_model_interface.py
+-rw-r--r--   0        0        0        0 2022-12-24 21:55:05.417836 ned-1.7.0/ned/entity_recognition/model_data/__init__.py
+-rw-r--r--   0        0        0     3028 2022-12-27 21:34:19.574114 ned-1.7.0/ned/entity_recognition/model_data/feature_store.py
+-rw-r--r--   0        0        0      793 2023-01-10 07:41:22.021841 ned-1.7.0/ned/entity_recognition/model_data/main.py
+-rw-r--r--   0        0        0     1257 2022-12-26 21:45:11.971032 ned-1.7.0/ned/entity_recognition/oracle_model.py
+-rw-r--r--   0        0        0     1950 2022-12-25 20:56:44.480688 ned-1.7.0/ned/entity_recognition/training.py
+-rw-r--r--   0        0        0     7685 2023-01-07 06:04:25.163154 ned-1.7.0/ned/metrics.py
+-rw-r--r--   0        0        0        0 2022-12-25 00:55:21.719406 ned-1.7.0/ned/training_helpers/__init__.py
+-rw-r--r--   0        0        0      580 2023-01-11 23:24:25.899320 ned-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 ned-1.7.0/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ned-1.7.0/PKG-INFO
```

### Comparing `ned-1.11.1/LICENSE` & `ned-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/actors/__main__.py` & `ned-1.7.0/ned/actors/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
-from ned.actors.db import DBActor
 
 import yada
 from loguru import logger
 from osin.apis.osin import Osin
 from osin.integrations.ream import OsinActor
 from ream.prelude import ActorGraph, ReamWorkspace, configure_loguru
 
 from kgdata.wikidata.db import WikidataDB
 from ned.actors.candidate_generation import CanGenActor
 from ned.actors.candidate_ranking import CanRankActor
 from ned.actors.entity_recognition import EntityRecognitionActor
-from ned.actors.dataset.prelude import NEDDatasetActor, NEDAutoDatasetActor
+from ned.actors.dataset import NEDDatasetActor
 from ned.actors.evaluate_helper import EvalArgs
 
 ########################################################
 # CONFIG REAM AND DEFINE ACTOR GRAPH
 HOME_DIR = Path(os.environ["HOME_DIR"]).absolute()
 REMOTE_OSIN = os.environ.get("REMOTE_OSIN", None)
 DATABASE_DIR = HOME_DIR / "databases"
@@ -34,17 +33,15 @@
         OsinActor._osin = Osin.local(HOME_DIR / "osin-dev")
     else:
         OsinActor._osin = Osin.remote(REMOTE_OSIN, "/tmp/osin")
 ReamWorkspace.init(HOME_DIR / "ream")
 WikidataDB.init(DATABASE_DIR)
 # fmt: off
 graph: ActorGraph = ActorGraph.auto({
-    "db": DBActor,
-    "ad": NEDAutoDatasetActor, "d": NEDDatasetActor, 
-    "er": EntityRecognitionActor, "cg": CanGenActor, "cr": CanRankActor
+    "d": NEDDatasetActor, "er": EntityRecognitionActor, "cg": CanGenActor, "cr": CanRankActor
 })
 # fmt: on
 ########################################################
 
 
 @dataclass
 class MainArgs:
```

### Comparing `ned-1.11.1/ned/actors/candidate_generation.py` & `ned-1.7.0/ned/actors/candidate_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 from __future__ import annotations
-import os
 
 import pickle
 from dataclasses import dataclass, field, fields
 from functools import partial
 from typing import Literal, Optional
 
 from hugedict.prelude import HugeMutableMapping, RocksDBDict, RocksDBOptions
 from kgdata.wikidata.db import WikidataDB
-from ned.actors.dataset.prelude import NEDDatasetActor
+from ned.actors.dataset import NEDDatasetActor, ned_dsdict_cache_filename
 from ned.actors.entity_recognition import EntityRecognitionActor
 from ned.actors.evaluate_helper import EvalArgs, evaluate
-from ned.candidate_generation.mtab_wrapper import MTabWrapper, MTabArgs
 from ned.candidate_generation.oracle_semtyper import OracleSemTyper, OracleSemTyperArgs
 from ned.candidate_generation.pyserini_wrapper import PyseriniArgs, PyseriniWrapper
 from ned.data_models.prelude import (
     DatasetCandidateEntities,
     CandidateEntity,
     NEDExample,
 )
-from ream.actor_version import ActorVersion
 from ream.cache_helper import CacheArgsHelper
 from ream.dataset_helper import DatasetDict
 from ream.prelude import FS, ActorState, DatasetQuery, EnumParams, Cache, ReamWorkspace
-from sm.misc.ray_helper import get_instance
 from timer import Timer
 from sm.misc.funcs import assert_not_null
 from osin.integrations.ream import OsinActor
-from ned.candidate_generation.localsearch import LocalSearchArgs, LocalSearch
 
 
 @dataclass
 class CGParams(EnumParams):
-    method: Literal["pyserini", "oracle_semtyper", "mtab"] = field(
+    method: Literal["pyserini", "oracle_semtyper"] = field(
         metadata={
             "help": "Candidate generation method",
             "variants": {
                 "pyserini": PyseriniWrapper,
                 "oracle_semtyper": OracleSemTyper,
-                "mtab": MTabWrapper,
             },
         }
     )
     pyserini: Optional[PyseriniArgs] = None
     oracle_semtyper: Optional[OracleSemTyperArgs] = None
-    mtab: Optional[MTabArgs] = None
-    localsearch: Optional[LocalSearchArgs] = field(
-        default=None,
-        metadata={
-            "help": "Search for more candidates by matching the entity's properties with the table's cells"
-        },
-    )
     cache: bool = field(
         default=True,
         metadata={"help": "Whether to cache candidate generation results. "},
     )
 
 
 class CGDatasetDict(DatasetDict[DatasetCandidateEntities]):
-    serde = (DatasetCandidateEntities.save, DatasetCandidateEntities.load, None)
+    serde = (DatasetCandidateEntities.save, DatasetCandidateEntities.load, "parq")
 
 
 class CanGenActor(
     OsinActor[
         NEDExample,
         CGParams,
     ]
@@ -74,26 +61,26 @@
     as headers or the surrounding context of the cell to generate candidates.
     """
 
     """CHANGELOG:
     - 200: new ream
     - 21x: same dataset shares the same cache dir for key-value store only.
     """
-    VERSION = ActorVersion.create(220, [LocalSearch])
-    EXP_NAME = "Candidate Generation"
+    NAME = "Candidate Generation"
+    VERSION = 213
     EXP_VERSION = 3
 
     def __init__(
         self,
         params: CGParams,
         dataset_actor: NEDDatasetActor,
         entity_recognition_actor: EntityRecognitionActor,
     ):
         super().__init__(params, dep_actors=[dataset_actor, entity_recognition_actor])
-        self.db_actor = dataset_actor.auto_dataset_actor.db_actor
+        self.db = WikidataDB.get_instance()
         self.dataset_actor = dataset_actor
         self.entity_recognition_actor = entity_recognition_actor
         self.dataset_name = ""
 
     def run(self, example: NEDExample) -> DatasetCandidateEntities:
         return self.batch_run([example])
 
@@ -102,156 +89,120 @@
         return self.get_method(self.dataset_name).get_candidates(
             examples, entity_columns
         )
 
     def get_provenance(self):
         return self.entity_recognition_actor.get_provenance()
 
-    @Cache.mem(cache_self_args=CacheArgsHelper.gen_cache_self_args(get_provenance))
-    def run_dataset(self, query: str):
-        dsquery = DatasetQuery.from_string(query)
-        dsdict = CGDatasetDict(dsquery.dataset, {}, provenance=self.get_provenance())
-        for subset, sub_dsquery in dsquery.iter_subset():
-            tmp_dsdict = self._run_dataset(sub_dsquery.strip().get_query())
-            assert tmp_dsdict.provenance == dsdict.provenance
-            dsdict[subset] = tmp_dsdict[""]
-        return dsdict
-
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CGDatasetDict,
         cache_self_args=CacheArgsHelper.gen_cache_self_args(get_provenance),
         mem_persist=True,
-        dirname=lambda self, query: DatasetQuery.from_string(query).dataset,
         compression="lz4",
         log_serde_time=True,
     )
-    def _run_dataset(self, query: str):
-        dsdict = self.dataset_actor.run_dataset(query)
-        er_dsdict = self.entity_recognition_actor.run_dataset(query)
-
-        localsearch = (
-            None
-            if self.params.localsearch is None
-            else LocalSearch(self.params.localsearch, self.db_actor.db)
-        )
+    def run_dataset(self, dataset_query: str):
+        dsdict = self.dataset_actor.run(dataset_query)
+        er_dsdict = self.entity_recognition_actor.run_dataset(dataset_query)
 
         out = CGDatasetDict(dsdict.name, {}, er_dsdict.provenance)
         method = self.get_method(dsdict.name)
         timer = Timer()
         for name, ds in dsdict.items():
             with timer.watch("run candidate generation"):
-                cans = method.get_candidates(ds, er_dsdict[name])
-                if localsearch is not None:
-                    cans = localsearch.augment_candidates(ds, cans)
-                out[name] = cans
+                out[name] = method.get_candidates(ds, er_dsdict[name])
         timer.report(self.logger.debug)
         return out
 
-    def evaluate(self, eval_args: EvalArgs):
-        for dsquery_s in eval_args.dsqueries:
+    def evaluate(self, evalargs: EvalArgs):
+        for dsquery_s in evalargs.dsqueries:
             dsquery = DatasetQuery.from_string(dsquery_s)
-            dsdict = self.dataset_actor.run_dataset(dsquery_s)
+            dsdict = self.dataset_actor.run(dsquery_s)
             er_dsdict = self.entity_recognition_actor.run_dataset(dsquery_s)
             cangen_dsdict = self.run_dataset(dsquery_s)
 
             for name, examples in dsdict.items():
                 candidates = cangen_dsdict[name]
                 entity_columns = er_dsdict[name]
                 self.logger.debug("Running evaluation on dataset {}", dsquery_s)
                 dsname = dsquery.get_query(name)
                 with self.new_exp_run(
-                    dataset=dsname, exprun_type=eval_args.exprun_type
+                    dataset=dsname, exprun_type=evalargs.exprun_type
                 ) as exprun:
                     evaluate(
-                        self.db_actor.entities,
                         examples,
                         entity_columns,
                         candidates,
-                        eval_ignore_nil=eval_args.eval_ignore_nil,
-                        eval_ignore_non_entity_cell=eval_args.eval_ignore_non_entity_cell,
+                        eval_ignore_nil=evalargs.eval_ignore_nil,
+                        eval_ignore_non_entity_cell=evalargs.eval_ignore_non_entity_cell,
                         dsname=dsname,
                         logger=self.logger,
                         exprun=exprun,
                         report_unique=True,
-                        exprun_type=eval_args.exprun_type,
+                        exprun_type=evalargs.exprun_type,
                     )
                     if exprun is not None:
                         exprun.update_output(
                             primitive={"workdir": str(self.get_working_fs().root)}
                         )
 
     @Cache.mem()
     def _get_kv_cache(
         self, dataset_name: str
-    ) -> HugeMutableMapping[str, list[tuple[str, float]]]:
-        dbname = dataset_name + "_cache_db"
+    ) -> HugeMutableMapping[str, list[CandidateEntity]]:
+        deps = [actor.get_actor_state() for actor in self.dep_actors]
         if self.params.method == "pyserini":
             state = ActorState.create(
-                PyseriniWrapper, self.params.pyserini, dependencies=[]
+                PyseriniWrapper, self.params.pyserini, dependencies=deps
             )
         elif self.params.method == "oracle_semtyper":
             # leverage the fact that oracle_semtyper is just a wrapper of pyserini
             # so the cache is the same
             args = PyseriniArgs(
                 **{
                     field.name: getattr(self.params.oracle_semtyper, field.name)
                     for field in fields(PyseriniArgs)
                 }
             )
-            state = ActorState.create(PyseriniWrapper, args, dependencies=[])
-        elif self.params.method == "mtab":
-            state = ActorState.create(MTabWrapper, self.params.mtab, dependencies=[])
-            dbname = dataset_name[:2] + "_cache_db"
+            state = ActorState.create(PyseriniWrapper, args, dependencies=deps)
         else:
             raise NotImplementedError()
 
         cache_dir = ReamWorkspace.get_instance().reserve_working_dir(state)
         self.logger.debug(
             "Using directory: {} for key-value store caching",
             cache_dir,
         )
         wfs = FS(cache_dir)
+        # old code, try this if the new code doesn't work
+        # wfs = self.get_working_fs()
 
-        dsdir = wfs.get(dbname, {}, save_key=True)
+        dsdir = wfs.get(dataset_name + "_cache_db", {}, save_key=True)
         if not dsdir.exists():
             with wfs.acquire_write_lock(), dsdir.reserve_and_track() as realdir:
                 dbpath = str(realdir)
         else:
             dbpath = str(dsdir.get())
 
-        return get_instance(
-            lambda: RocksDBDict(
-                path=dbpath,
-                options=RocksDBOptions(create_if_missing=True),
-                deser_key=partial(str, encoding="utf-8"),
-                deser_value=pickle.loads,
-                ser_value=pickle.dumps,
-                # allow to control if the cache should be opened in read-only mode
-                # to run multiple experiments in parallel
-                readonly=os.environ.get("CANGEN_ROCKSDB_READONLY", "0") == "1",
-            ),
-            f"rockdb[{dbpath}]",
+        return RocksDBDict(
+            path=dbpath,
+            options=RocksDBOptions(create_if_missing=True),
+            deser_key=partial(str, encoding="utf-8"),
+            deser_value=pickle.loads,
+            ser_value=pickle.dumps,
+            readonly=False,
         )
 
     @Cache.mem()
     def get_method(self, dataset_name: str):
         kvstore = self._get_kv_cache(dataset_name) if self.params.cache else None
 
         if self.params.method == "pyserini":
-            return PyseriniWrapper(
-                assert_not_null(self.params.pyserini), self.db_actor.db, kvstore
-            )
+            return PyseriniWrapper(assert_not_null(self.params.pyserini), kvstore)
         elif self.params.method == "oracle_semtyper":
             args = assert_not_null(self.params.oracle_semtyper)
             return OracleSemTyper(
-                PyseriniWrapper(args, self.db_actor.db, kvstore),
-                self.db_actor.db,
+                PyseriniWrapper(args, kvstore),
                 args,
             )
-        elif self.params.method == "mtab":
-            return MTabWrapper(
-                assert_not_null(self.params.mtab),
-                self.db_actor.db,
-                kvstore,
-            )
         else:
             raise NotImplementedError(self.params.method)
```

### Comparing `ned-1.11.1/ned/actors/candidate_ranking.py` & `ned-1.7.0/ned/actors/candidate_ranking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
-import copy
 
 import os
 from dataclasses import dataclass, field
-from typing import Literal, Optional, cast
+from functools import partial
+from typing import Literal, Optional
 from ned.candidate_ranking.cr_searchscore import CRSearchScore
 from ned.candidate_ranking.cr_string_similarity import (
     CRStringSimilarity,
     CRStringSimilarityArgs,
 )
 from ned.candidate_ranking.helpers.dataset import MyDatasetDict
-from ned.entity_recognition.oracle_model import OracleERModelArgs
 from slugify import slugify
 import torch
 from osin.integrations.ream import OsinActor
 from ream.actors.base import BaseActor
 from ream.cache_helper import Cache, CacheArgsHelper
 from ream.dataset_helper import DatasetQuery
 from ream.fs import ItemStatus
@@ -26,16 +25,16 @@
     DatasetDict,
     DatasetQuery,
     EnumParams,
     NoParams,
 )
 from timer import Timer
 
-from ned.actors.candidate_generation import CanGenActor
-from ned.actors.dataset.prelude import NEDDatasetActor
+from ned.actors.candidate_generation import CanGenActor, CGDatasetDict
+from ned.actors.dataset import NEDDatasetActor, ned_dsdict_cache_filename
 from ned.actors.entity_recognition import (
     EntityRecognitionActor,
     ERParams,
 )
 from ned.actors.evaluate_helper import EvalArgs, evaluate
 from ned.candidate_ranking.columnwise_model import ColumnwiseModel, ColumnwiseModelArgs
 from ned.candidate_ranking.contrastive_pairwise_model import (
@@ -50,62 +49,58 @@
 from ned.candidate_ranking.helpers.training_helper import (
     CkptHelper,
     ModifiedTrainingArguments,
 )
 from ned.candidate_ranking.pairwise_model import PairwiseModel, PairwiseModelArgs
 from ned.data_models.prelude import DatasetCandidateEntities, NEDExample
 from sm.misc.prelude import assert_not_null
-import scripts.ned.candidate_ranking.notebooks.models as new_models
 
 
 @dataclass
 class CRParams(EnumParams):
     method: Literal[
         "pairwise",
-        "crv3",
         "columnwise",
         "contrastive_pairwise",
         "searchscore",
         "strsim",
     ] = field(
         metadata={
             "variants": {
                 "pairwise": PairwiseModel,
-                "crv3": new_models.CRV3,
                 "columnwise": ColumnwiseModel,
                 "contrastive_pairwise": ContrastivePairwiseModel,
                 "searchscore": CRSearchScore,
                 "strsim": CRStringSimilarity,
             }
         }
     )
     training: Optional[ModifiedTrainingArguments] = None
-    crv3: Optional[new_models.CRV3Args] = None
     pairwise: Optional[PairwiseModelArgs] = None
     columnwise: Optional[ColumnwiseModelArgs] = None
     contrastive_pairwise: Optional[ContrastivePairwiseModelArgs] = None
     searchscore: Optional[NoParams] = field(default_factory=NoParams)
     strsim: Optional[CRStringSimilarityArgs] = None
 
 
 class CRDatasetDict(DatasetDict[CandidateEntityScores]):
-    serde = (CandidateEntityScores.save, CandidateEntityScores.load, None)
+    serde = (CandidateEntityScores.save, CandidateEntityScores.load, "parq")
 
 
 class CanRankActor(OsinActor[NEDExample, CRParams]):
     """Different methods in ranking candidate entities for Record Linkage problem"""
 
     """CHANGELOG:
     - 10X: fixing bugs
     - 110: switching to use pyarrow
     - 111: add missing depenedency which is canrank_dataset
     - 200: new version of ream
     """
-    EXP_NAME = "Candidate Ranking"
-    VERSION = 204
+    NAME = "Candidate Ranking"
+    VERSION = 203
     EXP_VERSION = 3
 
     def __init__(
         self,
         params: CRParams,
         dataset_actor: NEDDatasetActor,
         cangen_actor: CanGenActor,
@@ -118,16 +113,15 @@
             params,
             [
                 dataset_actor,
                 cangen_actor,
                 canrank_dataset,
             ],
         )
-        self.db_actor = dataset_actor.auto_dataset_actor.db_actor
-        self.db = self.db_actor.db
+        self.db = cangen_actor.db
         self.dataset_actor = dataset_actor
         self.cangen_actor = cangen_actor
         self.canrank_dataset = canrank_dataset
         self.model: CandidateRankingMethod | None = None
         self.is_eval: bool = False
         self.timer = Timer()
 
@@ -149,30 +143,30 @@
         ds = method.generate_dataset(examples, candidates)
         return method.rank_datasets(examples, candidates, ds)
 
     def get_provenance(self):
         method, provenance = self.get_trained_method()
         return self._fmt_provenance(self.cangen_actor.get_provenance(), provenance)
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetDict,
         cache_self_args=CacheArgsHelper.gen_cache_self_args(get_provenance),
         mem_persist=True,
         compression="lz4",
         log_serde_time=True,
     )
     def run_dataset(self, dataset_query: str) -> CRDatasetDict:
         # run the candidate ranking on the dataset and return the result
         # we want to cache the result here. but we almost have to rerun
         # unless we can retrieve the result from the cache.
-        dsdict = self.dataset_actor.run_dataset(dataset_query)
+        dsdict = self.dataset_actor.run(dataset_query)
         cg_dsdict = self.cangen_actor.run_dataset(dataset_query)
 
         method, provenance = self.get_trained_method()
-        canrank_dsdict = self.canrank_dataset.run_dataset(
+        canrank_dsdict = self.canrank_dataset.run(
             self.get_method(),
             dataset_query,
             for_training=False,
         )
 
         if not method.EVAL_ON_CPU:
             method = method.to(torch.device("cpu"))
@@ -191,24 +185,24 @@
             # candidates = getattr(canrank_dsdict[name], "candidates")
             out[name] = method.rank_datasets(
                 examples, candidates, canrank_dsdict[name], verbose=True
             )
 
         return out
 
-    def evaluate(self, eval_args: EvalArgs):
+    def evaluate(self, evalargs: EvalArgs):
         retrain = int(os.environ.get("CR_RETRAIN", "0")) == 1
         fromstep = int(os.environ.get("CR_RETRAIN_FROMSTEP", "0"))
         fromfile = os.environ.get("CR_RETRAIN_FROMFILE", None)
         self.get_trained_method(retrain=retrain, fromstep=fromstep, fromfile=fromfile)
 
-        for dsquery_s in eval_args.dsqueries:
+        for dsquery_s in evalargs.dsqueries:
             dsquery = DatasetQuery.from_string(dsquery_s)
 
-            dsdict = self.dataset_actor.run_dataset(dsquery_s)
+            dsdict = self.dataset_actor.run(dsquery_s)
             er_dsdict = self.cangen_actor.entity_recognition_actor.run_dataset(
                 dsquery_s
             )
             cg_dsdict = self.cangen_actor.run_dataset(dsquery_s)
             cr_dsdict = self.run_dataset(dsquery_s)
 
             self.logger.debug("Running evaluation on dataset {}", dsquery_s)
@@ -217,28 +211,27 @@
                 entity_columns = er_dsdict[name]
                 can_scores = cr_dsdict[name]
                 candidates = cg_dsdict[name].replace("score", can_scores.score)
 
                 subdsquery_s = dsquery.get_query(name)
                 with self.new_exp_run(
                     dataset=subdsquery_s,
-                    exprun_type=eval_args.exprun_type,
-                    eval_ignore_nil=eval_args.eval_ignore_nil,
+                    exprun_type=evalargs.exprun_type,
+                    eval_ignore_nil=evalargs.eval_ignore_nil,
                 ) as exprun:
                     evaluate(
-                        self.db_actor.entities,
                         examples,
                         entity_columns,
                         candidates,
-                        eval_ignore_nil=eval_args.eval_ignore_nil,
-                        dsname=subdsquery_s,
+                        eval_ignore_nil=evalargs.eval_ignore_nil,
+                        dsname=dsquery_s,
                         logger=self.logger,
                         exprun=exprun,
                         report_unique=True,
-                        exprun_type=eval_args.exprun_type,
+                        exprun_type=evalargs.exprun_type,
                     )
                     if exprun is not None:
                         exprun.update_output(
                             primitive={"workdir": str(self.get_working_fs().root)}
                         )
 
     @Cache.mem()
@@ -251,44 +244,35 @@
             model = ContrastivePairwiseModel.from_args(
                 assert_not_null(self.params.contrastive_pairwise)
             )
         elif self.params.method == "searchscore":
             model = CRSearchScore()
         elif self.params.method == "strsim":
             model = CRStringSimilarity.from_args(assert_not_null(self.params.strsim))
-        elif self.params.method == "crv3":
-            model = new_models.CRV3.from_args(assert_not_null(self.params.crv3))
         else:
             raise NotImplementedError()
         return model
 
     @Cache.mem()
     def get_trained_method(
-        self,
-        retrain: bool = False,
-        fromstep: int = 0,
-        fromfile: Optional[str] = None,
+        self, retrain: bool = False, fromstep: int = 0, fromfile: Optional[str] = None
     ) -> tuple[CandidateRankingMethod, str]:
         if self.params.method in ["searchscore", "strsim"]:
             # return no trained methods
             method = self.get_method()
             return method, f"{self.params.method}_{method.VERSION}"
 
         wfs = self.get_working_fs()
         model_file = wfs.get("model.pt")
 
         if not model_file.exists() or retrain:
             # train the model again or resume training
             with wfs.acquire_write_lock():
                 ckpt = CkptHelper(self.get_working_fs().root, fromstep, fromfile)
-                eval_ds_mode: str = cast(
-                    Literal["train", "test"], os.environ.get("EVAL_DS_MODE", "train")
-                )
-                assert eval_ds_mode in ["train", "test"]
-                model, trained_file = cr_training(self, ckpt, eval_ds_mode)
+                model, trained_file = cr_training(self, ckpt)
 
                 if model_file.exists():
                     linked_file = model_file.get()
                 else:
                     linked_file = model_file.reserve()
                     model_file.update_status(ItemStatus.Success)
 
@@ -318,49 +302,44 @@
 
 
 class CRModelDataActor(BaseActor[str, NoParams]):
     """CHANGELOG:
     - 200: switch to new ream version
     """
 
-    VERSION = 219
+    VERSION = 218
 
     def __init__(
         self,
         dataset_actor: NEDDatasetActor,
         cangen_actor: CanGenActor,
     ):
         super().__init__(NoParams(), dep_actors=[dataset_actor, cangen_actor])
         self.dataset_actor = dataset_actor
         self.cangen_actor = cangen_actor
 
-        oracle_er_params = ERParams(
-            method="oracle", oracle=OracleERModelArgs(), training=None
-        )
+        oracle_er_params = ERParams(method="oracle", oracle=NoParams(), training=None)
         oracle_er_actor = EntityRecognitionActor(oracle_er_params, dataset_actor)
-        cangen_params = copy.copy(cangen_actor.params)
-        cangen_params.localsearch = None  # always disable local search
         self.train_cangen_actor = CanGenActor(
-            cangen_params, dataset_actor, oracle_er_actor
+            cangen_actor.params, dataset_actor, oracle_er_actor
         )
 
-    def run_dataset(
+    def run(
         self,
         method: CandidateRankingMethod,
         dataset_query: str,
         for_training: bool = False,
     ):
         cg_dsdict = self.cangen_actor.run_dataset(dataset_query)
 
-        # @Cache.cls.dir(
-        #     cls=MyDatasetDict,
-        #     cache_key=CRModelDataActor.get_cache_key,
-        #     dirname=CRModelDataActor.get_cache_dirname,
-        #     compression="lz4",
-        # )
+        @Cache.cls.file(
+            cls=MyDatasetDict,
+            cache_key=CRModelDataActor.get_cache_key,
+            filename=CRModelDataActor.get_cache_filename,
+        )
         def exec(
             self,
             method: CandidateRankingMethod,
             dataset_query: str,
             for_training: bool,
             cg_provenance: str,
         ):
@@ -386,15 +365,15 @@
             with builddir.reserve_and_track() as builddir_path:
                 pass
         self.logger.debug(
             "Cache common model data to a build directory: {}", builddir_path
         )
 
         self.logger.debug("Retrieve candidates of dataset: {}", dataset_query)
-        dsdict = self.dataset_actor.run_dataset(dataset_query)
+        dsdict = self.dataset_actor.run(dataset_query)
 
         if for_training:
             # for training, we always use an oracle entity recognition to generate the candidates
             # as the entity recognition model may not produce the correct entity columns
             cg_dsdict = self.train_cangen_actor.run_dataset(dataset_query)
         else:
             cg_dsdict = self.cangen_actor.run_dataset(dataset_query)
@@ -438,17 +417,20 @@
                 "state": state.to_dict(),
                 "dsquery": dsquery,
                 "for_training": for_training,
                 "cg_provenance": cg_provenance,
             }
         )
 
-    def get_cache_dirname(
+    def get_cache_filename(
         self: CRModelDataActor,
         method: CandidateRankingMethod,
         dsquery: str,
         for_training: bool,
         cg_provenance: str,
     ):
-        return slugify(
-            f"{method.__class__.__name__}_{getattr(method, 'VERSION')}_{dsquery}_{for_training}"
-        ).replace("-", "_")
+        return (
+            slugify(
+                f"{method.__class__.__name__}_{getattr(method, 'VERSION')}_{dsquery}_{for_training}"
+            ).replace("-", "_")
+            + ".lz4"
+        )
```

### Comparing `ned-1.11.1/ned/actors/dataset/dataset.py` & `ned-1.7.0/ned/actors/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,121 @@
 from __future__ import annotations
-
+from pathlib import Path
+from slugify import slugify
 import random
+from collections import defaultdict
+from copy import deepcopy
 from dataclasses import dataclass
-from pathlib import Path
-from typing import Callable, Mapping, Optional, Union
-from ned.data_models.pymodels import EntityWithScore
-
+from typing import Mapping, Optional, cast
+from ned.actors.evaluate_helper import EvalArgs
+import ray
 import numpy as np
 import serde.jl
 import serde.json
 import serde.textline
 from osin.integrations.ream import OsinActor
+from osin.types import OTable
 from rdflib.namespace import RDFS
-from ream.prelude import Cache, DatasetQuery
-from slugify import slugify
-from sm.inputs.link import WIKIDATA, EntityId
+from ream.prelude import Cache, DatasetDict, DatasetQuery
 from sm_datasets import Datasets
-
+from functools import partial
 from grams.algorithm.literal_matchers.text_parser import TextParser
 from kgdata.wikidata.db import WikidataDB
 from kgdata.wikidata.models import WDEntity
-from ned.actors.db import to_wikidata_db
-from ned.actors.evaluate_helper import AuxComplexTableObject, EvalArgs
-from ned.data_models.prelude import NEDExample
+from ned.data_models.prelude import CellLink, Entity, NEDExample
 from sm.dataset import Example, FullTable
-from sm.misc.ray_helper import ray_map, ray_put
-from sm.namespaces.namespace import KnowledgeGraphNamespace
 from sm.namespaces.wikidata import WikidataNamespace
 from sm.prelude import M
-
-from ned.actors.dataset.auto_dataset import NEDAutoDatasetActor
-from ned.actors.dataset.utils import (
-    NEDDatasetDict,
-    has_non_unique_mention,
-    normalize_table,
-    is_column_entity,
-    get_cell_links,
-    should_be_column_entity,
-)
+from sm.misc.ray_helper import ray_map, get_instance, ray_put
 
 
 @dataclass
 class NEDDatasetParams:
     skip_non_unique_mention: bool = False
 
 
+class NEDDatasetDict(DatasetDict[list[NEDExample]]):
+    serde = (serde.jl.ser, partial(serde.jl.deser, cls=NEDExample), "jl")
+
+
+def ned_dsdict_cache_filename(
+    self, dsquery: str, provenance: str = "", compression: Optional[str] = None
+):
+    ext = f".{compression}" if compression is not None else ""
+    return DatasetQuery.from_string(dsquery).dataset + ext
+
+
 class NEDDatasetActor(OsinActor[str, NEDDatasetParams]):
     """An actor that will output the dataset for entity linking."""
 
     """CHANGELOG:
     - 401: add option to skip tables that the same mention at different cells are linked to different entities
     - 41x: add entity column types to the example, ignore tables with empty entity columns, 
     """
 
-    EXP_NAME = "Dataset"
-    VERSION = 505
+    NAME = "Dataset"
+    VERSION = 413
     EXP_VERSION = 2
 
-    kgns = WikidataNamespace.create()
-
-    def __init__(
-        self, params: NEDDatasetParams, auto_dataset_actor: NEDAutoDatasetActor
-    ):
-        super().__init__(params, [auto_dataset_actor])
-        self.auto_dataset_actor = auto_dataset_actor
+    def __init__(self, params: NEDDatasetParams):
+        super().__init__(params)
         self.text_parser = TextParser.default()
+        self.kgns = WikidataNamespace.create()
 
-    @Cache.mem()
-    def run_dataset(self, query: str) -> NEDDatasetDict:
-        dsquery = DatasetQuery.from_string(query)
-        if dsquery.dataset.startswith("wtauto"):
-            assert (
-                self.auto_dataset_actor.params.skip_non_unique_mention
-                == self.params.skip_non_unique_mention
-            )
-            return self.auto_dataset_actor.run_dataset(query)
-
-        dsdict = NEDDatasetDict(dsquery.dataset, {})
-        for subset, sub_dsquery in dsquery.iter_subset():
-            dsdict[subset] = self._run_dataset(sub_dsquery.strip().get_query())[""]
-        return dsdict
-
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=NEDDatasetDict,
         mem_persist=True,
-        dirname=lambda self, query: DatasetQuery.from_string(query).dataset,
+        filename=partial(ned_dsdict_cache_filename, compression="lz4"),
         log_serde_time=True,
-        compression="lz4",
     )
-    def _run_dataset(
+    def run(
         self,
         query: str,
     ) -> NEDDatasetDict:
         dsquery = DatasetQuery.from_string(query)
         ned_examples = self.ned_examples(dsquery.dataset)
 
         infodir = self.get_working_fs().root / (f"info_" + slugify(dsquery.dataset))
         infodir.mkdir(exist_ok=True)
 
+        if dsquery.shuffle:
+            index = list(range(len(ned_examples)))
+            random.Random(dsquery.seed).shuffle(index)
+
+            shuffle_index = [ned_examples[i].table.table_id for i in index]
+            serde.json.ser(
+                shuffle_index,
+                infodir / f"shuffle_{dsquery.seed or 'none'}.json",
+            )
+            id2e = {e.table.table_id: e for e in ned_examples}
+            ned_examples = [id2e[i] for i in shuffle_index]
+
         if self.params.skip_non_unique_mention:
             non_unique_table_ids = [
-                e.table.table_id for e in ned_examples if has_non_unique_mention(e)
+                e.table.table_id for e in ned_examples if self.has_non_unique_mention(e)
             ]
             serde.textline.ser(
                 non_unique_table_ids,
                 infodir / f"non_unique_tables.txt",
             )
             non_unique_table_ids = set(non_unique_table_ids)
             ned_examples = [
                 e for e in ned_examples if e.table.table_id not in non_unique_table_ids
             ]
             self.logger.info(
                 "Skip {} tables with non-unique mentions",
                 len(non_unique_table_ids),
             )
 
-        if dsquery.shuffle:
-            shuffle_file = infodir / f"shuffle_{dsquery.seed or 'none'}.json"
-            if not shuffle_file.exists():
-                index = list(range(len(ned_examples)))
-                random.Random(dsquery.seed).shuffle(index)
-                shuffle_index = [ned_examples[i].table.table_id for i in index]
-                serde.json.ser(
-                    shuffle_index,
-                    shuffle_file,
-                )
-
         return NEDDatasetDict.molt(dsquery.select(ned_examples))
 
-    def evaluate(self, eval_args: EvalArgs):
-        for query in eval_args.dsqueries:
+    def evaluate(self, evalargs: EvalArgs):
+        for query in evalargs.dsqueries:
             dsquery = DatasetQuery.from_string(query)
-            dsdict = self.run_dataset(query)
+            dsdict = self.run(query)
             for name, examples in dsdict.items():
                 n_cells = [np.prod(e.table.shape()) for e in examples]
                 n_rows = [e.table.shape()[0] for e in examples]
 
                 metrics = {
                     "# examples": len(examples),
                     "average # cells": float(np.mean(n_cells)),
@@ -166,119 +146,192 @@
                 )
                 for k, v in metrics.items():
                     self.logger.info("\t - {}: {}", k, v)
 
                 with self.new_exp_run(dataset=dsquery.get_query(name)) as exprun:
                     if exprun is not None:
                         for ei, example in enumerate(examples):
+                            columns = example.table.columns
+                            header = [
+                                c.clean_name or f"column-{i}"
+                                for i, c in enumerate(columns)
+                            ]
+
+                            nrows, ncols = example.table.shape()
+                            otbl = []
+                            for ri in range(nrows):
+                                otbl.append(
+                                    dict(
+                                        zip(
+                                            header,
+                                            (
+                                                str(columns[ci].values[ri])
+                                                for ci in range(ncols)
+                                            ),
+                                        )
+                                    )
+                                )
                             exprun.update_example_output(
                                 example_id=str(ei),
                                 example_name=example.table.table_id,
-                                complex={
-                                    "table": AuxComplexTableObject(
-                                        self.auto_dataset_actor.db_actor.entities
-                                    ).get_table(example, None)
-                                },
+                                complex={"table": OTable(otbl)},
                             )
 
                         exprun.update_output(primitive=metrics)
 
     @Cache.jl.file(mem_persist=True, compression="lz4", cls=NEDExample)
     def ned_examples(self, dataset: str) -> list[NEDExample]:
         dbdir_ref = ray_put(WikidataDB.get_instance().database_dir)
         list_exs = ray_map(
-            sm2ned_example,
+            sm2ned_example.remote,
             [(dbdir_ref, item) for item in M.batch(48, self.sm_examples(dataset))],
             verbose=True,
             desc="generate ned examples",
-            using_ray=True,
-            is_func_remote=False,
         )
         return [e for lst in list_exs for e in lst]
 
     @Cache.pickle.file(mem_persist=True, compression="lz4")
     def sm_examples(self, dataset: str) -> list[Example[FullTable]]:
         ds = Datasets()
         db = WikidataDB.get_instance()
         examples = getattr(ds, dataset)()
         examples = ds.fix_redirection(
             examples, db.wdentities, db.wdredirections, self.kgns
         )
         return examples
 
+    def has_non_unique_mention(self, example: NEDExample) -> bool:
+        """Check if the example table has the same mention at different cells linked to different entities"""
+        col2mention = defaultdict(lambda: defaultdict(set))
+
+        for ri, ci, link in example.cell_links.enumerate_flat_iter():
+            if link is None:
+                continue
+
+            text = example.table[ri, ci]
+            assert isinstance(text, str), text
+
+            for entid, (start, end) in link.mentions.items():
+                mention = text[start:end]
+                col2mention[ci][mention].add(entid)
+                if len(col2mention[ci][mention]) > 1:
+                    return True
+
+        return False
+
+    @classmethod
+    def _get_cell_links(
+        cls,
+        example: Example[FullTable],
+        wdents: Mapping[str, WDEntity],
+        wdpopularity: Mapping[str, float],
+    ) -> M.Matrix[CellLink | None]:
+        cell_links = M.Matrix.default(
+            example.table.table.shape(), cast(Optional[CellLink], None)
+        )
+
+        for ci, col in enumerate(example.table.table.columns):
+            if not cls._is_column_entity(example, ci):
+                continue
+            for ri in range(len(col.values)):
+                links = [
+                    link
+                    for link in example.table.links[ri, ci]
+                    if len(link.entities) > 0
+                ]
+                if len(links) == 0:
+                    continue
 
+                mentions = {}
+                ents = []
+                for link in links:
+                    for entid in link.entities:
+                        _ent = wdents[entid]
+                        ent = Entity(
+                            id=_ent.id,
+                            label=str(_ent.label),
+                            description=str(_ent.description),
+                            aliases=Entity.encode_aliases(_ent.aliases),
+                            popularity=wdpopularity.get(_ent.id, 0.0),
+                        )
+                        ents.append(ent)
+                        mentions[ent.id] = (link.start, link.end)
+
+                cell_links[ri, ci] = CellLink(
+                    entities=ents,
+                    mentions=mentions,
+                )
+        return cell_links
+
+    @classmethod
+    def _is_column_entity(cls, example: Example[FullTable], ci: int):
+        for sm in example.sms:
+            stypes = sm.get_semantic_types_of_column(ci)
+            if any(stype.predicate_abs_uri == str(RDFS.label) for stype in stypes):
+                return True
+        return False
+
+
+@ray.remote
 def sm2ned_example(
-    db: Union[WikidataDB, Path], sm_examples: list[Example[FullTable]]
+    dbdir: Path, sm_examples: list[Example[FullTable]]
 ) -> list[NEDExample]:
-    db = to_wikidata_db(db)
-
     text_parser = TextParser.default()
     kgns = WikidataNamespace.create()
-
+    db = get_instance(
+        lambda: WikidataDB(dbdir),
+        f"kgdata.wikidata.db[{dbdir}]",
+    )
     wdents = db.wdentities.cache()
-    wdprops = db.wdprops.cache()
     wdpopularity = db.wdpagerank
     new_examples = []
 
     for example in sm_examples:
+        table = deepcopy(example.table.table)
+        for col in table.columns:
+            assert col.name is not None
+            col.name = text_parser._norm_string(col.name)
+
+        # normalize cells
+        for ci, col in enumerate(table.columns):
+            for ri, cell in enumerate(col.values):
+                if isinstance(cell, str):
+                    col.values[ri] = text_parser._norm_string(cell)
+
+        entity_columns = []
+        entity_column_types = []
+
+        for ci in range(example.table.table.shape()[1]):
+            if NEDDatasetActor._is_column_entity(example, ci):
+                entity_columns.append(ci)
+                ctypes = []
+                for sm in example.sms:
+                    for stype in sm.get_semantic_types_of_column(ci):
+                        if stype.predicate_abs_uri == str(RDFS.label):
+                            ctypes.append(kgns.get_entity_id(stype.class_abs_uri))
+                entity_column_types.append(
+                    [
+                        Entity(
+                            id=entid,
+                            label=(_ent := db.wdentities[entid]).label,
+                            description=_ent.description,
+                            aliases=Entity.encode_aliases(_ent.aliases),
+                            popularity=db.wdpagerank[entid],
+                        )
+                        for entid in M.filter_duplication(ctypes)
+                    ]
+                )
+
+        if len(entity_columns) == 0:
+            continue
+
         new_examples.append(
-            to_ned_example(
-                example,
-                text_parser,
-                kgns,
-                wdents,
-                wdpopularity,
-                is_column_entity=is_column_entity,
-                should_be_column_entity=lambda tbl, ci: should_be_column_entity(
-                    tbl, ci, wdprops, kgns
+            NEDExample(
+                table=example.table.table,
+                entity_columns=entity_columns,
+                entity_column_types=entity_column_types,
+                cell_links=NEDDatasetActor._get_cell_links(
+                    example, wdents, wdpopularity
                 ),
             )
         )
     return new_examples
-
-
-def to_ned_example(
-    example: Example[FullTable],
-    text_parser: TextParser,
-    kgns: KnowledgeGraphNamespace,
-    entities: Mapping[str, WDEntity],
-    pagerank: Mapping[str, float],
-    is_column_entity: Callable[[Example[FullTable], int], bool],
-    should_be_column_entity: Callable[[Example[FullTable], int], bool],
-) -> Optional[NEDExample]:
-    table = normalize_table(example.table.table, text_parser)
-
-    should_be_entity_columns = []
-    entity_columns = []
-    entity_column_types: list[list[EntityWithScore]] = []
-
-    for ci in range(example.table.table.shape()[1]):
-        if is_column_entity(example, ci):
-            entity_columns.append(ci)
-            ctypes = []
-            for sm in example.sms:
-                for stype in sm.get_semantic_types_of_column(ci):
-                    if stype.predicate_abs_uri == str(RDFS.label):
-                        ctypes.append(kgns.get_entity_id(stype.class_abs_uri))
-            entity_column_types.append(
-                [
-                    EntityWithScore(
-                        EntityId(entid, WIKIDATA),
-                        1.0,
-                    )
-                    for entid in M.filter_duplication(ctypes)
-                ]
-            )
-        elif should_be_column_entity(example, ci):
-            should_be_entity_columns.append(ci)
-
-    if len(entity_columns) + len(should_be_entity_columns) == 0:
-        # there is no entity column in this table
-        return None
-
-    return NEDExample(
-        table=table,
-        entity_columns=entity_columns,
-        entity_column_types=entity_column_types,
-        cell_links=get_cell_links(example, is_column_entity),
-        should_be_entity_columns=should_be_entity_columns,
-    )
```

### Comparing `ned-1.11.1/ned/actors/entity_recognition.py` & `ned-1.7.0/ned/actors/entity_recognition.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,22 +18,26 @@
     DatasetDict,
     DatasetQuery,
     EnumParams,
     NoParams,
 )
 from slugify import slugify
 
-from ned.actors.dataset.prelude import NEDDatasetActor, NEDDatasetDict
+from ned.actors.dataset import (
+    NEDDatasetActor,
+    NEDDatasetDict,
+    ned_dsdict_cache_filename,
+)
 from ned.actors.evaluate_helper import EvalArgs
 from ned.candidate_ranking.helpers.dataset import MyDatasetDict
 from ned.candidate_ranking.helpers.training_helper import ModifiedTrainingArguments
 from ned.data_models.prelude import NEDExample
 from ned.entity_recognition.ensemble_model import EnsembleModel, EnsembleModelArgs
 from ned.entity_recognition.er_model_interface import ERModelInterface
-from ned.entity_recognition.oracle_model import OracleERModel, OracleERModelArgs
+from ned.entity_recognition.oracle_model import OracleERModel
 from ned.entity_recognition.training import sklearn_train
 from sm.misc.funcs import assert_not_null, get_incremental_path
 
 
 @dataclass
 class ERParams(EnumParams):
     method: Literal["ensemble", "oracle"] = field(
@@ -42,23 +46,23 @@
             "variants": {
                 "ensemble": EnsembleModel,
                 "oracle": OracleERModel,
             },
         }
     )
     ensemble: Optional[EnsembleModelArgs] = field(default_factory=EnsembleModelArgs)
-    oracle: Optional[OracleERModelArgs] = field(default_factory=OracleERModelArgs)
+    oracle: Optional[NoParams] = field(default_factory=NoParams)
     training: Optional[ModifiedTrainingArguments] = field(
         default_factory=ModifiedTrainingArguments
     )
 
 
 class EntityRecognitionActor(OsinActor[NEDExample, ERParams]):
-    EXP_NAME = "Entity Column Recognition"
-    VERSION = 110
+    NAME = "Entity Column Recognition"
+    VERSION = 101
     EXP_VERSION = 1
 
     def __init__(self, params: ERParams, dataset_actor: NEDDatasetActor):
         model_data_actor = ERModelDataActor(dataset_actor)
         super().__init__(params, [dataset_actor, model_data_actor])
         self.dataset_actor = dataset_actor
         self.model_data_actor = model_data_actor
@@ -70,39 +74,26 @@
         method, provenance = self.get_trained_method()
         return method.predict_data(examples, method.gen_data(examples))
 
     def get_provenance(self):
         method, provenance = self.get_trained_method()
         return provenance
 
-    @Cache.mem(cache_self_args=CacheArgsHelper.gen_cache_self_args(get_provenance))
-    def run_dataset(self, query: str):
-        dsquery = DatasetQuery.from_string(query)
-        dsdict: DatasetDict[list[list[int]]] = DatasetDict(
-            dsquery.dataset, {}, provenance=self.get_provenance()
-        )
-        for subset, sub_dsquery in dsquery.iter_subset():
-            tmp_dsdict = self._run_dataset(sub_dsquery.strip().get_query())
-            dsdict[subset] = tmp_dsdict[""]
-            assert tmp_dsdict.provenance == dsdict.provenance
-        return dsdict
-
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=DatasetDict,
         cache_self_args=CacheArgsHelper.gen_cache_self_args(get_provenance),
         mem_persist=True,
-        dirname=lambda self, query: DatasetQuery.from_string(query).dataset,
         compression="lz4",
         log_serde_time=True,
     )
-    def _run_dataset(self, query: str):
+    def run_dataset(self, dataset_query: str):
         method, provenance = self.get_trained_method()
-        dsdict = self.dataset_actor.run_dataset(query)
-        method_dsdict = self.model_data_actor.run_dataset(
-            method, query, for_training=False
+        dsdict = self.dataset_actor.run(dataset_query)
+        method_dsdict = self.model_data_actor.run(
+            method, dataset_query, for_training=False
         )
         out: DatasetDict[list[list[int]]] = DatasetDict(
             dsdict.name, {}, provenance=provenance
         )
         for name, ds in method_dsdict.items():
             examples = dsdict[name]
             out[name] = method.predict_data(examples, method_dsdict[name])
@@ -126,15 +117,15 @@
         wfs = self.get_working_fs()
         model_file = wfs.get("model.pkl")
 
         if not model_file.exists() or retrain:
             # train the model again or resume training
             method = sklearn_train(
                 method,
-                self.model_data_actor.run_dataset,
+                self.model_data_actor.run,
                 assert_not_null(self.params.training),
                 ["precision", "recall", "f1"],
             )
 
             dir = get_incremental_path(wfs.root / "training_v")
             trained_file = dir / "model.pkl"
             with open(trained_file, "wb") as f:
@@ -160,28 +151,26 @@
         provenance = os.path.relpath(provenance, wfs.root)
         return method, provenance
 
     def get_method(self):
         if self.params.method == "ensemble":
             return EnsembleModel(assert_not_null(self.params.ensemble))
         if self.params.method == "oracle":
-            return OracleERModel(assert_not_null(self.params.oracle))
+            return OracleERModel()
         raise NotImplementedError()
 
 
 class ERModelDataActor(BaseActor[str, NoParams]):
     VERSION = 100
 
     def __init__(self, dataset_actor: NEDDatasetActor):
         super().__init__(NoParams(), [dataset_actor])
         self.dataset_actor = dataset_actor
 
-    def run_dataset(
-        self, method: ERModelInterface, dataset_query: str, for_training: bool
-    ):
+    def run(self, method: ERModelInterface, dataset_query: str, for_training: bool):
         return self.gen_data(method, dataset_query, for_training)
 
     def gen_data(
         self, method: ERModelInterface, dataset_query: str, for_training: bool
     ):
         parsed_dsquery = DatasetQuery.from_string(dataset_query)
 
@@ -194,15 +183,15 @@
         else:
             with builddir.reserve_and_track() as builddir_path:
                 pass
 
         self.logger.debug(
             "Cache common model data to a build directory: {}", builddir_path
         )
-        dsdict = self.dataset_actor.run_dataset(dataset_query)
+        dsdict = self.dataset_actor.run(dataset_query)
         out = MyDatasetDict(parsed_dsquery.dataset, {})
         for split, ds in dsdict.items():
             out[split] = method.gen_data(ds, for_training=for_training)
 
         return out
 
     def get_cache_key(
@@ -219,24 +208,26 @@
             {
                 "state": state.to_dict(),
                 "dsquery": dataset_query,
                 "for_training": for_training,
             }
         )
 
-    def get_cache_dirname(
+    def get_cache_filename(
         self,
         method: ERModelInterface,
         dataset_query: str,
         for_training: bool,
     ):
-        return slugify(
-            f"{method.__class__.__name__}_{getattr(method, 'VERSION')}_{DatasetQuery.from_string(dataset_query).dataset}_{for_training}"
-        ).replace("-", "_")
+        return (
+            slugify(
+                f"{method.__class__.__name__}_{getattr(method, 'VERSION')}_{dataset_query}_{for_training}"
+            ).replace("-", "_")
+            + ".pkl.lz4"
+        )
 
 
-ERModelDataActor.run_dataset = Cache.cls.dir(
+ERModelDataActor.run = Cache.cls.file(
     cls=MyDatasetDict,
     cache_key=ERModelDataActor.get_cache_key,
-    dirname=ERModelDataActor.get_cache_dirname,
-    compression="lz4",
-)(ERModelDataActor.run_dataset)
+    filename=ERModelDataActor.get_cache_filename,
+)(ERModelDataActor.run)
```

### Comparing `ned-1.11.1/ned/actors/evaluate_helper.py` & `ned-1.7.0/ned/actors/evaluate_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-from collections import defaultdict
 import json
 from dataclasses import dataclass, field
-from pathlib import Path
-from typing import List, Literal, Mapping, Optional, Union, Generator, Sequence
-from kgdata.wikidata.db import WikidataDB
-from kgdata.wikidata.models.wdentity import WDEntity
-from ned.actors.db import to_wikidata_db
-from ned.data_models.pymodels import CellLink
+from typing import List, Literal, Optional
 
 import numpy as np
 from loguru import logger as glogger
 from osin.apis.remote_exp import RemoteExpRun
 from osin.types import OTable
 from osin.types.primitive_type import NestedPrimitiveOutput
-from osin.types.pyobject.html import OHTML, OListHTML
-from sm.dataset import Example
-from sm.misc.ray_helper import enhance_error_info
-from sm.namespaces.wikidata import WikidataNamespace
-from tqdm.auto import tqdm
+from tqdm import tqdm
 
 import ned.metrics as ned_metrics
 from ned.data_models.prelude import (
     DatasetCandidateEntities,
     NEDExample,
     NO_ENTITY,
     NIL_ENTITY,
@@ -49,96 +39,194 @@
         metadata={
             "help": "If True, ignore non-entity cell when evaluating entity linking."
         },
     )
 
 
 def evaluate(
-    entities: Mapping[str, WDEntity],
     examples: List[NEDExample],
     entity_columns: List[List[int]],
     candidates: DatasetCandidateEntities,
     eval_ignore_nil: bool = True,
     eval_ignore_non_entity_cell: bool = True,
     dsname: str = "",
     logger=None,
     exprun: Optional[RemoteExpRun] = None,
     verbose: bool = True,
     report_unique: bool = True,
-    exprun_type: Literal["cell", "table"] = "table",
-    top_ks: list[int] = [1, 5, 20, 100, 1000],
+    exprun_type: Literal["cell", "table"] = "cell",
 ):
     logger = logger or glogger
-    queries, ytrue, ypreds = defaultdict(list), [], []
-
-    for ei, example in enumerate(
-        tqdm(
-            examples,
-            disable=not verbose,
-            desc="evaluating" + (" " + dsname if dsname != "" else ""),
-        )
+    ytrue = []
+    ypreds = []
+    queries = {}
+    top_ks = [1, 5, 20, 100, 1000]
+
+    for ei, example in tqdm(
+        enumerate(examples),
+        disable=not verbose,
+        desc="evaluating" + (" " + dsname if dsname != "" else ""),
     ):
-        equery, eytrue, eypreds = evaluate_example(
-            example,
-            entity_columns[ei],
-            candidates,
-            eval_ignore_nil,
-            eval_ignore_non_entity_cell,
-        )
-        ytrue.extend(eytrue)
-        ypreds.extend(eypreds)
+        eytrue = []
+        eypreds = []
+        otbl = []
+
+        nrows, ncols = example.cell_links.shape()
+        pred_entity_columns = set(entity_columns[ei])
+
+        for ci in pred_entity_columns.union(example.entity_columns):
+            if ci not in example.entity_columns or ci not in pred_entity_columns:
+                continue
+
+            for ri in range(nrows):
+                link = example.cell_links[ri, ci]
 
-        if exprun is not None:
-            if exprun_type == "cell":
-                for expex in report_cell_level(
-                    example,
-                    entity_columns[ei],
-                    candidates,
-                    eval_ignore_nil,
-                    eval_ignore_non_entity_cell,
-                ):
-                    exprun.update_example_output(**expex)
-            elif exprun_type == "table":
-                exprun.update_example_output(
-                    **report_table_level(
-                        entities, ei, example, candidates, eytrue, eypreds, top_ks
+                if eval_ignore_non_entity_cell and link is None:
+                    # link is None, the cell is not linked to any entity
+                    continue
+
+                if eval_ignore_nil and link is not None and len(link.entities) == 0:
+                    # the cell is linked to NIL entity
+                    continue
+
+                if link is None:
+                    gold_entities = {NO_ENTITY}
+                elif len(link.entities) == 0:
+                    gold_entities = {NIL_ENTITY}
+                else:
+                    gold_entities = {ent.id for ent in link.entities}
+
+                query = str(example.table[ri, ci])
+                if candidates.has_cell_candidates(example.table.table_id, ri, ci):
+                    cans = candidates.get_cell_candidates(
+                        example.table.table_id, ri, ci
                     )
-                )
+                else:
+                    cans = CellCandidateEntities.empty()
 
-        if report_unique:
-            for i, query in enumerate(equery):
-                if all(res["entities"] != eytrue[i] for res in queries.get(query, [])):
+                # sort by negative score for stable descending order ([::-1] won't work correctly)
+                sortedindex = np.argsort(-cans.score, kind="stable")
+                can_ids = cans.id[sortedindex]
+
+                assert len(gold_entities) > 0, "Does not handle NIL yet"
+                eytrue.append(gold_entities)
+                eypreds.append(can_ids)
+
+                is_new = query not in queries
+                if query not in queries:
+                    queries[query] = [
+                        {
+                            "entities": gold_entities,
+                            "candidate_ids": can_ids,
+                        }
+                    ]
+                elif all(res["entities"] != gold_entities for res in queries[query]):
                     # same query but mapped to different entities, it is a new example
                     queries[query].append(
                         {
-                            "entities": eytrue[i],
-                            "candidate_ids": eypreds[i],
+                            "entities": gold_entities,
+                            "candidate_ids": can_ids,
                         }
                     )
+                    is_new = True
+
+                if exprun is not None:
+                    if is_new and exprun_type == "cell":
+                        otbl = []
+                        max_rank = max(10000, len(cans) + 100)
+                        rank = max_rank
+                        for i, idx in enumerate(sortedindex):
+                            can_id = cans.id[idx]
+                            otbl.append(
+                                {
+                                    "id": can_id,
+                                    "table": example.table.table_id,
+                                    "row": ri,
+                                    "label": str(cans.label[idx]),
+                                    "score": float(cans.score[idx]),
+                                    "found": can_id in gold_entities,
+                                }
+                            )
+                            if can_id in gold_entities:
+                                rank = i + 1
+                        exprun.update_example_output(
+                            example_id=query.replace("/", "-slash-")
+                            if query != ""
+                            else "<empty>",
+                            example_name=query,
+                            primitive={
+                                "id": " | ".join(gold_entities),
+                                "found": rank < max_rank,
+                                "rank": rank,
+                            },
+                            complex={"candidates": OTable(otbl)},
+                        )
+                    elif exprun_type == "table":
+                        max_rank = max(10000, len(cans) + 100)
+                        otbl.append(
+                            {
+                                "row": ri,
+                                "col": ci,
+                                "cell": query,
+                                "gold": " | ".join(gold_entities),
+                                "rank": int(t[0]) + 1
+                                if len(
+                                    t := [
+                                        i
+                                        for i, idx in enumerate(sortedindex)
+                                        if cans.id[idx] in gold_entities
+                                    ]
+                                )
+                                > 0
+                                else max_rank,
+                            }
+                        )
+
+        ytrue.extend(eytrue)
+        ypreds.extend(eypreds)
+
+        if exprun_type == "table" and exprun is not None:
+            # each example is a table
+            exprun.update_example_output(
+                example_id=str(ei),
+                example_name=example.table.table_id,
+                primitive={
+                    "total": len(eytrue),
+                    "mrr": ned_metrics.mrr(eytrue, eypreds),
+                    "recall": ned_metrics.recall(eytrue, eypreds, top_ks),
+                },  # type: ignore
+                complex={
+                    "candidates": OTable(otbl),
+                    "columns": OTable(
+                        [
+                            {
+                                "column": example.table.columns[ci].clean_name or "",
+                                "column_index": ci,
+                                "type_id": ctype.id,
+                                "type_name": ctype.label,
+                            }
+                            for ci, ctypes in zip(
+                                example.entity_columns, example.entity_column_types
+                            )
+                            for ctype in ctypes
+                        ]
+                    ),
+                },  # type: ignore
+            )
+            otbl = []
 
     # sort the candidates by their score (bigger is better)
     recall = ned_metrics.recall(ytrue, ypreds, k=top_ks)
     mrr = ned_metrics.mrr(ytrue, ypreds)
     logger.info(
-        "dsname = {} | total = {} | mrr = {:.5f} | metrics: {}",
-        dsname,
+        "total = {} | mrr = {:.5f} | metrics: {}",
         len(ytrue),
         mrr,
         json.dumps(recall, indent=4),
     )
-    # fmt: off
-    logger.info(
-        "for copying...\nrun-id\tmrr\t{}\n{}",
-        "\t".join(f"{k}"for k in recall.keys()),
-        ",".join(
-            [str(0 if exprun is None else exprun.id)] +
-            ["%.5f" % x for x in [mrr]] +
-            ["%.2f" % x for x in recall.values()]
-    ))
-    # fmt: on
 
     if report_unique:
         unique_ytrue = []
         unique_ypreds = []
         for res in queries.values():
             for obj in res:
                 unique_ytrue.append(obj["entities"])
@@ -148,24 +236,14 @@
         unique_mrr = ned_metrics.mrr(unique_ytrue, unique_ypreds)
         logger.info(
             "unique total = {} | unique mrr = {:.5f} | unique metrics: {}",
             len(unique_ytrue),
             unique_mrr,
             json.dumps(unique_recall, indent=4),
         )
-        # fmt: off
-        logger.info(
-            "for copying...\nrun-id\tmrr\tunique-mrr\t{}\n{}",
-            "\t".join(f"uni-{k}"for k in unique_recall.keys()),
-            ",".join(
-                [str(0 if exprun is None else exprun.id)] +
-                ["%.5f" % x for x in [mrr, unique_mrr]] +
-                ["%.2f" % x for x in unique_recall.values()]
-        ))
-        # fmt: on
 
     if exprun is not None:
         primitive = {
             "total": len(ytrue),
             "mrr": mrr,
             "recall": recall,
         }
@@ -178,290 +256,7 @@
                 }
             )
         exprun.update_output(
             primitive=primitive,
         )
 
     return {"recall": recall, "mrr": mrr, "total": len(ytrue)}
-
-
-def evaluate_example(
-    example: NEDExample,
-    entity_columns: list[int],
-    candidates: DatasetCandidateEntities,
-    eval_ignore_nil: bool = True,
-    eval_ignore_non_entity_cell: bool = True,
-):
-    equery = []
-    eytrue = []
-    eypreds = []
-
-    for ri, ci, link in iter_eval_cell(
-        example, entity_columns, eval_ignore_nil, eval_ignore_non_entity_cell
-    ):
-        if link is None:
-            gold_entities = {NO_ENTITY}
-        elif len(link.entities) == 0:
-            gold_entities = {NIL_ENTITY}
-        else:
-            gold_entities = set(link.entities)
-
-        query = str(example.table[ri, ci])
-        if candidates.has_cell_candidates(example.table.table_id, ri, ci):
-            cans = candidates.get_cell_candidates(example.table.table_id, ri, ci)
-        else:
-            cans = CellCandidateEntities.empty()
-
-        # sort by negative score for stable descending order ([::-1] won't work correctly)
-        sortedindex = np.argsort(-cans.score, kind="stable")
-        can_ids = cans.id[sortedindex]
-
-        assert len(gold_entities) > 0, "Does not handle NIL yet"
-        equery.append(query)
-        eytrue.append(gold_entities)
-        eypreds.append(can_ids)
-
-    return equery, eytrue, eypreds
-
-
-def report_cell_level(
-    example: NEDExample,
-    entity_columns: list[int],
-    candidates: DatasetCandidateEntities,
-    eval_ignore_nil: bool = True,
-    eval_ignore_non_entity_cell: bool = True,
-) -> list[dict]:
-    exp_examples = []
-
-    for ri, ci, link in iter_eval_cell(
-        example, entity_columns, eval_ignore_nil, eval_ignore_non_entity_cell
-    ):
-        query = str(example.table[ri, ci])
-
-        if link is None:
-            gold_entities = {NO_ENTITY}
-        elif len(link.entities) == 0:
-            gold_entities = {NIL_ENTITY}
-        else:
-            gold_entities = set(link.entities)
-
-        if candidates.has_cell_candidates(example.table.table_id, ri, ci):
-            cans = candidates.get_cell_candidates(example.table.table_id, ri, ci)
-        else:
-            cans = CellCandidateEntities.empty()
-
-        # sort by negative score for stable descending order ([::-1] won't work correctly)
-        sortedindex = np.argsort(-cans.score, kind="stable")
-
-        # each exp example is a cell
-        max_rank = max(10000, len(cans) + 100)
-        rank = max_rank
-        otable = []
-        for i, idx in enumerate(sortedindex):
-            can_id = cans.id[idx]
-            otable.append(
-                {
-                    "id": can_id,
-                    "table": example.table.table_id,
-                    "row": ri,
-                    "label": str(cans.label[idx]),
-                    "score": float(cans.score[idx]),
-                    "found": can_id in gold_entities,
-                }
-            )
-            if can_id in gold_entities:
-                rank = i + 1
-
-        exp_examples.append(
-            {
-                "example_id": query.replace("/", "-slash-")
-                if query != ""
-                else "<empty>",
-                "example_name": query,
-                "primitive": {
-                    "id": " | ".join(gold_entities),
-                    "found": rank < max_rank,
-                    "rank": rank,
-                },
-                "complex": {"candidates": OTable(otable)},
-            }
-        )
-
-    return exp_examples
-
-
-def report_table_level(
-    entities: Mapping[str, WDEntity],
-    example_index: int,
-    example: NEDExample,
-    candidates: DatasetCandidateEntities,
-    eytrue: list[set[str]],
-    eypreds: list[list[str]],
-    top_ks: Sequence[Optional[int]],
-) -> dict:
-
-    return {
-        "example_id": "%03d" % example_index,
-        "example_name": example.table.table_id,
-        "primitive": {
-            "total": len(eytrue),
-            "mrr": ned_metrics.mrr(eytrue, eypreds),
-            "recall": ned_metrics.recall(eytrue, eypreds, top_ks),
-        },
-        "complex": {
-            "table": AuxComplexTableObject(entities).get_table(example, candidates),
-            "columns": OTable(
-                [
-                    {
-                        "column": example.table.columns[ci].clean_name or "",
-                        "column_index": ci,
-                        "type_id": ctype.entity,
-                        "type_name": entities[ctype.entity].label,
-                    }
-                    for ci, ctypes in zip(
-                        example.entity_columns, example.entity_column_types
-                    )
-                    for ctype in ctypes
-                ]
-            ),
-        },
-    }
-
-
-def iter_eval_cell(
-    example: NEDExample,
-    entity_columns: list[int],
-    eval_ignore_nil: bool = True,
-    eval_ignore_non_entity_cell: bool = True,
-) -> Generator[tuple[int, int, Optional[CellLink]], None, None]:
-    nrows, ncols = example.cell_links.shape()
-    for ci in set(entity_columns).union(example.entity_columns):
-        for ri in range(nrows):
-            link = example.cell_links[ri, ci]
-
-            if eval_ignore_non_entity_cell and link is None:
-                # link is None, the cell is not linked to any entity
-                continue
-
-            if eval_ignore_nil and link is not None and len(link.entities) == 0:
-                # the cell is linked to NIL entity
-                continue
-
-            yield ri, ci, link
-
-
-class AuxComplexTableObject:
-    def __init__(
-        self,
-        entities: Mapping[str, WDEntity],
-    ) -> None:
-        self.wdns = WikidataNamespace.create()
-        self.entities = entities
-
-    def get_table(
-        self, example: NEDExample, ex_candidates: Optional[DatasetCandidateEntities]
-    ) -> OTable:
-        nrows, ncols = example.table.shape()
-        columns = [
-            f"{ci}. " + (c.clean_name or "")
-            for ci, c in enumerate(example.table.columns)
-        ]
-        return OTable(
-            [
-                {
-                    columns[ci]: self._get_cell(example, ex_candidates, ri, ci)
-                    for ci in range(ncols)
-                }
-                for ri in range(nrows)
-            ]
-        )
-
-    def _get_cell(
-        self,
-        example: NEDExample,
-        ex_candidates: Optional[DatasetCandidateEntities],
-        row: int,
-        col: int,
-    ):
-        from htbuilder import a, b, code, div, li, pre, span, ul
-
-        cell_link = example.cell_links[row, col]
-        if cell_link is None:
-            return str(example.table[row, col])
-
-        cell = str(example.table[row, col])
-        ent_el = []
-        can_el = []
-
-        for entid in cell_link.entities:
-            for start, end in cell_link.mentions[entid]:
-                x = div(style="margin-left: 8px")(
-                    "-&nbsp;",
-                    a(href=self.wdns.get_entity_abs_uri(entid))(f"{cell[start:end]}: "),
-                    span(
-                        a(href=self.wdns.get_entity_abs_uri(entid))(entid),
-                    ),
-                )
-                popx = div(self.get_ent_label_with_description(entid))
-                ent_el.append(OHTML(str(x), str(popx)))
-
-        gold_ents = set(cell_link.entities)
-
-        if ex_candidates is not None:
-            # showing the top 5 candidates, as longer won't give more info.
-            cans = ex_candidates.get_cell_candidates(example.table.table_id, row, col)
-            # sort by negative score for stable descending order ([::-1] won't work correctly)
-            sortedindex = np.argsort(-cans.score, kind="stable")
-            discans = [
-                (i, cans.get_candidate_by_index(oi))
-                for i, oi in enumerate(sortedindex[:5])
-            ]
-            if all(can.entity.id not in gold_ents for _, can in discans):
-                # add missing pred gold
-                discans.extend(
-                    [
-                        (i, cans.get_candidate_by_index(oi))
-                        for i, oi in enumerate(sortedindex)
-                        if cans.id[oi] in gold_ents
-                    ]
-                )
-
-            for i, canid in discans:
-                x = div(style="margin-left: 8px")(
-                    f"- {i}.&nbsp;",
-                    span(
-                        "(",
-                        code(style="color: green; font-weight: bold")("C"),
-                        ")&nbsp;",
-                    )
-                    if canid.entity.id in gold_ents
-                    else "",
-                    a(href=self.wdns.get_entity_abs_uri(canid.entity.id))(
-                        canid.entity.id
-                    ),
-                    ": ",
-                    span(title=canid.score)(round(canid.score, 4)),
-                )
-                popx = self.get_ent_label_with_description(canid.entity.id)
-                can_el.append(OHTML(str(x), str(popx)))
-
-        items = [
-            OHTML(
-                str(
-                    span(
-                        b("Cell: "),
-                        cell,
-                    )
-                ),
-            ),
-            OHTML(str(b("Ground-truth: "))),
-            *ent_el,
-            OHTML(str(b("Candidates: "))),
-            *can_el,
-        ]
-        return OListHTML(items)
-
-    def get_ent_label_with_description(self, entid: str):
-        if entid not in self.entities:
-            return entid
-        ent = self.entities[entid]
-        return f"{ent.label} ({entid}): {ent.description}"
```

### Comparing `ned-1.11.1/ned/candidate_generation/oracle_semtyper.py` & `ned-1.7.0/ned/candidate_generation/oracle_semtyper.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,23 +36,18 @@
 class OracleSemTyperArgs(PyseriniArgs):
     filter_mode: FilterMode = "exact"
 
 
 class OracleSemTyper(CandidateRankingComplexMethod):
     VERSION = PyseriniWrapper.VERSION
 
-    def __init__(
-        self,
-        pyserini_wrapper: PyseriniWrapper,
-        db: WikidataDB,
-        args: OracleSemTyperArgs,
-    ):
+    def __init__(self, pyserini_wrapper: PyseriniWrapper, args: OracleSemTyperArgs):
         self.pyserini_wrapper = pyserini_wrapper
         self.args = args
-        self.db = db
+        self.db = WikidataDB.get_instance()
 
     def get_candidates(
         self, examples: list[NEDExample], entity_columns: list[list[int]]
     ) -> DatasetCandidateEntities:
         candidates = self.pyserini_wrapper.get_candidates(examples, entity_columns)
         indexchecker = ContiguousIndexChecker()
 
@@ -81,15 +76,15 @@
                 #     {ent.id for ent in entity_column_types[ci]},
                 #     self.args.filter_mode,
                 # )
                 rayargs.append(
                     (
                         dbref,
                         cans,
-                        {ent.entity for ent in entity_column_types[ci]},
+                        {ent.id for ent in entity_column_types[ci]},
                         self.args.filter_mode,
                     )
                 )
                 provenanceargs.append((tid, ci))
 
         resp = ray_map(filter_column_candidates_by_types.remote, rayargs)
         filtered_cans = defaultdict(dict)
```

### Comparing `ned-1.11.1/ned/candidate_generation/pyserini/analyzer.py` & `ned-1.7.0/ned/candidate_generation/pyserini/analyzer.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_generation/pyserini/configuration.py` & `ned-1.7.0/ned/candidate_generation/pyserini/configuration.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_generation/pyserini/search.py` & `ned-1.7.0/ned/candidate_generation/pyserini/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,31 +56,28 @@
         self.analyzer = self.index_settings.get_analyzer()
         self.lucene_analyzer = Analyzer(get_lucene_analyzer())
         n_processes = os.cpu_count()
         assert isinstance(n_processes, int)
         self.n_processes = n_processes
 
     def search(
-        self, query: Union[str, JQuery], limit: int = 10, pre_analyzed: bool = False
+        self, query: str, limit: int = 10, pre_analyzed: bool = False
     ) -> List[SearchReturnType]:
         if not pre_analyzed:
             query = self.analyzer(query)
         res = self.searcher.search(query, k=limit)
         return [
             SearchReturnType(
                 docid=x.docid, score=x.score, docraw=x.raw, contents=x.contents
             )
             for x in res
         ]
 
     def batch_search(
-        self,
-        queries: List[Union[str, JQuery]],
-        limit: int = 10,
-        pre_analyzed: bool = False,
+        self, queries: List[str], limit: int = 10, pre_analyzed: bool = False
     ) -> List[List[SearchReturnType]]:
         if not pre_analyzed:
             queries = [self.analyzer(query) for query in queries]
 
         query_ids = [str(i) for i in range(len(queries))]
 
         if len(queries) > 0 and isinstance(queries[0], str):
```

### Comparing `ned-1.11.1/ned/candidate_generation/table_linker.py` & `ned-1.7.0/ned/candidate_generation/table_linker.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/columnwise_model.py` & `ned-1.7.0/ned/candidate_ranking/columnwise_model.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/contrastive_pairwise_model.py` & `ned-1.7.0/ned/candidate_ranking/contrastive_pairwise_model.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/cr_dataset.py` & `ned-1.7.0/ned/candidate_ranking/cr_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from typing import Literal, Optional
-from kgdata.wikidata.db import WikidataDB
 
 import numpy as np
 import ray
 import torch
 from loguru import logger
 from ream.actor_state import ActorState
 from ream.actors.base import BaseActor
@@ -17,94 +16,95 @@
 from ream.dataset_helper import DatasetQuery
 from ream.helper import orjson_dumps
 from ream.params_helper import NoParams
 from slugify import slugify
 from tqdm import tqdm
 
 from ned.actors.candidate_generation import CanGenActor
-from ned.actors.dataset.prelude import NEDDatasetActor
+from ned.actors.dataset import NEDDatasetActor
 from ned.candidate_ranking.cr_method import CandidateRankingMethod
 from ned.candidate_ranking.dataset.base import (
     CRDatasetCan,
     CRDatasetEnt,
 )
 from ned.candidate_ranking.dataset.basic_features import CRDatasetFeatures
 from ned.candidate_ranking.dataset.matched_prop_feature import CRDatasetMatchedProps
 from ned.candidate_ranking.dataset.types import CRDatasetTypes
 from ned.candidate_ranking.helpers.dataset import MyDatasetDict
 from ned.data_models.prelude import DatasetCandidateEntities
 from ned.data_models.pymodels import NEDExample
 
 
 class CRDataset(Cacheable):
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetEnt,
         cache_args=["provenance"],
         mem_persist=True,
+        fileext="parq",
         compression="lz4",
     )
     def base_ent(
         self,
         examples: list[NEDExample],
         candidates: DatasetCandidateEntities,
         provenance: str = "",
     ):
-        return CRDatasetEnt.create(WikidataDB.get_instance(), examples, candidates)
+        return CRDatasetEnt.create(examples, candidates)
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetCan,
         cache_args=["provenance"],
         mem_persist=True,
+        fileext="parq",
         compression="lz4",
     )
     def base_can(
         self,
         examples: list[NEDExample],
         candidates: DatasetCandidateEntities,
         provenance: str = "",
     ):
         return CRDatasetCan.create(examples, candidates)
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetFeatures,
         cache_args=["provenance"],
         mem_persist=True,
+        fileext="parq",
         compression="lz4",
     )
     def can_features(
         self,
         candidates: DatasetCandidateEntities,
         basecan: CRDatasetCan,
         provenance: str = "",
     ):
         return CRDatasetFeatures.create(
             basecan.cell, candidates.label, candidates.aliases, candidates.popularity
         )
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=[DatasetCandidateEntities, CRDatasetFeatures, CRDatasetCan],
         cache_args=["top_k", "provenance"],
         mem_persist=True,
+        fileext="parq",
     )
     def can_topk(
         self,
         candidates: DatasetCandidateEntities,
         can_feats: Optional[CRDatasetFeatures] = None,
         can_base: Optional[CRDatasetCan] = None,
         baseent: Optional[CRDatasetEnt] = None,
         top_k: int = 100,
-        remove_nil_entity: bool = False,
         provenance: str = "",
     ) -> tuple[
         DatasetCandidateEntities, Optional[CRDatasetFeatures], Optional[CRDatasetCan]
     ]:
-        # assume that the candidates's scores are already computed.
-        newcandidates, index_remap = candidates.top_k_candidates(
-            top_k, baseent, return_index_remap=True, remove_nil_entity=remove_nil_entity
-        )
+        # assume that the candidates are already sorted by the score.
+        newcandidates, index_remap = candidates.top_k_candidates(top_k, baseent, True)
         if can_feats is None and can_base is None:
             return newcandidates, None, None
 
         newidx = np.arange(len(newcandidates))
         ent_item_flag = index_remap == -1
         can_item_flag = index_remap != -1
 
@@ -161,70 +161,68 @@
         if can_base is not None:
             if baseent is not None and impute_pos.shape[0] > 0:
                 cell = np.empty(len(newcandidates), dtype=can_base.cell.dtype)
                 cell_id = np.empty(len(newcandidates), dtype=can_base.cell_id.dtype)
                 table_index = np.empty(
                     len(newcandidates), dtype=can_base.table_index.dtype
                 )
-                row_index = np.empty(len(newcandidates), dtype=can_base.row_index.dtype)
                 col_index = np.empty(len(newcandidates), dtype=can_base.col_index.dtype)
                 is_correct = np.empty(
                     len(newcandidates), dtype=can_base.is_correct.dtype
                 )
 
                 can_index = newidx[can_item_flag]
                 can_old_index = index_remap[can_item_flag]
                 cell[can_index] = can_base.cell[can_old_index]
                 cell_id[can_index] = can_base.cell_id[can_old_index]
                 table_index[can_index] = can_base.table_index[can_old_index]
-                row_index[can_index] = can_base.row_index[can_old_index]
                 col_index[can_index] = can_base.col_index[can_old_index]
                 is_correct[can_index] = can_base.is_correct[can_old_index]
 
                 cell[impute_pos] = baseent.cell[ent_index]
                 cell_id[impute_pos] = baseent.cell_id[ent_index]
                 table_index[impute_pos] = baseent.table_index[ent_index]
-                row_index[impute_pos] = baseent.row_index[ent_index]
                 col_index[impute_pos] = baseent.col_index[ent_index]
                 is_correct[impute_pos] = 1
                 can_base = CRDatasetCan(
-                    cell, cell_id, table_index, row_index, col_index, is_correct
+                    cell, cell_id, table_index, col_index, is_correct
                 )
             else:
                 can_base = CRDatasetCan(
                     can_base.cell[index_remap],
                     can_base.cell_id[index_remap],
                     can_base.table_index[index_remap],
-                    can_base.row_index[index_remap],
                     can_base.col_index[index_remap],
                     can_base.is_correct[index_remap],
                 )
 
         return newcandidates, can_feats, can_base
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetTypes,
         cache_args=["extended_mode", "provenance"],
         mem_persist=True,
+        fileext="parq",
     )
     def can_types(
         self,
         examples: list[NEDExample],
         candidates: DatasetCandidateEntities,
         extended_mode: Literal[
             "no", "parent1", "child_parent2prime", "clustered_parent1"
         ] = "no",
         provenance: str = "",
     ):
         return CRDatasetTypes.create(examples, candidates, extended_mode=extended_mode)
 
-    @Cache.cls.dir(
+    @Cache.cls.file(
         cls=CRDatasetMatchedProps,
         cache_args=["provenance"],
         mem_persist=True,
+        fileext="parq",
     )
     def can_matched_props(
         self,
         examples: list[NEDExample],
         candidates: DatasetCandidateEntities,
         provenance: str = "",
     ):
@@ -479,15 +477,15 @@
             with builddir.reserve_and_track() as builddir_path:
                 pass
         self.logger.debug(
             "Cache common sub-datasets to a build directory: {}", builddir_path
         )
 
         self.logger.debug("Retrieve candidates of dataset: {}", dsquery)
-        dsdict = self.dataset_actor.run_dataset(dsquery)
+        dsdict = self.dataset_actor.run(dsquery)
         cangen_dsdict = self.cangen_actor.run_dataset(dsquery)
         # # fmt: off
         # from pathlib import Path
         # Path("/tmp/test.csv").write_text("\n".join(cangen_dsdict['train'].id))
         # # fmt: on
         self.logger.debug("Extract features of dataset: {}", dsquery)
         canrank_dsdict = MyDatasetDict(dsquery_.dataset, {})
@@ -519,25 +517,25 @@
         state = ActorState.create(
             method.__class__, method.get_generating_dataset_args(), dependencies=deps
         )
         return orjson_dumps(
             {"state": state.to_dict(), "dsquery": dsquery, "for_training": for_training}
         )
 
-    def get_cache_dirname(
+    def get_cache_filename(
         self: CanRankDataset,
         method: CandidateRankingMethod,
         dsquery: str,
         for_training: bool = False,
         num_proc: Optional[int] = None,
     ):
         return slugify(
             f"{method.__class__.__name__}_{getattr(method, 'VERSION')}_{dsquery}_{for_training}"
         ).replace("-", "_")
 
 
 # CanRankDataset.run = CanRankDataset.run_without_cache
-CanRankDataset.run_dataset = Cache.cls.dir(
+CanRankDataset.run = Cache.cls.file(
     cls=MyDatasetDict,
     cache_key=CanRankDataset.get_cache_key,
-    dirname=CanRankDataset.get_cache_dirname,
+    filename=CanRankDataset.get_cache_filename,
 )(CanRankDataset.run_without_cache)
```

### Comparing `ned-1.11.1/ned/candidate_ranking/cr_method.py` & `ned-1.7.0/ned/candidate_ranking/cr_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,20 +98,15 @@
             batch_size=self.EVAL_BATCH_SIZE,
             shuffle=False,
             pin_memory=params.is_cuda,
         )
 
         with torch.no_grad():
             probs = []
-            for batch in tqdm(
-                dloader,
-                total=len(dloader),
-                desc="ranking candidates in a dataset",
-                disable=not verbose,
-            ):
+            for batch in tqdm(dloader, total=len(dloader), disable=not verbose):
                 kwargs = {}
                 for arg in self.EXPECTED_EVAL_ARGS:
                     kwargs[arg] = batch[arg].to(device)
                 output = self.forward(**kwargs)
                 probs.append(output.probs.cpu())
 
             probs = torch.cat(probs)
```

### Comparing `ned-1.11.1/ned/candidate_ranking/cr_searchscore.py` & `ned-1.7.0/ned/candidate_ranking/cr_searchscore.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/cr_string_similarity.py` & `ned-1.7.0/ned/candidate_ranking/cr_string_similarity.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/cr_training.py` & `ned-1.7.0/ned/candidate_ranking/cr_training.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,169 +1,164 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from contextlib import contextmanager
 from os import cpu_count
 from pathlib import Path
-from typing import TYPE_CHECKING, Literal, Optional, Tuple
+from typing import TYPE_CHECKING, Tuple
 
 import evaluate
 from ned.candidate_ranking.cr_dataset import NoCacheCRDataset
 from ned.data_models.pymodels import Entity
 import orjson
 import torch
-from torch.utils.data import DataLoader
 import wandb.util
 from accelerate import Accelerator
 from accelerate.utils import set_seed
 from loguru import logger
-from tqdm.auto import tqdm
+from tqdm import tqdm
 import serde.json
 import wandb
 from ned.candidate_ranking.columnwise_model import ColumnwiseModel
 from ned.candidate_ranking.cr_method import CandidateRankingMethod
 from ned.candidate_ranking.helpers import SmoothingMetric, describe, loop_dl
 from ned.candidate_ranking.helpers.training_helper import (
     CkptHelper,
-    ModifiedTrainingArguments,
     calculate_balanced_class_weights,
     get_data_loader,
 )
 from ned.candidate_ranking.pairwise_model import PairwiseModel
 from sm.prelude import M
 
 if TYPE_CHECKING:
     from ned.actors.candidate_ranking import CanRankActor
 
 
 def cr_training(
-    actor: CanRankActor, ckpt_helper: CkptHelper, eval_ds_mode: Literal["train", "test"]
+    actor: CanRankActor, ckpt_helper: CkptHelper
 ) -> Tuple[CandidateRankingMethod, Path]:
-    """
-    Args:
-        actor: can rank actor from which we get all necessary information
-        ckpt_helper: helper to deal with saving and resuming training
-        eval_ds_mode: whether to create dev/test datasets for_training mode.
-    """
-
     # --------------------------------------------------------------------------------
     # prepare parameters and configurations
     logger.info("Saving checkpoints to {}", ckpt_helper.ckpt_dir)
 
     params = actor.params
     trainargs = params.training
 
     assert trainargs is not None
     assert trainargs.logging_strategy == "steps"
 
+    use_wandb = "wandb" in M.assert_not_null(trainargs.report_to)
+
+    # https://huggingface.co/docs/accelerate/concept_guides/performance#setting-the-seed
+    # one command to rule all the seeds
+    set_seed(72)
+
     if params.method == "columnwise":
         trainargs.per_device_train_batch_size = 1
         trainargs.per_device_eval_batch_size = 1
 
-    # --------------------------------------------------------------------------------
-    # prepare datasets
+    if use_wandb:
+        resume = None
+        if ckpt_helper.is_resuming():
+            restore_traindir = ckpt_helper.get_restore_training_dir()
+            assert restore_traindir is not None
+            if (restore_traindir / "wandb.json").exists():
+                id = serde.json.deser(restore_traindir / "wandb.json")["id"]
+                resume = "allow"
+
+        if resume is None:
+            id = wandb.util.generate_id()
+
+        if not (ckpt_helper.get_training_dir() / "wandb.json").exists():
+            (ckpt_helper.get_training_dir() / "wandb.json").write_bytes(
+                orjson.dumps(
+                    {
+                        "id": id,  # type: ignore
+                    }
+                )
+            )
+
+        wandb.init(
+            id=id,  # type: ignore
+            project="ned",
+            config={
+                "method": params.method,
+                "ckpt_dir": ckpt_helper.ckpt_dir,
+                "dataset": trainargs.dataset,
+            },
+            resume=resume,
+        )
+
     accelerator = Accelerator()
-    set_seed(trainargs.seed)
+
     model = actor.get_method()
+    model_argnames = model.EXPECTED_ARGS
+    model_evalargnames = model.EXPECTED_EVAL_ARGS
+
+    # --------------------------------------------------------------------------------
+    # prepare datasets
 
     with accelerator.main_process_first():
-        train_ds = actor.canrank_dataset.run_dataset(
+        dsdict = actor.canrank_dataset.run(
             model,
-            trainargs.train_dataset,
+            trainargs.dataset,
             for_training=True,
-        ).into_single_value()
-
-        eval_dsdict = {}
-        for eval_dsname in trainargs.eval_datasets:
-            dsdict = actor.canrank_dataset.run_dataset(
+        )
+        if params.method in {"contrastive_pairwise"}:
+            eval_dsdict = actor.canrank_dataset.run(
                 model,
-                eval_dsname,
-                for_training=eval_ds_mode == "train",
+                trainargs.dataset,
+                for_training=False,
             )
-            for name, ds in dsdict.items():
-                assert name not in eval_dsdict
-                eval_dsdict[name] = ds
-
-        assert "train" in eval_dsdict, eval_dsdict.keys()
+        else:
+            eval_dsdict = dsdict
 
     train_dl = get_data_loader(
-        train_ds, "train", trainargs.per_device_train_batch_size, shuffle=True
+        dsdict, "train", trainargs.per_device_train_batch_size, shuffle=True
     )
     eval_dls = {
         split: get_data_loader(
-            eval_ds, split, trainargs.per_device_eval_batch_size, shuffle=False
+            dsdict, split, trainargs.per_device_eval_batch_size, shuffle=False
         )
-        for split, eval_ds in eval_dsdict.items()
+        for split in eval_dsdict.keys()
     }
 
     # --------------------------------------------------------------------------------
     # prepare the model
 
     # calculate the class weights
-    if hasattr(model, "class_weights"):
-        if params.method == "pairwise":
-            assert params.pairwise is not None
-            assert isinstance(model, PairwiseModel)
-            cfg_class_weight = params.pairwise.class_weight
-        elif params.method == "columnwise":
-            assert params.columnwise is not None
-            assert isinstance(model, ColumnwiseModel)
-            cfg_class_weight = params.columnwise.class_weight
-        elif params.method == "crv3":
-            cfg_class_weight = 0
-        else:
-            raise NotImplementedError()
-
-        if cfg_class_weight == 0:
+    if params.method == "pairwise":
+        assert params.pairwise is not None
+        assert isinstance(model, PairwiseModel)
+        if params.pairwise.class_weight == 0:
             model.class_weights = calculate_balanced_class_weights(train_dl)
         else:
-            assert len(model.class_weights) == 2
-            total = 1 + cfg_class_weight
+            total = 1 + params.pairwise.class_weight
             model.class_weights[0] = 1 / total
             model.class_weights[1] = 1 - 1 / total
 
         logger.info(
             "Update the class weights of the model to be: {}", model.class_weights
         )
-
-    use_wandb = "wandb" in M.assert_not_null(trainargs.report_to)
-    with with_wandb(
-        ckpt_helper,
-        {"method": params.method, "dataset": trainargs.train_dataset},
-        enable=use_wandb,
-    ):
-        return train_loop(
-            model,
-            ckpt_helper,
-            accelerator,
-            train_dl,
-            eval_dls,
-            trainargs,
-            use_wandb,
+    elif params.method == "columnwise":
+        assert params.columnwise is not None
+        assert isinstance(model, ColumnwiseModel)
+        if params.columnwise.class_weight == 0:
+            model.class_weights = calculate_balanced_class_weights(train_dl)
+        else:
+            total = 1 + params.columnwise.class_weight
+            model.class_weights[0] = 1 / total
+            model.class_weights[1] = 1 - 1 / total
+        logger.info(
+            "Update the class weights of the model to be: {}", model.class_weights
         )
-
-
-def train_loop(
-    model: CandidateRankingMethod,
-    ckpt_helper: CkptHelper,
-    accelerator: Accelerator,
-    train_dl: DataLoader,
-    eval_dls: dict[str, DataLoader],
-    trainargs: ModifiedTrainingArguments,
-    use_wandb: bool = False,
-):
-    model_argnames = model.EXPECTED_ARGS
-    model_evalargnames = model.EXPECTED_EVAL_ARGS
+    else:
+        raise NotImplementedError()
 
     metrics = [evaluate.load(str(Path(__file__).parent / "metrics/ned_metric.py"))]
-    optimizer = torch.optim.AdamW(
-        params=model.parameters(),
-        lr=trainargs.learning_rate,
-        weight_decay=trainargs.weight_decay,
-    )
+    optimizer = torch.optim.AdamW(params=model.parameters(), lr=trainargs.learning_rate)
 
     start_step = ckpt_helper.resume_if_needed(model, optimizer)
     model, optimizer, train_dataloader = accelerator.prepare(model, optimizer, train_dl)
 
     tmp = list(eval_dls.items())
     eval_dataloaders = {
         key: dataloader
@@ -171,14 +166,15 @@
             [x[0] for x in tmp], accelerator.prepare(*[x[1] for x in tmp])
         )
     }
 
     num_epoch_steps = len(train_dl)
     num_train_steps = num_epoch_steps * int(trainargs.num_train_epochs)
     num_eval_steps = sum(len(dl) for dl in eval_dataloaders.values())
+    gradient_accumulation_steps = 1
 
     dev_check_interval, train_check_interval, ckpt_interval = trainargs.get_steps(
         num_epoch_steps
     )
 
     describe(
         "Config:",
@@ -214,22 +210,23 @@
             start_step,
             progress_bar,
             num_epoch_steps,
         ),
         start=start_step + 1,
     ):
         try:
-            with accelerator.accumulate(model):
-                outputs = model(**{name: batch[name] for name in model_argnames})
-                loss = outputs.loss
+            outputs = model(**{name: batch[name] for name in model_argnames})
+            loss = outputs.loss
+            loss = loss / gradient_accumulation_steps
 
-                step_loss += loss.item()
-                epoch_loss += loss.item()
+            step_loss += loss.item()
+            epoch_loss += loss.item()
 
-                accelerator.backward(loss)
+            accelerator.backward(loss)
+            if step % gradient_accumulation_steps == 0:
                 optimizer.step()
                 # lr_scheduler.step()
                 optimizer.zero_grad()
 
             progress_bar.update(1)
             postfix["loss"] = step_loss.mean()
 
@@ -348,48 +345,7 @@
     unwrapped_model = accelerator.unwrap_model(model)
     if latest_ckpt_file is None or (
         ckpt_interval is not None and step % ckpt_interval != 0
     ):
         latest_ckpt_file = ckpt_helper.save(step, unwrapped_model, optimizer)
 
     return unwrapped_model, latest_ckpt_file
-
-
-@contextmanager
-def with_wandb(ckpt_helper: CkptHelper, metadata: dict, enable=True):
-    if not enable:
-        yield None
-        return
-
-    resume = None
-    if ckpt_helper.is_resuming():
-        restore_traindir = ckpt_helper.get_restore_training_dir()
-        assert restore_traindir is not None
-        if (restore_traindir / "wandb.json").exists():
-            id = serde.json.deser(restore_traindir / "wandb.json")["id"]
-            resume = "allow"
-
-    if resume is None:
-        id = wandb.util.generate_id()
-
-    if not (ckpt_helper.get_training_dir() / "wandb.json").exists():
-        (ckpt_helper.get_training_dir() / "wandb.json").write_bytes(
-            orjson.dumps(
-                {
-                    "id": id,  # type: ignore
-                }
-            )
-        )
-
-    wandb.init(
-        id=id,  # type: ignore
-        project="ned",
-        config={
-            "ckpt_dir": ckpt_helper.ckpt_dir,
-            **metadata,
-        },
-        resume=resume,
-    )
-    try:
-        yield None
-    finally:
-        wandb.finish()
```

### Comparing `ned-1.11.1/ned/candidate_ranking/dataset/base.py` & `ned-1.7.0/ned/candidate_ranking/dataset/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
-from kgdata.wikidata.db import WikidataDB
 
 import numpy as np
 from nptyping import Int32, NDArray, Object, Shape, Bool
-import orjson
 from ream.data_model_helper import NumpyDataModel
 from tqdm import tqdm
 
 from ned.data_models.prelude import DatasetCandidateEntities, DatasetIndex
 from ned.data_models.pymodels import NEDExample
 
 
@@ -31,20 +29,15 @@
     entity_id: NDArray[Shape["*"], Object]
     entity_label: NDArray[Shape["*"], Object]
     entity_description: NDArray[Shape["*"], Object]
     entity_aliases: NDArray[Shape["*"], Object]
     entity_popularity: NDArray[Shape["*"], Object]
 
     @staticmethod
-    def create(
-        db: WikidataDB, examples: list[NEDExample], candidates: DatasetCandidateEntities
-    ):
-        pagerank = db.wdpagerank
-        entities = db.wdentity_metadata
-
+    def create(examples: list[NEDExample], candidates: DatasetCandidateEntities):
         index = {}
         cell = []
         cell_id = []
         table_index = []
         col_index = []
         row_index = []
         entity_id = []
@@ -65,26 +58,25 @@
                 index[tid][ci] = {}
                 for ri in cindex:
                     cell_index = cell_index_offset + ri * ncols + ci
                     rowstart = len(cell)
                     link = example.cell_links[ri, ci]
                     text = example.table[ri, ci]
                     if link is not None:
-                        for entid in link.entities:
-                            ent = entities[entid]
+                        for ent in link.entities:
                             cell.append(text)
                             cell_id.append(cell_index)
                             table_index.append(ti)
                             col_index.append(ci)
                             row_index.append(ri)
-                            entity_id.append(entid)
+                            entity_id.append(ent.id)
                             entity_label.append(ent.label)
                             entity_description.append(ent.description)
-                            entity_aliases.append(orjson.dumps(ent.aliases).decode())
-                            entity_popularity.append(pagerank[entid])
+                            entity_aliases.append(ent.aliases)
+                            entity_popularity.append(ent.popularity)
                     index[tid][ci][ri] = (rowstart, len(cell))
             cell_index_offset += nrows * ncols
 
         return CRDatasetEnt(
             index=index,
             cell=np.asarray(cell, dtype=np.object_),
             cell_id=np.asarray(cell_id, dtype=np.int32),
@@ -98,33 +90,29 @@
             entity_popularity=np.array(entity_popularity, dtype=np.float64),
         )
 
 
 class CRDatasetCan(NumpyDataModel):
     # fmt: off
     __slots__ = [
-        "cell", "cell_id", "table_index", "row_index", "col_index", "is_correct"
+        "cell", "cell_id", "table_index", "col_index", "is_correct"
     ]
     # fmt: on
     # the order of this object and candidates are the same
     cell: NDArray[Shape["*"], Object]  # content of the cell
-    # unique number for each cell across all tables
-    # calculated by (ri * ncols + ci) for each table so it can be used to retrieve row index using `get_row_index` function
-    cell_id: NDArray[Shape["*"], Int32]
+    cell_id: NDArray[Shape["*"], Int32]  # unique number for each cell across all tables
     table_index: NDArray[Shape["*"], Int32]
-    row_index: NDArray[Shape["*"], Int32]
     col_index: NDArray[Shape["*"], Int32]
     is_correct: NDArray[Shape["*"], Bool]  # whether the cell is correct
 
     @staticmethod
     def create(examples: list[NEDExample], candidates: DatasetCandidateEntities):
         cell = []
         cell_id = np.zeros_like(candidates.id, dtype=np.int32)
         table_index = np.zeros_like(candidates.id, dtype=np.int32)
-        row_index = np.zeros_like(candidates.id, dtype=np.int32)
         col_index = np.zeros_like(candidates.id, dtype=np.int32)
         is_correct = np.zeros_like(candidates.id, dtype=np.bool_)
 
         cell_index_offset = 0
         # using a pointer to make sure that the order of this object and candidates are the same
         pointer = 0
 
@@ -143,43 +131,31 @@
                     # the order is matched, move the pointer forward
                     pointer = rend
                     cell_index = cell_index_offset + ri * ncols + ci
                     cans = candidates.get_cell_candidates(tid, ri, ci)
                     cell_id[rstart:rend] = cell_index
                     table_index[rstart:rend] = ti
                     col_index[rstart:rend] = ci
-                    row_index[rstart:rend] = ri
                     cell.extend([example.table[ri, ci]] * len(cans))
 
                     link = example.cell_links[ri, ci]
                     if link is None or len(link.entities) == 0:
                         is_correct[rstart:rend] = False
                     else:
-                        gold_entities_id = np.asarray(link.entities)
+                        gold_entities_id = np.asarray([ent.id for ent in link.entities])
                         is_correct[rstart:rend] = np.isin(
                             candidates.id[rstart:rend], gold_entities_id
                         )
 
             cell_index_offset += nrows * ncols
 
         return CRDatasetCan(
             cell=np.asarray(cell, dtype=np.object_),
             cell_id=cell_id,
             table_index=table_index,
             col_index=col_index,
-            row_index=row_index,
             is_correct=is_correct,
         )
 
-    def slice(self, start: int, end: int):
-        return CRDatasetCan(
-            cell=self.cell[start:end],
-            cell_id=self.cell_id[start:end],
-            table_index=self.table_index[start:end],
-            row_index=self.row_index[start:end],
-            col_index=self.col_index[start:end],
-            is_correct=self.is_correct[start:end],
-        )
-
 
 CRDatasetEnt.init()
 CRDatasetCan.init()
```

### Comparing `ned-1.11.1/ned/candidate_ranking/dataset/basic_features.py` & `ned-1.7.0/ned/candidate_ranking/dataset/basic_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 import enum
 from operator import itemgetter
 import re, pickle
 
 from typing import Union
 import numpy as np
-import orjson
 import ray
 from nptyping import Float64, NDArray, Shape, Object
 from ream.data_model_helper import NumpyDataModel
 from tqdm import tqdm
 from ned.data_models.pymodels import Entity
 from sm.misc.funcs import batch, filter_duplication
 from sm.misc.ray_helper import ray_map
@@ -27,47 +26,49 @@
     def create(
         cell: NDArray[Shape["*"], Object],
         entity_label: NDArray[Shape["*"], Object],
         entity_aliases: NDArray[Shape["*"], Object],
         entity_popularity: NDArray[Shape["*"], Float64],
     ):
         features = ray_map(
-            extract_features,
+            ray_extract_features.remote,
             batch(512, cell, entity_label, entity_aliases, entity_popularity),
             verbose=True,
             desc="extract features",
-            is_func_remote=False,
         )
         features = np.concatenate(features, axis=0)
         return CRDatasetFeatures(features)
 
 
 CRDatasetFeatures.init()
 
 
-def extract_features(
+@ray.remote
+def ray_extract_features(
     cells: np.ndarray,
     labels: np.ndarray,
     aliases: np.ndarray,
     popularities: np.ndarray,
 ):
     feats = []
 
     for i in range(len(labels)):
         cell = cells[i]
 
-        feat = np.zeros((N_PAIRWISE_FEATURES + N_EXTRA_FEATURES,), dtype=np.float64)
-        label_feat = extract_pairwise_features_v1(cell, labels[i])
-        for alias in orjson.loads(aliases[i]):
-            label_feat = np.maximum(
-                label_feat, extract_pairwise_features_v1(cell, alias)
-            )
+        feat = extract_pairwise_features_v1(cell, labels[i])
 
-        feat[:N_PAIRWISE_FEATURES] = label_feat
-        feat[N_PAIRWISE_FEATURES] = popularities[i]
+        ali_feat = np.zeros_like(feat)
+        for alias in Entity.decode_aliases(aliases[i]):
+            ali_feat = np.maximum(ali_feat, extract_pairwise_features_v1(cell, alias))
+
+        all_feat = np.maximum(feat, ali_feat)
+        feat.extend(ali_feat)
+        feat.extend(all_feat)
+
+        feat.append(popularities[i])
         feats.append(feat)
 
     return np.array(feats, dtype=np.float64)
 
 
 # number of extracted pairwise features
 # for setting default gold_features for NIL entity
@@ -78,15 +79,15 @@
     monge_elkan_sim = 2
     sym_monge_elkan_sim = 3
     hybrid_jaccard_sim = 4
     numeric_sym_monge_elkan_sim = 5
     numeric_hybrid_jaccard_sim = 6
 
 
-N_PAIRWISE_FEATURES = len(list(PairwiseFeatures))
+N_PAIRWISE_FEATURES = len(list(PairwiseFeatures)) * 2
 N_EXTRA_FEATURES = 1
 
 
 def extract_pairwise_features_v1(text: str, entity_label: str):
     """Extract feature from mention and entity.
 
     When this function is changed, the version number should be updated in this function and all step functions
```

### Comparing `ned-1.11.1/ned/candidate_ranking/dataset/matched_prop_feature.py` & `ned-1.7.0/ned/candidate_ranking/dataset/matched_prop_feature.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/dataset/types.py` & `ned-1.7.0/ned/candidate_ranking/dataset/types.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/helpers/dataset.py` & `ned-1.7.0/ned/candidate_ranking/helpers/dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,17 @@
 from __future__ import annotations
 
-import pickle, numpy as np, pandas as pd
+import pickle, numpy as np
 from typing import Any, Dict, Optional, Union, Callable
 import orjson
 from torch.utils.data import Dataset
 from pathlib import Path
 from ream.dataset_helper import DatasetDict
 
 
-class ColumnarDataset(Dataset):
-    """A columnar dataset"""
-
-    def __init__(
-        self,
-        columns: dict[str, np.ndarray | list],
-        dtypes: Optional[dict[str, Any]] = None,
-        collate_fn: Optional[Callable] = None,
-    ):
-        self.collate_fn = collate_fn
-        self.columns = columns
-        self.size = len(next(iter(self.columns.values())))
-        self.dtypes = dtypes
-
-        if dtypes is not None:
-            for name, feat in self.columns.items():
-                if name in dtypes and isinstance(feat, np.ndarray):
-                    self.columns[name] = feat.astype(dtypes[name])
-                    dtypes.pop(name)
-
-    def __len__(self):
-        return self.size
-
-    def __getitem__(self, idx: int):
-        return {name: feat[idx] for name, feat in self.columns.items()}
-
-    def to_df(self):
-        cols = {}
-        for name, feat in self.columns.items():
-            if not isinstance(feat, np.ndarray):
-                raise ValueError(
-                    f"Column {name} is not a numpy array, cannot convert dataset to dataframe"
-                )
-            if len(feat.shape) > 2:
-                raise ValueError(
-                    f"Column {name} has more than 2 dimensions, cannot convert dataset to dataframe"
-                )
-            if len(feat.shape) == 2:
-                for i in range(feat.shape[1]):
-                    cols[f"{name}_{i}"] = feat[:, i]
-            else:
-                cols[name] = feat
-        return pd.DataFrame(cols)
-
-
 class MyDataset(Dataset):
     """A columnar dataset"""
 
     def __init__(
         self,
         examples: Union[dict, list],
         dtypes: Optional[Dict[str, Any]] = None,
@@ -79,14 +34,18 @@
             self.size = len(self.examples)
 
         self.dtypes = dtypes
 
     def __len__(self):
         return self.size
 
+    @property
+    def shape(self):
+        return self.size
+
     def __getitem__(self, idx: int):
         if self.is_dict:
             out = {name: feat[idx] for name, feat in self.examples.items()}
         else:
             out = self.examples[idx]
 
         if self.dtypes is not None:
@@ -100,13 +59,13 @@
             return pickle.load(f)
 
     def save_to_disk(self, path: Path):
         with open(str(path), "wb") as f:
             pickle.dump(self, f)
 
 
-class MyDatasetDict(DatasetDict[Dataset]):
+class MyDatasetDict(DatasetDict[MyDataset]):
     serde = (MyDataset.save_to_disk, MyDataset.load_from_disk, "pkl")
 
     @property
     def shape(self):
-        return {subset: len(dataset) for subset, dataset in self.items()}
+        return {subset: dataset.shape for subset, dataset in self.items()}
```

### Comparing `ned-1.11.1/ned/candidate_ranking/helpers/db_helper.py` & `ned-1.7.0/ned/candidate_ranking/helpers/db_helper.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/helpers/debug_helper.py` & `ned-1.7.0/ned/candidate_ranking/helpers/debug_helper.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/candidate_ranking/helpers/training_helper.py` & `ned-1.7.0/ned/candidate_ranking/helpers/training_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from __future__ import annotations
 from abc import abstractmethod
 from collections import Sequence
 from dataclasses import _MISSING_TYPE, MISSING, dataclass, field
 import functools
 from pathlib import Path
 from loguru import logger
 from ned.candidate_ranking.helpers.dataset import MyDatasetDict
 import numpy as np
-from typing import List, Literal, Mapping, Optional, Protocol, Union
+from typing import List, Mapping, Optional, Union
 from sm.misc.funcs import get_incremental_path, get_latest_path, get_latest_version
 import torch
 from torch.utils.data import DataLoader
-from torch.utils.data.dataset import Dataset
 from tqdm import tqdm
 from transformers.training_args import IntervalStrategy, TrainingArguments
 
 
 class SmoothingMetric:
     def __init__(self, window_size: int = 7):
         self.lst: List[float] = [0] * window_size
@@ -108,37 +106,32 @@
 
     def get_training_dir(self):
         return self.ckpt_dir.parent
 
     def is_resuming(self):
         return self.restore_ckpt_file is not None
 
-    def resume_if_needed(self, model, optimizer, device=None) -> int:
+    def resume_if_needed(self, model, optimizer) -> int:
         if self.restore_ckpt_file is None:
             return 0
 
         # https://pytorch.org/tutorials/recipes/recipes/saving_and_loading_a_general_checkpoint.html
-        ckpt = torch.load(self.restore_ckpt_file, map_location=device)
+        ckpt = torch.load(self.restore_ckpt_file)
         model.load_state_dict(ckpt["model"])
-        if optimizer is not None:
-            optimizer.load_state_dict(ckpt["optimizer"])
+        optimizer.load_state_dict(ckpt["optimizer"])
 
         logger.info(
             "Resuming the training from step {} from checkpoint at {}",
             ckpt["step"],
             self.restore_ckpt_file,
         )
         return ckpt["step"]
 
     def skip_to_step(
-        self,
-        dl,
-        step: int,
-        progress_bar: ProgressBarProtocol,
-        num_epoch_steps: Optional[int] = None,
+        self, dl, step: int, progress_bar: tqdm, num_epoch_steps: Optional[int] = None
     ):
         """Skip the dataloader to the given step.
         Note that step starts counting from 1.
         If step is 0, then it does nothing and works as expected"""
         prev_desc = progress_bar.desc
         progress_bar.set_description(f"Skipping to step {step}")
         if num_epoch_steps is None or num_epoch_steps > 1:
@@ -162,24 +155,18 @@
             savefile,
         )
         return savefile
 
 
 @dataclass
 class ModifiedTrainingArguments(TrainingArguments):
-    train_dataset: str = field(
+    dataset: str = field(
         default="",
         metadata={
-            "help": "The dataset to use for training. Following the ream.dataset_helper.DatasetQuery format"
-        },
-    )
-    eval_datasets: list[str] = field(
-        default_factory=list,
-        metadata={
-            "help": "The datasets used for evaluation. Following the ream.dataset_helper.DatasetQuery format"
+            "help": "The dataset to use for training and development. Following the ream.dataset_helper.DatasetQuery format"
         },
     )
     output_dir: str = ""
     # so that they do not generate this field automatically
     # making it difficult to cache
     logging_dir: str = "logs"
     train_eval_strategy: IntervalStrategy = IntervalStrategy.EPOCH
@@ -241,24 +228,24 @@
         bpos = (label == 1).sum()
         pos += bpos
         neg += label.numel() - bpos
 
     return torch.FloatTensor([1 - neg / total, 1 - pos / total])
 
 
-def get_data_loader(dataset: Dataset, name, batch_size: int, shuffle: bool):
+def get_data_loader(dataset: MyDatasetDict, split, batch_size: int, shuffle: bool):
     logger.info(
-        "{} dataset: #examples {} - batch size {}", name, len(dataset), batch_size
+        "{} dataset: shape {} - batch size {}", split, str(dataset.shape), batch_size
     )
 
     return DataLoader(
-        dataset,
+        dataset[split],
         batch_size=batch_size,
         shuffle=shuffle,
-        collate_fn=dataset.collate_fn,
+        collate_fn=dataset[split].collate_fn,
     )
 
 
 class SklearnClassifier:
     TRAIN_ARGS: Sequence[str]
     EVAL_ARGS: Sequence[str]
     # mapping from metric class name to metric auxiliary args (no predictions) to dataset args
@@ -279,17 +266,7 @@
     @abstractmethod
     def state_dict(self) -> dict:
         pass
 
     @abstractmethod
     def load_state_dict(self, state_dict: dict):
         pass
-
-
-class ProgressBarProtocol(Protocol):
-    desc: str
-
-    def update(self, n: int) -> Optional[bool]:
-        ...
-
-    def set_description(self, desc: str):
-        ...
```

### Comparing `ned-1.11.1/ned/candidate_ranking/metrics/ned_metric.py` & `ned-1.7.0/ned/candidate_ranking/metrics/ned_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,79 +54,67 @@
     def _compute(
         self,
         predictions: list[float],
         references: list[int],
         cells: list[int],
     ):
         # group predictions and references by cell
-        return compute_ned_metrics(
-            torch.tensor(predictions),
-            torch.tensor(references),
-            torch.tensor(cells),
-            self.threshold,
-        )
-
-
-def compute_ned_metrics(
-    predictions: torch.Tensor,
-    references: torch.Tensor,
-    cells: torch.Tensor,
-    threshold: float,
-):
-    # group predictions and references by cell
-
-    # using stable sort to make sure we have closest results to evaluating
-    # outside of training
-    cells, reorder_index = torch.sort(cells, stable=True)
-    predictions = predictions[reorder_index]
-    references = references[reorder_index]
-
-    # get [start, end) boundaries of each cell
-    range = (cells[:-1] != cells[1:]).nonzero() + 1
-    groups = []
-    start = 0
-    for end in range:
-        end = end.item()
-        groups.append((start, end))
-        start = end
-    groups.append((start, predictions.shape[0]))
-
-    # go through each group, and calculate mrr and other metrics
-    mrr = 0.0
-    recall = [0.0, 0.0, 0.0, 0.0]
-
-    for start, end in groups:
-        # don't use descending to make sure it has the same order as our other code
-        preds, reorder = torch.sort(-predictions[start:end], stable=True)
-        preds = -preds
-        refs = references[start:end][reorder]
-
-        gt_rank = refs.nonzero(as_tuple=True)[0] + 1
-        if gt_rank.shape[0] == 0:
-            # no ground-truth, predict when the top preds is less than a threshold
-            if preds[0] < threshold:
-                # predict correctly
-                mrr += 1
-                recall[0] += 1
-                recall[1] += 1
-                recall[2] += 1
-                recall[3] += 1
-        else:
-            # have ground-truth, we need to filter out the preds that are less than a threshold
-            gt_rank = gt_rank[preds[gt_rank - 1] >= threshold]
-            mrr += 1 / gt_rank.max().item()
-            recall[0] += (gt_rank == 1).sum().item()
-            recall[1] += (gt_rank <= 5).sum().item()
-            recall[2] += (gt_rank <= 10).sum().item()
-            recall[3] += (gt_rank <= 20).sum().item()
-
-    n = max(1, len(groups))
-    mrr /= n
-    recall = [r / n * 100 for r in recall]
-    return {
-        "total": n,
-        "mrr": mrr,
-        "recall@1": recall[0],
-        "recall@5": recall[1],
-        "recall@10": recall[2],
-        "recall@20": recall[3],
-    }
+        predictions = torch.tensor(predictions)
+        references = torch.tensor(references)
+        cells = torch.tensor(cells)
+
+        # using stable sort to make sure we have closest results to evaluating
+        # outside of training
+        cells, reorder_index = torch.sort(cells, stable=True)
+        predictions = predictions[reorder_index]
+        references = references[reorder_index]
+
+        # get [start, end) boundaries of each cell
+        range = (cells[:-1] != cells[1:]).nonzero() + 1
+        groups = []
+        start = 0
+        for end in range:
+            end = end.item()
+            groups.append((start, end))
+            start = end
+        groups.append((start, predictions.shape[0]))
+
+        # go through each group, and calculate mrr and other metrics
+        mrr = 0.0
+        recall = [0.0, 0.0, 0.0, 0.0]
+
+        for start, end in groups:
+            # don't use descending to make sure it has the same order as our other code
+            preds, reorder = torch.sort(-predictions[start:end], stable=True)
+            preds = -preds
+            refs = references[start:end][reorder]
+
+            gt_rank = refs.nonzero(as_tuple=True)[0] + 1
+            if gt_rank.shape[0] == 0:
+                # no ground-truth, predict when the top preds is less than a threshold
+                if preds[0] < self.threshold:
+                    # predict correctly
+                    mrr += 1
+                    recall[0] += 1
+                    recall[1] += 1
+                    recall[2] += 1
+                    recall[3] += 1
+            else:
+                # have ground-truth, we need to filter out the preds that are less than a threshold
+                gt_rank = gt_rank[preds[gt_rank - 1] >= self.threshold]
+                mrr += 1 / gt_rank.max().item()
+                recall[0] += (gt_rank == 1).sum().item()
+                recall[1] += (gt_rank <= 5).sum().item()
+                recall[2] += (gt_rank <= 10).sum().item()
+                recall[3] += (gt_rank <= 20).sum().item()
+
+        n = max(1, len(groups))
+        mrr /= n
+        recall = [r / n * 100 for r in recall]
+        return {
+            "total": n,
+            "mrr": mrr,
+            "recall@1": recall[0],
+            "recall@5": recall[1],
+            "recall@10": recall[2],
+            "recall@20": recall[3],
+        }
```

### Comparing `ned-1.11.1/ned/candidate_ranking/pairwise_model.py` & `ned-1.7.0/ned/candidate_ranking/pairwise_model.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/data_models/deprecated/np_candidate_arrays.py` & `ned-1.7.0/ned/data_models/deprecated/np_candidate_arrays.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/data_models/deprecated/py_candidate_arrays.py` & `ned-1.7.0/ned/data_models/deprecated/py_candidate_arrays.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/data_models/npmodels.py` & `ned-1.7.0/ned/data_models/npmodels.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 
 from collections import Sequence
 from copy import deepcopy
 from typing import Generic, Literal, TypeVar, Optional, Union, Protocol, overload
 
 import numpy as np
 from nptyping import Float64, NDArray, Shape, Object
-from ream.data_model_helper import (
-    NumpyDataModel,
-    NumpyDataModelHelper,
-    OffsetIndex,
-    ContiguousIndexChecker,
-)
+from ream.data_model_helper import NumpyDataModel, OffsetIndex, ContiguousIndexChecker
 
 from ned.data_models.pymodels import CandidateEntity, Entity
-from sm.misc.funcs import is_non_decreasing_sequence
 
 # mapping from { row_index => [start, end] }
 ColumnIndex = dict[int, tuple[int, int]]
 # mapping from { col_index => [start, end, ColumnIndex] }
 TableIndex = dict[int, tuple[int, int, ColumnIndex]]
 # mapping from: { table_id => [start, end, TableIndex] }
 DatasetIndex = dict[str, tuple[int, int, TableIndex]]
@@ -92,27 +86,14 @@
                 aliases=self.aliases[i],
                 popularity=self.popularity[i],
             ),
             score=self.score[i],
             provenance=self.provenance[i],
         )
 
-    def get_candidate_by_index(self, i: int) -> CandidateEntity:
-        return CandidateEntity(
-            entity=Entity(
-                id=self.id[i],
-                label=self.label[i],
-                description=self.description[i],
-                aliases=self.aliases[i],
-                popularity=self.popularity[i],
-            ),
-            score=self.score[i],
-            provenance=self.provenance[i],
-        )
-
 
 class DatasetCandidateEntities(CandidateEntities[DatasetIndex]):
     index: DatasetIndex
 
     @classmethod
     def from_pymodel_candidates(
         cls,
@@ -197,40 +178,14 @@
             description=np.concatenate(description, axis=0),
             aliases=np.concatenate(aliases, axis=0),
             popularity=np.concatenate(popularity, axis=0),
             score=np.concatenate(score, axis=0),
             provenance=np.concatenate(provenance, axis=0),
         )
 
-    @staticmethod
-    def from_table_candidates(candidates: dict[str, TableCandidateEntities]):
-        index = {}
-        lst = []
-        start = 0
-        for table_id, table_cans in candidates.items():
-            lst.append(table_cans)
-            index[table_id] = (
-                start,
-                start + len(table_cans),
-                NumpyDataModelHelper.offset_index(table_cans.index.index, start),
-            )
-            start += len(table_cans)
-        ds = DatasetCandidateEntities(
-            index=index,
-            id=np.concatenate([c.id for c in lst]),
-            label=np.concatenate([c.label for c in lst]),
-            description=np.concatenate([c.description for c in lst]),
-            aliases=np.concatenate([c.aliases for c in lst]),
-            popularity=np.concatenate([c.popularity for c in lst]),
-            score=np.concatenate([c.score for c in lst]),
-            provenance=np.concatenate([c.provenance for c in lst]),
-        )
-        assert ds.score.shape == ds.id.shape, (ds.score.shape, ds.id.shape)
-        return ds
-
     def get_row_index(self):
         row_index = np.zeros_like(self.id, dtype=np.int32)
         for tstart, tend, tindex in self.index.values():
             for cstart, cend, cindex in tindex.values():
                 for ri, (rstart, rend) in cindex.items():
                     row_index[rstart:rend] = ri
         return row_index
@@ -264,72 +219,55 @@
             self.description[start:end],
             self.aliases[start:end],
             self.popularity[start:end],
             self.score[start:end],
             self.provenance[start:end],
         )
 
-    def get_table_candidates(self, table: str):
-        start, end, tindex = self.index[table]
-        return TableCandidateEntities(
-            OffsetIndex(tindex, start),
-            self.id[start:end],
-            self.label[start:end],
-            self.description[start:end],
-            self.aliases[start:end],
-            self.popularity[start:end],
-            self.score[start:end],
-            self.provenance[start:end],
-        )
-
     @overload
     def top_k_candidates(
         self,
         k: int,
         gold_ents: Optional[
             Union[DatasetGoldEntities, dict[str, dict[int, dict[int, list[Entity]]]]]
         ] = None,
         return_index_remap: Literal[False] = False,
-        remove_nil_entity: bool = False,
     ) -> DatasetCandidateEntities:
         ...
 
     @overload
     def top_k_candidates(
         self,
         k: int,
         gold_ents: Optional[
             Union[DatasetGoldEntities, dict[str, dict[int, dict[int, list[Entity]]]]]
         ] = None,
         return_index_remap: Literal[True] = True,
-        remove_nil_entity: bool = False,
     ) -> tuple[DatasetCandidateEntities, np.ndarray]:
         ...
 
     def top_k_candidates(
         self,
         k: int,
         gold_ents: Optional[
             Union[DatasetGoldEntities, dict[str, dict[int, dict[int, list[Entity]]]]]
         ] = None,
         return_index_remap: bool = False,
-        remove_nil_entity: bool = False,
     ):
         """Keep top K candidates for each cell based on the score. To customize the score, use
         the replace method, which returns a shallow copy of the dataset.
 
         Args:
             k: number of candidates per cell to keep.
             gold_ents: (optional) a dictionary of missing gold entities for each cell. If provided, will be added to
                 the candidates if missing. The dictionary is of the form {table: {col: {row: [Entity]}}}.
             return_index_map: whether to return an array has the same shape of the new dataset and contains indices of the
                 old elements, so that we can map between old elements and new elements. For each item where the new element
                 is added from gold_ents, the value will be -1. This is useful when we want to reuse some data that is aligned
                 with the old dataset.
-            remove_nil_entity: whether to remove the NIL entity from the candidates. Applicable only when gold_ents is provided
 
         Returns:
             A new dataset with top K candidates per cell.
             (optionally) index maps of candidates
         """
         newindex = {}
         newid = []
@@ -433,25 +371,14 @@
                                 newpopularity[-1][-n:] = gold_ents.entity_popularity[
                                     erstart:erend
                                 ]
                                 newscore[-1][-n:] = 0.0
                                 newprovenance[-1][-n:] = "oracle"
                                 sortedindex[-n:] = -1
 
-                        if n == 0 and remove_nil_entity:
-                            # there is no gold entity for this cell, and NIL entity is removed
-                            newid.pop()
-                            newlabel.pop()
-                            newdescription.pop()
-                            newaliases.pop()
-                            newpopularity.pop()
-                            newscore.pop()
-                            newprovenance.pop()
-                            continue
-
                     if return_index_remap:
                         idx_map.append(sortedindex)
                     newcindex[ri] = (count, count + len(newid[-1]))
                     count += len(newid[-1])
 
                 newtindex[ci] = (coloffset, count, newcindex)
                 coloffset = count
@@ -475,26 +402,24 @@
 
     def select(self, table: Union[str, list[str]]):
         """Select candidates of a single table or multiple tables.
         If passing multiple tables, they must be consecutive in the dataset.
         """
         if isinstance(table, str):
             tables = [table]
-            # could do [:2] but type checker complains
-            start, end = (tmp := self.index[table])[0], tmp[1]
+            start, end = self.index[table][:2]
         else:
             tables = table
             if len(tables) == 0:
                 raise ValueError("No tables passed")
 
             # verify that the tables are consecutive
             checker = ContiguousIndexChecker(self.index[tables[0]][0])
             for table in tables:
-                # could do [:2] but type checker complains
-                start, end = (tmp := self.index[table])[0], tmp[1]
+                start, end = self.index[table][:2]
                 checker.next(start, end)
 
             start = self.index[tables[0]][0]
             end = self.index[tables[-1]][1]
 
         newindex = {
             table: (
@@ -523,81 +448,14 @@
             self.aliases[start:end],
             self.popularity[start:end],
             self.score[start:end],
             self.provenance[start:end],
         )
 
 
-class TableCandidateEntities(CandidateEntities[OffsetIndex[TableIndex]]):
-    index: OffsetIndex[TableIndex]
-
-    def get_column_candidates(self, col: int):
-        start, end, cindex = self.index.index[col]
-        start -= self.index.offset
-        end -= self.index.offset
-        return ColumnCandidateEntities(
-            OffsetIndex(cindex, start),
-            self.id[start:end],
-            self.label[start:end],
-            self.description[start:end],
-            self.aliases[start:end],
-            self.popularity[start:end],
-            self.score[start:end],
-            self.provenance[start:end],
-        )
-
-    def has_cell_candidates(self, row: int, col: int) -> bool:
-        return col in self.index.index and row in self.index.index[col][2]
-
-    def get_cell_candidates(self, row: int, col: int):
-        start, end = self.index.index[col][2][row]
-        start -= self.index.offset
-        end -= self.index.offset
-        return CellCandidateEntities(
-            None,
-            self.id[start:end],
-            self.label[start:end],
-            self.description[start:end],
-            self.aliases[start:end],
-            self.popularity[start:end],
-            self.score[start:end],
-            self.provenance[start:end],
-        )
-
-    @staticmethod
-    def from_cell_candidates(
-        cell_cans: dict[int, dict[int, CellCandidateEntities]]
-    ) -> TableCandidateEntities:
-        index = {}
-        start = 0
-        lst = []
-
-        for ci in cell_cans:
-            col_start = start
-            col_index = {}
-
-            cindex = cell_cans[ci]
-            for ri in cindex:
-                cans = cindex[ri]
-                lst.append(cans)
-                col_index[ri] = (start, start + len(cans))
-                start += len(cans)
-            index[ci] = (col_start, start, col_index)
-        return TableCandidateEntities(
-            OffsetIndex(index, 0),
-            id=np.concatenate([cans.id for cans in lst]),
-            label=np.concatenate([cans.label for cans in lst]),
-            description=np.concatenate([cans.description for cans in lst]),
-            aliases=np.concatenate([cans.aliases for cans in lst]),
-            popularity=np.concatenate([cans.popularity for cans in lst]),
-            score=np.concatenate([cans.score for cans in lst]),
-            provenance=np.concatenate([cans.provenance for cans in lst]),
-        )
-
-
 class ColumnCandidateEntities(CandidateEntities[OffsetIndex[ColumnIndex]]):
     index: OffsetIndex[ColumnIndex]
 
     def get_cell_candidates(self, row: int):
         start, end = self.index.index[row]
         start -= self.index.offset
         end -= self.index.offset
@@ -639,10 +497,9 @@
             self.popularity[items],
             self.score[items],
             self.provenance[items],
         )
 
 
 DatasetCandidateEntities.init()
-TableCandidateEntities._metadata = deepcopy(DatasetCandidateEntities._metadata)
 ColumnCandidateEntities._metadata = deepcopy(DatasetCandidateEntities._metadata)
 CellCandidateEntities.init()
```

### Comparing `ned-1.11.1/ned/data_models/prelude.py` & `ned-1.7.0/ned/data_models/prelude.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,17 @@
     NIL_ENTITY,
     ALIAS_SEP_TOKEN,
     ESCAPE_ALIAS_SEP_TOKEN,
     Entity,
     CandidateEntity,
     CellLink,
     NEDExample,
-    EntityWithScore,
 )
 from .npmodels import (
     DatasetCandidateEntities,
-    TableCandidateEntities,
     ColumnCandidateEntities,
     CellCandidateEntities,
     DatasetIndex,
     TableIndex,
     ColumnIndex,
 )
 
@@ -24,16 +22,14 @@
     "NIL_ENTITY",
     "ALIAS_SEP_TOKEN",
     "ESCAPE_ALIAS_SEP_TOKEN",
     "Entity",
     "CandidateEntity",
     "CellLink",
     "NEDExample",
-    "EntityWithScore",
     "DatasetCandidateEntities",
-    "TableCandidateEntities",
     "ColumnCandidateEntities",
     "CellCandidateEntities",
     "DatasetIndex",
     "TableIndex",
     "ColumnIndex",
 ]
```

### Comparing `ned-1.11.1/ned/data_models/pymodels.py` & `ned-1.7.0/ned/data_models/pymodels.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 from copy import deepcopy
 
 from dataclasses import dataclass
 from typing import Any, cast
 from typing_extensions import Self
-from ned.candidate_generation.pyserini.document import StringEncoder
 
 from sm.inputs.table import ColumnBasedTable
-from sm.inputs.link import WIKIDATA_NIL_ENTITY, EntityId
+from sm.inputs.link import WIKIDATA_NIL_ENTITY
 from sm.misc.matrix import Matrix
 from sm.outputs.semantic_model import SemanticModel
 from kgdata.wikidata.models.multilingual import MultiLingualStringList
 
 
 ALIAS_SEP_TOKEN = "\n"
 ESCAPE_ALIAS_SEP_TOKEN = "\\-n"
@@ -67,22 +66,48 @@
     @staticmethod
     def decode_aliases(aliases: str) -> list:
         return [
             v.replace(ESCAPE_ALIAS_SEP_TOKEN, ALIAS_SEP_TOKEN)
             for v in aliases.split(ALIAS_SEP_TOKEN)
         ]
 
-    def iter_names(self):
-        yield self.label
-        assert self.aliases is not None
-        for alias in self.decode_aliases(self.aliases):
-            yield alias
+    @staticmethod
+    def full_encode_aliases(aliases: MultiLingualStringList):
+        main_lang = ""
+        other_langs = {}
+        for lang, values in aliases.lang2values.items():
+            assert all(ESCAPE_ALIAS_SEP_TOKEN not in v for v in values)
+            newvalues = ALIAS_SEP_TOKEN.join(
+                value.replace(ALIAS_SEP_TOKEN, ESCAPE_ALIAS_SEP_TOKEN)
+                for value in values
+            )
+            if lang == aliases.lang:
+                main_lang = f"{lang}:{newvalues}"
+            else:
+                other_langs[lang] = f"{lang}:{newvalues}"
+
+        out = [main_lang]
+        out.extend(other_langs.values())
+        return (ALIAS_SEP_TOKEN + ALIAS_SEP_TOKEN).join(out)
+
+    @staticmethod
+    def full_decode_aliases(aliases: str) -> MultiLingualStringList:
+        lst = aliases.split(ALIAS_SEP_TOKEN + ALIAS_SEP_TOKEN)
+        lang2values = []
+        for item in lst:
+            lang, values = item.split(":", 1)
+            values = [
+                v.replace(ESCAPE_ALIAS_SEP_TOKEN, ALIAS_SEP_TOKEN)
+                for v in values.split(ALIAS_SEP_TOKEN)
+            ]
+            lang2values.append((lang, values))
 
-    def __str__(self):
-        return f"{self.label} ({self.id})"
+        if len(lang2values) == 0:
+            return MultiLingualStringList({}, "en")
+        return MultiLingualStringList(dict(lang2values), lang2values[0][0])
 
 
 @dataclass
 class CandidateEntity:
     entity: Entity
     # score of the candidate entity
     score: float
@@ -103,93 +128,63 @@
 
 
 @dataclass
 class CellLink:
     # if the cell is not linked any entity, self is None
     # if the cell does linked to an entity, but the list is empty, it means
     # the cell is linked to NIL.
-    entities: list[EntityId]
-    # mapping from entity id to the range (exclusive), a cell may appear multiple times
-    mentions: dict[str, list[tuple[int, int]]]
+    entities: list[Entity]
+    # mapping from entity id to the range (exclusive)
+    mentions: dict[str, tuple[int, int]]
+    # candidates: list[CandidateEntity]
 
     def to_dict(self):
         return {
-            "mentions": [
-                (k, v[0], v[1]) for k, vs in self.mentions.items() for v in vs
-            ],
-            "entities": [e.to_dict() for e in self.entities],
+            "mentions": [(k, v[0], v[1]) for k, v in self.mentions.items()],
+            "entities": [e.to_tuple() for e in self.entities],
+            # "candidates": [c.to_dict() for c in self.candidates],
         }
 
     @classmethod
     def from_dict(cls, d):
-        mentions = {}
-        for k, s, e in d["mentions"]:
-            if k not in mentions:
-                mentions[k] = []
-            mentions[k].append((s, e))
         return cls(
-            [EntityId.from_dict(e) for e in d["entities"]],
-            mentions,
-        )
-
-
-@dataclass
-class EntityWithScore:
-    entity: EntityId
-    score: float  # a normalized score from 0 to 1
-
-    def to_dict(self):
-        return {
-            "entity": self.entity.to_dict(),
-            "score": self.score,
-        }
-
-    @classmethod
-    def from_dict(cls, d):
-        return cls(
-            EntityId.from_dict(d["entity"]),
-            d["score"],
+            [Entity.from_tuple(e) for e in d["entities"]],
+            {k: (s, e) for k, s, e in d["mentions"]},
+            # [CandidateEntity.from_dict(c) for c in d["candidates"]],
         )
 
 
 @dataclass
 class NEDExample:
     table: ColumnBasedTable
     # list of columns that are entity columns (size != #columns)
     entity_columns: list[int]
     # list of types of entity columns, corresponding with entity_columns (size != #columns)
-    # a column can have more than 1 type, and also with a score to specify the confidence or preference
-    entity_column_types: list[list[EntityWithScore]]
+    entity_column_types: list[list[Entity]]
     # (row, col) -> cell link (can have more than one entity)
     cell_links: Matrix[CellLink | None]
-    # list of columns that should be entity columns but are not linked to any entities (size != #columns)
-    # for example: column position is linked with an object property (played position) but the values are text not
-    # links in Wikipedia. Hence, the auto-label algorithm misses this column.
-    should_be_entity_columns: list[int]
 
     def to_dict(self):
         return {
             "table": self.table.to_dict(),
             "entity_columns": self.entity_columns,
             "entity_column_types": [
                 [e.to_dict() for e in ents] for ents in self.entity_column_types
             ],
             "cell_links": [
                 [l.to_dict() if l is not None else None for l in row]
                 for row in self.cell_links.data
             ],
-            "should_be_entity_columns": self.should_be_entity_columns,
         }
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
         obj["table"] = ColumnBasedTable.from_dict(obj["table"])
         obj["entity_column_types"] = [
-            [EntityWithScore.from_dict(e) for e in ents]
-            for ents in obj["entity_column_types"]
+            [Entity.from_dict(e) for e in ents] for ents in obj["entity_column_types"]
         ]
         obj["cell_links"] = Matrix(
             [
                 [CellLink.from_dict(l) if l is not None else None for l in row]
                 for row in obj["cell_links"]
             ]
         )
@@ -212,18 +207,8 @@
 
         cell_links = self.cell_links.shallow_copy()
         for row in cell_links.data:
             for ci in range(len(row)):
                 if ci not in set_columns:
                     row[ci] = None
 
-        should_be_entity_columns = [
-            ec for ec in self.should_be_entity_columns if ec in set_columns
-        ]
-
-        return NEDExample(
-            self.table,
-            entity_columns,
-            entity_column_types,
-            cell_links,
-            should_be_entity_columns,
-        )
+        return NEDExample(self.table, entity_columns, entity_column_types, cell_links)
```

### Comparing `ned-1.11.1/ned/entity_recognition/ensemble_model.py` & `ned-1.7.0/ned/entity_recognition/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/entity_recognition/er_model_interface.py` & `ned-1.7.0/ned/entity_recognition/er_model_interface.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/entity_recognition/model_data/feature_store.py` & `ned-1.7.0/ned/entity_recognition/model_data/feature_store.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/entity_recognition/model_data/main.py` & `ned-1.7.0/ned/entity_recognition/model_data/main.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/entity_recognition/oracle_model.py` & `ned-1.7.0/ned/entity_recognition/oracle_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,43 @@
 from __future__ import annotations
-from dataclasses import dataclass, field
 
 from pathlib import Path
 from ned.candidate_ranking.helpers.dataset import MyDataset
 from ned.data_models.prelude import NEDExample
 from ream.params_helper import NoParams
 from ned.entity_recognition.er_model_interface import ERModelInterface
 
 
-@dataclass
-class OracleERModelArgs:
-    include_should_be_entity_columns: bool = field(
-        default=False,
-        metadata={
-            "help": "Whether to include should_be_entity_columns in the prediction",
-        },
-    )
-
-
 class OracleERModel(ERModelInterface):
-    VERSION = 101
-
-    def __init__(self, args: OracleERModelArgs):
-        self.args = args
+    VERSION = 100
 
     def gen_data(
         self,
         examples: list[NEDExample],
         for_training: bool = False,
         cache_dir: Path | None = None,
     ):
         entity_columns = [e.entity_columns for e in examples]
-        should_be_entity_columns = [e.should_be_entity_columns for e in examples]
-
         return MyDataset(
             {
                 "entity_columns": entity_columns,
-                "should_be_entity_columns": should_be_entity_columns,
                 "example_id": [e.table.table_id for e in examples],
             }
         )
 
     def get_gen_data_args(self):
         return NoParams()
 
     def predict_data(
         self, examples: list[NEDExample], ds: MyDataset
     ) -> list[list[int]]:
         assert isinstance(ds.examples, dict)
         example_id = ds.examples["example_id"]
         entity_columns = ds.examples["entity_columns"]
-
         assert example_id == [e.table.table_id for e in examples]
-        if self.args.include_should_be_entity_columns:
-            should_be_entity_columns = ds.examples["should_be_entity_columns"]
-            return entity_columns + should_be_entity_columns
         return entity_columns
 
     def state_dict(self) -> dict:
         return {}
 
     def load_state_dict(self, state_dict: dict):
         pass
```

### Comparing `ned-1.11.1/ned/entity_recognition/training.py` & `ned-1.7.0/ned/entity_recognition/training.py`

 * *Files identical despite different names*

### Comparing `ned-1.11.1/ned/metrics.py` & `ned-1.7.0/ned/metrics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 from dataclasses import dataclass
-from typing import Optional, Protocol, Sequence, TypedDict, Union, cast
+from typing import Optional, Sequence, TypedDict, Union, cast
 from typing_extensions import TypeGuard
 
 from ned.candidate_generation.common import CandidateEntity
 from ned.data_models.pymodels import NIL_ENTITY, NO_ENTITY
-import numpy as np
 from sm.misc.matrix import Matrix
-from sm.evaluation.prelude import PrecisionRecallF1, recall_at_k
 
 
 @dataclass
 class ConfusionMatrix:
     tp: int = 0  # true positive
     fn: int = 0  # false negative
     fp: int = 0  # false positive
@@ -48,14 +46,20 @@
             self.tp + another.tp,
             self.fn + another.fn,
             self.fp + another.fp,
             self.tn + another.tn,
         )
 
 
+class PrecisionRecallF1(TypedDict):
+    precision: float
+    recall: float
+    f1: float
+
+
 def inkb_eval_table(
     gold_ents: Matrix[set[str]],
     pred_ents: Matrix[list[str]],
     k: Optional[Union[int, Sequence[Optional[int]]]] = None,
 ) -> tuple[dict[str, PrecisionRecallF1], dict[str, ConfusionMatrix]]:
     """Evaluate entity linking performance on a table using InKB metrics. As defined in Gerbil framework, InKB metrics
     only consider entities in KB as correct entities, NIL entity or entities outside of KB are consider incorrect and eliminated.
@@ -99,19 +103,19 @@
                         confusion_matrices[name].tp += 1
                     else:
                         confusion_matrices[name].fn += 1
 
     output = {}
     for name, ki in name2k.items():
         cm = confusion_matrices[name]
-        output[name] = PrecisionRecallF1(
-            recall=cm.recall(),
-            precision=cm.precision(),
-            f1=cm.f1(),
-        )
+        output[name] = {
+            "recall": cm.recall(),
+            "precision": cm.precision(),
+            "f1": cm.f1(),
+        }
 
     return output, confusion_matrices
 
 
 def recall(
     ytrue: list[str] | list[set[str]],
     ypreds: Union[list[list[CandidateEntity]], list[list[str]]],
@@ -125,15 +129,47 @@
     Args:
         ytrue: List of true entities for each query. When there are more than one true entities of a query, we classify
             the prediction as correct if the prediction is one of the true entities.
         ypreds: List of predicted (candidate) entities for each query, sorted by their likelihood in decreasing order.
         k: Number of predicted (candidate) entities to consider. If None, all predicted entities are considered.
     """
     ypreds = _norm_ypreds(ypreds)
-    return recall_at_k(ytrue, ypreds, k)
+    name2k = _norm_k("recall", k)
+    metrics = {name: 0.0 for name in name2k}
+
+    if len(ytrue) == 0:
+        return metrics
+
+    if isinstance(ytrue[0], str):
+        ytrue = cast(list[str], ytrue)
+        for i in range(len(ytrue)):
+            for name, ki in name2k.items():
+                if ki is None:
+                    yipreds = ypreds[i]
+                else:
+                    yipreds = ypreds[i][:ki]
+
+                if ytrue[i] in yipreds:
+                    metrics[name] += 1.0
+    else:
+        ytrue = cast(list[set[str]], ytrue)
+        for i in range(len(ytrue)):
+            for name, ki in name2k.items():
+                if ki is None:
+                    yipreds = ypreds[i]
+                else:
+                    yipreds = ypreds[i][:ki]
+                if len(ytrue[i].intersection(yipreds)) > 0:
+                    metrics[name] += 1.0
+
+    if len(ytrue) > 0:
+        for name in name2k:
+            metrics[name] = metrics[name] * 100 / len(ytrue)
+
+    return metrics
 
 
 def mrr(
     ytrue: list[str] | list[set[str]],
     ypreds: list[list[CandidateEntity]] | list[list[str]],
 ) -> float:
     """Calculate MRR for a list of queries.
@@ -170,7 +206,21 @@
     if any(isinstance(ypred[0], CandidateEntity) for ypred in ypreds if len(ypred) > 0):
         return [
             [c.entity.id for c in ypred]
             for ypred in cast(list[list[CandidateEntity]], ypreds)
         ]
     else:
         return cast(list[list[str]], ypreds)
+
+
+def _norm_k(
+    metric_name: str, k: Optional[Union[int, Sequence[Optional[int]]]] = None
+) -> dict[str, Optional[int]]:
+    if k is None or isinstance(k, int):
+        k = [k]
+    out = {}
+    for i in k:
+        if i is None:
+            out[f"{metric_name}@all"] = None
+        else:
+            out[f"{metric_name}@{i}"] = i
+    return out
```

### Comparing `ned-1.11.1/setup.py` & `ned-1.7.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['ned',
  'ned.actors',
- 'ned.actors.dataset',
- 'ned.autodata',
  'ned.candidate_generation',
  'ned.candidate_generation.pyserini',
  'ned.candidate_ranking',
  'ned.candidate_ranking.dataset',
  'ned.candidate_ranking.helpers',
  'ned.candidate_ranking.metrics',
  'ned.data_models',
  'ned.data_models.deprecated',
  'ned.entity_recognition',
  'ned.entity_recognition.model_data',
- 'ned.models_and_training']
+ 'ned.training_helpers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['hugedict>=2.9.1,<3.0.0',
- 'kgdata>=3.4.2,<4.0.0',
- 'nptyping>=2.5.0,<3.0.0',
- 'osin>=1.11.3,<2.0.0',
- 'pyarrow>=11.0.0,<12.0.0',
- 'ream2>=2.2.0,<3.0.0',
- 'sem-desc>=4.8.0,<5.0.0',
- 'serde2>=1.6.0,<2.0.0',
- 'sm-datasets>=1.1.3,<2.0.0',
+['hugedict>=2.8.0,<3.0.0',
+ 'kgdata>=3.3.1,<4.0.0',
+ 'nptyping>=2.3.1,<3.0.0',
+ 'osin>=1.9.2,<2.0.0',
+ 'pyarrow>=9.0.0,<10.0.0',
+ 'ream2>=1.7.0,<2.0.0',
+ 'sem-desc>=4.2.1,<5.0.0',
+ 'serde2>=1.5.0,<2.0.0',
+ 'sm-datasets>=1.1.1,<2.0.0',
  'torch>=1.12.1,<2.0.0',
  'torchaudio>=0.12.1,<0.13.0',
  'torchvision>=0.13.1,<0.14.0']
 
 setup_kwargs = {
     'name': 'ned',
-    'version': '1.11.1',
+    'version': '1.7.0',
     'description': 'entity linking, named-entity disambiguation, record linkage',
     'long_description': 'None',
     'author': 'Binh Vu',
     'author_email': 'binh@toan2.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ned-1.11.1/PKG-INFO` & `ned-1.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ned
-Version: 1.11.1
+Version: 1.7.0
 Summary: entity linking, named-entity disambiguation, record linkage
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hugedict (>=2.9.1,<3.0.0)
-Requires-Dist: kgdata (>=3.4.2,<4.0.0)
-Requires-Dist: nptyping (>=2.5.0,<3.0.0)
-Requires-Dist: osin (>=1.11.3,<2.0.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
-Requires-Dist: ream2 (>=2.2.0,<3.0.0)
-Requires-Dist: sem-desc (>=4.8.0,<5.0.0)
-Requires-Dist: serde2 (>=1.6.0,<2.0.0)
-Requires-Dist: sm-datasets (>=1.1.3,<2.0.0)
+Requires-Dist: hugedict (>=2.8.0,<3.0.0)
+Requires-Dist: kgdata (>=3.3.1,<4.0.0)
+Requires-Dist: nptyping (>=2.3.1,<3.0.0)
+Requires-Dist: osin (>=1.9.2,<2.0.0)
+Requires-Dist: pyarrow (>=9.0.0,<10.0.0)
+Requires-Dist: ream2 (>=1.7.0,<2.0.0)
+Requires-Dist: sem-desc (>=4.2.1,<5.0.0)
+Requires-Dist: serde2 (>=1.5.0,<2.0.0)
+Requires-Dist: sm-datasets (>=1.1.1,<2.0.0)
 Requires-Dist: torch (>=1.12.1,<2.0.0)
 Requires-Dist: torchaudio (>=0.12.1,<0.13.0)
 Requires-Dist: torchvision (>=0.13.1,<0.14.0)
```

