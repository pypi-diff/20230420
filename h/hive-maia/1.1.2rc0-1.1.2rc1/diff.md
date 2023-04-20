# Comparing `tmp/hive-maia-1.1.2rc0.tar.gz` & `tmp/hive-maia-1.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-maia-1.1.2rc0.tar", last modified: Thu Apr 20 09:40:07 2023, max compression
+gzip compressed data, was "hive-maia-1.1.2rc1.tar", last modified: Thu Apr 20 10:07:06 2023, max compression
```

## Comparing `hive-maia-1.1.2rc0.tar` & `hive-maia-1.1.2rc1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.357307 hive-maia-1.1.2rc0/Hive/
--rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive/__init__.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.357307 hive-maia-1.1.2rc0/Hive/configs/
--rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/ATM_nnUNet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive/configs/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/configs/nnDet_config_template.json
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.357307 hive-maia-1.1.2rc0/Hive/evaluation/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/abstract.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.357307 hive-maia-1.1.2rc0/Hive/evaluation/detection/
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/detection/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/detection/coco.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/detection/froc.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/detection/hist.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive/evaluation/detection/matching.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.357307 hive-maia-1.1.2rc0/Hive/utils/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive/utils/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    23360 2023-04-19 14:39:29.000000 hive-maia-1.1.2rc0/Hive/utils/file_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive/utils/log_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive/utils/seg_mask_utils.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive/utils/volume_utils.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/Hive_scripts/
--rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_create_subset.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_extract_experiment_predictions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_order_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1815 2023-04-20 07:57:32.000000 hive-maia-1.1.2rc0/Hive_scripts/Hive_run_pipeline_from_file.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/Hive_scripts/nndet_compute_metric_results.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     5731 2023-04-20 09:39:16.000000 hive-maia-1.1.2rc0/Hive_scripts/nndet_create_pipeline.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/nndet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/nndet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3296 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/nndet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/nnunet_prepare_data_folder.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_prediction.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_preprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_training.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc0/Hive_scripts/script_template.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/Hive_scripts/upload_DICOM_to_Orthanc.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.2rc0/LICENSE
--rw-rw-r--   0 simone    (1000) simone    (1000)     1650 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/PKG-INFO
--rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)        7 2023-04-20 09:39:25.000000 hive-maia-1.1.2rc0/VERSION
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/hive_maia.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1650 2023-04-20 09:40:06.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-20 09:40:07.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-20 09:40:06.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-20 09:40:07.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-20 09:40:07.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-20 09:40:07.000000 hive-maia-1.1.2rc0/hive_maia.egg-info/top_level.txt
--rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.2rc0/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 14:25:55.000000 hive-maia-1.1.2rc0/requirements.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc0/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 09:40:07.361307 hive-maia-1.1.2rc0/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc0/tests/test_file_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.210913 hive-maia-1.1.2rc1/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.202913 hive-maia-1.1.2rc1/Hive/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      554 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive/__init__.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.202913 hive-maia-1.1.2rc1/Hive/configs/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      458 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/ATM_nnUNet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      301 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/AutoPET_Positive_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      883 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/LymphNodeSeg_ABD_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)      272 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/LymphNodeSeg_MED_nnDet_3D_fullres_config.json
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive/configs/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1043 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/configs/nnDet_config_template.json
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.202913 hive-maia-1.1.2rc1/Hive/evaluation/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3946 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/abstract.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/Hive/evaluation/detection/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/detection/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16106 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/detection/coco.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    15779 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/detection/froc.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7868 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/detection/hist.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11722 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive/evaluation/detection/matching.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/Hive/utils/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive/utils/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    23360 2023-04-19 14:39:29.000000 hive-maia-1.1.2rc1/Hive/utils/file_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1978 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive/utils/log_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1484 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive/utils/seg_mask_utils.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    12126 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive/utils/volume_utils.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/Hive_scripts/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     6963 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1204 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3080 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3052 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_create_subset.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-04-19 12:05:41.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_extract_experiment_predictions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4047 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_order_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1815 2023-04-20 07:57:32.000000 hive-maia-1.1.2rc1/Hive_scripts/Hive_run_pipeline_from_file.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11048 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/Hive_scripts/nndet_compute_metric_results.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     5731 2023-04-20 09:39:16.000000 hive-maia-1.1.2rc1/Hive_scripts/nndet_create_pipeline.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8268 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/nndet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2744 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/nndet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3340 2023-04-20 10:05:41.000000 hive-maia-1.1.2rc1/Hive_scripts/nndet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8706 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/nnunet_prepare_data_folder.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3645 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_prediction.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2064 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_preprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3996 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_training.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1139 2023-01-18 15:13:07.000000 hive-maia-1.1.2rc1/Hive_scripts/script_template.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3471 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/Hive_scripts/upload_DICOM_to_Orthanc.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    35149 2023-01-18 15:01:57.000000 hive-maia-1.1.2rc1/LICENSE
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1650 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/PKG-INFO
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      914 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)        9 2023-04-20 10:06:21.000000 hive-maia-1.1.2rc1/VERSION
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/hive_maia.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1650 2023-04-20 10:07:05.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1825 2023-04-20 10:07:06.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-20 10:07:05.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      872 2023-04-20 10:07:05.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)      133 2023-04-20 10:07:05.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       18 2023-04-20 10:07:06.000000 hive-maia-1.1.2rc1/hive_maia.egg-info/top_level.txt
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      330 2023-01-18 15:01:52.000000 hive-maia-1.1.2rc1/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      132 2023-04-19 14:25:55.000000 hive-maia-1.1.2rc1/requirements.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2023-04-20 10:07:06.210913 hive-maia-1.1.2rc1/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2938 2023-04-19 14:03:53.000000 hive-maia-1.1.2rc1/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-20 10:07:06.206913 hive-maia-1.1.2rc1/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      157 2023-04-19 14:25:50.000000 hive-maia-1.1.2rc1/tests/test_file_utils.py
```

### Comparing `hive-maia-1.1.2rc0/Hive/__init__.py` & `hive-maia-1.1.2rc1/Hive/__init__.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json` & `hive-maia-1.1.2rc1/Hive/configs/LungLobeSeg_nnUNet_3D_fullres_In_config.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/configs/nnDet_config_template.json` & `hive-maia-1.1.2rc1/Hive/configs/nnDet_config_template.json`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/evaluation/abstract.py` & `hive-maia-1.1.2rc1/Hive/evaluation/abstract.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/evaluation/detection/coco.py` & `hive-maia-1.1.2rc1/Hive/evaluation/detection/coco.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/evaluation/detection/froc.py` & `hive-maia-1.1.2rc1/Hive/evaluation/detection/froc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/evaluation/detection/hist.py` & `hive-maia-1.1.2rc1/Hive/evaluation/detection/hist.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/evaluation/detection/matching.py` & `hive-maia-1.1.2rc1/Hive/evaluation/detection/matching.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/utils/file_utils.py` & `hive-maia-1.1.2rc1/Hive/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/utils/log_utils.py` & `hive-maia-1.1.2rc1/Hive/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/utils/seg_mask_utils.py` & `hive-maia-1.1.2rc1/Hive/utils/seg_mask_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive/utils/volume_utils.py` & `hive-maia-1.1.2rc1/Hive/utils/volume_utils.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_DICOM_dataset_to_NIFTI_dataset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_NIFTI_predictions_to_DICOM_SEG.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_convert_semantic_to_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_create_subset.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_create_subset.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_extract_experiment_predictions.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_extract_experiment_predictions.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_order_data_folder.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_order_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/Hive_run_pipeline_from_file.py` & `hive-maia-1.1.2rc1/Hive_scripts/Hive_run_pipeline_from_file.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nndet_compute_metric_results.py` & `hive-maia-1.1.2rc1/Hive_scripts/nndet_compute_metric_results.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nndet_create_pipeline.py` & `hive-maia-1.1.2rc1/Hive_scripts/nndet_create_pipeline.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nndet_prepare_data_folder.py` & `hive-maia-1.1.2rc1/Hive_scripts/nndet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nndet_run_preprocessing.py` & `hive-maia-1.1.2rc1/Hive_scripts/nndet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nndet_run_training.py` & `hive-maia-1.1.2rc1/Hive_scripts/nndet_run_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             "-o",
             "exp.fold={}".format(args["run_fold"]),
         ]
 
         if args["resume_training"]:
             arguments.append("train.mode=resume")
 
+        arguments.extend(unknown_arguments)
         os.environ["det_data"] = data["base_folder"]
         os.environ["OMP_NUM_THREADS"] = "1"
         os.environ["det_num_threads"] = os.environ["N_THREADS"]
         os.environ["nnUNet_def_n_proc"] = os.environ["N_THREADS"]
         os.environ["det_models"] = data["results_folder"]
 
         if "receiver_email" in data:
```

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nnunet_prepare_data_folder.py` & `hive-maia-1.1.2rc1/Hive_scripts/nnunet_prepare_data_folder.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_prediction.py` & `hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_prediction.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_preprocessing.py` & `hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/nnunet_run_training.py` & `hive-maia-1.1.2rc1/Hive_scripts/nnunet_run_training.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/script_template.py` & `hive-maia-1.1.2rc1/Hive_scripts/script_template.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/Hive_scripts/upload_DICOM_to_Orthanc.py` & `hive-maia-1.1.2rc1/Hive_scripts/upload_DICOM_to_Orthanc.py`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/LICENSE` & `hive-maia-1.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/PKG-INFO` & `hive-maia-1.1.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.2rc0
+Version: 1.1.2rc1
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.2rc0/README.md` & `hive-maia-1.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/hive_maia.egg-info/PKG-INFO` & `hive-maia-1.1.2rc1/hive_maia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-maia
-Version: 1.1.2rc0
+Version: 1.1.2rc1
 Summary: Python Package to support Deep Learning data preparation, pre-processing. training, result visualization and model deployment across different frameworks (nnUNet, nnDetection, MONAI).
 Home-page: https://github.com/MAIA-KTH/Hive.git
 Author: Simone Bendazzoli
 Author-email: simben@kth.se
 License: GPLv3
 Project-URL: Documentation, https://hive-maia.readthedocs.io
 Project-URL: Source, https://github.com/MAIA-KTH/Hive
```

### Comparing `hive-maia-1.1.2rc0/hive_maia.egg-info/SOURCES.txt` & `hive-maia-1.1.2rc1/hive_maia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/hive_maia.egg-info/entry_points.txt` & `hive-maia-1.1.2rc1/hive_maia.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hive-maia-1.1.2rc0/setup.py` & `hive-maia-1.1.2rc1/setup.py`

 * *Files identical despite different names*

