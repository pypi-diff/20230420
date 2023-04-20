# Comparing `tmp/Simba-UW-tf-dev-1.56.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.56.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.8.tar", last modified: Wed Apr 19 14:56:18 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.9.tar", last modified: Thu Apr 20 01:49:27 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.8.tar` & `Simba-UW-tf-dev-1.56.9.tar`

### file list

```diff
@@ -1,391 +1,393 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.8/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11585 2023-04-19 14:00:17.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     1759 2023-04-18 23:05:39.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     5384 2023-04-17 20:49:22.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/grd_search_cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-19 14:11:27.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7061 2023-04-18 19:40:55.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     6681 2023-04-19 12:53:45.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    10557 2023-04-18 23:05:39.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    18462 2023-04-18 17:25:40.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8392 2023-04-17 17:37:22.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.56.8/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-19 14:11:32.000000 Simba-UW-tf-dev-1.56.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.8/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.8/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8217 2023-04-18 15:24:14.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     5584 2023-04-18 16:54:56.000000 Simba-UW-tf-dev-1.56.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.8/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.56.8/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.8/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.8/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.8/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    46900 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.8/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.8/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.8/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.8/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.8/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.8/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.8/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.8/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.8/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.8/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.8/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56935 2023-04-18 14:46:46.000000 Simba-UW-tf-dev-1.56.8/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.8/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.8/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.8/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.8/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.8/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.8/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.8/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.8/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.8/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.56.8/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.8/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.8/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.8/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.8/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13367 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.8/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-19 14:54:56.000000 Simba-UW-tf-dev-1.56.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-19 14:56:18.000000 Simba-UW-tf-dev-1.56.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.9/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11585 2023-04-19 14:00:17.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     3364 2023-04-20 00:29:41.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-19 14:11:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7088 2023-04-19 15:24:28.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5375 2023-04-19 17:04:26.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-19 18:57:16.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)    10253 2023-04-19 15:20:53.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    43774 2023-04-20 00:55:59.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2267 2023-04-19 15:23:44.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8383 2023-04-19 19:54:15.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.56.9/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-19 18:06:57.000000 Simba-UW-tf-dev-1.56.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.9/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.9/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8217 2023-04-18 15:24:14.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.9/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.56.9/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.9/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.9/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.9/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    47110 2023-04-20 01:48:23.000000 Simba-UW-tf-dev-1.56.9/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.9/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.9/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.9/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.9/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.9/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.9/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.9/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.9/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.9/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56935 2023-04-18 14:46:46.000000 Simba-UW-tf-dev-1.56.9/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.9/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.9/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.9/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.9/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.9/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.9/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.9/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.56.9/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.9/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13424 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.9/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-20 01:49:18.000000 Simba-UW-tf-dev-1.56.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.8/PKG-INFO` & `Simba-UW-tf-dev-1.56.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.8
+Version: 1.56.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/video_processing.py` & `Simba-UW-tf-dev-1.56.9/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/unsupervised_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
                                      FileSelect)
 from PIL import ImageTk
 import PIL.Image
 import os
 from simba.utils.lookups import get_icons_paths
 import tkinter.ttk as ttk
 from simba.enums import Formats
+from simba.mixins.config_reader import ConfigReader
 from simba.enums import ReadConfig, Dtypes
 from simba.train_model_functions import get_all_clf_names
 from simba.unsupervised.dataset_creator import DatasetCreator
 from simba.unsupervised.pop_up_classes import (GridSearchClusterVisualizerPopUp,
                                                BatchDataExtractorPopUp,
                                                FitDimReductionPopUp,
                                                FitClusterModelsPopUp,
@@ -24,18 +25,20 @@
                                                ClusterVisualizerPopUp,
                                                ClusterFrequentistStatisticsPopUp,
                                                ClusterMLStatisticsPopUp,
                                                EmbedderCorrelationsPopUp,
                                                PrintEmBeddingInfoPopUp,
                                                DBCVPopUp)
 
-class UnsupervisedGUI(object):
+class UnsupervisedGUI(ConfigReader):
     def __init__(self,
                  config_path: str):
 
+        super().__init__(config_path=config_path)
+
         self.config, self.config_path = read_config_file(config_path), config_path
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.main = Toplevel()
         self.main.minsize(1000, 800)
         self.main.wm_title("UNSUPERVISED ANALYSIS")
         self.main.columnconfigure(0, weight=1)
         self.main.rowconfigure(0, weight=1)
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/grd_search_cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from simba.unsupervised.misc import check_directory_exists
+from simba.train_model_functions import check_if_dir_exists
 import glob, os
 import pandas as pd
 from simba.misc_tools import check_if_filepath_list_is_empty
 from simba.unsupervised.enums import Clustering, Unsupervised
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 import seaborn as sns
 import matplotlib.pyplot as plt
@@ -13,18 +13,17 @@
 class GridSearchVisualizer(UnsupervisedMixin):
     def __init__(self,
                  model_dir: str,
                  save_dir: str,
                  settings: dict):
 
         super().__init__()
-        check_directory_exists(save_dir)
+        check_if_dir_exists(in_dir=save_dir)
+        check_if_dir_exists(in_dir=model_dir)
         self.save_dir, self.settings, self.model_dir = save_dir, settings, model_dir
-        check_directory_exists(save_dir)
-        check_directory_exists(model_dir)
         self.data_path = glob.glob(model_dir + '/*.pickle')
         check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {model_dir}')
 
     def cluster_visualizer(self):
         data = self.read_pickle(self.model_dir)
         for k, v in data.items():
             self.check_key_exist_in_object(object=v, key=Clustering.CLUSTER_MODEL.value)
@@ -45,15 +44,15 @@
         for k, v in data.items():
             self.check_key_exist_in_object(object=v, key=Unsupervised.DR_MODEL.value)
         for k, v in data.items():
             for variable in categoricals:
                 save_path = os.path.join(self.save_dir, f'{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{variable}.png')
                 data = pd.DataFrame(v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
                 data = pd.concat([v[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value][variable], data], axis=1)
-                plot = sns.scatterplot(data=data, x='X', y='Y', hue=variable, palette=self.settings['PALETTE'])
+                plot = sns.scatterplot(data=data, x='X', y='Y', hue=variable, palette=self.settings['CATEGORICAL_PALETTE'])
                 plt.savefig(save_path)
                 stdout_success(msg=f'Saved {save_path}...')
                 plt.close('all')
         self.timer.stop_timer()
         stdout_success(msg='All cluster images created.', elapsed_time=self.timer.elapsed_time_str)
 
     def continuous_visualizer(self,
@@ -65,15 +64,15 @@
             for variable in continuous_vars:
                 save_path = os.path.join(self.save_dir, f'{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{variable}.png')
                 fig, ax = plt.subplots()
                 plt.xlabel('X')
                 plt.ylabel('Y')
                 data = pd.DataFrame(v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
                 data = pd.concat([v[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value][variable], data], axis=1)
-                points = ax.scatter(data['X'], data['Y'], c=data[variable], s=self.settings['SCATTER_SIZE'], cmap=self.settings['PALETTE'])
+                points = ax.scatter(data['X'], data['Y'], c=data[variable], s=self.settings['SCATTER_SIZE'], cmap=self.settings['CONTINUOUS_PALETTE'])
                 cbar = fig.colorbar(points)
                 cbar.set_label(variable, loc='center')
                 title = v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]
                 plt.title(title, ha="center", fontsize=15, bbox={"facecolor": "orange", "alpha": 0.5, "pad": 0})
                 fig.savefig(save_path)
                 plt.close('all')
                 stdout_success(msg=f'Saved {save_path}...')
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/dataset_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pandas as pd
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_file_exist_and_readable)
-from simba.unsupervised.misc import bout_aggregator
+from simba.unsupervised.bout_aggregator import bout_aggregator
 from simba.misc_tools import get_fn_ext
 from simba.unsupervised.enums import Unsupervised
 from simba.mixins.config_reader import ConfigReader
 from simba.drop_bp_cords import getBpNames
 from simba.rw_dfs import read_df
 from simba.utils.errors import NoDataError
 from simba.utils.printing import stdout_success
@@ -108,16 +108,16 @@
 
         with open(self.save_path, 'wb') as f:
             pickle.dump(results, f, protocol=pickle.HIGHEST_PROTOCOL)
         self.timer.stop_timer()
         self.__aggregate_dataset_stats()
         stdout_success(msg=f'Dataset for unsupervised learning saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-settings = {'data_slice': 'ALL FEATURES (EXCLUDING POSE)',
-            'clf_slice': 'Attack',
-            'bout_aggregation_type': 'MEDIAN',
-            'min_bout_length': 66,
-            'feature_path': '/Users/simon/Desktop/envs/simba_dev/simba/assets/unsupervised/features.csv'}
-#
-_ = DatasetCreator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
-                   settings=settings)
+# settings = {'data_slice': 'ALL FEATURES (EXCLUDING POSE)',
+#             'clf_slice': 'Attack',
+#             'bout_aggregation_type': 'MEDIAN',
+#             'min_bout_length': 66,
+#             'feature_path': '/Users/simon/Desktop/envs/simba_dev/simba/assets/unsupervised/features.csv'}
+# #
+# _ = DatasetCreator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
+#                    settings=settings)
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pandas as pd
 
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.unsupervised.enums import Unsupervised, Clustering
-from simba.unsupervised.misc import check_directory_exists
+from simba.train_model_functions import check_if_dir_exists
 from simba.utils.printing import stdout_success
 from simba.misc_tools import check_file_exist_and_readable
 import json
 
 CLUSTERER_PARAMETERS = 'CLUSTERER HYPER-PARAMETERS'
 DIMENSIONALITY_REDUCTION_PARAMETERS = 'DIMENSIONALITY REDUCTION HYPER-PARAMETERS'
 SCALER = 'SCALER'
@@ -28,15 +28,15 @@
                  data_path: str,
                  data_type: str,
                  settings: dict or None=None):
 
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         if os.path.isdir(data_path):
-            check_directory_exists(directory=data_path)
+            check_if_dir_exists(in_dir=data_path)
             self.data = self.read_pickle(data_path=data_path)
         else:
             check_file_exist_and_readable(file_path=data_path)
             self.data = {0: self.read_pickle(data_path=data_path)}
         self.settings, self.data_type = settings, data_type
 
     def run(self):
@@ -108,13 +108,13 @@
                 save_path = os.path.join(self.logs_path, f'bout_targets_{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}.csv')
                 v[Unsupervised.DATA.value][Unsupervised.BOUTS_TARGETS.value].to_csv(save_path)
                 stdout_success(msg=f'Bout target data saved at {save_path}')
 
 
 
 
-test = DataExtractor(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle',
-                     data_type='BOUTS_TARGETS',
-                     settings=None,
-                     config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
-
-test.run()
+# test = DataExtractor(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle',
+#                      data_type='BOUTS_TARGETS',
+#                      settings=None,
+#                      config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+#
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/umap_embedder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import random
 from copy import deepcopy
 from simba.misc_tools import SimbaTimer
 from simba.read_config_unit_tests import check_file_exist_and_readable
-from simba.unsupervised.misc import check_that_directory_is_empty
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.unsupervised.enums import Unsupervised
 from simba.utils.printing import stdout_success
 
 import itertools
 import pandas as pd
 
@@ -29,15 +28,15 @@
             hyper_parameters: dict):
 
         self.data_path = data_path
         check_file_exist_and_readable(file_path=self.data_path)
         self.data = self.read_pickle(data_path=data_path)
         self.umap_df = deepcopy(self.data[Unsupervised.BOUTS_FEATURES.value]).set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value])
         self.save_dir = save_dir
-        check_that_directory_is_empty(directory=self.save_dir)
+        self.check_that_directory_is_empty(directory=self.save_dir)
         self.low_var_cols, self.hyper_parameters = None, hyper_parameters
         self.check_umap_hyperparameters(hyper_parameters=hyper_parameters)
         self.search_space = list(itertools.product(*[hyper_parameters[Unsupervised.N_NEIGHBORS.value],
                                                      hyper_parameters[Unsupervised.MIN_DISTANCE.value],
                                                      hyper_parameters[Unsupervised.SPREAD.value]]))
         print(f'Building {len(self.search_space)} UMAP model(s)...')
         if hyper_parameters[Unsupervised.VARIANCE.value] > 0:
@@ -90,16 +89,15 @@
 
     def transform(self,
                   data_path: str,
                   model: str or dict,
                   settings: dict,
                   save_dir: str or None=None):
 
-        timer = SimbaTimer()
-        timer.start_timer()
+        timer = SimbaTimer(start=True)
         if isinstance(model, str):
             check_file_exist_and_readable(file_path=model)
             model = self.read_pickle(data_path=model)
 
         check_file_exist_and_readable(file_path=data_path)
         data = self.read_pickle(data_path=data_path)
         self.umap_df = deepcopy(data[Unsupervised.BOUTS_FEATURES.value]).set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value])
@@ -114,69 +112,14 @@
         if save_dir:
             save_path = os.path.join(save_dir, f'Transformed_{model[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}.csv')
             if settings[Unsupervised.FORMAT.value] is Unsupervised.CSV.value:
                 self.results.to_csv(save_path)
             timer.stop_timer()
             print(f'Transformed data saved at {save_dir} (elapsed time: {timer.elapsed_time_str}s)')
 
-
-
-    #                 results.to_csv(save_path, index=False)
-
-
-
-
-
-
-
-
-
-# def UMAPTransform(model: str or object,
-#                   data_path: str,
-#                   settings: dict or None=None,
-#                   save_dir: str or None=None):
-#
-#         timer = SimbaTimer()
-#         timer.start_timer()
-#         if save_dir is not None:
-#             check_directory_exists(directory=save_dir)
-#         if type(model) == 'str':
-#             check_file_exist_and_readable(file_path=model)
-#             embedder = read_pickle(data_path=model)
-#         else:
-#             embedder = model
-#         check_file_exist_and_readable(file_path=data_path)
-#         data = read_pickle(data_path=data_path)
-#         data_df = drop_low_variance_fields(data=data['DATA'], fields=embedder['LOW_VARIANCE_FIELDS'])
-#         check_expected_fields(data_fields=data_df.columns, expected_fields=embedder['OUT_FEATURE_NAMES'])
-#         scaled_data = scaler_transform(data=data_df, scaler=embedder['SCALER'])
-#         transformed_data = pd.DataFrame(embedder['MODEL'].transform(scaled_data), columns=['X', 'Y'])
-#
-#         results = pd.concat([data['VIDEO_NAMES'],
-#                              data['START_FRAME'],
-#                              data['END_FRAME'],
-#                              data['CLF'],
-#                              data['CLF_PROBABILITY'],
-#                              transformed_data], axis=1)
-#         if settings:
-#             if settings['features'] == 'INCLUDE: ORIGINAL':
-#                 results = pd.concat([results, data_df], axis=1)
-#             if settings['features'] == 'INCLUDE: SCALED':
-#                 results = pd.concat([results, scaled_data], axis=1)
-#             if settings['save_format'] is 'csv':
-#                 save_path = os.path.join(save_dir, f'transformed_{embedder["HASH"]}.csv')
-#                 results.to_csv(save_path, index=False)
-#
-#         else:
-#             return transformed_data
-#
-#         timer.stop_timer()
-#         print('Transformed data saved at {} (elapsed time: {}s)'.format(save_dir, timer.elapsed_time_str))
-#
-
 # data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
 # save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/transformed_umap'
 # settings = {'DATA': 'RAW', 'format': 'csv'}
 # embedder = UmapEmbedder(data_path=data_path, save_dir=save_dir)
 # embedder.transform(model='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/boring_lederberg.pickle', settings=settings)
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/pop_up_classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,831 +1,698 @@
-import glob
-import os.path
+import os, glob
+from simba.mixins.pop_up_mixin import PopUpMixin
+from simba.mixins.config_reader import ConfigReader
 from tkinter import *
+from simba.enums import Formats, Options
+from simba.misc_tools import check_file_exist_and_readable
+from simba.unsupervised.enums import UnsupervisedOptions, Unsupervised, Clustering
 import numpy as np
 from simba.tkinter_functions import (FolderSelect,
                                      DropDownMenu,
                                      FileSelect,
                                      Entry_Box)
-from simba.enums import Formats, Options
-from simba.unsupervised.visualizers import (GridSearchClusterVisualizer,
-                                            ClusterVisualizer)
-from simba.unsupervised.data_extractors import DataExtractorMultipleModels
-from simba.unsupervised.umap_embedder import (UMAPGridSearch, UMAPTransform)
+from simba.train_model_functions import check_if_dir_exists
+from simba.read_config_unit_tests import check_int
+from simba.unsupervised.grid_search_visualizers import GridSearchVisualizer
+from simba.unsupervised.data_extractor import DataExtractor
+from simba.utils.errors import NoSpecifiedOutputError
+from simba.unsupervised.umap_embedder import UmapEmbedder
 from simba.unsupervised.tsne import TSNEGridSearch
-from simba.unsupervised.hdbscan_clusterer import (HDBSCANClusterer,
-                                                  HDBSCANTransform)
-from simba.unsupervised.dbcv import DBCVCalculator
-from simba.read_config_unit_tests import (check_float,
-                                          check_int,
-                                          check_file_exist_and_readable,
-                                          check_if_dir_exists,
-                                          check_if_filepath_list_is_empty)
-from simba.unsupervised.misc import read_pickle
+from simba.unsupervised.hdbscan_clusterer import HDBSCANClusterer
+from simba.unsupervised.cluster_visualizer import ClusterVisualizer
 from simba.unsupervised.cluster_statistics import (ClusterFrequentistCalculator,
                                                    ClusterXAICalculator,
                                                    EmbeddingCorrelationCalculator)
-from simba.mixins.pop_up_mixin import PopUpMixin
+# from simba.enums import Formats, Options
+# from simba.unsupervised.visualizers import (GridSearchClusterVisualizer,
+#                                             ClusterVisualizer)
+# from simba.unsupervised.data_extractors import DataExtractorMultipleModels
+# from simba.unsupervised.umap_embedder import (UMAPGridSearch, UMAPTransform)
+
+# from simba.unsupervised.hdbscan_clusterer import (HDBSCANClusterer,
+#                                                   HDBSCANTransform)
+# from simba.unsupervised.dbcv import DBCVCalculator
+# from simba.read_config_unit_tests import (check_float,
+#                                           check_int,
+#                                           check_file_exist_and_readable,
+#                                           check_if_dir_exists,
+#                                           check_if_filepath_list_is_empty)
+# from simba.unsupervised.misc import read_pickle
+# from simba.unsupervised.cluster_statistics import (ClusterFrequentistCalculator,
+#                                                    ClusterXAICalculator,
+#                                                    EmbeddingCorrelationCalculator)
+# from simba.mixins.pop_up_mixin import PopUpMixin
 
-
-class GridSearchClusterVisualizerPopUp(PopUpMixin):
+#
+class GridSearchVisualizerPopUp(PopUpMixin):
     def __init__(self,
                  config_path: str):
 
-        super().__init__(config_path=config_path, title='DIMENSIONALITY REDUCTION: GRID SEARCH')
+        super().__init__(config_path=config_path, title='GRID SEARCH VISUALIZER')
 
-        self.graph_cnt_options = list(range(1, 11))
-        self.scatter_sizes_options = list(range(10, 110, 10))
-        self.graph_cnt_options.insert(0, 'None')
-        self.field_types_options = ['START FRAME', 'VIDEO NAMES', 'CLASSIFIER', 'CLASSIFIER PROBABILITY']
-        data_frm = LabelFrame(self.main_frm,text='DATA',font=Formats.LABELFRAME_HEADER_FORMAT.value,padx=5,pady=5,fg='black')
-        self.clusterers_dir_select = FolderSelect(data_frm, "CLUSTERERS DIRECTORY:", lblwidth=25)
-        self.save_dir_select = FolderSelect(data_frm, "IMAGE SAVE DIRECTORY: ", lblwidth=25)
+        data_frm = LabelFrame(self.main_frm, text='DATA', fg='black', font=Formats.LABELFRAME_HEADER_FORMAT.value)
+        self.data_dir_select = FolderSelect(data_frm, "DATA DIRECTORY:", lblwidth=25)
+        self.save_dir_select = FolderSelect(data_frm, "OUTPUT DIRECTORY: ", lblwidth=25)
+        data_frm.grid(row=0, column=0, sticky=NW)
+        self.data_dir_select.grid(row=0, column=0, sticky=NW)
+        self.save_dir_select.grid(row=1, column=0, sticky=NW)
 
+        self.visualization_options = UnsupervisedOptions.CATEGORICAL_OPTIONS.value + UnsupervisedOptions.CONTINUOUS_OPTIONS.value
         settings_frm = LabelFrame(self.main_frm,text='SETTINGS',font=Formats.LABELFRAME_HEADER_FORMAT.value,padx=5,pady=5,fg='black')
-        self.scatter_size_dropdown = DropDownMenu(settings_frm, 'SCATTER SIZE:', self.scatter_sizes_options, '25')
-        self.scatter_size_dropdown.setChoices(50)
+        self.scatter_size_dropdown = DropDownMenu(settings_frm, 'SCATTER SIZE:', UnsupervisedOptions.SCATTER_SIZE.value, '25')
+        self.scatter_size_dropdown.setChoices(5)
         self.categorical_palette_dropdown = DropDownMenu(settings_frm, 'CATEGORICAL PALETTE:', Options.PALETTE_OPTIONS_CATEGORICAL.value, '25')
         self.categorical_palette_dropdown.setChoices('Set1')
         self.continuous_palette_dropdown = DropDownMenu(settings_frm, 'CONTINUOUS PALETTE:', Options.PALETTE_OPTIONS.value, '25')
         self.continuous_palette_dropdown.setChoices('magma')
 
-        run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        run_btn = Button(run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        plot_select_cnt_frm = LabelFrame(self.main_frm, text='SELECT PLOTS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        self.plot_cnt_dropdown = DropDownMenu(plot_select_cnt_frm, '# PLOTS:', self.graph_cnt_options, '25', com= lambda x:self.show_plot_table())
-        self.plot_cnt_dropdown.setChoices(self.graph_cnt_options[0])
-
-        data_frm.grid(row=0, column=0, sticky=NW)
-        self.clusterers_dir_select.grid(row=0, column=0, sticky=NW)
-        self.save_dir_select.grid(row=1, column=0, sticky=NW)
-
         settings_frm.grid(row=1, column=0, sticky=NW)
         self.scatter_size_dropdown.grid(row=0, column=0, sticky=NW)
         self.categorical_palette_dropdown.grid(row=1, column=0, sticky=NW)
         self.continuous_palette_dropdown.grid(row=2, column=0, sticky=NW)
 
-        run_frm.grid(row=2, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
-
-        plot_select_cnt_frm.grid(row=3, column=0, sticky=NW)
+        self.define_plots_frm = LabelFrame(self.main_frm, text='DEFINE PLOTS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
+        self.plot_cnt_dropdown = DropDownMenu(self.define_plots_frm, '# PLOTS:', UnsupervisedOptions.GRAPH_CNT.value, '25', com= lambda x:self.show_plot_table())
+        self.plot_cnt_dropdown.setChoices(UnsupervisedOptions.GRAPH_CNT.value[0])
+        self.show_plot_table()
+        self.define_plots_frm.grid(row=2, column=0, sticky=NW)
         self.plot_cnt_dropdown.grid(row=0, column=0, sticky=NW)
 
-
+        self.create_run_frm(title='RUN', run_function=self.run)
         self.main_frm.mainloop()
 
     def show_plot_table(self):
         if hasattr(self, 'plot_table'):
             self.plot_table.destroy()
 
-        if self.plot_cnt_dropdown.getChoices() != 'NONE':
-            self.plot_rows = {}
-            self.plot_table = LabelFrame(self.main_frm, text='SELECT PLOTS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-            self.plot_table.grid(row=4, column=0, sticky=NW)
-            self.scatter_name_header = Label(self.plot_table, text='PLOT NAME').grid(row=0, column=0)
-            self.field_type_header = Label(self.plot_table, text='FIELD TYPE').grid(row=0, column=1)
-            self.field_name_header = Label(self.plot_table, text='FIELD NAME').grid(row=0, column=2)
-            for idx in range(int(self.plot_cnt_dropdown.getChoices())):
-                row_name = idx
-                self.plot_rows[row_name] = {}
-                self.plot_rows[row_name]['label'] = Label(self.plot_table, text=f'Scatter {str(idx+1)}:')
-                self.plot_rows[row_name]['field_type_dropdown'] = DropDownMenu(self.plot_table, ' ', self.field_types_options, '10', com=lambda k, x=idx: self.change_field_name_state(k, x))
-                self.plot_rows[row_name]['field_type_dropdown'].setChoices(self.field_types_options[0])
-                self.plot_rows[row_name]['field_name_dropdown'] = DropDownMenu(self.plot_table, ' ', self.clf_names, '10', com=None)
-                self.plot_rows[row_name]['field_name_dropdown'].disable()
-                self.plot_rows[idx]['label'].grid(row=idx+1, column=0, sticky=NW)
-                self.plot_rows[idx]['field_type_dropdown'].grid(row=idx+1, column=1, sticky=NW)
-                self.plot_rows[idx]['field_name_dropdown'].grid(row=idx+1, column=2, sticky=NW)
-
-    def change_field_name_state(self, k, x):
-        if (k == 'CLASSIFIER'):
-            self.plot_rows[x]['field_name_dropdown'].enable()
-            self.plot_rows[x]['field_name_dropdown'].setChoices(self.clf_names[0])
-        else:
-            self.plot_rows[x]['field_name_dropdown'].disable()
-            self.plot_rows[x]['field_name_dropdown'].setChoices(None)
+        self.plot_data = {}
+        self.plot_table = LabelFrame(self.define_plots_frm, text='PLOTS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
+        self.scatter_name_header = Label(self.plot_table, text='PLOT NAME').grid(row=0, column=0)
+        self.field_name_header = Label(self.plot_table, text='COLOR VARIABLE').grid(row=0, column=1)
+        for idx in range(int(self.plot_cnt_dropdown.getChoices())):
+            row_name = idx
+            self.plot_data[row_name] = {}
+            self.plot_data[row_name]['label'] = Label(self.plot_table, text=f'Scatter {str(idx+1)}:')
+            self.plot_data[row_name]['variable'] = DropDownMenu(self.plot_table, ' ', self.visualization_options, '10', com=None)
+            self.plot_data[row_name]['variable'].setChoices(self.visualization_options[0])
+            self.plot_data[idx]['label'].grid(row=idx+1, column=0, sticky=NW)
+            self.plot_data[idx]['variable'].grid(row=idx+1, column=1, sticky=NW)
+        self.plot_table.grid(row=1, column=0, sticky=NW)
 
     def run(self):
-        clusterers_path = self.clusterers_dir_select.folder_path
-        save_dir = self.save_dir_select.folder_path
-
+        if len(self.plot_data.keys()) < 1:
+            raise NoSpecifiedOutputError(msg='Specify at least one plot')
+        #check_if_dir_exists(in_dir=self.save_dir_select.folder_path)
+        #check_if_dir_exists(in_dir=self.data_dir_select.folder_path)
         settings = {}
         settings['SCATTER_SIZE'] = int(self.scatter_size_dropdown.getChoices())
         settings['CATEGORICAL_PALETTE'] = self.categorical_palette_dropdown.getChoices()
         settings['CONTINUOUS_PALETTE'] = self.continuous_palette_dropdown.getChoices()
-        hue_dict = None
-        if self.plot_cnt_dropdown.getChoices() != 'NONE':
-            hue_dict = {}
-            for cnt, (k, v) in enumerate(self.plot_rows.items()):
-                hue_dict[cnt] = {}
-                hue_dict[cnt]['FIELD_TYPE'] = v['field_type_dropdown'].getChoices()
-                hue_dict[cnt]['FIELD_NAME'] = v['field_name_dropdown'].getChoices()
-        settings['HUE'] = hue_dict
-        if not os.path.isdir(clusterers_path):
-            print('SIMBA ERROR: Save path is not a valid directory.')
-            raise NotADirectoryError()
-
-        print(settings['HUE'])
-        grid_search_visualizer = GridSearchClusterVisualizer(clusterers_path=clusterers_path,
-                                                             save_dir=save_dir,
-                                                             settings=settings)
-        grid_search_visualizer.create_datasets()
-        grid_search_visualizer.create_imgs()
-
 
-class BatchDataExtractorPopUp(PopUpMixin):
-    def __init__(self):
-        super().__init__(title='VISUALIZATION OF GRID SEARCH')
-        self.hyperparameter_log_var = BooleanVar(value=True)
+        continuous_vars, categorical_vars = [], []
+        for k, v in self.plot_data.items():
+            if v['variable'].getChoices() in UnsupervisedOptions.CONTINUOUS_OPTIONS.value:
+                continuous_vars.append(v['variable'].getChoices())
+            else:
+                categorical_vars.append(v['variable'].getChoices())
+        grid_search_visualizer = GridSearchVisualizer(model_dir=self.data_dir_select.folder_path,
+                                                      save_dir=self.save_dir_select.folder_path,
+                                                      settings=settings)
+        grid_search_visualizer.continuous_visualizer(continuous_vars=continuous_vars)
+        grid_search_visualizer.categorical_visualizer(categoricals=categorical_vars)
 
-        data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        self.embedding_model_select = FolderSelect(data_frm, "EMBEDDING DIRECTORY (PICKLES):", lblwidth=25)
-        self.cluster_model_select = FolderSelect(data_frm, "CLUSTER DIRECTORY (PICKLES):", lblwidth=25)
-        self.save_dir_select = FolderSelect(data_frm, "SAVE DIRECTORY: ", lblwidth=25)
+# _ = GridSearchVisualizerPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
 
 
-        settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        self.features_dropdown = DropDownMenu(settings_frm, 'SCATTER SIZE:', Options.UNSUPERVISED_FEATURE_OPTIONS.value, '25')
-        self.include_log_cb = Checkbutton(settings_frm, text='INCLUDE HYPERPARAMETER LOG', variable=self.hyperparameter_log_var)
+class DataExtractorPopUp(PopUpMixin, ConfigReader):
+    def __init__(self,
+                 config_path: str):
 
-        run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        run_btn = self.create_btn = Button(run_frm, text='RUN', fg='blue', command=lambda: self.run())
+        PopUpMixin.__init__(self, title='DATA EXTRACTOR')
+        ConfigReader.__init__(self, config_path=config_path)
+        data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.data_dir_select = FolderSelect(data_frm, "DATA DIRECTORY:", lblwidth=25)
 
         data_frm.grid(row=0, column=0, sticky=NW)
-        self.embedding_model_select.grid(row=0, column=0, sticky=NW)
-        self.cluster_model_select.grid(row=1, column=0, sticky=NW)
-        self.save_dir_select.grid(row=2, column=0, sticky=NW)
-
-        settings_frm.grid(row=1, column=0, sticky=NW)
-        self.features_dropdown.grid(row=1, column=0, sticky=NW)
-        self.include_log_cb.grid(row=2, column=0, sticky=NW)
+        self.data_dir_select.grid(row=0, column=0, sticky=NW)
 
-        run_frm.grid(row=2, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
+        data_type_frm = LabelFrame(self.main_frm, text='DATA TYPE', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.data_type_dropdown = DropDownMenu(data_type_frm, 'DATA TYPE:', UnsupervisedOptions.DATA_TYPES.value, '25')
+        self.data_type_dropdown.setChoices(UnsupervisedOptions.DATA_TYPES.value[0])
+        data_type_frm.grid(row=1, column=0, sticky=NW)
+        self.data_type_dropdown.grid(row=0, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run, title='RUN')
+        self.main_frm.mainloop()
 
     def run(self):
-        embedding_dir = self.embedding_model_select.folder_path
-        cluster_dir = self.cluster_model_select.folder_path
-        save_dir = self.save_dir_select.folder_path
-        if not os.path.isdir(cluster_dir):
-            cluster_dir = None
-
-        settings = {'include_features': False, 'scaled_features': False, 'parameter_log': False}
-        if self.features_dropdown.getChoices() == Options.UNSUPERVISED_FEATURE_OPTIONS.value[0]:
-            settings['include_features'] = True
-        if self.features_dropdown.getChoices() == Options.UNSUPERVISED_FEATURE_OPTIONS.value[1]:
-            settings['include_features'] = True
-            settings['scaled_features'] = True
-        if self.hyperparameter_log_var.get():
-            settings['parameter_log'] = True
-
-        _ = DataExtractorMultipleModels(embeddings_dir=embedding_dir,
-                                        clusterer_dir=cluster_dir,
-                                        save_dir=save_dir)
+        check_if_dir_exists(self.data_dir_select.folder_path)
+        DataExtractor(config_path=self.config_path,
+                      data_path=self.data_dir_select.folder_path,
+                      data_type=self.data_type_dropdown.getChoices())
+
+#_ = DataExtractorPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+
+
+class FitDimReductionPopUp(PopUpMixin, ConfigReader):
 
-class FitDimReductionPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='FIT DIMENSIONALITY REDUCTION MODELS')
-        self.scaler_options = Options.SCALER_NAMES.value
-        self.dim_reduction_algo_options = ['UMAP',
-                                           'TSNE']
-        self.feature_removal_options = list(range(10, 100, 10))
-        self.feature_removal_options = [str(x) + '%' for x in self.feature_removal_options]
-        self.feature_removal_options.insert(0, 'NONE')
-
-
-        self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.dataset_file_selected = FileSelect(self.dataset_frm, "DATASET (PICKLE): ")
-        self.save_frm = LabelFrame(self.main_frm, text='SAVE', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.dr_save_dir = FolderSelect(self.save_frm, "SAVE DIRECTORY: ")
-        settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.scaling_dropdown = DropDownMenu(settings_frm, 'SCALING:', self.scaler_options, '20')
-        self.scaling_dropdown.setChoices(self.scaler_options[0])
-        self.feature_removal_dropdown = DropDownMenu(settings_frm, 'VARIANCE THRESHOLD:', self.feature_removal_options, '20')
-        self.feature_removal_dropdown.setChoices(self.feature_removal_options[0])
-        self.choose_algo_dropdown = DropDownMenu(settings_frm, 'ALGORITHM:', self.dim_reduction_algo_options, '20', com=lambda x: self.show_dr_algo_hyperparameters())
-        self.choose_algo_dropdown.setChoices(self.dim_reduction_algo_options[0])
-        self.show_dr_algo_hyperparameters()
-
+        self.variance_options = [str(x) + '%' for x in UnsupervisedOptions.VARIANCE_OPTIONS.value]
 
+        self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.dataset_file_selected = FileSelect(self.dataset_frm, "DATASET (PICKLE):", lblwidth=25)
         self.dataset_frm.grid(row=0, column=0, sticky=NW)
         self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
+
+        self.save_frm = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.save_dir = FolderSelect(self.save_frm, "SAVE DIRECTORY:", lblwidth=25)
         self.save_frm.grid(row=1, column=0, sticky=NW)
-        self.dr_save_dir.grid(row=0, column=0, sticky=NW)
-        settings_frm.grid(row=2, column=0, sticky=NW)
-        self.choose_algo_dropdown.grid(row=0, column=0, sticky=NW)
-        self.feature_removal_dropdown.grid(row=1, column=0, sticky=NW)
-        self.scaling_dropdown.grid(row=2, column=0, sticky=NW)
+        self.save_dir.grid(row=0, column=0, sticky=NW)
 
+        settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.scaling_dropdown = DropDownMenu(settings_frm, 'SCALING:', Options.SCALER_NAMES.value, '25')
+        self.scaling_dropdown.setChoices(Options.SCALER_NAMES.value[0])
+        self.var_threshold_dropdown = DropDownMenu(settings_frm, 'VARIANCE THRESHOLD:', self.variance_options, '25')
+        self.var_threshold_dropdown.setChoices(self.variance_options[0])
+        self.algo_dropdown = DropDownMenu(settings_frm, 'ALGORITHM:', UnsupervisedOptions.DR_ALGO_OPTIONS.value, '25', com=lambda x: self.show_dr_hyperparameters())
+        self.algo_dropdown.setChoices(UnsupervisedOptions.DR_ALGO_OPTIONS.value[0])
+        self.show_dr_hyperparameters()
+
+        settings_frm.grid(row=2, column=0, sticky=NW)
+        self.scaling_dropdown.grid(row=0, column=0, sticky=NW)
+        self.var_threshold_dropdown.grid(row=1, column=0, sticky=NW)
+        self.algo_dropdown.grid(row=2, column=0, sticky=NW)
         self.main_frm.mainloop()
 
-    def add_to_listbox(self,
-                       list_box: Listbox,
-                       entry_box: Entry_Box):
-        value = entry_box.entry_get
-        check_float(name='VALUE', value=value)
-        list_box_content = [float(x) for x in list_box.get(0, END)]
-        if float(value) not in list_box_content:
-            list_box.insert(0, value)
-
-    def add_defaults_to_listbox(self,
-                                list_box: Listbox,
-                                value: float):
-        list_box.insert(0, value)
-
-    def remove_from_listbox(self,
-                       list_box: Listbox):
-        selection = list_box.curselection()
-        if selection:
-            list_box.delete(selection[0])
-
-    def show_dr_algo_hyperparameters(self):
-        if hasattr(self, 'dr_hyperparameters_frm'):
-            self.dr_hyperparameters_frm.destroy()
-            self.dr_value_frm.destroy()
+    def show_dr_hyperparameters(self):
+        if hasattr(self, 'hyperparameters_frm'):
+            self.hyperparameters_frm.destroy()
+            self.value_frm.destroy()
             self.run_frm.destroy()
 
-        self.dr_hyperparameters_frm = LabelFrame(self.main_frm, text='GRID SEARCH HYPER-PARAMETERS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.dr_value_frm = LabelFrame(self.main_frm, fg='black')
-        self.dr_value_entry_box = Entry_Box(self.dr_value_frm, 'VALUE: ', '12')
-        self.dr_value_frm.grid(row=3, column=0, sticky=NW)
+        self.hyperparameters_frm = LabelFrame(self.main_frm, text='GRID SEARCH HYPER-PARAMETERS', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.value_frm = LabelFrame(self.main_frm, fg='black')
+        self.dr_value_entry_box = Entry_Box(self.value_frm, 'VALUE: ', '12')
+        self.value_frm.grid(row=3, column=0, sticky=NW)
         self.dr_value_entry_box.grid(row=0, column=1, sticky=NW)
-        self.dr_hyperparameters_frm.grid(row=4, column=0, sticky=NW)
-        if self.choose_algo_dropdown.getChoices() == 'UMAP':
-            n_neighbors_estimators_lbl = Label(self.dr_hyperparameters_frm, text='N NEIGHBOURS')
-            min_distance_lbl = Label(self.dr_hyperparameters_frm, text='MIN DISTANCE')
-            spread_lbl = Label(self.dr_hyperparameters_frm, text='SPREAD')
-            add_min_distance_btn = Button(self.dr_hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox(list_box=self.min_distance_listb, entry_box=self.dr_value_entry_box))
-            add_neighbours_btn = Button(self.dr_hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox(list_box=self.n_neighbors_estimators_listb, entry_box=self.dr_value_entry_box))
-            add_spread_btn = Button(self.dr_hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox(list_box=self.spread_listb, entry_box=self.dr_value_entry_box))
-            remove_min_distance_btn = Button(self.dr_hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.min_distance_listb))
-            remove_neighbours_btn = Button(self.dr_hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.n_neighbors_estimators_listb))
-            remove_spread_btn = Button(self.dr_hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.spread_listb))
-            self.n_neighbors_estimators_listb = Listbox(self.dr_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            self.min_distance_listb = Listbox(self.dr_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            self.spread_listb = Listbox(self.dr_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-
-            self.add_defaults_to_listbox(list_box=self.n_neighbors_estimators_listb, value=15)
-            self.add_defaults_to_listbox(list_box=self.min_distance_listb, value=0.1)
-            self.add_defaults_to_listbox(list_box=self.spread_listb, value=1)
-
-            n_neighbors_estimators_lbl.grid(row=1, column=0)
-            min_distance_lbl.grid(row=1, column=1)
-            spread_lbl.grid(row=1, column=2)
-            add_neighbours_btn.grid(row=2, column=0)
-            add_min_distance_btn.grid(row=2, column=1)
-            add_spread_btn.grid(row=2, column=2)
-            remove_neighbours_btn.grid(row=3, column=0)
-            remove_min_distance_btn.grid(row=3, column=1)
-            remove_spread_btn.grid(row=3, column=2)
-            self.n_neighbors_estimators_listb.grid(row=4, column=0, sticky=NW)
-            self.min_distance_listb.grid(row=4, column=1, sticky=NW)
-            self.spread_listb.grid(row=4, column=2, sticky=NW)
-            self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-            run_btn = Button(self.run_frm, text='RUN', fg='blue', command= lambda: self.run_gridsearch())
-            self.run_frm.grid(row=5, column=0, sticky=NW)
-            run_btn.grid(row=0, column=1, sticky=NW)
-
-        if self.choose_algo_dropdown.getChoices() == 'TSNE':
-            perplexity_lbl = Label(self.dr_hyperparameters_frm, text='PERPLEXITY')
-            add_perplexity_btn = Button(self.dr_hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox(list_box=self.perplexity_listb, entry_box=self.dr_value_entry_box))
-            remove_perplexity_btn = Button(self.dr_hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.perplexity_listb))
-            self.perplexity_listb = Listbox(self.dr_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            perplexity_lbl.grid(row=1, column=0)
-            add_perplexity_btn.grid(row=2, column=0)
-            remove_perplexity_btn.grid(row=3, column=0)
-            self.perplexity_listb.grid(row=4, column=0, sticky=NW)
-            self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-            run_btn = Button(self.run_frm, text='RUN', fg='blue', command= lambda: self.run_gridsearch())
-            self.run_frm.grid(row=5, column=0, sticky=NW)
-            run_btn.grid(row=0, column=1, sticky=NW)
-
-    def run_gridsearch(self):
-        variance = None
-        if self.feature_removal_dropdown.getChoices() != 'NONE':
-            variance = int(self.feature_removal_dropdown.getChoices()[:-1]) / 100
-        save_path = self.dr_save_dir.folder_path
-        data_path = self.dataset_file_selected.file_path
-
-        if self.choose_algo_dropdown.getChoices() == 'UMAP':
-            min_distance = [float(x) for x in self.min_distance_listb.get(0, END)]
-            n_neighbours = [float(x) for x in self.n_neighbors_estimators_listb.get(0, END)]
-            spread = [float(x) for x in self.spread_listb.get(0, END)]
-            if len(min_distance) == 0 or len(n_neighbours) == 0 or len(spread) == 0:
-                print('SIMBA ERROR: Provide values for neighbors, min distances, and spread')
-                raise ValueError('SIMBA ERROR: Provide at least one hyperparameter value for neighbors, min distances, and spread')
-            hyperparameters = {'n_neighbors': n_neighbours,
-                                'min_distance': min_distance,
-                                'spread': spread,
-                                'scaler': self.scaling_dropdown.getChoices(),
-                                'variance': variance}
-            umap_searcher = UMAPGridSearch(data_path=data_path,
-                                           save_dir=save_path)
-
-            umap_searcher.fit(hyper_parameters=hyperparameters)
-
-        if self.choose_algo_dropdown.getChoices() == 'TSNE':
-            perplexity = [int(x) for x in self.perplexity_listb.get(0, END)]
-            if len(perplexity) == 0:
-                print('SIMBA ERROR: Provide value(s) for perplexity')
-                raise ValueError('SIMBA ERROR: Provide value(s) for perplexity')
-
-            hyperparameters = {'perplexity': perplexity,
-                               'scaler': self.scaling_dropdown.getChoices(),
-                               'variance': variance}
-            tsne_searcher = TSNEGridSearch(data_path=data_path,
-                                           save_dir=save_path)
-            tsne_searcher.fit(hyperparameters=hyperparameters)
+        self.hyperparameters_frm.grid(row=4, column=0, sticky=NW)
+
+        if self.algo_dropdown.getChoices() == Unsupervised.UMAP.value:
+            Label(self.hyperparameters_frm, text=Unsupervised.N_NEIGHBORS.value).grid(row=1, column=0)
+            Label(self.hyperparameters_frm, text=Unsupervised.MIN_DISTANCE.value).grid(row=1, column=1)
+            Label(self.hyperparameters_frm, text=Unsupervised.SPREAD.value).grid(row=1, column=2)
+
+            self.n_neighbors_estimators_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            self.min_distance_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            self.spread_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+
+            neighbours_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox_from_entrybox(list_box=self.n_neighbors_estimators_listbox, entry_box=self.dr_value_entry_box))
+            min_distance_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox_from_entrybox(list_box=self.min_distance_listbox, entry_box=self.dr_value_entry_box))
+            spread_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox_from_entrybox(list_box=self.spread_listbox, entry_box=self.dr_value_entry_box))
+
+            neighbours_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.n_neighbors_estimators_listbox))
+            min_distance_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.min_distance_listbox))
+            spread_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.spread_listbox))
+
+            self.add_values_to_several_listboxes(list_boxes=[self.n_neighbors_estimators_listbox, self.min_distance_listbox, self.spread_listbox], values= [15, 0.1, 1])
+
+            neighbours_add_btn.grid(row=2, column=0)
+            min_distance_add_btn.grid(row=2, column=1)
+            spread_add_btn.grid(row=2, column=2)
+            neighbours_remove_btn.grid(row=3, column=0)
+            min_distance_remove_btn.grid(row=3, column=1)
+            spread_remove_btn.grid(row=3, column=2)
+
+            self.n_neighbors_estimators_listbox.grid(row=4, column=0, sticky=NW)
+            self.min_distance_listbox.grid(row=4, column=1, sticky=NW)
+            self.spread_listbox.grid(row=4, column=2, sticky=NW)
+            self.create_run_frm(run_function=self.__run_umap_gridsearch)
+
+        elif self.algo_dropdown.getChoices() == Unsupervised.TSNE.value:
+            Label(self.hyperparameters_frm, text='PERPLEXITY').grid(row=1, column=0)
+            self.perplexity_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            perplexity_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox_from_entrybox(list_box=self.perplexity_listbox, entry_box=self.dr_value_entry_box))
+            perplexity_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.perplexity_listbox))
+            perplexity_add_btn.grid(row=2, column=0)
+            perplexity_remove_btn.grid(row=3, column=0)
+            self.perplexity_listbox.grid(row=4, column=0, sticky=NW)
+            self.create_run_frm(run_function=self.__run_tsne_gridsearch)
+
+    def __run_tsne_gridsearch(self):
+        self.__get_settings()
+        perplexities = [int(x) for x in self.perplexity_listbox.get(0, END)]
+        if len(perplexities) == 0:
+            raise NoSpecifiedOutputError('Provide value(s) for perplexity')
+        hyperparameters = {'perplexity': perplexities,
+                           'scaler': self.scaling_dropdown.getChoices(),
+                           'variance': self.variance_selected}
+        tsne_searcher = TSNEGridSearch(data_path=self.data_path,
+                                       save_dir=self.save_path)
+        #tsne_searcher.fit(hyperparameters=hyperparameters)
+
+    def __run_umap_gridsearch(self):
+        self.__get_settings()
+        n_neighbours = [float(x) for x in self.n_neighbors_estimators_listbox.get(0, END)]
+        min_distances = [float(x) for x in self.min_distance_listbox.get(0, END)]
+        spreads = [float(x) for x in self.spread_listbox.get(0, END)]
+        if len(min_distances) == 0 or len(n_neighbours) == 0 or len(spreads) == 0:
+            raise NoSpecifiedOutputError('Provide at least one hyperparameter value for neighbors, min distances, and spread')
+        hyper_parameters = {'n_neighbors': n_neighbours,
+                           'min_distance': min_distances,
+                           'spread': spreads,
+                           'scaler': self.scaling_dropdown.getChoices(),
+                           'variance': self.variance_selected}
+        umap_searcher = UmapEmbedder()
+        umap_searcher.fit(data_path=self.data_path,
+                          save_dir=self.save_path,
+                          hyper_parameters=hyper_parameters)
+
+    def __get_settings(self):
+        self.variance_selected = int(self.var_threshold_dropdown.getChoices()[:-1]) / 100
+        self.save_path = self.save_dir.folder_path
+        self.data_path = self.dataset_file_selected.file_path
+        self.scaler = self.scaling_dropdown.getChoices()
+        check_if_dir_exists(self.save_path)
+        check_if_dir_exists(self.data_path)
+
 
+# _ = FitDimReductionPopUp()
 
 class TransformDimReductionPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='DIMENSIONALITY REDUCTION: TRANSFORM')
-        self.features_options = ['EXCLUDE', 'INCLUDE: ORIGINAL', 'INCLUDE: SCALED']
-
-        self.dim_reduction_frm = LabelFrame(self.main_frm, text='DIMENSIONALITY REDUCTION: TRANSFORM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.dim_reduction_model = FileSelect(self.dim_reduction_frm, 'MODEL (PICKLE):', lblwidth=25)
-        self.dim_reduction_dataset = FileSelect(self.dim_reduction_frm, 'DATASET (PICKLE):', lblwidth=25)
+        self.dim_reduction_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.model_select = FileSelect(self.dim_reduction_frm, 'MODEL (PICKLE):', lblwidth=25)
+        self.dataset_select = FileSelect(self.dim_reduction_frm, 'DATASET (PICKLE):', lblwidth=25)
         self.save_dir = FolderSelect(self.dim_reduction_frm, "SAVE DIRECTORY: ", lblwidth=25)
-        self.features_dropdown = DropDownMenu(self.dim_reduction_frm, 'FEATURES:', self.features_options, '12')
-
-        run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        run_btn = self.create_btn = Button(run_frm, text='RUN', fg='blue', command=lambda: self.run())
+        self.features_dropdown = DropDownMenu(self.dim_reduction_frm, 'INCLUDE FEATURES:', UnsupervisedOptions.DATA_FORMATS.value, '25')
+        self.features_dropdown.setChoices(UnsupervisedOptions.DATA_FORMATS.value[0])
+        self.save_format_dropdown = DropDownMenu(self.dim_reduction_frm, 'SAVE FORMATS:', UnsupervisedOptions.SAVE_FORMATS.value, '25')
+        self.save_format_dropdown.setChoices(UnsupervisedOptions.SAVE_FORMATS.value[0])
 
         self.dim_reduction_frm.grid(row=0, column=0, sticky=NW)
-        self.dim_reduction_model.grid(row=0, column=0, sticky=NW)
-        self.dim_reduction_dataset.grid(row=1, column=0, sticky=NW)
+        self.model_select.grid(row=0, column=0, sticky=NW)
+        self.dataset_select.grid(row=1, column=0, sticky=NW)
         self.save_dir.grid(row=2, column=0, sticky=NW)
+        self.features_dropdown.grid(row=3, column=0, sticky=NW)
+        self.save_format_dropdown.grid(row=4, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
 
-        run_frm.grid(row=1, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
+        self.main_frm.mainloop()
 
     def run(self):
-        model_path = self.dim_reduction_model.file_path
-        data_path = self.dim_reduction_dataset.file_path
-        save_dir = self.save_dir.folder_path
-        settings = {}
-        settings['features'] = self.features_dropdown.getChoices()
-        settings['save_format'] = 'csv'
+        check_if_dir_exists(in_dir=self.save_dir.folder_path)
+        check_file_exist_and_readable(file_path=self.model_select.file_path)
+        check_file_exist_and_readable(file_path=self.dataset_select.file_path)
+
+        umap_searcher = UmapEmbedder()
+        umap_searcher.transform(data_path=self.dataset_select.file_path,
+                                model=self.model_select.file_path,
+                                save_dir=self.save_dir.folder_path,
+                                settings=None)
 
-        _ = UMAPTransform(model_path=model_path,
-                          data_path=data_path,
-                          save_dir=save_dir,
-                          settings=settings)
+#_ = TransformDimReductionPopUp()
 
 class FitClusterModelsPopUp(PopUpMixin):
     def __init__(self):
-        super().__init__(title='CLUSTERING: GRID SEARCH')
-        self.cluster_algo_options = ['HDBSCAN']
-        self.clustering_frm = LabelFrame(self.main_frm, text='CLUSTERING', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.cluster_dataset_frm = LabelFrame(self.clustering_frm, text='DATASET', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.dimensionality_reduction_data_selected = FolderSelect(self.cluster_dataset_frm, "EMBEDDING DIRECTORY: ")
-        self.clustering_save_dir_frm = LabelFrame(self.clustering_frm, text='SAVE', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.clustering_save_dir_folder = FolderSelect(self.clustering_save_dir_frm, "SAVE DIRECTORY: ")
-        self.choose_cluster_algo_frm = LabelFrame(self.clustering_frm, text='ALGORITHM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.choose_cluster_algo_dropdown = DropDownMenu(self.choose_cluster_algo_frm, 'ALGORITHM:', self.cluster_algo_options, '12', com=lambda x: self.show_cluster_algo_hyperparameters())
-        self.choose_cluster_algo_dropdown.setChoices(self.cluster_algo_options[0])
-        self.show_cluster_algo_hyperparameters()
-
-        self.clustering_frm.grid(row=0, column=0, sticky=NW)
-        self.cluster_dataset_frm.grid(row=0, column=0, sticky=NW)
-        self.dimensionality_reduction_data_selected.grid(row=0, column=0, sticky=NW)
-        self.clustering_save_dir_frm.grid(row=1, column=0, sticky=NW)
-        self.clustering_save_dir_folder.grid(row=0, column=0, sticky=NW)
-        self.choose_cluster_algo_frm.grid(row=2, column=0, sticky=NW)
-        self.choose_cluster_algo_dropdown.grid(row=0, column=0, sticky=NW)
-
-    def show_cluster_algo_hyperparameters(self):
-        if hasattr(self, 'cluster_hyperparameters_frm'):
-            self.cluster_hyperparameters_frm.destroy()
+        super().__init__(title='CLUSTERING FIT: GRID SEARCH')
+        self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.data_dir_selected = FolderSelect(self.dataset_frm, "DATA DIRECTORY: ", lblwidth=25)
+        self.save_frm = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.save_dir = FolderSelect(self.save_frm, "SAVE DIRECTORY: ", lblwidth=25)
+        self.algo_frm = LabelFrame(self.main_frm, text='ALGORITHM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.algo_dropdown = DropDownMenu(self.algo_frm, 'ALGORITHM:', UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value, '25', com=lambda x: self.show_hyperparameters())
+        self.algo_dropdown.setChoices(UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value[0])
+        self.value_frm = LabelFrame(self.main_frm, fg='black')
+        self.value_entry_box = Entry_Box(self.value_frm, 'VALUE:', '25')
+
+        self.dataset_frm.grid(row=0, column=0, sticky=NW)
+        self.data_dir_selected.grid(row=0, column=0, sticky=NW)
+        self.save_frm.grid(row=1, column=0, sticky=NW)
+        self.save_dir.grid(row=0, column=0, sticky=NW)
+        self.algo_frm.grid(row=2, column=0, sticky=NW)
+        self.algo_dropdown.grid(row=0, column=0, sticky=NW)
+        self.value_frm.grid(row=3, column=0, sticky=NW)
+        self.value_entry_box.grid(row=0, column=0, sticky=NW)
+        self.show_hyperparameters()
+        self.main_frm.mainloop()
+
+    def show_hyperparameters(self):
+        if hasattr(self, 'hyperparameters_frm'):
+            self.hyperparameters_frm.destroy()
+            self.value_frm.destroy()
             self.run_frm.destroy()
+#
+        if self.algo_dropdown.getChoices() == Unsupervised.HDBSCAN.value:
+            self.hyperparameters_frm = LabelFrame(self.main_frm, text='GRID SEARCH CLUSTER HYPER-PARAMETERS', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+
+            Label(self.hyperparameters_frm, text=Clustering.ALPHA.value).grid(row=1, column=0)
+            Label(self.hyperparameters_frm, text=Clustering.MIN_CLUSTER_SIZE.value).grid(row=1, column=1)
+            Label(self.hyperparameters_frm, text=Clustering.MIN_SAMPLES.value).grid(row=1, column=2)
+            Label(self.hyperparameters_frm, text=Clustering.EPSILON.value).grid(row=1, column=3)
+
+            self.alpha_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            self.min_cluster_size_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            self.min_samples_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+            self.epsilon_listbox = Listbox(self.hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
+
+            alpha_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox_from_entrybox(list_box=self.alpha_listbox, entry_box=self.value_entry_box))
+            min_cluster_size_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox_from_entrybox(list_box=self.min_cluster_size_listbox, entry_box=self.value_entry_box))
+            min_samples_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox_from_entrybox(list_box=self.min_samples_listbox, entry_box=self.value_entry_box))
+            epsilon_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox_from_entrybox(list_box=self.epsilon_listbox, entry_box=self.value_entry_box))
+
+            alpha_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.alpha_listbox))
+            min_cluster_size_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_cluster_size_listbox))
+            min_samples_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_samples_listbox))
+            epsilon_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.epsilon_listbox))
+
+            self.add_values_to_several_listboxes(list_boxes=[self.alpha_listbox, self.min_cluster_size_listbox, self.min_samples_listbox, self.epsilon_listbox], values= [15, 5, 0, 1])
+
+            self.hyperparameters_frm.grid(row=4, column=0, sticky=NW)
+            alpha_add_btn.grid(row=2, column=0)
+            min_cluster_size_add_btn.grid(row=2, column=1)
+            min_samples_add_btn.grid(row=2, column=2)
+            epsilon_add_btn.grid(row=2, column=3)
+
+            alpha_remove_btn.grid(row=3, column=0)
+            min_cluster_size_remove_btn.grid(row=3, column=1)
+            min_samples_remove_btn.grid(row=3, column=2)
+            epsilon_remove_btn.grid(row=3, column=3)
+
+            self.alpha_listbox.grid(row=4, column=0, sticky=NW)
+            self.min_cluster_size_listbox.grid(row=4, column=1, sticky=NW)
+            self.min_samples_listbox.grid(row=4, column=2, sticky=NW)
+            self.epsilon_listbox.grid(row=4, column=3, sticky=NW)
+
+            self.create_run_frm(run_function=self.run_hdbscan_clustering)
+
+    def __get_settings(self):
+        self.data_path = self.data_dir_selected.folder_path
+        self.save_dir = self.save_dir.folder_path
+        check_if_dir_exists(self.data_path)
+        check_if_dir_exists(self.save_dir)
 
-        if self.choose_cluster_algo_dropdown.getChoices() == 'HDBSCAN':
-            self.cluster_hyperparameters_frm = LabelFrame(self.clustering_frm, text='GRID SEARCH CLUSTER HYPER-PARAMETERS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-            self.cluster_value_frm = LabelFrame(self.clustering_frm, fg='black')
-            self.cluster_value_entry_box = Entry_Box(self.cluster_value_frm, 'VALUE: ', '12')
-
-            alpha_lbl = Label(self.cluster_hyperparameters_frm, text='ALPHA')
-            min_cluster_size_lbl = Label(self.cluster_hyperparameters_frm, text='MIN CLUSTER SIZE')
-            min_samples_lbl = Label(self.cluster_hyperparameters_frm, text='MIN SAMPLES')
-            cluster_selection_epsilon_lbl = Label(self.cluster_hyperparameters_frm, text='EPSILON')
-
-            add_alpha_btn = Button(self.cluster_hyperparameters_frm, text='ADD', fg='blue', command= lambda: self.add_to_listbox(list_box=self.alpha_listb, entry_box=self.cluster_value_entry_box))
-            add_min_cluster_size_btn = Button(self.cluster_hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox(list_box=self.min_cluster_size_listb, entry_box=self.cluster_value_entry_box))
-            add_min_samples_btn = Button(self.cluster_hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox(list_box=self.min_samples_listb, entry_box=self.cluster_value_entry_box))
-            add_epsilon_btn = Button(self.cluster_hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox(list_box=self.epsilon_listb, entry_box=self.cluster_value_entry_box))
-
-            remove_alpha_btn = Button(self.cluster_hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.alpha_listb))
-            remove_min_cluster_size_btn = Button(self.cluster_hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_cluster_size_listb))
-            remove_min_samples_btn = Button(self.cluster_hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_samples_listb))
-            remove_epsilon_btn = Button(self.cluster_hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.epsilon_listb))
-
-            self.alpha_listb = Listbox(self.cluster_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            self.min_cluster_size_listb = Listbox(self.cluster_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            self.min_samples_listb = Listbox(self.cluster_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-            self.epsilon_listb = Listbox(self.cluster_hyperparameters_frm, bg='lightgrey', fg='black', height=5, width=15)
-
-            self.add_defaults_to_listbox(list_box=self.min_cluster_size_listb, value=15)
-            self.add_defaults_to_listbox(list_box=self.min_samples_listb, value=5)
-            self.add_defaults_to_listbox(list_box=self.epsilon_listb, value=0)
-            self.add_defaults_to_listbox(list_box=self.alpha_listb, value=1)
-
-            self.cluster_value_frm.grid(row=3, column=0, sticky=NW)
-            self.cluster_value_entry_box.grid(row=0, column=1, sticky=NW)
-            self.cluster_hyperparameters_frm.grid(row=4, column=0, sticky=NW)
-
-            alpha_lbl.grid(row=1, column=0)
-            min_cluster_size_lbl.grid(row=1, column=1)
-            min_samples_lbl.grid(row=1, column=2)
-            cluster_selection_epsilon_lbl.grid(row=1, column=3)
-
-            add_alpha_btn.grid(row=2, column=0)
-            add_min_cluster_size_btn.grid(row=2, column=1)
-            add_min_samples_btn.grid(row=2, column=2)
-            add_epsilon_btn.grid(row=2, column=3)
-
-            remove_alpha_btn.grid(row=3, column=0)
-            remove_min_cluster_size_btn.grid(row=3, column=1)
-            remove_min_samples_btn.grid(row=3, column=2)
-            remove_epsilon_btn.grid(row=3, column=3)
-
-            self.alpha_listb.grid(row=4, column=0)
-            self.min_cluster_size_listb.grid(row=4, column=1)
-            self.min_samples_listb.grid(row=4, column=2)
-            self.epsilon_listb.grid(row=4, column=3)
-
-            self.run_frm = LabelFrame(self.cluster_hyperparameters_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-            run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run_hdbscan_clustering())
-            self.run_frm.grid(row=5, column=0, sticky=NW)
-            run_btn.grid(row=0, column=1, sticky=NW)
-
-    def add_to_listbox(self,
-                       list_box: Listbox,
-                       entry_box: Entry_Box):
-        value = entry_box.entry_get
-        check_float(name='VALUE', value=value)
-        list_box_content = [float(x) for x in list_box.get(0, END)]
-        if float(value) not in list_box_content:
-            list_box.insert(0, value)
-
-    def add_defaults_to_listbox(self,
-                                list_box: Listbox,
-                                value: float):
-        list_box.insert(0, value)
-
-
-    def remove_from_listbox(self,
-                       list_box: Listbox):
-        selection = list_box.curselection()
-        if selection:
-            list_box.delete(selection[0])
 
     def run_hdbscan_clustering(self):
-        alpha = [float(x) for x in self.alpha_listb.get(0, END)]
-        min_cluster_size = [int(x) for x in self.min_cluster_size_listb.get(0, END)]
-        min_samples = [int(x) for x in self.min_samples_listb.get(0, END)]
-        epsilon = [float(x) for x in self.epsilon_listb.get(0, END)]
-        hyper_parameters = {'alpha': alpha,
-                            'min_cluster_size': min_cluster_size,
+        self.__get_settings()
+        alphas = [float(x) for x in self.alpha_listbox.get(0, END)]
+        min_cluster_sizes = [int(x) for x in self.min_cluster_size_listbox.get(0, END)]
+        min_samples = [int(x) for x in self.min_samples_listbox.get(0, END)]
+        epsilons = [float(x) for x in self.epsilon_listbox.get(0, END)]
+        hyper_parameters = {'alpha': alphas,
+                            'min_cluster_size': min_cluster_sizes,
                             'min_samples': min_samples,
-                            'cluster_selection_epsilon': epsilon}
-        data_path = self.dimensionality_reduction_data_selected.folder_path
-        save_dir = self.clustering_save_dir_folder.folder_path
-        clusterer = HDBSCANClusterer(data_path=data_path, save_dir=save_dir)
-        clusterer.fit(hyper_parameters=hyper_parameters)
-
+                            'cluster_selection_epsilon': epsilons}
+        clusterer = HDBSCANClusterer()
+        clusterer.fit(data_path=self.data_path, save_dir=self.save_dir, hyper_parameters=hyper_parameters)
 
+#_ = FitClusterModelsPopUp()
 
 class TransformClustererPopUp(PopUpMixin):
     def __init__(self):
-        super().__init__(title='CLUSTERER: TRANSFORM')
-        self.features_options = ['EXCLUDE', 'INCLUDE: ORIGINAL', 'INCLUDE: SCALED']
-        self.transform_clusterer_frm = LabelFrame(self.main_frm, text='CLUSTERER: TRANSFORM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.cluster_model_select = FileSelect(self.transform_clusterer_frm, 'CLUSTER MODEL (PICKLE):', lblwidth=25)
-        self.dataset_select = FileSelect(self.transform_clusterer_frm, 'DATASET (PICKLE):',  lblwidth=25)
-        self.save_dir = FolderSelect(self.transform_clusterer_frm, "SAVE DIRECTORY:",  lblwidth=25)
-        self.feature_option_dropdown = DropDownMenu(self.transform_clusterer_frm, 'INCLUDE FEATURES:', self.features_options, '25')
-
-        run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        run_btn = self.create_btn = Button(run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.transform_clusterer_frm.grid(row=0, column=0, sticky=NW)
-        self.cluster_model_select.grid(row=0, column=0, sticky=NW)
-        self.save_dir.grid(row=1, column=0, sticky=NW)
-        self.feature_option_dropdown.grid(row=2, column=0, sticky=NW)
+        super().__init__(title='CLUSTERING: TRANSFORM')
+        self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.model_select = FileSelect(self.settings_frm, 'CLUSTER MODEL (PICKLE):', lblwidth=25)
+        self.data_select = FileSelect(self.settings_frm, 'DATASET (PICKLE):',  lblwidth=25)
+        self.save_dir = FolderSelect(self.settings_frm, "SAVE DIRECTORY:",  lblwidth=25)
+        self.features_dropdown = DropDownMenu(self.settings_frm, 'INCLUDE FEATURES:', UnsupervisedOptions.DATA_FORMATS.value, '25')
+        self.features_dropdown.setChoices(UnsupervisedOptions.DATA_FORMATS.value[0])
+        self.save_format_dropdown = DropDownMenu(self.settings_frm, 'SAVE FORMATS:', UnsupervisedOptions.SAVE_FORMATS.value, '25')
+        self.save_format_dropdown.setChoices(UnsupervisedOptions.SAVE_FORMATS.value[0])
+        self.settings_frm.grid(row=0, column=0, sticky=NW)
+        self.model_select.grid(row=0, column=0, sticky=NW)
+        self.data_select.grid(row=1, column=0, sticky=NW)
+        self.save_dir.grid(row=2, column=0, sticky=NW)
+        self.features_dropdown.grid(row=3, column=0, sticky=NW)
+        self.save_format_dropdown.grid(row=4, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
 
-        run_frm.grid(row=1, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
+        self.main_frm.mainloop()
 
     def run(self):
-        clusterer_path = self.cluster_model_select.file_path
-        data_path = self.dataset_select.file_path
-        save_dir = self.save_dir.folder_path
-        settings = {'features': self.feature_option_dropdown.getChoices()}
-
-        _ = HDBSCANTransform(clusterer_model_path=clusterer_path,
-                             data_path=data_path,
-                             save_dir=save_dir,
-                             settings=settings)
+        check_file_exist_and_readable(self.model_select.file_path)
+        check_file_exist_and_readable(self.data_select.file_path)
+        check_if_dir_exists(self.save_dir.folder_path)
+        settings = {Unsupervised.DATA.value: self.features_dropdown.getChoices(),
+                    Unsupervised.FORMAT.value: self.save_format_dropdown.getChoices()}
+
+        clusterer = HDBSCANClusterer()
+        clusterer.transform(data_path=self.data_select.file_path,
+                            model=self.model_select.file_path,
+                            save_dir=self.save_dir.folder_path,
+                            settings=settings)
+
 
-class ClusterVisualizerPopUp(PopUpMixin):
+#_ = TransformClustererPopUp()
+
+class ClusterVisualizerPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
-        super().__init__(title='CLUSTER EXAMPLE VISUALIZATIONS')
-        self.config_path = config_path
+        PopUpMixin.__init__(self, title='CLUSTER VIDEO VISUALIZATIONS')
+        ConfigReader.__init__(self, config_path=config_path)
         self.include_pose_var = BooleanVar(value=True)
-        self.speed_options = list(np.arange(0.1, 2.1, 0.1))
-        self.speed_options = [round(x, 1) for x in self.speed_options]
 
-        self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.videos_dir_select = FolderSelect(self.data_frm, "VIDEOS DIRECTORY:", lblwidth=25)
         self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ", lblwidth=25)
-        self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.include_pose = Checkbutton(self.settings_frm, text='INCLUDE POSE-ESTIMATION', variable=self.include_pose_var, command=lambda: self.toggle_pose_settings())
+        self.data_frm.grid(row=0, column=0, sticky=NW)
+        self.videos_dir_select.grid(row=0, column=0, sticky=NW)
+
+        self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
+        self.include_pose = Checkbutton(self.settings_frm, text='INCLUDE POSE-ESTIMATION', variable=self.include_pose_var, command=lambda: self.enable_entrybox_from_checkbox(check_box_var=self.include_pose_var,entry_boxes=[self.circle_size_entry]))
         self.circle_size_entry = Entry_Box(self.settings_frm, 'CIRCLE SIZE: ', '25', validation='numeric')
+        self.circle_size_entry.entry_set(val=5)
         self.circle_size_entry.set_state(setstatus='disable')
-        self.speed_dropdown = DropDownMenu(self.settings_frm, 'VIDEO SPEED:', self.speed_options, '25')
 
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.videos_dir_select.grid(row=0, column=0, sticky=NW)
-        self.dataset_file_selected.grid(row=1, column=0, sticky=NW)
+        self.speed_dropdown = DropDownMenu(self.settings_frm, 'VIDEO SPEED:', UnsupervisedOptions.SPEED_OPTIONS.value, '25')
+        self.speed_dropdown.setChoices(1.0)
         self.settings_frm.grid(row=1, column=0, sticky=NW)
         self.include_pose.grid(row=0, column=0, sticky=NW)
         self.circle_size_entry.grid(row=1, column=0, sticky=NW)
         self.speed_dropdown.grid(row=2, column=0, sticky=NW)
-        self.run_frm.grid(row=2, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
 
-    def toggle_pose_settings(self):
-        if self.include_pose_var.get():
-            self.circle_size_entry.set_state(setstatus='normal')
-        else:
-            self.circle_size_entry.set_state(setstatus='disable')
+        self.main_frm.mainloop()
 
     def run(self):
-        circle_size = np.inf
-        include_pose = self.include_pose_var.get()
+        check_file_exist_and_readable(file_path=self.dataset_file_selected.file_path)
+        check_if_dir_exists(in_dir=self.videos_dir_select.folder_path)
         speed = float(self.speed_dropdown.getChoices())
-        data_path = self.dataset_file_selected.file_path
-        check_file_exist_and_readable(file_path=data_path)
-        videos_dir = self.videos_dir_select.folder_path
-
-        if include_pose:
+        if self.include_pose_var.get():
+            check_int(name='CIRCLE SIZE', value=self.circle_size_entry.entry_get)
             circle_size = self.circle_size_entry.entry_get
-            check_int(name='CIRCLE SIZE', value=self.circle_size_entry.entry_get, min_value=1)
-
+        else:
+            circle_size = np.inf
         settings = {'videos_speed': speed,
-                    'pose': {'include': include_pose, 'circle_size': circle_size}}
-
+                    'pose': {'include': self.include_pose_var.get(),
+                             'circle_size': circle_size}}
         cluster_visualizer = ClusterVisualizer(config_path=self.config_path,
                                                settings=settings,
-                                               video_dir=videos_dir,
-                                               data_path=data_path)
-        cluster_visualizer.create()
-
-
-class ClusterFrequentistStatisticsPopUp(PopUpMixin):
+                                               video_dir=self.videos_dir_select.folder_path,
+                                               data_path=self.dataset_file_selected.file_path)
+        cluster_visualizer.run()
+
+#_ = ClusterVisualizerPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+#
+class ClusterFrequentistStatisticsPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
-        super().__init__(title='CLUSTER FREQUENTIST STATISTICS')
-        self.config_path = config_path
-        self.feature_descriptive_stats_var = BooleanVar(value=True)
-        self.feature_oneway_anova_var = BooleanVar(value=True)
-        self.feature_tukey_var = BooleanVar(value=True)
+        PopUpMixin.__init__(self, title='CLUSTER FREQUENTIST STATISTICS')
+        ConfigReader.__init__(self, config_path=config_path)
+        self.descriptive_stats_var = BooleanVar(value=True)
+        self.oneway_anova_var = BooleanVar(value=True)
+        self.tukey_var = BooleanVar(value=True)
         self.use_scaled_var = BooleanVar(value=False)
 
-        self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.dim_reduction_model = FileSelect(self.data_frm, 'CLUSTERER PATH:', lblwidth=25)
-
-        self.d_stats_frm = LabelFrame(self.main_frm, text='CLUSTER STATISTICS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.feature_means_cb = Checkbutton(self.d_stats_frm, text='CLUSTER DESCRIPTIVE STATISTICS', variable=self.feature_descriptive_stats_var)
-        self.feature_anova_cb = Checkbutton(self.d_stats_frm, text='CLUSTER FEATURE ONE-WAY ANOVA', variable=self.feature_oneway_anova_var)
-        self.feature_tukey_posthoc_cb = Checkbutton(self.d_stats_frm, text='CLUSTER FEATURE POST-HOC (TUKEY)', variable=self.feature_tukey_var)
-        self.use_scaled_cb = Checkbutton(self.d_stats_frm, text='USE SCALED FEATURE VALUES', variable=self.use_scaled_var)
-
-
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
+        self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.model_select = FileSelect(self.data_frm, 'CLUSTERER PATH:', lblwidth=25)
         self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.dim_reduction_model.grid(row=0, column=0, sticky=NW)
+        self.model_select.grid(row=0, column=0, sticky=NW)
 
-        self.d_stats_frm.grid(row=1, column=0, sticky=NW)
-        self.feature_means_cb.grid(row=0, column=0, sticky=NW)
-        self.feature_anova_cb.grid(row=1, column=0, sticky=NW)
+        self.stats_frm = LabelFrame(self.main_frm, text='STATISTICS', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.descriptive_stats_cb = Checkbutton(self.stats_frm, text='CLUSTER DESCRIPTIVE STATISTICS', variable=self.descriptive_stats_var)
+        self.oneway_anova_cb = Checkbutton(self.stats_frm, text='CLUSTER FEATURE ONE-WAY ANOVA', variable=self.oneway_anova_var)
+        self.feature_tukey_posthoc_cb = Checkbutton(self.stats_frm, text='CLUSTER FEATURE POST-HOC (TUKEY)', variable=self.tukey_var)
+        self.use_scaled_cb = Checkbutton(self.stats_frm, text='USE SCALED FEATURE VALUES', variable=self.use_scaled_var)
+
+        self.stats_frm.grid(row=1, column=0, sticky=NW)
+        self.descriptive_stats_cb.grid(row=0, column=0, sticky=NW)
+        self.oneway_anova_cb.grid(row=1, column=0, sticky=NW)
         self.feature_tukey_posthoc_cb.grid(row=2, column=0, sticky=NW)
         self.use_scaled_cb.grid(row=3, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
+
+        self.main_frm.mainloop()
 
-        self.run_frm.grid(row=2, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
 
     def run(self):
+        check_file_exist_and_readable(self.model_select.file_path)
         settings = {'scaled': self.use_scaled_var.get(),
-                    'anova': self.feature_oneway_anova_var.get(),
-                    'tukey_posthoc': self.feature_oneway_anova_var.get(),
-                    'descriptive_statistics': self.feature_descriptive_stats_var.get()}
-        model_path = self.dim_reduction_model.file_path
-        check_file_exist_and_readable(model_path)
-
-        descriptive_calculator = ClusterFrequentistCalculator(config_path=self.config_path,
-                                                              data_path=model_path,
-                                                              settings=settings)
+                    'anova': self.oneway_anova_var.get(),
+                    'tukey_posthoc': self.tukey_var.get(),
+                    'descriptive_statistics': self.descriptive_stats_var.get()}
+
+        calculator = ClusterFrequentistCalculator(config_path=self.config_path,
+                                                  data_path=self.model_select.file_path,
+                                                  settings=settings)
+        calculator.run()
 
-        descriptive_calculator.run()
+#_ = ClusterFrequentistStatisticsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
 
-
-class ClusterMLStatisticsPopUp(PopUpMixin):
+class ClusterXAIPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
         super().__init__(title='CLUSTER XAI STATISTICS')
-        self.config_path = config_path
+        ConfigReader.__init__(self, config_path=config_path)
         self.gini_importance_var = BooleanVar(value=True)
         self.permutation_importance_var = BooleanVar(value=True)
         self.shap_var = BooleanVar(value=False)
-        self.shap_method_options = ['Paired clusters']
-        self.shap_sample_options = list(range(100, 1100, 100))
 
-        self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.clusterer_data = FileSelect(self.data_frm, 'CLUSTERER PATH:', lblwidth=25)
+        self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.model_select = FileSelect(self.data_frm, 'MODEL PATH:', lblwidth=25)
+        self.data_frm.grid(row=0, column=0, sticky=NW)
+        self.model_select.grid(row=0, column=0, sticky=NW)
 
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.rf_gini_importance_cb = Checkbutton(self.settings_frm, text='CLUSTER RF GINI IMPORTANCE', variable=self.gini_importance_var)
-        self.rf_permutation_cb = Checkbutton(self.settings_frm, text='CLUSTER RF PERMUTATION IMPORTANCE', variable=self.permutation_importance_var)
-        self.cluster_shap_cb = Checkbutton(self.settings_frm, text='CLUSTER RF SHAPLEY VALUES', variable=self.shap_var, command=self.activate_shap_menu)
-        self.shap_method_dropdown = DropDownMenu(self.settings_frm, 'SHAP METHOD:', self.shap_method_options, '25')
-        self.shap_method_dropdown.setChoices(self.shap_method_options[0])
-        self.shap_sample_dropdown = DropDownMenu(self.settings_frm, 'SHAP SAMPLES:', self.shap_sample_options, '25')
-        self.shap_sample_dropdown.setChoices(self.shap_sample_options[0])
+        self.gini_importance_cb = Checkbutton(self.settings_frm, text='CLUSTER RF GINI IMPORTANCE', variable=self.gini_importance_var)
+        self.permutation_cb = Checkbutton(self.settings_frm, text='CLUSTER RF PERMUTATION IMPORTANCE', variable=self.permutation_importance_var)
+        self.shap_method_dropdown = DropDownMenu(self.settings_frm, 'SHAP METHOD:', UnsupervisedOptions.SHAP_CLUSTER_METHODS.value, '25')
+        self.shap_method_dropdown.setChoices(UnsupervisedOptions.SHAP_CLUSTER_METHODS.value[0])
+        self.shap_sample_dropdown = DropDownMenu(self.settings_frm, 'SHAP SAMPLES:', UnsupervisedOptions.SHAP_SAMPLE_OPTIONS.value, '25')
+        self.shap_sample_dropdown.setChoices(100)
         self.shap_method_dropdown.disable()
         self.shap_sample_dropdown.disable()
-
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.clusterer_data.grid(row=0, column=0, sticky=NW)
+        self.shap_cb = Checkbutton(self.settings_frm, text='CLUSTER RF SHAP VALUES', variable=self.shap_var, command= lambda:self.enable_dropdown_from_checkbox(check_box_var=self.shap_var, dropdown_menus=[self.shap_method_dropdown, self.shap_sample_dropdown]))
 
         self.settings_frm.grid(row=1, column=0, sticky=NW)
-        self.rf_gini_importance_cb.grid(row=0, column=0, sticky=NW)
-        self.rf_permutation_cb.grid(row=1, column=0, sticky=NW)
-        self.cluster_shap_cb.grid(row=2, column=0, sticky=NW)
+        self.gini_importance_cb.grid(row=0, column=0, sticky=NW)
+        self.permutation_cb.grid(row=1, column=0, sticky=NW)
+        self.shap_cb.grid(row=2, column=0, sticky=NW)
         self.shap_method_dropdown.grid(row=3, column=0, sticky=NW)
         self.shap_sample_dropdown.grid(row=4, column=0, sticky=NW)
-        self.run_frm.grid(row=5, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
 
-    def activate_shap_menu(self):
-        if self.shap_var.get():
-            self.shap_method_dropdown.enable()
-            self.shap_sample_dropdown.enable()
-        else:
-            self.shap_method_dropdown.disable()
-            self.shap_sample_dropdown.disable()
+        self.main_frm.mainloop()
 
     def run(self):
-        clusterer_path = self.clusterer_data.file_path
-        check_file_exist_and_readable(file_path=clusterer_path)
-        gini_importance = self.gini_importance_var.get()
-        permutation_importance = self.permutation_importance_var.get()
-        shap = self.shap_var.get()
-        shap_method = self.shap_method_dropdown.getChoices()
-        shap_sample = self.shap_sample_dropdown.getChoices()
-
-
-        settings = {'gini_importance': gini_importance, 'permutation_importance': permutation_importance,
-                    'shap': {'method': shap_method, 'run': shap, 'sample': shap_sample}}
-
-        xai_calculator = ClusterXAICalculator(data_path=clusterer_path,
+        check_file_exist_and_readable(file_path=self.model_select.file_path)
+        settings = {'gini_importance': self.gini_importance_var.get(), 'permutation_importance': self.permutation_importance_var.get(),
+                    'shap': {'method': self.shap_method_dropdown.getChoices(), 'run': self.shap_var.get(), 'sample': self.shap_sample_dropdown.getChoices()}}
+        xai_calculator = ClusterXAICalculator(data_path=self.model_select.file_path,
                                               settings=settings,
                                               config_path=self.config_path)
         xai_calculator.run()
 
 
-class EmbedderCorrelationsPopUp(PopUpMixin):
+#_ = ClusterXAIPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+
+class EmbedderCorrelationsPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
-        super().__init__(title='EMBEDDING CORRELATIONS')
-        self.config_path = config_path
-        self.config_path = config_path
-        self.correlation_options = ['SPEARMAN', 'PEARSONS', 'KENDALL']
-
+        PopUpMixin.__init__(self, title='EMBEDDING CORRELATIONS')
+        ConfigReader.__init__(self, config_path=config_path)
         self.spearman_var = BooleanVar(value=True)
         self.pearsons_var = BooleanVar(value=True)
         self.kendall_var = BooleanVar(value=True)
         self.plots_var = BooleanVar(value=False)
 
         self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ")
+        self.data_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE):")
+        self.data_frm.grid(row=0, column=0, sticky=NW)
+        self.data_file_selected.grid(row=0, column=0, sticky=NW)
 
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.spearman_cb = Checkbutton(self.settings_frm, text='SPEARMAN', variable=self.spearman_var)
         self.pearsons_cb = Checkbutton(self.settings_frm, text='PEARSONS', variable=self.pearsons_var)
         self.kendall_cb = Checkbutton(self.settings_frm, text='KENDALL', variable=self.kendall_var)
-        self.plots_cb = Checkbutton(self.settings_frm, text='PLOTS', variable=self.plots_var, command=lambda: self.activate_plots())
-        self.plot_correlation_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', self.correlation_options, '25')
+        self.plot_correlation_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', UnsupervisedOptions.CORRELATION_OPTIONS.value, '25')
         self.plot_correlation_clr_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', Options.PALETTE_OPTIONS.value, '25')
-        self.plot_correlation_dropdown.setChoices(self.correlation_options[0])
+        self.plot_correlation_dropdown.setChoices(UnsupervisedOptions.CORRELATION_OPTIONS.value[0])
         self.plot_correlation_dropdown.disable()
         self.plot_correlation_clr_dropdown.setChoices(Options.PALETTE_OPTIONS.value[0])
         self.plot_correlation_clr_dropdown.disable()
+        self.plots_cb = Checkbutton(self.settings_frm, text='PLOTS', variable=self.plots_var, command=lambda: self.enable_dropdown_from_checkbox(check_box_var=self.plots_var, dropdown_menus=[self.plot_correlation_dropdown, self.plot_correlation_clr_dropdown]))
 
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
         self.settings_frm.grid(row=1, column=0, sticky=NW)
         self.spearman_cb.grid(row=0, column=0, sticky=NW)
         self.pearsons_cb.grid(row=1, column=0, sticky=NW)
         self.kendall_cb.grid(row=2, column=0, sticky=NW)
         self.plots_cb.grid(row=3, column=0, sticky=NW)
         self.plot_correlation_dropdown.grid(row=4, column=0, sticky=NW)
         self.plot_correlation_clr_dropdown.grid(row=5, column=0, sticky=NW)
-        self.run_frm.grid(row=2, column=0, sticky=NW)
-        run_btn.grid(row=0, column=0, sticky=NW)
 
+        self.create_run_frm(run_function=self.run)
+        self.main_frm.mainloop()
 
-    def activate_plots(self):
-        if self.plots_var.get():
-            self.plot_correlation_dropdown.enable()
-            self.plot_correlation_clr_dropdown.enable()
-        else:
-            self.plot_correlation_dropdown.disable()
-            self.plot_correlation_clr_dropdown.disable()
 
     def run(self):
+        check_file_exist_and_readable(self.data_file_selected.file_path)
         settings = {'correlations': [], 'plots': {'create': False, 'correlations': None, 'palette': None}}
         if self.spearman_var.get(): settings['correlations'].append('spearman')
         if self.pearsons_var.get(): settings['correlations'].append('pearson')
         if self.kendall_var.get(): settings['correlations'].append('kendall')
 
-        if self.plots_var.get():
-            settings['plots']['create'] = True
-            settings['plots']['correlations'] = self.plot_correlation_dropdown.getChoices()
-            settings['plots']['palette'] = self.plot_correlation_clr_dropdown.getChoices()
-
-        data_path = self.dataset_file_selected.file_path
-
-        _ = EmbeddingCorrelationCalculator(config_path=self.config_path,
-                                           data_path=data_path,
-                                           settings=settings)
-
-
-class PrintEmBeddingInfoPopUp(PopUpMixin):
-    def __init__(self,
-                 config_path: str):
-        super().__init__(title='PRINT EMBEDDING MODEL INFO')
-        self.config_path = config_path
-        self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ")
-
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
-        self.run_frm.grid(row=1, column=0, sticky=NW)
-        run_btn.grid(row=1, column=0, sticky=NW)
-
-    def run(self):
-        check_file_exist_and_readable(file_path=self.dataset_file_selected.file_path)
-        data = read_pickle(data_path=self.dataset_file_selected.file_path)
-        parameters = {**data['PARAMETERS'], **data['EMBEDDER']['PARAMETERS']}
-        print(parameters)
-
-class DBCVPopUp(PopUpMixin):
-    def __init__(self,
-                 config_path: str):
-        super().__init__(title='DENSITY BASED CLUSTER VALIDATION')
-        self.config_path = config_path
-
-        self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.folder_selected = FolderSelect(self.data_frm, "DATASET (FOLDER WITH PICKLES): ")
-
-        self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-
-        self.data_frm.grid(row=0, column=0, sticky=NW)
-        self.folder_selected.grid(row=0, column=0, sticky=NW)
-        self.run_frm.grid(row=1, column=0, sticky=NW)
-        run_btn.grid(row=1, column=0, sticky=NW)
-
-    def run(self):
-        check_if_dir_exists(in_dir=self.folder_selected.folder_path)
-        data_paths = glob.glob(self.folder_selected.folder_path + '/*.pickle')
-        check_if_filepath_list_is_empty(filepaths=data_paths, error_msg=f'No pickle files in {self.folder_selected.folder_path}')
-        dbcv_calculator = DBCVCalculator(clusterers_path=self.folder_selected.folder_path, config_path=self.config_path)
-        dbcv_calculator.run()
+        calculator = EmbeddingCorrelationCalculator(config_path=self.config_path,
+                                                   data_path=self.data_file_selected.file_path,
+                                                   settings=settings)
+        calculator.run()
+
+#_ = EmbedderCorrelationsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+
+
+#
+#
+# class PrintEmBeddingInfoPopUp(PopUpMixin):
+#     def __init__(self,
+#                  config_path: str):
+#         super().__init__(title='PRINT EMBEDDING MODEL INFO')
+#         self.config_path = config_path
+#         self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+#         self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ")
+#
+#         self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+#         run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
+#
+#         self.data_frm.grid(row=0, column=0, sticky=NW)
+#         self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
+#         self.run_frm.grid(row=1, column=0, sticky=NW)
+#         run_btn.grid(row=1, column=0, sticky=NW)
+#
+#     def run(self):
+#         check_file_exist_and_readable(file_path=self.dataset_file_selected.file_path)
+#         data = read_pickle(data_path=self.dataset_file_selected.file_path)
+#         parameters = {**data['PARAMETERS'], **data['EMBEDDER']['PARAMETERS']}
+#         print(parameters)
+#
+# class DBCVPopUp(PopUpMixin):
+#     def __init__(self,
+#                  config_path: str):
+#         super().__init__(title='DENSITY BASED CLUSTER VALIDATION')
+#         self.config_path = config_path
+#
+#         self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+#         self.folder_selected = FolderSelect(self.data_frm, "DATASET (FOLDER WITH PICKLES): ")
+#
+#         self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+#         run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
+#
+#         self.data_frm.grid(row=0, column=0, sticky=NW)
+#         self.folder_selected.grid(row=0, column=0, sticky=NW)
+#         self.run_frm.grid(row=1, column=0, sticky=NW)
+#         run_btn.grid(row=1, column=0, sticky=NW)
+#
+#     def run(self):
+#         check_if_dir_exists(in_dir=self.folder_selected.folder_path)
+#         data_paths = glob.glob(self.folder_selected.folder_path + '/*.pickle')
+#         check_if_filepath_list_is_empty(filepaths=data_paths, error_msg=f'No pickle files in {self.folder_selected.folder_path}')
+#         dbcv_calculator = DBCVCalculator(clusterers_path=self.folder_selected.folder_path, config_path=self.config_path)
+#         dbcv_calculator.run()
 
 
 
 
 
 #_ = PrintEmBeddingInfoPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,19 +271,19 @@
                 results_cluster_two = mean_df_cluster_two.join(stdev_df_cluster_two).sort_values(by='MEAN', ascending=False)
                 self.__save_results(df=results_cluster_one, name=f'SHAP CLUSTER {str(cluster_one_id)} vs. {str(cluster_two_id)}')
                 self.__save_results(df=results_cluster_two, name=f'SHAP CLUSTER {str(cluster_two_id)} vs. {str(cluster_one_id)}')
             timer.stop_timer()
             stdout_success(msg=f"Paired clusters SHAP values complete", elapsed_time=timer.elapsed_time_str)
 
 
-settings = {'gini_importance': True, 'permutation_importance': True, 'shap': {'method': 'cluster_paired', 'create': True, 'sample': 100}}
-test = ClusterXAICalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
-                            data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
-                            settings=settings)
-test.run()
+# settings = {'gini_importance': True, 'permutation_importance': True, 'shap': {'method': 'cluster_paired', 'create': True, 'sample': 100}}
+# test = ClusterXAICalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
+#                             data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
+#                             settings=settings)
+# test.run()
 
 
 
 
 # settings = {'correlation_methods': ['pearson', 'kendall', 'spearman'], 'plots': {'create': True, 'correlations': 'pearson', 'palette': 'jet'}}
 # test = EmbeddingCorrelationCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/quizzical_rhodes.pickle',
 #                                    config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_file_exist_and_readable)
 from simba.misc_tools import SimbaTimer
-from simba.unsupervised.misc import (check_directory_exists,
-                                     check_that_directory_is_empty)
+from simba.train_model_functions import check_if_dir_exists
 from simba.unsupervised.enums import Clustering, Unsupervised
 import itertools
 import os, glob
 import random
 import pandas as pd
 from simba.utils.printing import stdout_success
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
-from simba.unsupervised.umap_embedder_2 import UmapEmbedder
+from simba.unsupervised.umap_embedder import UmapEmbedder
 try:
     from cuml.cluster.hdbscan import HDBSCAN
     from cuml.cluster import hdbscan
     gpu_flag = True
 except ModuleNotFoundError:
     from hdbscan import HDBSCAN
     import hdbscan
 
 
 class HDBSCANClusterer(UnsupervisedMixin):
-    def __init__(self,
-                 data_path: str,
-                 save_dir: str):
-
+    def __init__(self):
         super().__init__()
+
+    def fit(self,
+            data_path: str,
+            save_dir: str,
+            hyper_parameters: dict):
+
         self.save_dir, self.data_path = save_dir, data_path
-        check_directory_exists(directory=save_dir)
+        self.check_that_directory_is_empty(directory=self.save_dir)
         if os.path.isdir(data_path):
-            check_directory_exists(directory=data_path)
+            check_if_dir_exists(in_dir=data_path)
             self.data_path = glob.glob(data_path + '/*.pickle')
             check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
+        else:
+            check_file_exist_and_readable(file_path=data_path)
+            self.data_path = data_path
 
-    def fit(self,
-            hyper_parameters: dict):
-
-        check_that_directory_is_empty(directory=self.save_dir)
         self.search_space = list(itertools.product(*[hyper_parameters[Clustering.ALPHA.value],
                                                      hyper_parameters[Clustering.MIN_CLUSTER_SIZE.value],
                                                      hyper_parameters[Clustering.MIN_SAMPLES.value],
                                                      hyper_parameters[Clustering.EPSILON.value]]))
         self.embeddings = self.read_pickle(data_path=self.data_path)
         print(f'Fitting {str(len(self.search_space) * len(self.embeddings.keys()))} HDBSCAN model(s)...')
         self.__fit_hdbscan()
@@ -117,18 +118,18 @@
 # embedding_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
 # save_dir = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models'
 # config_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini'
 # clusterer = HDBSCANClusterer(data_path=embedding_dir, save_dir=save_dir)
 # clusterer.fit(hyper_parameters=hyper_parameters)
 
 
-data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
-save_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
-clusterer = HDBSCANClusterer(data_path=data_path, save_dir=save_path)
-clusterer.transform(model='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle', settings={'DATA': None}, data_path=data_path)
+# data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230416145821.pickle'
+# save_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
+# clusterer = HDBSCANClusterer(data_path=data_path, save_dir=save_path)
+# clusterer.transform(model='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/awesome_curran.pickle', settings={'DATA': None}, data_path=data_path)
 
 #settings = {'feature_values': True, 'scaled_features': True, 'save_format': 'csv'}
 # clusterer_model_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models/amazing_burnell.pickle'
 # data_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/logs/unsupervised_data_20230215093552.pickle'
 # save_path = '/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models'
 
 # _ = HDBSCANTransform(clusterer_model_path=clusterer_model_path,
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/tsne.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 from datetime import datetime
 import os
 from simba.enums import Paths
 import pandas as pd
 from simba.misc_tools import (check_file_exist_and_readable,
                               SimbaTimer)
-from simba.unsupervised.misc import (check_that_directory_is_empty,
-                                     check_directory_exists,
-                                     read_pickle,
-                                     write_pickle,
-                                     define_scaler,
-                                     drop_low_variance_fields,
-                                     find_low_variance_fields,
-                                     scaler_transform)
+# from simba.unsupervised.misc import (check_that_directory_is_empty,
+#                                      check_directory_exists,
+#                                      read_pickle,
+#                                      write_pickle,
+#                                      define_scaler,
+#                                      drop_low_variance_fields,
+#                                      find_low_variance_fields,
+#                                      scaler_transform)
 from sklearn.manifold import TSNE
 import random
 import simba
 
 class TSNEGridSearch(object):
     def __init__(self,
                  data_path: str,
                  save_dir: str
                  ):
+        pass
 
-        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
-        self.data_path = data_path
-        self.save_dir = save_dir
-        check_file_exist_and_readable(file_path=self.data_path)
-        check_directory_exists(directory=self.save_dir)
-        check_that_directory_is_empty(directory=self.save_dir)
-        model_names_dir = os.path.join(os.path.dirname(simba.__file__), Paths.UNSUPERVISED_MODEL_NAMES.value)
-        self.model_names = list(pd.read_parquet(model_names_dir)['NAMES'])
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
-
-    def fit(self,
-            hyperparameters: dict):
-        self.hyp, self.low_var_cols = hyperparameters, []
-        self.data = read_pickle(data_path=self.data_path)
-        self.original_feature_names = self.data['DATA'].columns
-        if self.hyp['variance']:
-            self.low_var_cols = find_low_variance_fields(data=self.data['DATA'], variance=self.hyp['variance'])
-            self.data['DATA'] = drop_low_variance_fields(data=self.data['DATA'], fields=self.low_var_cols)
-        self.out_feature_names = [x for x in self.original_feature_names if x not in self.low_var_cols]
-        self.scaler = define_scaler(scaler_name=self.hyp['scaler'])
-        self.scaler.fit(self.data['DATA'])
-        self.scaled_data = scaler_transform(data=self.data['DATA'],scaler=self.scaler)
-        self.__fit_tsne()
-
-    def __fit_tsne(self):
-        self.model_timer = SimbaTimer()
-        self.model_timer.start_timer()
-        self.results = {}
-        self.results['SCALER'] = self.scaler
-        self.results['LOW_VARIANCE_FIELDS'] = self.low_var_cols
-        self.results['ORIGINAL_FEATURE_NAMES'] = self.original_feature_names
-        self.results['OUT_FEATURE_NAMES'] = self.out_feature_names
-        self.results['VIDEO NAMES'] = self.data['VIDEO_NAMES']
-        self.results['START FRAME'] = self.data['START_FRAME']
-        self.results['END FRAME'] = self.data['END_FRAME']
-        self.results['POSE'] = self.data['POSE']
-        self.results['DATA'] = self.scaler
-        self.results['CLASSIFIER'] = self.data['CLF']
-        self.results['CLASSIFIER PROBABILITY'] = self.data['CLF_PROBABILITY']
-
-        for h_cnt, perplexity in enumerate(self.hyp['perplexity']):
-            self.h_cnt = h_cnt
-            self.parameters = {'perplexity': perplexity}
-            embedder = TSNE(n_components=2, perplexity=perplexity)
-            embedder.fit(self.scaled_data.values)
-            self.results['MODEL'] = embedder
-            self.results['HASH'] = random.sample(self.model_names, 1)[0]
-            self.results['TYPE'] = 'TSNE'
-            write_pickle(data=self.results, save_path=os.path.join(self.save_dir, '{}.pickle'.format(self.results['HASH'])))
-        self.timer.stop_timer()
-        print('SIMBA COMPLETE: {} TSNE model(s) saved in {} (elapsed time: {}s)'.format(str(len(self.hyp['perplexity'])), self.save_dir, self.timer.elapsed_time_str))
+    #     self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
+    #     self.data_path = data_path
+    #     self.save_dir = save_dir
+    #     check_file_exist_and_readable(file_path=self.data_path)
+    #     check_directory_exists(directory=self.save_dir)
+    #     check_that_directory_is_empty(directory=self.save_dir)
+    #     model_names_dir = os.path.join(os.path.dirname(simba.__file__), Paths.UNSUPERVISED_MODEL_NAMES.value)
+    #     self.model_names = list(pd.read_parquet(model_names_dir)['NAMES'])
+    #     self.timer = SimbaTimer()
+    #     self.timer.start_timer()
+    #
+    # def fit(self,
+    #         hyperparameters: dict):
+    #     self.hyp, self.low_var_cols = hyperparameters, []
+    #     self.data = read_pickle(data_path=self.data_path)
+    #     self.original_feature_names = self.data['DATA'].columns
+    #     if self.hyp['variance']:
+    #         self.low_var_cols = find_low_variance_fields(data=self.data['DATA'], variance=self.hyp['variance'])
+    #         self.data['DATA'] = drop_low_variance_fields(data=self.data['DATA'], fields=self.low_var_cols)
+    #     self.out_feature_names = [x for x in self.original_feature_names if x not in self.low_var_cols]
+    #     self.scaler = define_scaler(scaler_name=self.hyp['scaler'])
+    #     self.scaler.fit(self.data['DATA'])
+    #     self.scaled_data = scaler_transform(data=self.data['DATA'],scaler=self.scaler)
+    #     self.__fit_tsne()
+    #
+    # def __fit_tsne(self):
+    #     self.model_timer = SimbaTimer()
+    #     self.model_timer.start_timer()
+    #     self.results = {}
+    #     self.results['SCALER'] = self.scaler
+    #     self.results['LOW_VARIANCE_FIELDS'] = self.low_var_cols
+    #     self.results['ORIGINAL_FEATURE_NAMES'] = self.original_feature_names
+    #     self.results['OUT_FEATURE_NAMES'] = self.out_feature_names
+    #     self.results['VIDEO NAMES'] = self.data['VIDEO_NAMES']
+    #     self.results['START FRAME'] = self.data['START_FRAME']
+    #     self.results['END FRAME'] = self.data['END_FRAME']
+    #     self.results['POSE'] = self.data['POSE']
+    #     self.results['DATA'] = self.scaler
+    #     self.results['CLASSIFIER'] = self.data['CLF']
+    #     self.results['CLASSIFIER PROBABILITY'] = self.data['CLF_PROBABILITY']
+    #
+    #     for h_cnt, perplexity in enumerate(self.hyp['perplexity']):
+    #         self.h_cnt = h_cnt
+    #         self.parameters = {'perplexity': perplexity}
+    #         embedder = TSNE(n_components=2, perplexity=perplexity)
+    #         embedder.fit(self.scaled_data.values)
+    #         self.results['MODEL'] = embedder
+    #         self.results['HASH'] = random.sample(self.model_names, 1)[0]
+    #         self.results['TYPE'] = 'TSNE'
+    #         write_pickle(data=self.results, save_path=os.path.join(self.save_dir, '{}.pickle'.format(self.results['HASH'])))
+    #     self.timer.stop_timer()
+    #     print('SIMBA COMPLETE: {} TSNE model(s) saved in {} (elapsed time: {}s)'.format(str(len(self.hyp['perplexity'])), self.save_dir, self.timer.elapsed_time_str))
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/enums.py` & `Simba-UW-tf-dev-1.56.9/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 7800 0000 0800  ....Bud1..x.....
 00000010: 0000 7800 0000 100c 0000 700b 0000 200c  ..x.......p... .
 00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 007a  ...............z
+00000040: 0000 0000 0000 0003 0000 0001 0000 007b  ...............{
 00000050: 0000 0007 0000 1000 0074 0063 0068 005f  .........t.c.h._
 00000060: 0070 0072 0000 0000 0000 0000 0000 0000  .p.r............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,221 +250,221 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 000f 0000 000c  ................
+00001000: 0000 0000 0000 0000 0000 0010 0000 000c  ................
 00001010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-00001020: 0069 0073 0065 0064 6c73 7643 626c 6f62  .i.s.e.dlsvCblob
-00001030: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
-00001040: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
-00001050: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00001060: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00001070: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00001080: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00001090: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-000010a0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000010b0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000010c0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
-000010d0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
-000010e0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
-000010f0: 5a69 6465 6e74 6966 6965 7209 0911 018f  Zidentifier.....
-00001100: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
-00001110: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00001120: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
-00001130: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
-00001140: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
-00001150: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
-00001160: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
-00001170: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
-00001180: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
-00001190: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
-000011a0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
-000011b0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
-000011c0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
-000011d0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
-000011e0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
-000011f0: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
-00001200: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-00001210: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-00001220: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
-00001230: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
-00001240: e200 e800 f200 f300 f500 f600 ff01 0801  ................
-00001250: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
-00001260: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
-00001270: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
-00001280: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
-00001290: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
-000012a0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
-000012b0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-000012c0: 0000 0000 0000 0000 0001 dd00 0000 0c00  ................
-000012d0: 7500 6e00 7300 7500 7000 6500 7200 7600  u.n.s.u.p.e.r.v.
-000012e0: 6900 7300 6500 646c 7376 7062 6c6f 6200  i.s.e.dlsvpblob.
-000012f0: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
-00001300: 0506 0708 090a 0b1d 4546 0a48 5f10 1276  ........EF.H_..v
-00001310: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00001320: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-00001330: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00001340: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00001350: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-00001360: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-00001370: 6544 6174 6573 5869 636f 6e53 697a 6510  eDatesXiconSize.
-00001380: 0109 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
-00001390: 2d32 373c 4158 636f 6d6d 656e 7473 5e64  -27<AXcomments^d
-000013a0: 6174 654c 6173 744f 7065 6e65 645b 6461  ateLastOpened[da
-000013b0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-000013c0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-000013d0: 6e54 6e61 6d65 5c64 6174 654d 6f64 6966  nTname\dateModif
-000013e0: 6965 64d4 1617 1819 1a0a 1c1d 5569 6e64  ied.........Uind
-000013f0: 6578 5961 7363 656e 6469 6e67 5577 6964  exYascendingUwid
-00001400: 7468 5776 6973 6962 6c65 1007 0911 012c  thWvisible.....,
-00001410: 08d4 1617 1819 1f1d 211d 1008 0810 c808  ........!.......
-00001420: d416 1718 1924 1d26 1d10 0208 10b5 08d4  .....$.&........
-00001430: 1617 1819 291d 2b0a 1003 0810 6109 d416  ....).+.....a...
-00001440: 1718 192e 0a30 1d10 0509 1064 08d4 1617  .....0.....d....
-00001450: 1819 330a 350a 1004 0910 7309 d416 1718  ..3.5.....s.....
-00001460: 1938 0a3a 1d10 0609 104b 08d4 1617 1819  .8.:.....K......
-00001470: 3d0a 3f0a 1000 0911 018f 09d4 1617 1819  =.?.............
-00001480: 091d 260a 0809 0823 4028 0000 0000 0000  ..&....#@(......
-00001490: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-000014a0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-000014b0: 8300 8c00 8e00 8f00 a200 ab00 ba00 c600  ................
-000014c0: cb00 d100 d600 de00 e300 f000 f900 ff01  ................
-000014d0: 0901 0f01 1701 1901 1a01 1d01 1e01 2701  ..............'.
-000014e0: 2901 2a01 2c01 2d01 3601 3801 3901 3b01  ).*.,.-.6.8.9.;.
-000014f0: 3c01 4501 4701 4801 4a01 4b01 5401 5601  <.E.G.H.J.K.T.V.
-00001500: 5701 5901 5a01 6301 6501 6601 6801 6901  W.Y.Z.c.e.f.h.i.
-00001510: 7201 7401 7501 7701 7801 8101 8301 8401  r.t.u.w.x.......
-00001520: 8701 8801 9101 9201 9301 9401 9d01 a201  ................
-00001530: a300 0000 0000 0002 0100 0000 0000 0000  ................
-00001540: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00001550: ac00 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
-00001560: 6500 7200 7600 6900 7300 6500 646d 6f44  e.r.v.i.s.e.dmoD
-00001570: 4462 6c6f 6200 0000 08f2 efa7 b815 f8c4  Dblob...........
-00001580: 4100 0000 0c00 7500 6e00 7300 7500 7000  A.....u.n.s.u.p.
-00001590: 6500 7200 7600 6900 7300 6500 646d 6f64  e.r.v.i.s.e.dmod
-000015a0: 4462 6c6f 6200 0000 08f2 efa7 b815 f8c4  Dblob...........
-000015b0: 4100 0000 0c00 7500 6e00 7300 7500 7000  A.....u.n.s.u.p.
-000015c0: 6500 7200 7600 6900 7300 6500 6470 6831  e.r.v.i.s.e.dph1
-000015d0: 5363 6f6d 7000 0000 0000 0840 0000 0000  Scomp......@....
+00001020: 0069 0073 0065 0064 6c67 3153 636f 6d70  .i.s.e.dlg1Scomp
+00001030: 0000 0000 0005 fd3a 0000 000c 0075 006e  .......:.....u.n
+00001040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
+00001050: 0065 0064 6c73 7643 626c 6f62 0000 0297  .e.dlsvCblob....
+00001060: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00001070: 0809 0a0b 1949 4a0a 4c5f 1012 7669 6577  .....IJ.L_..view
+00001080: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00001090: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000010a0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000010b0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+000010c0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+000010d0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+000010e0: 7465 7358 6963 6f6e 5369 7a65 1001 09ab  tesXiconSize....
+000010f0: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
+00001100: 0a0a 1314 5776 6973 6962 6c65 5961 7363  ....WvisibleYasc
+00001110: 656e 6469 6e67 5577 6964 7468 5a69 6465  endingUwidthZide
+00001120: 6e74 6966 6965 7209 0911 018f 546e 616d  ntifier.....Tnam
+00001130: 65d4 1617 1810 191a 191c 5776 6973 6962  e.........Wvisib
+00001140: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00001150: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
+00001160: 0d0e 0f10 0a19 2021 0908 10b5 5c64 6174  ...... !....\dat
+00001170: 654d 6f64 6966 6965 64d4 0d0e 0f10 1919  eModified.......
+00001180: 2025 0808 5b64 6174 6543 7265 6174 6564   %..[dateCreated
+00001190: d40d 0e0f 100a 1929 2a09 0810 6154 7369  .......)*...aTsi
+000011a0: 7a65 d40d 0e0f 100a 0a2e 2f09 0910 7354  ze......../...sT
+000011b0: 6b69 6e64 d40d 0e0f 1019 0a33 3408 0910  kind.......34...
+000011c0: 6455 6c61 6265 6cd4 0d0e 0f10 190a 3839  dUlabel.......89
+000011d0: 0809 104b 5776 6572 7369 6f6e d40d 0e0f  ...KWversion....
+000011e0: 1019 0a3d 3e08 0911 012c 5863 6f6d 6d65  ...=>....,Xcomme
+000011f0: 6e74 73d4 0d0e 0f10 1919 4243 0808 10c8  nts.......BC....
+00001200: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+00001210: 1617 1810 1920 1947 0808 5964 6174 6541  ..... .G..YdateA
+00001220: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
+00001230: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
+00001240: 1900 2e00 4000 4800 5c00 6500 7000 8300  ....@.H.\.e.p...
+00001250: 8c00 8e00 8f00 9b00 a400 ac00 b600 bc00  ................
+00001260: c700 c800 c900 cc00 d100 da00 e200 e800  ................
+00001270: f200 f300 f500 f600 ff01 0801 0901 0a01  ................
+00001280: 0c01 1901 2201 2301 2401 3001 3901 3a01  ....".#.$.0.9.:.
+00001290: 3b01 3d01 4201 4b01 4c01 4d01 4f01 5401  ;.=.B.K.L.M.O.T.
+000012a0: 5d01 5e01 5f01 6101 6701 7001 7101 7201  ].^._.a.g.p.q.r.
+000012b0: 7401 7c01 8501 8601 8701 8a01 9301 9c01  t.|.............
+000012c0: 9d01 9e01 a001 af01 b801 b901 ba01 c401  ................
+000012d0: c501 ce01 d301 d400 0000 0000 0002 0100  ................
+000012e0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+000012f0: 0000 0000 0001 dd00 0000 0c00 7500 6e00  ............u.n.
+00001300: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
+00001310: 6500 646c 7376 7062 6c6f 6200 0002 5e62  e.dlsvpblob...^b
+00001320: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+00001330: 090a 0b1d 4546 0a48 5f10 1276 6965 774f  ....EF.H_..viewO
+00001340: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+00001350: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00001360: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00001370: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+00001380: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+00001390: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+000013a0: 6573 5869 636f 6e53 697a 6510 0109 d90c  esXiconSize.....
+000013b0: 0d0e 0f10 1112 1314 151e 2328 2d32 373c  ..........#(-27<
+000013c0: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
+000013d0: 6173 744f 7065 6e65 645b 6461 7465 4372  astOpened[dateCr
+000013e0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+000013f0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00001400: 6d65 5c64 6174 654d 6f64 6966 6965 64d4  me\dateModified.
+00001410: 1617 1819 1a0a 1c1d 5569 6e64 6578 5961  ........UindexYa
+00001420: 7363 656e 6469 6e67 5577 6964 7468 5776  scendingUwidthWv
+00001430: 6973 6962 6c65 1007 0911 012c 08d4 1617  isible.....,....
+00001440: 1819 1f1d 211d 1008 0810 c808 d416 1718  ....!...........
+00001450: 1924 1d26 1d10 0208 10b5 08d4 1617 1819  .$.&............
+00001460: 291d 2b0a 1003 0810 6109 d416 1718 192e  ).+.....a.......
+00001470: 0a30 1d10 0509 1064 08d4 1617 1819 330a  .0.....d......3.
+00001480: 350a 1004 0910 7309 d416 1718 1938 0a3a  5.....s......8.:
+00001490: 1d10 0609 104b 08d4 1617 1819 3d0a 3f0a  .....K......=.?.
+000014a0: 1000 0911 018f 09d4 1617 1819 091d 260a  ..............&.
+000014b0: 0809 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+000014c0: 6509 2340 3000 0000 0000 0000 0800 1900  e.#@0...........
+000014d0: 2e00 4000 4800 5c00 6500 7000 8300 8c00  ..@.H.\.e.p.....
+000014e0: 8e00 8f00 a200 ab00 ba00 c600 cb00 d100  ................
+000014f0: d600 de00 e300 f000 f900 ff01 0901 0f01  ................
+00001500: 1701 1901 1a01 1d01 1e01 2701 2901 2a01  ..........'.).*.
+00001510: 2c01 2d01 3601 3801 3901 3b01 3c01 4501  ,.-.6.8.9.;.<.E.
+00001520: 4701 4801 4a01 4b01 5401 5601 5701 5901  G.H.J.K.T.V.W.Y.
+00001530: 5a01 6301 6501 6601 6801 6901 7201 7401  Z.c.e.f.h.i.r.t.
+00001540: 7501 7701 7801 8101 8301 8401 8701 8801  u.w.x...........
+00001550: 9101 9201 9301 9401 9d01 a201 a300 0000  ................
+00001560: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+00001570: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+00001580: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
+00001590: 7600 6900 7300 6500 646d 6f44 4462 6c6f  v.i.s.e.dmoDDblo
+000015a0: 6200 0000 08b0 f569 2d29 f8c4 4100 0000  b......i-)..A...
+000015b0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
+000015c0: 7600 6900 7300 6500 646d 6f64 4462 6c6f  v.i.s.e.dmodDblo
+000015d0: 6200 0000 08b0 f569 2d29 f8c4 4100 0000  b......i-)..A...
 000015e0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
-000015f0: 7600 6900 7300 6500 6476 5372 6e6c 6f6e  v.i.s.e.dvSrnlon
-00001600: 6700 0000 0100 0000 0500 7500 7400 6900  g.........u.t.i.
-00001610: 6c00 7362 7773 7062 6c6f 6200 0000 c962  l.sbwspblob....b
-00001620: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00001630: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00001640: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00001650: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00001660: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00001670: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00001680: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00001690: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-000016a0: 7b7b 3734 362c 2033 3230 7d2c 207b 3737  {{746, 320}, {77
-000016b0: 302c 2034 3336 7d7d 0908 1725 313d 4960  0, 436}}...%1=I`
-000016c0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-000016d0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000016e0: 0000 0000 0000 009a 0000 0005 0075 0074  .............u.t
-000016f0: 0069 006c 0073 6473 636c 626f 6f6c 0000  .i.l.sdsclbool..
-00001700: 0000 0500 7500 7400 6900 6c00 736c 6731  ....u.t.i.l.slg1
-00001710: 5363 6f6d 7000 0000 0000 011e f300 0000  Scomp...........
-00001720: 0500 7500 7400 6900 6c00 736c 7376 4362  ..u.t.i.l.slsvCb
-00001730: 6c6f 6200 0002 9762 706c 6973 7430 30d8  lob....bplist00.
-00001740: 0102 0304 0506 0708 090a 0b19 494a 0a4c  ............IJ.L
-00001750: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001760: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-00001770: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00001780: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00001790: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-000017a0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-000017b0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
-000017c0: 697a 6510 0109 ab0c 151d 2226 2b30 353a  ize......."&+05:
-000017d0: 3f44 d40d 0e0f 100a 0a13 1457 7669 7369  ?D.........Wvisi
-000017e0: 626c 6559 6173 6365 6e64 696e 6755 7769  bleYascendingUwi
-000017f0: 6474 685a 6964 656e 7469 6669 6572 0909  dthZidentifier..
-00001800: 1102 0454 6e61 6d65 d416 1718 1019 1a19  ...Tname........
-00001810: 1c57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00001820: 6173 6365 6e64 696e 6708 1023 0858 7562  ascending..#.Xub
-00001830: 6971 7569 7479 d40d 0e0f 100a 1920 2109  iquity....... !.
-00001840: 0810 b55c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00001850: d40d 0e0f 1019 1920 2508 085b 6461 7465  ....... %..[date
-00001860: 4372 6561 7465 64d4 0d0e 0f10 0a19 292a  Created.......)*
-00001870: 0908 1061 5473 697a 65d4 0d0e 0f10 0a0a  ...aTsize.......
-00001880: 2e2f 0909 1073 546b 696e 64d4 0d0e 0f10  ./...sTkind.....
-00001890: 190a 3334 0809 1064 556c 6162 656c d40d  ..34...dUlabel..
-000018a0: 0e0f 1019 0a38 3908 0910 4b57 7665 7273  .....89...KWvers
-000018b0: 696f 6ed4 0d0e 0f10 190a 3d3e 0809 1101  ion.......=>....
-000018c0: 2c58 636f 6d6d 656e 7473 d40d 0e0f 1019  ,Xcomments......
-000018d0: 1942 4308 0810 c85e 6461 7465 4c61 7374  .BC....^dateLast
-000018e0: 4f70 656e 6564 d416 1718 1019 2019 4708  Opened...... .G.
-000018f0: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
-00001900: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
-00001910: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
-00001920: 0065 0070 0083 008c 008e 008f 009b 00a4  .e.p............
-00001930: 00ac 00b6 00bc 00c7 00c8 00c9 00cc 00d1  ................
-00001940: 00da 00e2 00e8 00f2 00f3 00f5 00f6 00ff  ................
-00001950: 0108 0109 010a 010c 0119 0122 0123 0124  ...........".#.$
-00001960: 0130 0139 013a 013b 013d 0142 014b 014c  .0.9.:.;.=.B.K.L
-00001970: 014d 014f 0154 015d 015e 015f 0161 0167  .M.O.T.].^._.a.g
-00001980: 0170 0171 0172 0174 017c 0185 0186 0187  .p.q.r.t.|......
-00001990: 018a 0193 019c 019d 019e 01a0 01af 01b8  ................
-000019a0: 01b9 01ba 01c4 01c5 01ce 01d3 01d4 0000  ................
-000019b0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-000019c0: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
-000019d0: 0005 0075 0074 0069 006c 0073 6c73 7670  ...u.t.i.l.slsvp
-000019e0: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
-000019f0: d801 0203 0405 0607 0809 0a0b 1d45 460a  .............EF.
-00001a00: 485f 1012 7669 6577 4f70 7469 6f6e 7356  H_..viewOptionsV
-00001a10: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00001a20: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00001a30: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00001a40: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00001a50: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00001a60: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
-00001a70: 5369 7a65 1001 09d9 0c0d 0e0f 1011 1213  Size............
-00001a80: 1415 1e23 282d 3237 3c41 5863 6f6d 6d65  ...#(-27<AXcomme
-00001a90: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-00001aa0: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00001ab0: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00001ac0: 6572 7369 6f6e 546e 616d 655c 6461 7465  ersionTname\date
-00001ad0: 4d6f 6469 6669 6564 d416 1718 191a 0a1c  Modified........
-00001ae0: 1d55 696e 6465 7859 6173 6365 6e64 696e  .UindexYascendin
-00001af0: 6755 7769 6474 6857 7669 7369 626c 6510  gUwidthWvisible.
-00001b00: 0709 1101 2c08 d416 1718 191f 1d21 1d10  ....,........!..
-00001b10: 0808 10c8 08d4 1617 1819 241d 261d 1002  ..........$.&...
-00001b20: 0810 b508 d416 1718 1929 1d2b 0a10 0308  .........).+....
-00001b30: 1061 09d4 1617 1819 2e0a 301d 1005 0910  .a........0.....
-00001b40: 6408 d416 1718 1933 0a35 0a10 0409 1073  d......3.5.....s
-00001b50: 09d4 1617 1819 380a 3a1d 1006 0910 4b08  ......8.:.....K.
-00001b60: d416 1718 193d 0a3f 0a10 0009 1102 0409  .....=.?........
-00001b70: d416 1718 1909 1d26 0a08 0908 2340 2800  .......&....#@(.
-00001b80: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
-00001b90: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
-00001ba0: 0065 0070 0083 008c 008e 008f 00a2 00ab  .e.p............
-00001bb0: 00ba 00c6 00cb 00d1 00d6 00de 00e3 00f0  ................
-00001bc0: 00f9 00ff 0109 010f 0117 0119 011a 011d  ................
-00001bd0: 011e 0127 0129 012a 012c 012d 0136 0138  ...'.).*.,.-.6.8
-00001be0: 0139 013b 013c 0145 0147 0148 014a 014b  .9.;.<.E.G.H.J.K
-00001bf0: 0154 0156 0157 0159 015a 0163 0165 0166  .T.V.W.Y.Z.c.e.f
-00001c00: 0168 0169 0172 0174 0175 0177 0178 0181  .h.i.r.t.u.w.x..
-00001c10: 0183 0184 0187 0188 0191 0192 0193 0194  ................
-00001c20: 019d 01a2 01a3 0000 0000 0000 0201 0000  ................
-00001c30: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
-00001c40: 0000 0000 01ac 0000 0005 0075 0074 0069  ...........u.t.i
-00001c50: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-00001c60: 54f1 87c2 44f6 c441 0000 0005 0075 0074  T...D..A.....u.t
-00001c70: 0069 006c 0073 6d6f 6444 626c 6f62 0000  .i.l.smodDblob..
-00001c80: 0008 b191 97e3 46f2 c441 0000 0005 0075  ......F..A.....u
-00001c90: 0074 0069 006c 0073 7068 3153 636f 6d70  .t.i.l.sph1Scomp
-00001ca0: 0000 0000 0001 6000 0000 0005 0075 0074  ......`......u.t
-00001cb0: 0069 006c 0073 7653 726e 6c6f 6e67 0000  .i.l.svSrnlong..
-00001cc0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015f0: 7600 6900 7300 6500 6470 6831 5363 6f6d  v.i.s.e.dph1Scom
+00001600: 7000 0000 0000 0740 0000 0000 0c00 7500  p......@......u.
+00001610: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
+00001620: 7300 6500 6476 5372 6e6c 6f6e 6700 0000  s.e.dvSrnlong...
+00001630: 0100 0000 0500 7500 7400 6900 6c00 7362  ......u.t.i.l.sb
+00001640: 7773 7062 6c6f 6200 0000 c962 706c 6973  wspblob....bplis
+00001650: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+00001660: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00001670: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00001680: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00001690: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+000016a0: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+000016b0: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+000016c0: 6562 6172 0808 0908 095f 1018 7b7b 3734  ebar....._..{{74
+000016d0: 362c 2033 3230 7d2c 207b 3737 302c 2034  6, 320}, {770, 4
+000016e0: 3336 7d7d 0908 1725 313d 4960 6d79 7a7b  36}}...%1=I`myz{
+000016f0: 7c7d 7e99 0000 0000 0000 0101 0000 0000  |}~.............
+00001700: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+00001710: 0000 009a 0000 0005 0075 0074 0069 006c  .........u.t.i.l
+00001720: 0073 6473 636c 626f 6f6c 0000 0000 0500  .sdsclbool......
+00001730: 7500 7400 6900 6c00 736c 6731 5363 6f6d  u.t.i.l.slg1Scom
+00001740: 7000 0000 0000 011e f300 0000 0500 7500  p.............u.
+00001750: 7400 6900 6c00 736c 7376 4362 6c6f 6200  t.i.l.slsvCblob.
+00001760: 0002 9762 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+00001770: 0506 0708 090a 0b19 494a 0a4c 5f10 1276  ........IJ.L_..v
+00001780: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00001790: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+000017a0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+000017b0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+000017c0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+000017d0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+000017e0: 6544 6174 6573 5869 636f 6e53 697a 6510  eDatesXiconSize.
+000017f0: 0109 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
+00001800: 0e0f 100a 0a13 1457 7669 7369 626c 6559  .......WvisibleY
+00001810: 6173 6365 6e64 696e 6755 7769 6474 685a  ascendingUwidthZ
+00001820: 6964 656e 7469 6669 6572 0909 1102 0454  identifier.....T
+00001830: 6e61 6d65 d416 1718 1019 1a19 1c57 7669  name.........Wvi
+00001840: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00001850: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
+00001860: 7479 d40d 0e0f 100a 1920 2109 0810 b55c  ty....... !....\
+00001870: 6461 7465 4d6f 6469 6669 6564 d40d 0e0f  dateModified....
+00001880: 1019 1920 2508 085b 6461 7465 4372 6561  ... %..[dateCrea
+00001890: 7465 64d4 0d0e 0f10 0a19 292a 0908 1061  ted.......)*...a
+000018a0: 5473 697a 65d4 0d0e 0f10 0a0a 2e2f 0909  Tsize......../..
+000018b0: 1073 546b 696e 64d4 0d0e 0f10 190a 3334  .sTkind.......34
+000018c0: 0809 1064 556c 6162 656c d40d 0e0f 1019  ...dUlabel......
+000018d0: 0a38 3908 0910 4b57 7665 7273 696f 6ed4  .89...KWversion.
+000018e0: 0d0e 0f10 190a 3d3e 0809 1101 2c58 636f  ......=>....,Xco
+000018f0: 6d6d 656e 7473 d40d 0e0f 1019 1942 4308  mments.......BC.
+00001900: 0810 c85e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+00001910: 6564 d416 1718 1019 2019 4708 0859 6461  ed...... .G..Yda
+00001920: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+00001930: 0054 6e61 6d65 0923 4030 0000 0000 0000  .Tname.#@0......
+00001940: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+00001950: 0083 008c 008e 008f 009b 00a4 00ac 00b6  ................
+00001960: 00bc 00c7 00c8 00c9 00cc 00d1 00da 00e2  ................
+00001970: 00e8 00f2 00f3 00f5 00f6 00ff 0108 0109  ................
+00001980: 010a 010c 0119 0122 0123 0124 0130 0139  .......".#.$.0.9
+00001990: 013a 013b 013d 0142 014b 014c 014d 014f  .:.;.=.B.K.L.M.O
+000019a0: 0154 015d 015e 015f 0161 0167 0170 0171  .T.].^._.a.g.p.q
+000019b0: 0172 0174 017c 0185 0186 0187 018a 0193  .r.t.|..........
+000019c0: 019c 019d 019e 01a0 01af 01b8 01b9 01ba  ................
+000019d0: 01c4 01c5 01ce 01d3 01d4 0000 0000 0000  ................
+000019e0: 0201 0000 0000 0000 004d 0000 0000 0000  .........M......
+000019f0: 0000 0000 0000 0000 01dd 0000 0005 0075  ...............u
+00001a00: 0074 0069 006c 0073 6c73 7670 626c 6f62  .t.i.l.slsvpblob
+00001a10: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
+00001a20: 0405 0607 0809 0a0b 1d45 460a 485f 1012  .........EF.H_..
+00001a30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001a40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001a50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001a60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001a70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+00001a80: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+00001a90: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+00001aa0: 1001 09d9 0c0d 0e0f 1011 1213 1415 1e23  ...............#
+00001ab0: 282d 3237 3c41 5863 6f6d 6d65 6e74 735e  (-27<AXcomments^
+00001ac0: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
+00001ad0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001ae0: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001af0: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
+00001b00: 6669 6564 d416 1718 191a 0a1c 1d55 696e  fied.........Uin
+00001b10: 6465 7859 6173 6365 6e64 696e 6755 7769  dexYascendingUwi
+00001b20: 6474 6857 7669 7369 626c 6510 0709 1101  dthWvisible.....
+00001b30: 2c08 d416 1718 191f 1d21 1d10 0808 10c8  ,........!......
+00001b40: 08d4 1617 1819 241d 261d 1002 0810 b508  ......$.&.......
+00001b50: d416 1718 1929 1d2b 0a10 0308 1061 09d4  .....).+.....a..
+00001b60: 1617 1819 2e0a 301d 1005 0910 6408 d416  ......0.....d...
+00001b70: 1718 1933 0a35 0a10 0409 1073 09d4 1617  ...3.5.....s....
+00001b80: 1819 380a 3a1d 1006 0910 4b08 d416 1718  ..8.:.....K.....
+00001b90: 193d 0a3f 0a10 0009 1102 0409 d416 1718  .=.?............
+00001ba0: 1909 1d26 0a08 0908 2340 2800 0000 0000  ...&....#@(.....
+00001bb0: 0054 6e61 6d65 0923 4030 0000 0000 0000  .Tname.#@0......
+00001bc0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+00001bd0: 0083 008c 008e 008f 00a2 00ab 00ba 00c6  ................
+00001be0: 00cb 00d1 00d6 00de 00e3 00f0 00f9 00ff  ................
+00001bf0: 0109 010f 0117 0119 011a 011d 011e 0127  ...............'
+00001c00: 0129 012a 012c 012d 0136 0138 0139 013b  .).*.,.-.6.8.9.;
+00001c10: 013c 0145 0147 0148 014a 014b 0154 0156  .<.E.G.H.J.K.T.V
+00001c20: 0157 0159 015a 0163 0165 0166 0168 0169  .W.Y.Z.c.e.f.h.i
+00001c30: 0172 0174 0175 0177 0178 0181 0183 0184  .r.t.u.w.x......
+00001c40: 0187 0188 0191 0192 0193 0194 019d 01a2  ................
+00001c50: 01a3 0000 0000 0000 0201 0000 0000 0000  ................
+00001c60: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00001c70: 01ac 0000 0005 0075 0074 0069 006c 0073  .......u.t.i.l.s
+00001c80: 6d6f 4444 626c 6f62 0000 0008 54f1 87c2  moDDblob....T...
+00001c90: 44f6 c441 0000 0005 0075 0074 0069 006c  D..A.....u.t.i.l
+00001ca0: 0073 6d6f 6444 626c 6f62 0000 0008 b191  .smodDblob......
+00001cb0: 97e3 46f2 c441 0000 0005 0075 0074 0069  ..F..A.....u.t.i
+00001cc0: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
+00001cd0: 0001 6000 0000 0005 0075 0074 0069 006c  ..`......u.t.i.l
+00001ce0: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -509,18 +509,18 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 0ef0 0000 000b 005f 005f 0070  ...B......._._.p
+00002030: 0000 0042 0f84 0000 000b 005f 005f 0070  ...B......._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 8577 e207  moDDblob.....w..
-00002060: 73f7 c441 0000 000b 005f 005f 0070 0079  s..A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 5692 9a09  moDDblob....V...
+00002060: 1cf8 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 6a13 8953 eaf6  dDblob....j..S..
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0050 0000 0000 0006  comp.....P......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
@@ -1049,21 +1049,21 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 01ad c200 0000 0600 6d00 6900 7800  ..........m.i.x.
+000041f0: 0000 01aa ba00 0000 0600 6d00 6900 7800  ..........m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 08e3 5739 7081 f7c4 4100 0000 0600 6d00  ..W9p...A.....m.
+00004210: 08cd 7da0 ce1e f8c4 4100 0000 0600 6d00  ..}.....A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
-00004230: 6200 0000 08ef 201d a05b f6c4 4100 0000  b..... ..[..A...
+00004230: 6200 0000 08cd 7da0 ce1e f8c4 4100 0000  b.....}.....A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
-00004250: 5363 6f6d 7000 0000 0000 0200 0000 0000  Scomp...........
+00004250: 5363 6f6d 7000 0000 0000 01f0 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00004290: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
 000042a0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000042b0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 000042c0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
@@ -1193,15 +1193,15 @@
 00004a80: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
 00004a90: 3135 392c 2031 3233 7d2c 207b 3130 3736  159, 123}, {1076
 00004aa0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
 00004ab0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
 00004ac0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00004ad0: 0000 0000 0000 9b00 0000 0800 7000 6c00  ............p.l.
 00004ae0: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00004af0: 6f6d 7000 0000 0000 0a18 fb00 0000 0800  omp.............
+00004af0: 6f6d 7000 0000 0000 0a1b 6500 0000 0800  omp.......e.....
 00004b00: 7000 6c00 6f00 7400 7400 6900 6e00 676c  p.l.o.t.t.i.n.gl
 00004b10: 7376 4362 6c6f 6200 0002 bb62 706c 6973  svCblob....bplis
 00004b20: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
 00004b30: 0d1a 4849 4a4b 4c0c 5f10 1276 6965 774f  ..HIJKL._..viewO
 00004b40: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00004b50: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00004b60: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
@@ -1276,16 +1276,16 @@
 00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 0014 0000 0008  ................
 00005010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00005020: 6d6f 4444 626c 6f62 0000 0008 e63c 5181  moDDblob.....<Q.
-00005030: 52f2 c441 0000 0008 0070 006c 006f 0074  R..A.....p.l.o.t
+00005020: 6d6f 4444 626c 6f62 0000 0008 7b27 5505  moDDblob....{'U.
+00005030: 1cf8 c441 0000 0008 0070 006c 006f 0074  ...A.....p.l.o.t
 00005040: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
 00005050: 0000 0008 65be f96a 3ef2 c441 0000 0008  ....e..j>..A....
 00005060: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00005070: 7068 3153 636f 6d70 0000 0000 000c 4000  ph1Scomp......@.
 00005080: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00005090: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
 000050a0: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
@@ -1776,15 +1776,15 @@
 00006ef0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 00006f00: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00006f10: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 00006f20: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00006f30: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00006f40: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00006f50: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00006f60: 0809 5f10 197b 7b32 3630 2c20 3136 327d  .._..{{260, 162}
+00006f60: 0809 5f10 197b 7b32 3633 2c20 3239 357d  .._..{{263, 295}
 00006f70: 2c20 7b31 3138 302c 2035 3538 7d7d 0908  , {1180, 558}}..
 00006f80: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 00006f90: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 00006fa0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1885,16 +1885,16 @@
 000075c0: e500 0000 0000 0002 0100 0000 0000 0000  ................
 000075d0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
 000075e0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
 000075f0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00007600: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
 00007610: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
 00007620: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00007630: 646c 6731 5363 6f6d 7000 0000 0000 06c2  dlg1Scomp.......
-00007640: 5369 005f 0074 006f 006f 006c 0073 6d6f  Si._.t.o.o.l.smo
+00007630: 6464 7363 6c62 6f6f 6c01 0009 0072 006f  ddsclbool....r.o
+00007640: 0069 005f 0074 006f 006f 006c 0073 6d6f  .i._.t.o.o.l.smo
 00007650: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
 00007660: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
 00007670: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
 00007680: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
 00007690: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 000076a0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
 000076b0: 2000 0000 0009 0072 006f 0069 005f 0074   ......r.o.i._.t
@@ -2013,16 +2013,16 @@
 00007dc0: e500 0000 0000 0002 0100 0000 0000 0000  ................
 00007dd0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
 00007de0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
 00007df0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00007e00: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
 00007e10: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
 00007e20: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00007e30: 646c 6731 5363 6f6d 7000 0000 0000 06c2  dlg1Scomp.......
-00007e40: 5369 005f 0074 006f 006f 006c 0073 6d6f  Si._.t.o.o.l.smo
+00007e30: 6464 7363 6c62 6f6f 6c01 0009 0072 006f  ddsclbool....r.o
+00007e40: 0069 005f 0074 006f 006f 006c 0073 6d6f  .i._.t.o.o.l.smo
 00007e50: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
 00007e60: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
 00007e70: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
 00007e80: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
 00007e90: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 00007ea0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
 00007eb0: 2000 0000 0009 0072 006f 0069 005f 0074   ......r.o.i._.t
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.56.9/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.56.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/severity_processor.py` & `Simba-UW-tf-dev-1.56.9/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.56.9/simba/mixins/pop_up_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tkinter import *
 from simba.read_config_unit_tests import (check_int,
                                           check_str,
+                                          check_float,
                                           check_if_dir_exists,
                                           read_project_path_and_file_type)
 from simba.pose_importers.read_DANNCE_mat import import_DANNCE_file, import_DANNCE_folder
 from simba.pose_importers.import_mars import MarsImporter
 from simba.pose_importers.dlc_multi_animal_importer import MADLC_Importer
 from simba.pose_importers.sleap_importer_csv import SLEAPImporterCSV
 from simba.pose_importers.sleap_importer_h5 import SLEAPImporterH5
@@ -38,48 +39,34 @@
 import simba
 
 
 class PopUpMixin(object):
     def __init__(self,
                  title: str,
                  config_path: str or None=None,
-                 size: tuple=(400,400),
-                 hyperlink: str or None=None):
+                 size: tuple=(400,400)):
 
         self.main_frm = Toplevel()
         self.main_frm.minsize(size[0], size[1])
         self.main_frm.wm_title(title)
-
-        # self.menu_icons = get_icons_paths()
-        # for k in self.menu_icons.keys():
-        #     self.menu_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname("__file__"), self.menu_icons[k]['icon_path'])))
-        # self.main_frm.overrideredirect(True)
-        # title_bar = Frame(self.main_frm, bg=Formats.HEADER_BG_CLR_FORMAT.value, relief='raised', bd=1)
-        # title_lbl = Label(title_bar, text=title, bg=Formats.HEADER_BG_CLR_FORMAT.value, fg='black', font=Formats.LABELFRAME_HEADER_CLICKABLE_FORMAT)
-        # if hyperlink:
-        #     title_lbl.bind("<Button-1>", lambda e: self.callback('https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md'))
-        # title_bar.pack(side=TOP, fill=X)
-        # title_lbl.place(relx=0.5, rely=0.5, anchor=CENTER)
-        # close_lbl = Label(title_bar, compound='left', image=self.menu_icons['close']['img'],bg=Formats.HEADER_BG_CLR_FORMAT.value, fg='red', relief='raised', bd=1)
-        # close_lbl.pack(side=LEFT, pady=4)
-        # close_lbl.bind("<Button-1>", self.quit)
-        # title_bar.bind("<B1-Motion>", self.move_app)
-
         self.main_frm.lift()
         self.main_frm = Canvas(hxtScrollbar(self.main_frm))
         self.main_frm.pack(fill="both", expand=True)
 
         self.palette_options = Options.PALETTE_OPTIONS.value
         self.resolutions = Options.RESOLUTION_OPTIONS.value
         self.shading_options = Options.HEATMAP_SHADING_OPTIONS.value
         self.heatmap_bin_size_options = Options.HEATMAP_BIN_SIZE_OPTIONS.value
         self.dpi_options = Options.DPI_OPTIONS.value
         self.colors = get_named_colors()
         self.colors_dict = get_color_dict()
         self.cpu_cnt, _ = find_core_cnt()
+        self.menu_icons = get_icons_paths()
+        for k in self.menu_icons.keys():
+            self.menu_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname(__file__), self.menu_icons[k]['icon_path'])))
 
         if config_path:
             self.config_path = config_path
             self.config = read_config_file(ini_path=config_path)
             self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
             self.project_animal_cnt = read_config_entry(config=self.config, section=ReadConfig.GENERAL_SETTINGS.value, option=ReadConfig.ANIMAL_CNT.value, data_type='int')
             self.multi_animal_status, self.multi_animal_id_lst = check_multi_animal_status(self.config, self.project_animal_cnt)
@@ -181,14 +168,42 @@
         self.bp_cnt_dropdown = DropDownMenu(self.bp_cnt_frm, '# of body-parts', list(range(1, len(project_body_parts))), '12')
         self.bp_cnt_dropdown.setChoices(1)
         self.bp_cnt_confirm_btn = Button(self.bp_cnt_frm, text="Confirm", command=lambda: self.create_choose_bp_frm(project_body_parts, run_function))
         self.bp_cnt_frm.grid(row=0, sticky=NW)
         self.bp_cnt_dropdown.grid(row=0, column=0, sticky=NW)
         self.bp_cnt_confirm_btn.grid(row=0, column=1, sticky=NW)
 
+    def add_to_listbox_from_entrybox(self, list_box: Listbox, entry_box: Entry_Box):
+        value = entry_box.entry_get
+        check_float(name='VALUE', value=value)
+        list_box_content = [float(x) for x in list_box.get(0, END)]
+        if float(value) not in list_box_content:
+            list_box.insert(0, value)
+
+    def add_value_to_listbox(self,
+                             list_box: Listbox,
+                             value: float):
+        list_box.insert(0, value)
+
+    def add_values_to_several_listboxes(self,
+                                        list_boxes: list,
+                                        values: list):
+        if len(list_boxes) != len(values):
+            raise CountError(msg='Value count and listboxes count are not equal')
+        for i in range(len(list_boxes)):
+            list_boxes[i].insert(0, values[i])
+
+
+
+    def remove_from_listbox(self,
+                            list_box: Listbox):
+        selection = list_box.curselection()
+        if selection:
+            list_box.delete(selection[0])
+
 
     def create_choose_bp_frm(self, project_body_parts, run_function):
         if hasattr(self, 'body_part_frm'):
             self.body_part_frm.destroy()
         self.body_parts_dropdowns = {}
         self.body_part_frm = LabelFrame(self.main_frm, text="CHOOSE ANIMAL BODY-PARTS", font=Formats.LABELFRAME_HEADER_FORMAT.value, name='choose animal body-parts')
         self.body_part_frm.grid(row=self.children_cnt_main(), sticky=NW)
@@ -264,16 +279,14 @@
             if check_box_var.get():
                 for box in entry_boxes:
                     box.set_state('normal')
             else:
                 for box in entry_boxes:
                     box.set_state('disable')
 
-
-
     def create_import_pose_menu(self,
                                 parent_frm: Frame,
                                 idx_row: int = 0,
                                 idx_column: int = 0):
 
         def run_call(data_type: str,
                      interpolation: str,
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.56.9/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.56.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.56.9/simba/mixins/unsupervised_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
                                    StandardScaler,
                                    QuantileTransformer)
 from simba.utils.errors import (InvalidInputError,
                                 NoDataError,
                                 NoFilesFoundError,
                                 InvalidFileTypeError,
                                 MissingColumnsError,
-                                IntegerError)
+                                IntegerError,
+                                DirectoryNotEmptyError)
 
 
 class UnsupervisedMixin(object):
     def __init__(self):
 
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.timer = SimbaTimer()
@@ -106,7 +107,16 @@
                         data: np.array,
                         clusterer_name: str,
                         minimum_clusters: int = 1) -> int:
         cnt = np.unique(data).shape[0]
         if cnt < minimum_clusters:
             raise IntegerError(msg=f'Clustrer {clusterer_name} has {str(cnt)} clusters, but {str(minimum_clusters)} clusters is required for the operation.')
         return cnt
+
+    def check_that_directory_is_empty(self, directory: str) -> None:
+        try:
+            all_files_in_folder = [f for f in next(os.walk(directory))[2] if not f[0] == '.']
+        except StopIteration:
+            return 0
+        else:
+            if len(all_files_in_folder) > 0:
+                raise DirectoryNotEmptyError(msg=f'The {directory} is not empty and contains {str(len(all_files_in_folder))} files. Use a directory that is empty.')
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.56.9/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.56.9/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.56.9/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.56.9/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.56.9/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/video_info_table.py` & `Simba-UW-tf-dev-1.56.9/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.56.9/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.56.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.56.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.56.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.56.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.56.9/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.56.9/simba/train_model_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,33 +80,33 @@
 
     timer = SimbaTimer()
     timer.start_timer()
     df_concat = pd.DataFrame()
     for file_cnt, file in enumerate(file_paths):
         print(f'Reading in file {str(file_cnt+1)}/{str(len(file_paths))}...')
         _, vid_name, _ = get_fn_ext(file)
-        df = read_df(file, file_type).dropna(axis=0, how='all').fillna(0)
+        df = read_df(file, file_type).dropna(axis=0, how='all').fillna(0).astype(np.float16)
         if classifier_names != None:
             for clf_name in classifier_names:
                 if not clf_name in df.columns:
                     raise MissingColumnsError(msg=f'Data for video {vid_name} does not contain any annotations for behavior {clf_name}. Delete classifier {clf_name} from the SimBA project, or add annotations for behavior {clf_name} to the video {vid_name}')
                 else:
-                    df_concat = pd.concat([df_concat, df], axis=0)
+                    df_concat = pd.concat([df_concat, df], axis=0).astype(np.float16)
         else:
-            df_concat = pd.concat([df_concat, df], axis=0)
+            df_concat = pd.concat([df_concat, df], axis=0).astype(np.float16)
     try:
-        df_concat = df_concat.set_index('scorer')
+        df_concat = df_concat.set_index('scorer').astype(np.float16)
     except KeyError:
         pass
     if len(df_concat) == 0:
         raise NoDataError(msg='SimBA found 0 annotated frames in the project_folder/csv/targets_inserted directory')
     df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')]
     timer.stop_timer()
     print('{} file(s) read (elapsed time: {}s) ...'.format(str(len(file_paths)), timer.elapsed_time_str))
-    return df_concat.reset_index(drop=True)
+    return df_concat.reset_index(drop=True).astype(np.float16)
 
 
 def read_in_all_model_names_to_remove(config, model_cnt, clf_name):
     """
     Helper to find all field names that contain annotations but are not the target.
 
     Parameters
@@ -1012,15 +1012,15 @@
 
 def _read_data_file_helper(file_path, file_type, clf_names):
     """ Private function called by ``simba.train_model_functions.read_all_files_in_folder_mp`` """
 
     timer = SimbaTimer()
     timer.start_timer()
     _, vid_name, _ = get_fn_ext(file_path)
-    df = read_df(file_path, file_type).dropna(axis=0, how='all').fillna(0)
+    df = read_df(file_path, file_type).dropna(axis=0, how='all').fillna(0).astype(np.float16)
     if clf_names != None:
         for clf_name in clf_names:
             if not clf_name in df.columns:
                 raise ColumnNotFoundError(column_name=clf_name, file_name=file_path)
     timer.stop_timer()
     print(f'Reading complete {vid_name} (elapsed time: {timer.elapsed_time_str}s)...')
     return df
@@ -1077,19 +1077,20 @@
         multiprocessing.set_start_method('spawn', force=True)
     cpu_cnt, _ = find_core_cnt()
     df_lst = []
     try:
         with ProcessPoolExecutor(int(np.ceil(cpu_cnt/2))) as pool:
             for res in pool.map(_read_data_file_helper, file_paths, repeat(file_type), repeat(classifier_names)):
                 df_lst.append(res)
-        df_concat = pd.concat(df_lst, axis=0)
+        df_concat = pd.concat(df_lst, axis=0).astype(np.float16)
         if 'scorer' in df_concat.columns:
             df_concat = df_concat.set_index('scorer')
         if len(df_concat) == 0:
             raise ValueError('ANNOTATION ERROR: SimBA found 0 observations (frames) in the project_folder/csv/targets_inserted directory')
-        df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')]
+        df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')].astype(np.float16)
+        #print(df_concat.memory_usage(index=True).sum())
         return df_concat.reset_index(drop=True)
 
     except BrokenProcessPool:
         return read_all_files_in_folder(file_paths=file_paths,
                                         file_type=file_type,
                                         classifier_names=classifier_names)
```

