# Comparing `tmp/icepy4d-1.4.0.tar.gz` & `tmp/icepy4d-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icepy4d-1.4.0.tar", last modified: Thu Apr 20 08:54:14 2023, max compression
+gzip compressed data, was "icepy4d-1.5.0.tar", last modified: Thu Apr 20 09:37:44 2023, max compression
```

## Comparing `icepy4d-1.4.0.tar` & `icepy4d-1.5.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.992865 icepy4d-1.4.0/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1071 2022-11-10 18:54:33.000000 icepy4d-1.4.0/LICENSE.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3869 2023-04-20 08:54:14.992865 icepy4d-1.4.0/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2017 2023-04-20 08:51:29.000000 icepy4d-1.4.0/README.md
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1623 2023-04-20 08:53:52.000000 icepy4d-1.4.0/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-20 08:54:14.992865 icepy4d-1.4.0/setup.cfg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/icepy4d/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-04-20 08:00:10.000000 icepy4d-1.4.0/src/icepy4d/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/__main__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-04-04 14:17:37.000000 icepy4d-1.4.0/src/icepy4d/binned_stats.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/classes/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      235 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    17269 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/camera.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/dsm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/epoch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    19126 2023-04-20 08:26:25.000000 icepy4d-1.4.0/src/icepy4d/classes/images.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/ortophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-04-20 08:36:17.000000 icepy4d-1.4.0/src/icepy4d/classes/point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18374 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/points.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3262 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/solution.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/classes/targets.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      789 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/classes/typed_dict_classes.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/io/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/__init__.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build_windows_app.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/clang_format_code.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/database.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_bundler.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/flickr_downloader.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/h5_to_db.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/merge_ply_files.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/plyfile.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_dense.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_model.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/colmap_utils/visualize_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8925 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2bundler.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2calge.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4751 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/io/export2colmap.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/export2textfile.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1617 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/io/importing.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/least_squares/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/rototra3d.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/least_squares/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/matching/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11728 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/match_by_preselection.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13680 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/match_pairs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7602 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/matching_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/retrieve_matches_from_npz.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4119 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_match_simple_old.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14758 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_matcher.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13567 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/superglue_tracker.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/templatematch.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16784 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/track_matches.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18740 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/matching/track_matches_bk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3440 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/tracking_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/matching/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/metashape/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/metashape/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20120 2023-04-20 08:37:45.000000 icepy4d-1.4.0/src/icepy4d/metashape/metashape.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18631 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/metashape/ms_utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12502 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/open3d_fun.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/point_cloud_proc/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/sfm/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14455 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/absolute_orientation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/interpolate_colors.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/reconstruction.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6342 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/triangulation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/sfm/two_view_geometry.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10683 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18127 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3417 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11781 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8142 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20039 2023-03-31 12:00:43.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/transformations.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/thirdparty/triangulation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7325 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/tiles.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16090 2023-04-20 08:06:11.000000 icepy4d-1.4.0/src/icepy4d/tracking_features_utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-04-20 08:50:34.000000 icepy4d-1.4.0/src/icepy4d/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7091 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/dsm_orthophoto.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12263 2023-04-20 08:30:14.000000 icepy4d-1.4.0/src/icepy4d/utils/initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5957 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/utils/logger.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6355 2023-04-03 09:10:13.000000 icepy4d-1.4.0/src/icepy4d/utils/rototranslation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1552 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/sensor_width_database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/utils/spatial_funs.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/timer.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4893 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/utils/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.988865 icepy4d-1.4.0/src/icepy4d/visualization/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/visualization/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6162 2023-03-31 11:55:23.000000 icepy4d-1.4.0/src/icepy4d/visualization/vis_o3d_advanced.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    27688 2023-04-20 07:59:46.000000 icepy4d-1.4.0/src/icepy4d/visualization/visualization.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.984865 icepy4d-1.4.0/src/icepy4d.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3869 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4254 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      246 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-20 08:54:14.000000 icepy4d-1.4.0/src/icepy4d.egg-info/top_level.txt
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 08:54:14.992865 icepy4d-1.4.0/tests/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_image.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-04-20 08:42:31.000000 icepy4d-1.4.0/tests/test_initialization.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_point_cloud.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_sfm_geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      518 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1457 2023-04-20 07:59:47.000000 icepy4d-1.4.0/tests/test_utils_spatial.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.868899 icepy4d-1.5.0/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1558 2023-04-20 09:19:34.000000 icepy4d-1.5.0/LICENSE.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3905 2023-04-20 09:37:44.868899 icepy4d-1.5.0/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1502 2023-04-20 09:25:41.000000 icepy4d-1.5.0/README.md
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1623 2023-04-20 09:37:38.000000 icepy4d-1.5.0/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-20 09:37:44.868899 icepy4d-1.5.0/setup.cfg
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.860899 icepy4d-1.5.0/src/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.860899 icepy4d-1.5.0/src/icepy4d/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       55 2023-04-20 09:37:38.000000 icepy4d-1.5.0/src/icepy4d/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      244 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/__main__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13046 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/binned_stats.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/classes/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      235 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    17269 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/camera.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/dsm.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/epoch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26531 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    19126 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/images.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1079 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/ortophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6786 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18374 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/points.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3262 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/solution.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11317 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/targets.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      789 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/classes/typed_dict_classes.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/io/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/__init__.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/__init__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22889 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/build.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3709 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/build_windows_app.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4731 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2622 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/clang_format_code.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5565 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15026 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/database.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3389 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     3237 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6730 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_to_bundler.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6402 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     6297 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/flickr_downloader.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5996 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/h5_to_db.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2692 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/merge_ply_files.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4743 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    25506 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/plyfile.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5172 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_dense.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5230 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    22035 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_model.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     7069 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/colmap_utils/visualize_model.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8925 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/export2bundler.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2922 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/export2calge.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4751 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/export2colmap.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2995 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/export2textfile.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1617 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/io/importing.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/least_squares/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/least_squares/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2845 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/least_squares/rototra3d.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2761 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/least_squares/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/matching/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11728 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/match_by_preselection.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13680 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/match_pairs.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7602 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/matching_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1656 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/retrieve_matches_from_npz.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4119 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/superglue_match_simple_old.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14758 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/superglue_matcher.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    13567 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/superglue_tracker.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    15735 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/templatematch.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16784 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/track_matches.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18740 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/track_matches_bk.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3440 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/tracking_base.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5879 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/matching/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/metashape/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/metashape/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20120 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/metashape/metashape.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    18631 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/metashape/ms_utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/point_cloud_proc/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/point_cloud_proc/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7242 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    12502 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/point_cloud_proc/open3d_fun.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      974 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/point_cloud_proc/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/sfm/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      218 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14455 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/absolute_orientation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4404 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/interpolate_colors.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1333 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/reconstruction.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6342 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/triangulation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8073 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/sfm/two_view_geometry.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/thirdparty/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10683 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18127 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3417 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11781 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8142 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    20039 2023-03-31 12:00:43.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11815 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/transformations.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    10133 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/thirdparty/triangulation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7325 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/tiles.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    16090 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/tracking_features_utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/utils/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      295 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7091 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/dsm_orthophoto.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    12263 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     5957 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/logger.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6355 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/rototranslation.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1552 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/sensor_width_database.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3783 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/spatial_funs.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1662 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/timer.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4893 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/utils/utils.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.864899 icepy4d-1.5.0/src/icepy4d/visualization/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       29 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/visualization/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6162 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/visualization/vis_o3d_advanced.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    27688 2023-04-20 09:18:56.000000 icepy4d-1.5.0/src/icepy4d/visualization/visualization.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.860899 icepy4d-1.5.0/src/icepy4d.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     3905 2023-04-20 09:37:44.000000 icepy4d-1.5.0/src/icepy4d.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4254 2023-04-20 09:37:44.000000 icepy4d-1.5.0/src/icepy4d.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-20 09:37:44.000000 icepy4d-1.5.0/src/icepy4d.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      246 2023-04-20 09:37:44.000000 icepy4d-1.5.0/src/icepy4d.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-20 09:37:44.000000 icepy4d-1.5.0/src/icepy4d.egg-info/top_level.txt
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-20 09:37:44.868899 icepy4d-1.5.0/tests/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     8220 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_features.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1484 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_image.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2394 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_initialization.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      775 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_matching.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2032 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_point_cloud.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2742 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_sfm_geometry.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      518 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_utils.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1457 2023-04-20 09:18:56.000000 icepy4d-1.5.0/tests/test_utils_spatial.py
```

### Comparing `icepy4d-1.4.0/LICENSE.txt` & `icepy4d-1.5.0/src/icepy4d/classes/dsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""
 MIT License
 
 Copyright (c) 2022 Francesco Ioli
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -15,7 +16,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+"""
```

### Comparing `icepy4d-1.4.0/PKG-INFO` & `icepy4d-1.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.4.0
+Version: 1.5.0
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
-License: MIT License
+License: BSD 3-Clause License
         
-        Copyright (c) 2022 Francesco Ioli
+        Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
+        All rights reserved.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/franioli/icepy4d
 Keywords: sfm,4d-reconstruction,glaciers,deep-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -37,84 +45,54 @@
 
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
-
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
-
-```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
-```
-
-Check that `gdal` is correctly installed with:
-
-```bash
-python -c "from osgeo import gdal"
-```
-
-##### Install Pytorch
+## Installation guide
 
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+Create a new Anaconda environment
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-##### Install other required packages
+Install Icepy4D from PyPi repository
 
 ```bash
-pip3 install -r requirements.txt
+pip install icepy4d
 ```
 
-##### Various
-
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-##### Install ICEpy4D
-
-Install ICEpy4D package by running from the root folder
-
-```bash
-pip install -e .
-```
-
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
+
+### For contributing
 
+Install additional requirements for development:
 
-#### For contributing
-`bash
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/README.md` & `icepy4d-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,53 @@
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
-
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
-
-```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
-```
-
-Check that `gdal` is correctly installed with:
-
-```bash
-python -c "from osgeo import gdal"
-```
-
-##### Install Pytorch
+## Installation guide
 
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+Create a new Anaconda environment
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-##### Install other required packages
+Install Icepy4D from PyPi repository
 
 ```bash
-pip3 install -r requirements.txt
+pip install icepy4d
 ```
 
-##### Various
-
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
-
-##### Install ICEpy4D
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-Install ICEpy4D package by running from the root folder
-
-```bash
-pip install -e .
-```
-
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
 
+### For contributing
 
-#### For contributing
-`bash
+Install additional requirements for development:
+
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/pyproject.toml` & `icepy4d-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icepy4d"
-version = "1.4.0"
+version = "1.5.0"
 description = "4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry."
 readme = "README.md"
 authors = [{ name = "Francesco Ioli", email = "francesco.ioli@polimi.it" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -45,15 +45,15 @@
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.isort]
 profile = "black"
 [tool.bumpver]
-current_version = "1.4.0"
+current_version = "1.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `icepy4d-1.4.0/src/icepy4d/binned_stats.py` & `icepy4d-1.5.0/src/icepy4d/binned_stats.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/camera.py` & `icepy4d-1.5.0/src/icepy4d/classes/camera.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/dsm.py` & `icepy4d-1.5.0/src/icepy4d/classes/epoch.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/epoch.py` & `icepy4d-1.5.0/src/icepy4d/classes/ortophoto.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/features.py` & `icepy4d-1.5.0/src/icepy4d/classes/features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/images.py` & `icepy4d-1.5.0/src/icepy4d/classes/images.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/point_cloud.py` & `icepy4d-1.5.0/src/icepy4d/classes/point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/points.py` & `icepy4d-1.5.0/src/icepy4d/classes/points.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/solution.py` & `icepy4d-1.5.0/src/icepy4d/classes/solution.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/targets.py` & `icepy4d-1.5.0/src/icepy4d/classes/targets.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/classes/typed_dict_classes.py` & `icepy4d-1.5.0/src/icepy4d/classes/typed_dict_classes.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/build.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/build_windows_app.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/build_windows_app.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/bundler_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/clang_format_code.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/clang_format_code.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/crawl_camera_specs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/database.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/database.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_inlier_matches.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_inlier_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_bundler.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_to_bundler.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/export_to_visualsfm.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/flickr_downloader.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/flickr_downloader.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/h5_to_db.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/h5_to_db.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/merge_ply_files.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/merge_ply_files.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/nvm_to_ply.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/plyfile.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/plyfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_dense.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_dense.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_fused_vis.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/read_write_model.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/read_write_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/colmap_utils/visualize_model.py` & `icepy4d-1.5.0/src/icepy4d/io/colmap_utils/visualize_model.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2bundler.py` & `icepy4d-1.5.0/src/icepy4d/io/export2bundler.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2calge.py` & `icepy4d-1.5.0/src/icepy4d/io/export2calge.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2colmap.py` & `icepy4d-1.5.0/src/icepy4d/io/export2colmap.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/export2textfile.py` & `icepy4d-1.5.0/src/icepy4d/io/export2textfile.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/io/importing.py` & `icepy4d-1.5.0/src/icepy4d/io/importing.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/least_squares/rototra3d.py` & `icepy4d-1.5.0/src/icepy4d/least_squares/rototra3d.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/least_squares/utils.py` & `icepy4d-1.5.0/src/icepy4d/least_squares/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/match_by_preselection.py` & `icepy4d-1.5.0/src/icepy4d/matching/match_by_preselection.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/match_pairs.py` & `icepy4d-1.5.0/src/icepy4d/matching/match_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/matching_base.py` & `icepy4d-1.5.0/src/icepy4d/matching/matching_base.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/retrieve_matches_from_npz.py` & `icepy4d-1.5.0/src/icepy4d/matching/retrieve_matches_from_npz.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_match_simple_old.py` & `icepy4d-1.5.0/src/icepy4d/matching/superglue_match_simple_old.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_matcher.py` & `icepy4d-1.5.0/src/icepy4d/matching/superglue_matcher.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/superglue_tracker.py` & `icepy4d-1.5.0/src/icepy4d/matching/superglue_tracker.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/templatematch.py` & `icepy4d-1.5.0/src/icepy4d/matching/templatematch.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/track_matches.py` & `icepy4d-1.5.0/src/icepy4d/matching/track_matches.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/track_matches_bk.py` & `icepy4d-1.5.0/src/icepy4d/matching/track_matches_bk.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/tracking_base.py` & `icepy4d-1.5.0/src/icepy4d/matching/tracking_base.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/matching/utils.py` & `icepy4d-1.5.0/src/icepy4d/matching/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/metashape/metashape.py` & `icepy4d-1.5.0/src/icepy4d/metashape/metashape.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/metashape/ms_utils.py` & `icepy4d-1.5.0/src/icepy4d/metashape/ms_utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py` & `icepy4d-1.5.0/src/icepy4d/point_cloud_proc/cloudcompare_fun.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/open3d_fun.py` & `icepy4d-1.5.0/src/icepy4d/point_cloud_proc/open3d_fun.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/point_cloud_proc/utils.py` & `icepy4d-1.5.0/src/icepy4d/point_cloud_proc/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/absolute_orientation.py` & `icepy4d-1.5.0/src/icepy4d/sfm/absolute_orientation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/geometry.py` & `icepy4d-1.5.0/src/icepy4d/sfm/geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/interpolate_colors.py` & `icepy4d-1.5.0/src/icepy4d/sfm/interpolate_colors.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/reconstruction.py` & `icepy4d-1.5.0/src/icepy4d/sfm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/triangulation.py` & `icepy4d-1.5.0/src/icepy4d/sfm/triangulation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/sfm/two_view_geometry.py` & `icepy4d-1.5.0/src/icepy4d/sfm/two_view_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/match_pairs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superglue.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/SuperGluePretrainedNetwork/models/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/templatematch_pyimgraft.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/transformations.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/transformations.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/thirdparty/triangulation.py` & `icepy4d-1.5.0/src/icepy4d/thirdparty/triangulation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/tiles.py` & `icepy4d-1.5.0/src/icepy4d/tiles.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/tracking_features_utils.py` & `icepy4d-1.5.0/src/icepy4d/tracking_features_utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/dsm_orthophoto.py` & `icepy4d-1.5.0/src/icepy4d/utils/dsm_orthophoto.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/initialization.py` & `icepy4d-1.5.0/src/icepy4d/utils/initialization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/logger.py` & `icepy4d-1.5.0/src/icepy4d/utils/logger.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/rototranslation.py` & `icepy4d-1.5.0/src/icepy4d/utils/rototranslation.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/sensor_width_database.py` & `icepy4d-1.5.0/src/icepy4d/utils/sensor_width_database.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/spatial_funs.py` & `icepy4d-1.5.0/src/icepy4d/utils/spatial_funs.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/timer.py` & `icepy4d-1.5.0/src/icepy4d/utils/timer.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/utils/utils.py` & `icepy4d-1.5.0/src/icepy4d/utils/utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/visualization/vis_o3d_advanced.py` & `icepy4d-1.5.0/src/icepy4d/visualization/vis_o3d_advanced.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d/visualization/visualization.py` & `icepy4d-1.5.0/src/icepy4d/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/src/icepy4d.egg-info/PKG-INFO` & `icepy4d-1.5.0/src/icepy4d.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: icepy4d
-Version: 1.4.0
+Version: 1.5.0
 Summary: 4D Image-based Continuos monitoring of glaciers Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>
-License: MIT License
+License: BSD 3-Clause License
         
-        Copyright (c) 2022 Francesco Ioli
+        Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
+        All rights reserved.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/franioli/icepy4d
 Keywords: sfm,4d-reconstruction,glaciers,deep-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -37,84 +45,54 @@
 
 # Welcome to ICEpy4D
 
 4D Image-based Continuos monitoring of glaciers' Evolution with low-cost stereo-cameras and Deep Learning photogrammetry.
 
 `ICEpy4D` is a under active development.
 
-## Installation guide
-
-##### Requirements
+## Requirements
 
 - 64-bit Python `>= 3.8` but `< 3.10`
 - a NVIDIA graphic card with CUDA capability is strongly reccomended.
 
-##### Create Anaconda environment
-
-```bash
-conda create -n icepy4d python=3.8
-conda activate icepy4d
-```
-
-##### Install gdal for raster manipulation
-
-First, install `gdal`, which is required for building and manipulating orthophotos and DSMs. As the dependacies of `gdal`, are quite strict, it is suggested to install it first with conda. If you don't intend to build orthophotos and DSM, you can skip this step (be careful to remove rasterio from requirements.txt as well in order to avoid unsatisfied dependencies).
-
-```bash
-conda update -n base -c conda-forge conda
-conda install -c conda-forge gdal
-```
-
-Check that `gdal` is correctly installed with:
-
-```bash
-python -c "from osgeo import gdal"
-```
-
-##### Install Pytorch
+## Installation guide
 
-Install pythorch following the official guidelines (<https://pytorch.org/get-started/locally/>). Be careful to select the correct CUDA version as that installed on your system.
+Create a new Anaconda environment
 
 ```bash
-pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu116
-
+conda create -n icepy4d python=3.9
+conda activate icepy4d
 ```
 
-##### Install other required packages
+Install Icepy4D from PyPi repository
 
 ```bash
-pip3 install -r requirements.txt
+pip install icepy4d
 ```
 
-##### Various
-
-- If you intend to use Jupyter Notebooks for running main scripts, install jupyterlab with
+Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
+Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).
 
 ```bash
-pip3 install jupyterlab
+wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
+pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
 ```
 
-- When using VScode and Matplotlib, use TkAgg as interactive backend.
+You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)
 
-##### Install ICEpy4D
-
-Install ICEpy4D package by running from the root folder
-
-```bash
-pip install -e .
-```
-
-and try to import it
+Try to import ICEpy4D package
 
 ```bash
 conda activate icepy4d
 python -c "import icepy4d"
 ```
 
-If no error is given, ICEpy4D is successfully installed and it can be imported with `import icepy4d`
+If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
+
+### For contributing
 
+Install additional requirements for development:
 
-#### For contributing
-`bash
+```bash
 pip install -r requirements-dev.txt
 pre-commit install
-`
+```
```

### Comparing `icepy4d-1.4.0/src/icepy4d.egg-info/SOURCES.txt` & `icepy4d-1.5.0/src/icepy4d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_features.py` & `icepy4d-1.5.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_image.py` & `icepy4d-1.5.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_initialization.py` & `icepy4d-1.5.0/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_matching.py` & `icepy4d-1.5.0/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_point_cloud.py` & `icepy4d-1.5.0/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_sfm_geometry.py` & `icepy4d-1.5.0/tests/test_sfm_geometry.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_utils.py` & `icepy4d-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `icepy4d-1.4.0/tests/test_utils_spatial.py` & `icepy4d-1.5.0/tests/test_utils_spatial.py`

 * *Files identical despite different names*

