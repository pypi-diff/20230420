# Comparing `tmp/nkululeko-0.43.6.tar.gz` & `tmp/nkululeko-0.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.43.6.tar", last modified: Tue Apr 18 14:14:02 2023, max compression
+gzip compressed data, was "nkululeko-0.44.0.tar", last modified: Thu Apr 20 16:55:45 2023, max compression
```

## Comparing `nkululeko-0.43.6.tar` & `nkululeko-0.44.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5159 2023-04-18 13:31:59.000000 nkululeko-0.43.6/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.43.6/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15883 2023-04-18 14:14:02.908260 nkululeko-0.43.6/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10171 2023-04-04 08:11:52.000000 nkululeko-0.43.6/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.43.6/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.43.6/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.43.6/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.43.6/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-18 13:31:33.000000 nkululeko-0.43.6/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.43.6/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1820 2023-03-23 14:42:03.000000 nkululeko-0.43.6/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.43.6/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.43.6/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.43.6/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19786 2023-04-04 12:53:16.000000 nkululeko-0.43.6/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1617 2023-03-13 09:54:10.000000 nkululeko-0.43.6/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.43.6/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.43.6/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.43.6/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.43.6/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.43.6/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.43.6/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.43.6/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2899 2023-02-09 12:01:24.000000 nkululeko-0.43.6/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.43.6/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2985 2023-02-08 10:22:44.000000 nkululeko-0.43.6/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.43.6/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.43.6/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.43.6/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.43.6/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.43.6/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.43.6/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.43.6/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.43.6/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.43.6/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.43.6/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.43.6/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.43.6/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.43.6/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.43.6/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.43.6/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.43.6/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.43.6/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.43.6/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.43.6/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.43.6/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.43.6/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4496 2023-02-28 14:44:32.000000 nkululeko-0.43.6/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.43.6/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.43.6/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10638 2023-02-16 12:26:38.000000 nkululeko-0.43.6/nkululeko/runmanager copy.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.43.6/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.43.6/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.43.6/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.43.6/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.43.6/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-18 14:14:02.908260 nkululeko-0.43.6/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15883 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1538 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      225 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-18 14:14:02.000000 nkululeko-0.43.6/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.43.6/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      901 2023-04-18 14:14:02.908260 nkululeko-0.43.6/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.43.6/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5286 2023-04-20 15:52:33.000000 nkululeko-0.44.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.44.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16010 2023-04-20 16:55:45.507060 nkululeko-0.44.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10171 2023-04-04 08:11:52.000000 nkululeko-0.44.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.44.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.44.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.44.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.44.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-20 15:51:53.000000 nkululeko-0.44.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.44.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1820 2023-03-23 14:42:03.000000 nkululeko-0.44.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.44.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.44.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.44.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20413 2023-04-20 16:45:58.000000 nkululeko-0.44.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1692 2023-04-20 13:43:01.000000 nkululeko-0.44.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.44.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.44.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3117 2023-04-19 15:46:17.000000 nkululeko-0.44.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.44.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.44.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.44.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.44.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.44.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.44.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.44.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3174 2023-04-19 15:22:07.000000 nkululeko-0.44.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.44.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.44.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.44.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.44.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.44.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.44.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.44.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.44.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.44.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.44.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.44.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.44.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.44.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.44.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.44.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.44.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.44.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.44.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.44.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.44.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.44.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.44.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.44.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10638 2023-02-16 12:26:38.000000 nkululeko-0.44.0/nkululeko/runmanager copy.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.44.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.44.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.44.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.44.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.44.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16010 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1562 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.44.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-04-20 16:55:45.507060 nkululeko-0.44.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.44.0/setup.py
```

### Comparing `nkululeko-0.43.6/CHANGELOG.md` & `nkululeko-0.44.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 0.44.0
+--------------
+* added scatter functions: tsne, pca, umap
+
+Version 0.43.7
+--------------
+* added clap features
+
 Version 0.43.6
 --------------
 * small bugs
 
 
 Version 0.43.5
 --------------