### Comparing `Simba-UW-tf-dev-1.56.8/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.56.9/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.56.9/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/movement_processor.py` & `Simba-UW-tf-dev-1.56.9/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pybursts.py` & `Simba-UW-tf-dev-1.56.9/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.56.9/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.56.9/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.56.9/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.56.9/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/setting_menu.py` & `Simba-UW-tf-dev-1.56.9/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.56.9/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/run_inference.py` & `Simba-UW-tf-dev-1.56.9/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.56.9/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.56.9/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/dash_app.py` & `Simba-UW-tf-dev-1.56.9/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.56.9/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.56.9/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.56.9/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/misc_tools.py` & `Simba-UW-tf-dev-1.56.9/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.9/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.56.9/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.56.9/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.56.9/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/pose_reset.py` & `Simba-UW-tf-dev-1.56.9/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.56.9/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.56.9/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.56.9/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.56.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.56.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.56.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.56.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.56.9/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.56.9/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.56.9/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.56.9/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/train_single_model.py` & `Simba-UW-tf-dev-1.56.9/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.56.9/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.56.9/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.56.9/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.56.9/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.8
+Version: 1.56.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -325,25 +325,27 @@
 simba/third_party_label_appenders/deepethogram_importer.py
 simba/third_party_label_appenders/ethovision_import.py
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
 simba/unsupervised/.DS_Store
+simba/unsupervised/bout_aggregator.py
 simba/unsupervised/cluster_statistics.py
 simba/unsupervised/cluster_visualizer.py
 simba/unsupervised/data_extractor.py
 simba/unsupervised/data_map.yaml
 simba/unsupervised/dataset_creator.py
 simba/unsupervised/dbcv_calculator.py
 simba/unsupervised/enums.py
-simba/unsupervised/grd_search_cluster_visualizer.py
+simba/unsupervised/grid_search_visualizers.py
 simba/unsupervised/hdbscan_clusterer.py
 simba/unsupervised/pop_up_classes.py
 simba/unsupervised/tsne.py
+simba/unsupervised/ui.py
 simba/unsupervised/umap_embedder.py
 simba/unsupervised/unsupervised_ui.py
 simba/unsupervised/visualizers.py
 simba/utils/.DS_Store
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
```

### Comparing `Simba-UW-tf-dev-1.56.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/LICENSE.md` & `Simba-UW-tf-dev-1.56.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/README.md` & `Simba-UW-tf-dev-1.56.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.8/setup.py` & `Simba-UW-tf-dev-1.56.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.8",
+    version="1.56.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

