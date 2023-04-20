# Comparing `tmp/hive-maia-1.1.2a0.tar.gz` & `tmp/hive-maia-1.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-maia-1.1.2a0.tar", last modified: Wed Apr 19 14:41:10 2023, max compression
+gzip compressed data, was "hive-maia-1.1.2b0.tar", last modified: Thu Apr 20 08:19:19 2023, max compression
```

## Comparing `hive-maia-1.1.2a0.tar` & `hive-maia-1.1.2b0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/
--rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/__init__.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/configs/
--rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/ATM_nnUNet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/configs/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/configs/nnDet_config_template.json
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/evaluation/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/abstract.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/evaluation/detection/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/coco.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/froc.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/hist.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive/evaluation/detection/matching.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.587450 hive-maia-1.1.2a0/Hive/utils/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    23360 2023-04-19 14:39:29.000000 hive-maia-1.1.2a0/Hive/utils/file_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/log_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive/utils/seg_mask_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive/utils/volume_utils.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/Hive_scripts/
--rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_create_subset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_extract_experiment_predictions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_order_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1413 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/Hive_run_pipeline_from_file.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_compute_metric_results.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     5238 2023-04-19 14:28:18.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_create_pipeline.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/nndet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_prediction.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/nnunet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.2a0/Hive_scripts/script_template.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/Hive_scripts/upload_DICOM_to_Orthanc.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.2a0/LICENSE
--rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/PKG-INFO
--rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)        7 2023-04-19 14:40:19.000000 hive-maia-1.1.2a0/VERSION
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/hive_maia.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-19 14:41:09.000000 hive-maia-1.1.2a0/hive_maia.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:41:09.000000 hive-maia-1.1.2a0/hive_maia.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-19 14:41:10.000000 hive-maia-1.1.2a0/hive_maia.egg-info/top_level.txt
--rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.2a0/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 14:25:55.000000 hive-maia-1.1.2a0/requirements.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 14:03:53.000000 hive-maia-1.1.2a0/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-19 14:41:10.591450 hive-maia-1.1.2a0/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 14:25:50.000000 hive-maia-1.1.2a0/tests/test_file_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.764877 hive-maia-1.1.2b0/Hive/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive/__init__.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.764877 hive-maia-1.1.2b0/Hive/configs/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/ATM_nnUNet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive/configs/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/configs/nnDet_config_template.json
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.764877 hive-maia-1.1.2b0/Hive/evaluation/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/abstract.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.764877 hive-maia-1.1.2b0/Hive/evaluation/detection/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/detection/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/detection/coco.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/detection/froc.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/detection/hist.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive/evaluation/detection/matching.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/Hive/utils/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive/utils/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    23360 2023-04-19 14:39:29.000000 hive-maia-1.1.2b0/Hive/utils/file_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive/utils/log_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive/utils/seg_mask_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive/utils/volume_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/Hive_scripts/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_create_subset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_extract_experiment_predictions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_order_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1815 2023-04-20 07:57:32.000000 hive-maia-1.1.2b0/Hive_scripts/Hive_run_pipeline_from_file.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/Hive_scripts/nndet_compute_metric_results.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     5663 2023-04-20 07:56:45.000000 hive-maia-1.1.2b0/Hive_scripts/nndet_create_pipeline.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/nndet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/nndet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/nndet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/nnunet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/nnunet_run_prediction.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/nnunet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/nnunet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.2b0/Hive_scripts/script_template.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/Hive_scripts/upload_DICOM_to_Orthanc.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.2b0/LICENSE
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/PKG-INFO
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)        7 2023-04-19 15:34:01.000000 hive-maia-1.1.2b0/VERSION
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/hive_maia.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1649 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-20 08:19:19.000000 hive-maia-1.1.2b0/hive_maia.egg-info/top_level.txt
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.2b0/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 14:25:55.000000 hive-maia-1.1.2b0/requirements.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 14:03:53.000000 hive-maia-1.1.2b0/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 08:19:19.768877 hive-maia-1.1.2b0/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 14:25:50.000000 hive-maia-1.1.2b0/tests/test_file_utils.py
```

### Comparing `hive-maia-1.1.2a0/Hive/__init__.py` & `hive-maia-1.1.2b0/Hive/__init__.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json` & `hive-maia-1.1.2b0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/configs/nnDet_config_template.json` & `hive-maia-1.1.2b0/Hive/configs/nnDet_config_template.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/evaluation/abstract.py` & `hive-maia-1.1.2b0/Hive/evaluation/abstract.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/evaluation/detection/coco.py` & `hive-maia-1.1.2b0/Hive/evaluation/detection/coco.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/evaluation/detection/froc.py` & `hive-maia-1.1.2b0/Hive/evaluation/detection/froc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/evaluation/detection/hist.py` & `hive-maia-1.1.2b0/Hive/evaluation/detection/hist.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/evaluation/detection/matching.py` & `hive-maia-1.1.2b0/Hive/evaluation/detection/matching.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/utils/file_utils.py` & `hive-maia-1.1.2b0/Hive/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/utils/log_utils.py` & `hive-maia-1.1.2b0/Hive/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/utils/seg_mask_utils.py` & `hive-maia-1.1.2b0/Hive/utils/seg_mask_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive/utils/volume_utils.py` & `hive-maia-1.1.2b0/Hive/utils/volume_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_create_subset.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_create_subset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_extract_experiment_predictions.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_extract_experiment_predictions.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_order_data_folder.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_order_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/Hive_run_pipeline_from_file.py` & `hive-maia-1.1.2b0/Hive_scripts/Hive_run_pipeline_from_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime
 import subprocess
 from argparse import ArgumentParser, RawTextHelpFormatter
 from pathlib import Path
 from textwrap import dedent
 