```

### Comparing `nkululeko-0.43.6/LICENSE` & `nkululeko-0.44.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/PKG-INFO` & `nkululeko-0.44.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.43.6
+Version: 0.44.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,14 +206,22 @@
 
 ## Licence
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.44.0
+--------------
+* added scatter functions: tsne, pca, umap
+
+Version 0.43.7
+--------------
+* added clap features
+
 Version 0.43.6
 --------------
 * small bugs
 
 
 Version 0.43.5
 --------------
```

### Comparing `nkululeko-0.43.6/README.md` & `nkululeko-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/augment.py` & `nkululeko-0.44.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/augmenter.py` & `nkululeko-0.44.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/cacheddataset.py` & `nkululeko-0.44.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/dataset.py` & `nkululeko-0.44.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/dataset_csv.py` & `nkululeko-0.44.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/dataset_ravdess.py` & `nkululeko-0.44.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/demo.py` & `nkululeko-0.44.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/demo_predictor.py` & `nkululeko-0.44.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/experiment.py` & `nkululeko-0.44.0/nkululeko/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,14 @@
             # encode the labels as numbers
             self.label_encoder = LabelEncoder()
             self.df_train[self.target] = self.label_encoder.fit_transform(self.df_train[self.target])
             self.df_test[self.target] = self.label_encoder.transform(self.df_test[self.target])
             glob_conf.set_label_encoder(self.label_encoder)
         if self.got_speaker:
             self.util.debug(f'{self.df_test.speaker.nunique()} speakers in test and {self.df_train.speaker.nunique()} speakers in train')
-        #augment = self.util.config_val('DATA', 'augment', 0)
-        #if augment:
-        #    self.augment_train()
 
         target_factor = self.util.config_val('DATA', 'target_divide_by', False)
         if target_factor:
             self.df_test[self.target] = self.df_test[self.target] / float(target_factor)
             self.df_train[self.target] = self.df_train[self.target] / float(target_factor)
             if not self.util.exp_is_classification():
                 self.df_test['class_label'] = self.df_test['class_label'] / float(target_factor)
@@ -258,22 +255,14 @@
                 plot.describe_df('dev_set', self.df_test, self.target, f'test_distplot')
             plot.describe_df('train_set', self.df_train, self.target, f'train_distplot')
         else:
             if self.df_test.shape[0] > 0:
                 plot.describe_df('dev_set', self.df_test, self.target, f'test_distplot')
             plot.describe_df('train_set', self.df_train, self.target, f'train_distplot')
 
-
-    def augment_train(self):
-        """Augment the train dataframe"""
-        from nkululeko.augmenter import Augmenter
-        augment_train = Augmenter(self.df_train)
-        df_train_aug = augment_train.augment()
-        self.df_train = self.df_train.append(df_train_aug)
-
     def extract_test_feats(self):
         self.feats_test = pd.DataFrame()
         feats_name = "_".join(ast.literal_eval(glob_conf.config['DATA']['tests']))
         self.feature_extractor = FeatureExtractor() 
         self.feature_extractor.set_data(self.df_test, feats_name, 'test')
         self.feats_test = self.feature_extractor.extract()
         self.util.debug(f'Test features shape:{self.feats_test.shape}')
@@ -298,17 +287,26 @@
 
         self._check_scale()
 
     def augment(self):
         """
         Augment the training set
         """
+        from nkululeko.augmenter import Augmenter
         augmenter = Augmenter(self.df_train)
         augmenter.augment()
 
+    # def augment_train(self):
+    #     """Augment the train dataframe"""
+    #     from nkululeko.augmenter import Augmenter
+    #     augment_train = Augmenter(self.df_train)
+    #     df_train_aug = augment_train.augment()
+    #     self.df_train = self.df_train.append(df_train_aug)
+
+
     def analyse_features(self):
         """
         Do a feature exploration
         
         """
 
         if self.util.config_val('EXPL', 'value_counts', False):