-from Hive.utils.log_utils import get_logger, add_verbosity_options_to_argparser, log_lvl_from_verbosity_args, DEBUG
+from Hive.utils.log_utils import get_logger, add_verbosity_options_to_argparser, log_lvl_from_verbosity_args, INFO
 
 TIMESTAMP = "{:%Y-%m-%d_%H-%M-%S}".format(datetime.datetime.now())
 
 DESC = dedent(
     """
     Run pipeline steps from a TXT file.
     """  # noqa: E501
@@ -32,14 +32,22 @@
     pars.add_argument(
         "--file",
         type=str,
         required=True,
         help="TXT file including list of commands to run.",
     )
 
+    pars.add_argument(
+        "--steps",
+        type=str,
+        nargs="+",
+        required=False,
+        help="Optional pipeline steps to run. When omitted, run all the steps.",
+    )
+
     add_verbosity_options_to_argparser(pars)
 
     return pars
 
 
 def main():
     parser = get_arg_parser()
@@ -50,14 +58,20 @@
         name=Path(__file__).name,
         level=log_lvl_from_verbosity_args(arguments),
     )
 
     with open(arguments["file"]) as f:
         commands = f.readlines()
 
-    for command in commands:
-        logger.log(DEBUG, "Running: {}".format(command))
-        subprocess.call(command[:-1].split(" "))
+    steps = range(len(commands))
+    if arguments["steps"] is not None:
+        steps = arguments["steps"]
+        steps = [int(step) for step in steps]
+
+    for it, command in enumerate(commands):
+        if it in steps:
+            logger.log(INFO, "Running Step {}: {}".format(it, command))
+            subprocess.call(command[:-1].split(" "))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nndet_compute_metric_results.py` & `hive-maia-1.1.2b0/Hive_scripts/nndet_compute_metric_results.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nndet_create_pipeline.py` & `hive-maia-1.1.2b0/Hive_scripts/nndet_create_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import datetime
 import importlib.resources
 import json