@@ -328,14 +326,28 @@
             pass
         else:
             self.util.error(f'unkown feature_distribution specifier {sample_selection}, should be [all | train | test]')
         if sample_selection in ('all', 'train', 'test'):
             feat_analyser = FeatureAnalyser(sample_selection, df_labels, df_feats)        
             feat_analyser.analyse()
 
+        # check if a scatterplot should be done
+        scatter_var = eval(self.util.config_val('EXPL', 'scatter', 'False'))
+        if scatter_var:
+            scatters = ast.literal_eval(glob_conf.config['EXPL']['scatter'])
+            if self.util.exp_is_classification():
+                plots = Plots()
+                all_feats =self.feats_train.append(self.feats_test)
+                all_labels = self.df_train['class_label'].append(self.df_test['class_label'])
+                for scatter in scatters:
+                    plots.scatter_plot(all_feats, all_labels, scatter)
+            else:
+                 self.util.debug('can\'t do scatterplot if not classification')
+
+
         # check if a tsne should be plotted
         tsne = eval(self.util.config_val('EXPL', 'tsne', 'False'))
         if tsne: 
             if self.util.exp_is_classification():
                 plots = Plots()
                 all_feats =self.feats_train.append(self.feats_test)
                 all_labels = self.df_train['class_label'].append(self.df_test['class_label'])
```

### Comparing `nkululeko-0.43.6/nkululeko/explore.py` & `nkululeko-0.44.0/nkululeko/explore.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
 
     plot_feats = eval(util.config_val('EXPL', 'feature_distributions', 'False'))
     tsne = eval(util.config_val('EXPL', 'tsne', 'False'))
-    if plot_feats or tsne: 
+    scatter = eval(util.config_val('EXPL', 'scatter', 'False'))
+    if plot_feats or tsne or scatter: 
         # extract features
         expr.extract_feats()
 
     # explore
     expr.analyse_features()
 
     print('DONE')
```

### Comparing `nkululeko-0.43.6/nkululeko/feats_analyser.py` & `nkululeko-0.44.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_audmodel.py` & `nkululeko-0.44.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_import.py` & `nkululeko-0.44.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_mld.py` & `nkululeko-0.44.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_opensmile.py` & `nkululeko-0.44.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_oxbow.py` & `nkululeko-0.44.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_praat.py` & `nkululeko-0.44.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feats_trill.py` & `nkululeko-0.44.0/nkululeko/feats_trill.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 assert tf.executing_eagerly()
 import tensorflow_hub as hub
 
 class TRILLset(Featureset):
     """A feature extractor for the Google TRILL embeddings"""
     """https://ai.googleblog.com/2020/06/improving-speech-representations-and.html"""
 
-# Initialization of the class
-def __init__(self, name, data_df):
-    """
-    Initialize the class with name, data and Util instance
-    Also loads the model from hub
-    
-    :param name: Name of the class
-    :type name: str
-    :param data_df: Data of the class
-    :type data_df: DataFrame
-    :return: None
-    """
-    self.name = name
-    self.data_df = data_df 
-    self.util = Util()
-    # Load the model from the configured path
-    model_path = self.util.config_val('FEATS', 'trill.model', \
-        'https://tfhub.dev/google/nonsemantic-speech-benchmark/trill/3')
-    self.module = hub.load(model_path)
+    # Initialization of the class
+    def __init__(self, name, data_df):
+        """
+        Initialize the class with name, data and Util instance
+        Also loads the model from hub
+        
+        :param name: Name of the class
+        :type name: str
+        :param data_df: Data of the class
+        :type data_df: DataFrame
+        :return: None
+        """
+        self.name = name
+        self.data_df = data_df 
+        self.util = Util()
+        # Load the model from the configured path
+        model_path = self.util.config_val('FEATS', 'trill.model', \
+            'https://tfhub.dev/google/nonsemantic-speech-benchmark/trill/3')
+        self.module = hub.load(model_path)
 
 
     def extract(self):
         store = self.util.get_path('store')
         storage = f'{store}{self.name}.pkl'
         extract = self.util.config_val('FEATS', 'needs_feature_extraction', False)
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
```

### Comparing `nkululeko-0.43.6/nkululeko/feats_wav2vec2.py` & `nkululeko-0.44.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feature_extractor.py` & `nkululeko-0.44.0/nkululeko/feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
                 self.featExtractor = TRILLset(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='wav2vec':
                 from nkululeko.feats_wav2vec2 import Wav2vec2
                 self.featExtractor = Wav2vec2(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='audmodel':
                 from nkululeko.feats_audmodel import AudModelSet
                 self.featExtractor = AudModelSet(f'{store_name}_{self.feats_designation}', self.data_df)
+            elif feats_type=='clap':
+                from nkululeko.feats_clap import Clap
+                self.featExtractor = Clap(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='praat':
                 from nkululeko.feats_praat import Praatset
                 self.featExtractor = Praatset(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='mld':
                 from nkululeko.feats_mld import MLD_set
                 self.featExtractor = MLD_set(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='import':
```

### Comparing `nkululeko-0.43.6/nkululeko/featureset.py` & `nkululeko-0.44.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/feinberg_praat.py` & `nkululeko-0.44.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/filter_data.py` & `nkululeko-0.44.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/loss_ccc.py` & `nkululeko-0.44.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/loss_softf1loss.py` & `nkululeko-0.44.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model.py` & `nkululeko-0.44.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_cnn.py` & `nkululeko-0.44.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_gmm.py` & `nkululeko-0.44.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_knn.py` & `nkululeko-0.44.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_knn_reg.py` & `nkululeko-0.44.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_mlp.py` & `nkululeko-0.44.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_mlp_regression.py` & `nkululeko-0.44.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/model_svm.py` & `nkululeko-0.44.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/modelrunner.py` & `nkululeko-0.44.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/nkululeko.py` & `nkululeko-0.44.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/plots.py` & `nkululeko-0.44.0/nkululeko/plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,14 +42,52 @@
                 df[target].value_counts().plot(kind='bar', ax=axes, \
                     title=f'samples ({sampl_num})')
             plt.tight_layout()
             plt.savefig(f'{fig_dir}{filename}.{self.format}')
             fig.clear()
             plt.close(fig)
 
+    def scatter_plot(self, feats, labels, dimred_type):
+        fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
+        filename = self.util.get_exp_name()+dimred_type
+        filename = f'{fig_dir}{filename}.{self.format}'
+        self.util.debug(f'computing {dimred_type}, this might take a while...')
+        data = None
+        if dimred_type == 'tsne':
+            data = self.getTsne(feats)
+        elif dimred_type == 'umap':
+            import umap
+            y_umap = umap.UMAP(n_neighbors=10, random_state=0,).fit_transform(feats.values)
+            data = pd.DataFrame(
+                y_umap,
+                feats.index,
+                columns=['Dim_1', 'Dim_2'],
+            )
+        elif dimred_type == 'pca':
+            from sklearn.decomposition import PCA
+            from sklearn.preprocessing import StandardScaler
+            scaler = StandardScaler()
+            pca = PCA(n_components=2)
+            y_pca = pca.fit_transform(scaler.fit_transform(feats.values))
+            data = pd.DataFrame(
+                y_pca,
+                feats.index,
+                columns=['Dim_1', 'Dim_2'],
+            )
+        else:
+            self.util.error(f'no such dimensionaity reduction functin: {dimred_type}')
+        plot_data = np.vstack((data.T, labels)).T
+        plot_df = pd.DataFrame(data=plot_data, columns=('Dim_1', 'Dim_2', 'label'))
+        plt.tight_layout()
+        ax = sns.FacetGrid(plot_df, hue='label', height=6).map(plt.scatter, 'Dim_1', 'Dim_2').add_legend()
+        fig = ax.figure
+        plt.savefig(filename)
+        fig.clear()
+        plt.close(fig)
+
     def plotTsne(self, feats, labels, filename, perplexity=30, learning_rate=200):
         """Make a TSNE plot to see whether features are useful for classification"""
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
         filename = f'{fig_dir}{filename}.{self.format}'
         self.util.debug(f'plotting tsne to {filename}, this might take a while...')
         model = TSNE(n_components=2, random_state=0, perplexity=perplexity, learning_rate=learning_rate)
         tsne_data = model.fit_transform(feats)
@@ -58,14 +96,20 @@
         plt.tight_layout()
         ax = sns.FacetGrid(tsne_df, hue='label', height=6).map(plt.scatter, 'Dim_1', 'Dim_2').add_legend()
         fig = ax.figure
         plt.savefig(filename)
         fig.clear()
         plt.close(fig)
 
+    def getTsne(self, feats, perplexity=30, learning_rate=200):
+        """Make a TSNE plot to see whether features are useful for classification"""
+        model = TSNE(n_components=2, random_state=0, perplexity=perplexity, learning_rate=learning_rate)
+        tsne_data = model.fit_transform(feats)
+        return tsne_data
+
     def plot_feature(self, title, feature, label, df_labels, df_features):
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
         filename = f'{fig_dir}feat_dist_{title}_{feature}.{self.format}'
         df_plot =  pd.DataFrame({label:df_labels[label], feature:df_features[feature]})
         ax = sns.violinplot(data=df_plot, x=label, y=feature)
         label = self.util.config_val('DATA', 'target', 'class_label')
         ax.set(title=f'{title} samples', xlabel = label)
```

### Comparing `nkululeko-0.43.6/nkululeko/reporter.py` & `nkululeko-0.44.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/runmanager copy.py` & `nkululeko-0.44.0/nkululeko/runmanager copy.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/runmanager.py` & `nkululeko-0.44.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/scaler.py` & `nkululeko-0.44.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/test.py` & `nkululeko-0.44.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/test_predictor.py` & `nkululeko-0.44.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko/util.py` & `nkululeko-0.44.0/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.43.6/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.44.0/nkululeko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.43.6
+Version: 0.44.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,14 +206,22 @@
 
 ## Licence
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.44.0
+--------------
+* added scatter functions: tsne, pca, umap
+
+Version 0.43.7
+--------------
+* added clap features
+
 Version 0.43.6
 --------------
 * small bugs
 
 
 Version 0.43.5
 --------------
```

### Comparing `nkululeko-0.43.6/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.44.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 nkululeko/dataset_ravdess.py
 nkululeko/demo.py
 nkululeko/demo_predictor.py
 nkululeko/experiment.py
 nkululeko/explore.py
 nkululeko/feats_analyser.py
 nkululeko/feats_audmodel.py
+nkululeko/feats_clap.py
 nkululeko/feats_import.py
 nkululeko/feats_mld.py
 nkululeko/feats_opensmile.py
 nkululeko/feats_oxbow.py
 nkululeko/feats_praat.py
 nkululeko/feats_trill.py
 nkululeko/feats_wav2vec2.py
```

### Comparing `nkululeko-0.43.6/setup.cfg` & `nkululeko-0.44.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.43.6
+version = 0.44.0
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers = 
@@ -21,27 +21,30 @@
 	audformat
 	audinterface
 	audiofile
 	audiomentations
 	audonnx
 	datasets
 	imageio
+	laion-clap
 	matplotlib
 	numpy
 	opensmile
 	pandas
 	praat-parselmouth
 	scikit_learn
 	scipy
 	seaborn
 	sounddevice
 	tensorflow
 	tensorflow_hub
 	torch
+	torchvision
 	transformers
+	umap-learn
 	xgboost
 python_requires = >=3.6
 include_package_data = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