+import logging
 import os
 from argparse import ArgumentParser, RawTextHelpFormatter
 from pathlib import Path
 from textwrap import dedent
 
 import Hive.configs
 from Hive.utils.log_utils import (
@@ -67,14 +68,21 @@
     pars.add_argument(
         "--config-file",
         type=str,
         required=True,
         help="Configuration JSON file with experiment and dataset parameters.",
     )
 
+    pars.add_argument(
+        "--output-file",
+        type=str,
+        required=False,
+        help="Output TXT file path  where to save the pipeline steps.",
+    )
+
     add_verbosity_options_to_argparser(pars)
 
     return pars
 
 
 def run_data_and_folder_preparation_step(arguments):
     try:
@@ -92,15 +100,15 @@
         "--task-ID",
         arguments["task_ID"],
         "--task-name",
         config_dict["DatasetName"] + "_" + config_dict["Experiment Name"],
         "--config-file",
         arguments["config_file"],
         "--test-split",
-        arguments["test_split"]
+        str(arguments["test_split"])
     ]
 
     return args
 
 
 def run_preprocessing_step(config_file):
     args = [
@@ -142,15 +150,15 @@
             config_dict = json.load(json_file)
     except FileNotFoundError:
         with importlib.resources.path(Hive.configs, arguments["config_file"]) as json_path:
             with open(json_path) as json_file:
                 config_dict = json.load(json_file)
 
     output_json_config_filename = (
-        config_dict["DatasetName"] + "_" + config_dict["Experiment Name"] + "_" + arguments["task_ID"] + ".json"
+            config_dict["DatasetName"] + "_" + config_dict["Experiment Name"] + "_" + arguments["task_ID"] + ".json"
     )
     os.environ["RESULTS_FOLDER"] = str(
         Path(os.environ["root_experiment_folder"]).joinpath(
             config_dict["Experiment Name"],
             "Task" + arguments["task_ID"] + "_" + config_dict["DatasetName"] + "_" + config_dict["Experiment Name"],
             "results",
         )
@@ -158,27 +166,33 @@
     output_json_config_file = str(Path(os.environ["RESULTS_FOLDER"]).joinpath(output_json_config_filename))
 
     pipeline_steps = []
 
     pipeline_steps.append(run_data_and_folder_preparation_step(arguments))
     pipeline_steps.append(run_preprocessing_step(output_json_config_file))
 
-    [pipeline_steps.append(step) for step in run_training_step(output_json_config_file, range(config_dict["n_folds"]))]
-
-    pipeline_steps.append(run_training_step(output_json_config_file, [-1]))
+    [pipeline_steps.append(step) for step in
+     run_training_step(output_json_config_file, list(range(config_dict["n_folds"])) + [-1, ])]
 
     Path(os.environ["root_experiment_folder"]).joinpath(config_dict["Experiment Name"]).mkdir(exist_ok=True,
                                                                                               parents=True)
-    pipeline_steps_summary = open(
-        Path(os.environ["root_experiment_folder"]).joinpath(
-            config_dict["Experiment Name"], "Task_" + arguments["task_ID"] + "_" + TIMESTAMP + ".txt"
-        ),
-        "w",
+
+    output_file = Path(os.environ["root_experiment_folder"]).joinpath(
+        config_dict["Experiment Name"], "Task_" + arguments["task_ID"] + "_" + TIMESTAMP + ".txt"
     )
-    for step in pipeline_steps:
+
+    if arguments["output_file"] is not None:
+        output_file = arguments["output_file"]
+
+    pipeline_steps_summary = open(output_file
+                                  ,
+                                  "w",
+                                  )
+    for it, step in enumerate(pipeline_steps):
+        logger.log(logging.INFO, "Step {}: {}".format(it, " ".join(step)))
         pipeline_steps_summary.write(" ".join(step) + "\n")
 
     pipeline_steps_summary.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nndet_prepare_data_folder.py` & `hive-maia-1.1.2b0/Hive_scripts/nndet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nndet_run_preprocessing.py` & `hive-maia-1.1.2b0/Hive_scripts/nndet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nndet_run_training.py` & `hive-maia-1.1.2b0/Hive_scripts/nndet_run_training.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nnunet_prepare_data_folder.py` & `hive-maia-1.1.2b0/Hive_scripts/nnunet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_prediction.py` & `hive-maia-1.1.2b0/Hive_scripts/nnunet_run_prediction.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_preprocessing.py` & `hive-maia-1.1.2b0/Hive_scripts/nnunet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/nnunet_run_training.py` & `hive-maia-1.1.2b0/Hive_scripts/nnunet_run_training.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/script_template.py` & `hive-maia-1.1.2b0/Hive_scripts/script_template.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/Hive_scripts/upload_DICOM_to_Orthanc.py` & `hive-maia-1.1.2b0/Hive_scripts/upload_DICOM_to_Orthanc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/LICENSE` & `hive-maia-1.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/PKG-INFO` & `hive-maia-1.1.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.2a0
+Version: 1.1.2b0
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.2a0/README.md` & `hive-maia-1.1.2b0/README.md`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/hive_maia.egg-info/PKG-INFO` & `hive-maia-1.1.2b0/hive_maia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.2a0
+Version: 1.1.2b0
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.2a0/hive_maia.egg-info/SOURCES.txt` & `hive-maia-1.1.2b0/hive_maia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/hive_maia.egg-info/entry_points.txt` & `hive-maia-1.1.2b0/hive_maia.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2a0/setup.py` & `hive-maia-1.1.2b0/setup.py`

 * *Files identical despite different names*

