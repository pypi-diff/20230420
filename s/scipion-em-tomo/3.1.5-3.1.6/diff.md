# Comparing `tmp/scipion-em-tomo-3.1.5.tar.gz` & `tmp/scipion-em-tomo-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomo-3.1.5.tar", last modified: Thu Mar 30 08:44:52 2023, max compression
+gzip compressed data, was "scipion-em-tomo-3.1.6.tar", last modified: Thu Apr 20 14:35:09 2023, max compression
```

## Comparing `scipion-em-tomo-3.1.5.tar` & `scipion-em-tomo-3.1.6.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.747563 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 08:44:52.000000 scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.751562 scipion-em-tomo-3.1.5/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.751562 scipion-em-tomo-3.1.5/tomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/convert/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    98681 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/tomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_assignTransformationTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_assign_tomo2subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_assign_tomo2tomoMask.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_consensus_classes_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ctf_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_extract_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_coordinates_from_scipion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_tomomasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_misalignTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_particles_to_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_rotate_astigmatism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_split_evenodd_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_tomo_to_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_consensus_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_convert_coords3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22389 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_correct_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/tomo/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/templates/HIV-Picking-with-Dynamo.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/templates/HIV-Reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/templates/HIV-Subtomogram-averaging.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/templates/Membrane picking-with-PySeg.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/tomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_base_centralized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)    40917 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    43285 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_tomo_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:44:52.755563 scipion-em-tomo-3.1.5/tomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/viewer_split_evenodd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/viewer_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-30 08:38:39.000000 scipion-em-tomo-3.1.5/tomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/tomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99969 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assignTransformationTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2tomoMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_consensus_classes_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ctf_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_extract_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates_from_scipion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomomasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_misalignTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_particles_to_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_rotate_astigmatism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_split_evenodd_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_tomo_to_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_consensus_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_convert_coords3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_correct_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Picking-with-Dynamo.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Subtomogram-averaging.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/Membrane picking-with-PySeg.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_base_centralized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_fit_vesicles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_tomo_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/viewer_split_evenodd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/wizards.py
```

### Comparing `scipion-em-tomo-3.1.5/LICENSE` & `scipion-em-tomo-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/PKG-INFO` & `scipion-em-tomo-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.5
+Version: 3.1.6
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.5/README.rst` & `scipion-em-tomo-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/PKG-INFO` & `scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.5
+Version: 3.1.6
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.5/scipion_em_tomo.egg-info/SOURCES.txt` & `scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 tomo/protocols/protocol_assign_tomo2subtomo.py
 tomo/protocols/protocol_assign_tomo2tomoMask.py
 tomo/protocols/protocol_base.py
 tomo/protocols/protocol_compose_TS.py
 tomo/protocols/protocol_consensus_classes_subtomo.py
 tomo/protocols/protocol_ctf_validate.py
 tomo/protocols/protocol_extract_coordinates.py
+tomo/protocols/protocol_fit_ellipsoid.py
 tomo/protocols/protocol_import_coordinates.py
 tomo/protocols/protocol_import_coordinates_from_scipion.py
 tomo/protocols/protocol_import_subtomograms.py
 tomo/protocols/protocol_import_tomograms.py
 tomo/protocols/protocol_import_tomomasks.py
 tomo/protocols/protocol_misalignTS.py
 tomo/protocols/protocol_particles_to_subtomograms.py
@@ -47,17 +48,17 @@
 tomo/templates/HIV-Reconstruction.json.template
 tomo/templates/HIV-Subtomogram-averaging.json.template
 tomo/templates/Membrane picking-with-PySeg.json.template
 tomo/templates/Ribosomes-Subtomogram-averaging.json.template
 tomo/tests/__init__.py
 tomo/tests/test_base_centralized_layer.py
 tomo/tests/test_compose_TS.py
+tomo/tests/test_fit_vesicles.py
 tomo/tests/test_import.py
 tomo/tests/test_objects.py
 tomo/tests/test_tomo_base.py
 tomo/tests/test_transformations.py
 tomo/viewers/__init__.py
 tomo/viewers/viewer_split_evenodd.py
-tomo/viewers/viewer_tomograms.py
 tomo/viewers/viewers_data.py
 tomo/viewers/views.py
 tomo/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-tomo-3.1.5/setup.py` & `scipion-em-tomo-3.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/__init__.py` & `scipion-em-tomo-3.1.6/tomo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
-__version__ = '3.1.5'
+__version__ = '3.1.6'
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwem.Plugin):
     @classmethod
     def _defineVariables(cls):
```

### Comparing `scipion-em-tomo-3.1.5/tomo/constants.py` & `scipion-em-tomo-3.1.6/tomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/convert/convert.py` & `scipion-em-tomo-3.1.6/tomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/convert/mdoc.py` & `scipion-em-tomo-3.1.6/tomo/convert/mdoc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/icon.png` & `scipion-em-tomo-3.1.6/tomo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/objects.py` & `scipion-em-tomo-3.1.6/tomo/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 
 class Tomogram(data.Volume):
     """ Class to hold the tomogram abstraction inside Scipion. The origin (self._origin) of the volume is set as the
     location of the first coordinate loaded from the binary file. The volume may be displaced by setting a different
     origin using the methods implemented in the inherited class data.Image in scipion-em plugin.
     """
     TS_ID_FIELD = '_tsId'
-
+    ORIGIN_MATRIX_FIELD = '_origin._matrix'
     def __init__(self, **kwargs):
         data.Volume.__init__(self, **kwargs)
         self._acquisition = None
         self._tsId = String(kwargs.get('tsId', None))
         self._dim = None
 
     def getTsId(self):
@@ -1327,33 +1327,40 @@
         """Return the vector that can be used to move the position of the Coordinate3D
         (referred to the center of the Tomogram or other origin specified by the user)
         to the bottom left corner of the Tomogram
         """
         vol = self.getVolume()
         if not vol:
             raise Exception("3D coordinate must be referred to a volume to get its origin.")
+
+        # Tomogram origin
+        origin = vol.getShiftsFromOrigin()
+
         if angstrom:
-            return vol.getShiftsFromOrigin()
+            return origin
         else:
             sr = vol.getSamplingRate()
-            origin = vol.getShiftsFromOrigin()
+
             return origin[0] / sr, origin[1] / sr, origin[2] / sr
 
     def getTomoId(self):
         return self._tomoId.get()
 
     def setTomoId(self, tomoId):
         self._tomoId.set(tomoId)
 
     def composeCoordId(self, sampligRate):
         return "%s,%s,%s,%s" % (self.getTomoId(),
                                 int(sampligRate * self._x.get()),
                                 int(sampligRate * self._y.get()),
                                 int(sampligRate * self._z.get()))
 
+    def __str__(self):
+        return "%s, G%s" % (self.composeCoordId(1), self.getGroupId())
+
 
 class SetOfCoordinates3D(data.EMSet):
     """ Encapsulate the logic of a set of volumes coordinates.
     Each coordinate has a (x,y,z) position and is related to a Volume
     The SetOfCoordinates3D can also have information about TiltPairs.
     """
     ITEM_TYPE = Coordinate3D
@@ -1389,15 +1396,15 @@
         return self.getPrecedents()
 
     def iterVolumeCoordinates(self, volume):
         """ Iterates over the set of coordinates belonging to that micrograph.
         """
         pass
 
-    def iterCoordinates(self, volume: Tomogram = None, orderBy='id'):
+    def iterCoordinates(self, volume: Tomogram = None, orderBy='id') -> Coordinate3D:
         """ Iterate over the coordinates associated with a tomogram.
         If volume=None, the iteration is performed over the whole
         set of coordinates.
 
         IMPORTANT NOTE: During the storing process in the database, Coordinates3D will lose their
         pointer to ther associated Tomogram. This method overcomes this problem by retrieving and
         relinking the Tomogram as if nothing would ever happened.
@@ -1411,31 +1418,53 @@
             >>>     print(coord.getVolName())
             >>>     Error: Tomogram associated to Coordinate3D is NoneType (pointer lost)
             >>> for coord in coordSet.iterCoordinates()
             >>>     print(coord.getVolName())
             >>>     '/path/to/Tomo.file' retrieved correctly
 
         """
+
+        # Iterate over all coordinates if tomoId is None,
+        # otherwise use tomoId to filter the where selection
         if volume is None:
             coordWhere = '1'
         elif isinstance(volume, int):
-            coordWhere = '_volId=%d' % int(volume)
-        elif isinstance(volume, data.Volume):
+            logger.warning("FOR DEVELOPERS: Do not use volId, use volName")
+            coordWhere = '_volId=%d' % volume
+        elif isinstance(volume, Tomogram):
             coordWhere = '%s="%s"' % (Coordinate3D.TOMO_ID_ATTR, volume.getTsId())
         else:
             raise Exception('Invalid input tomogram of type %s'
                             % type(volume))
 
+
         # Iterate over all coordinates if tomoId is None,
         # otherwise use tomoId to filter the where selection
-        tomos = self.getPrecedentsInvolved()
         for coord in self.iterItems(where=coordWhere, orderBy=orderBy):
-            coord.setVolume(tomos[coord.getTomoId()])
+            # Associate the tomogram
+            self._associateVolume(coord)
             yield coord
 
+    def _getTomogram(self, tsId):
+        """ Returns  the tomogram from a tsId"""
+        tomos = self._getTomograms()
+
+        if tsId not in tomos.keys():
+            tomo = self.getPrecedents()[{Tomogram.TS_ID_FIELD: tsId}]
+            self._tomos[tsId] = tomo
+            return tomo
+        else:
+            return self._tomos[tsId]
+
+    def _getTomograms(self):
+        if self._tomos is None:
+            self.initTomos()
+
+        return self._tomos
+
     def getPrecedents(self):
         """ Returns the SetOfTomograms associated with
                 this SetOfCoordinates"""
         return self._precedentsPointer.get()
 
     def getPrecedent(self, tomoId):
         return self.getPrecedentsInvolved()[tomoId]
@@ -1479,47 +1508,43 @@
         s = "%s (%d items, %s, %s Å/px%s)" % (self.getClassName(), self.getSize(), boxStr,
                                               self.getSamplingRate(), self._appendStreamState())
 
         return s
 
     def getFirstItem(self):
         coord = data.EMSet.getFirstItem(self)
-        coord.setVolume(self.getPrecedents()[coord.getVolId()])
+        self._associateVolume(coord)
         return coord
 
+    def _associateVolume(self, coord):
+        coord.setVolume(self._getTomogram(coord.getTomoId()))
+
     def __getitem__(self, itemId):
         """Add a pointer to a Tomogram before returning the Coordinate3D"""
         coord = data.EMSet.__getitem__(self, itemId)
-        # In case pointer is lost in a for loop
-        # clone = self.getPrecedents().getClass()()
-        # clone.copy(self)
-        # coord.setVolume(clone[coord.getVolId()])
-        coord.setVolume(self.getPrecedents()[coord.getVolId()])
+        self._associateVolume(coord)
         return coord
 
     def initTomos(self):
         """ Initialize internal _tomos to a dictionary if not done already"""
         if self._tomos is None:
             self._tomos = dict()
 
     def getPrecedentsInvolved(self):
         """ Returns a list  with only the tomograms involved in the subtomograms. May differ when
         subsets are done."""
 
         tomoId_attr = Coordinate3D.TOMO_ID_ATTR
-        if self._tomos is None:
 
-            self.initTomos()
-
-            uniqueTomos = self.aggregate(['count'], tomoId_attr, [tomoId_attr])
+        uniqueTomos = self.aggregate(['count'], tomoId_attr, [tomoId_attr])
 
-            for row in uniqueTomos:
-                tsId = row[tomoId_attr]
-                tomo = self.getPrecedents()[{Tomogram.TS_ID_FIELD: tsId}]
-                self._tomos[tsId] = tomo
+        for row in uniqueTomos:
+            tsId = row[tomoId_attr]
+            # This should register the tomogram in the internal _tomos
+            self._getTomogram(tsId)
 
         return self._tomos
 
     def append(self, item: Coordinate3D):
         if self.getBoxSize() is None and item._boxSize:
             self.setBoxSize(item._boxSize)
         super().append(item)
@@ -1528,29 +1553,32 @@
 class SubTomogram(data.Volume):
     """The coordinate associated to each subtomogram is not scaled. To do that, the coordinates and the subtomograms
     sampling rates should be compared (because of how the extraction protocol works). But when shifts are applied to
     the coordinates, it has to be considered that if we're operating with coordinates coming from subtomogrmas, those
     shifts will be scaled, but if the coordinates come from coordinates, they won't be."""
 
     VOL_NAME_FIELD = "_volName"
+    COORD_VOL_NAME_FIELD = "_coordinate.%s" % Coordinate3D.TOMO_ID_ATTR
     def __init__(self, **kwargs):
         data.Volume.__init__(self, **kwargs)
         self._acquisition = None
         self._volId = Integer()
+        # This coordinate is NOT SCALED. To do that, the coordinates and subtomograms sampling rates
+        # should be compared (because of how the extraction protocol works)
         self._coordinate = None
         self._volName = String()
 
     def hasCoordinate3D(self):
         return self._coordinate is not None
 
     def setCoordinate3D(self, coordinate):
         self._coordinate = coordinate
         self.setVolId(coordinate.getVolId())
 
-    def getCoordinate3D(self):
+    def getCoordinate3D(self)->Coordinate3D:
         """Since the object Coordinate3D needs a volume, use the information stored in the
         SubTomogram to reconstruct the corresponding Tomogram associated to its Coordinate3D"""
         # We do not do this here but in the set iterator tha will "plug" the volume (tomogram) is exists
         # tomo = Tomogram()
         # subtomoOrigin = self.getOrigin()
         # if subtomoOrigin:
         #     tomo.setOrigin(subtomoOrigin)
@@ -1619,15 +1647,15 @@
             matrix = np.eye(4)
         else:
             matrix = newTransform.getMatrix()
         newTransform.setMatrix(convertMatrix(matrix, direction=const.SET, convention=convention))
         self._transform = newTransform
 
     def getTransform(self, convention=None):
-        
+
         if convention is not None:
             matrix = self._transform.getMatrix()
             return Transform(convertMatrix(matrix, direction=const.GET, convention=convention))
         else:
             return self._transform
 
 class SetOfSubTomograms(data.SetOfVolumes):
@@ -1661,15 +1689,25 @@
         this set of particles.
          """
         if isinstance(coordinates, Pointer):
             self._coordsPointer = coordinates
         else:
             self._coordsPointer.set(coordinates)
 
-    def iterSubtomos(self, volume=None, orderBy='id'):
+    def iterCoordinates(self, volume: Tomogram = None, orderBy='id') -> Coordinate3D:
+        """ Mimics SetOfCoordinates.iterCoordinates so can be passed to viewers or protocols transparently"""
+        if self.hasCoordinates3D():
+            for subtomo in self.iterSubtomos(volume, orderBy=orderBy):
+                coord = subtomo.getCoordinate3D()
+                coord.setObjId(subtomo.getObjId())
+                yield coord
+        else:
+            yield
+
+    def iterSubtomos(self, volume: Tomogram =None, orderBy='id')->SubTomogram:
         """ Iterates over the sutomograms, enriching them with the related tomogram if apply so coordinate getters and setters will work
         If volume=None, the iteration is performed over the whole
         set of subtomograms.
 
         IMPORTANT NOTE: During the storing process in the database, Coordinates3D will lose their
         pointer to the associated Tomogram. This method overcomes this problem by retrieving and
         relinking the Tomogram as if nothing would ever happend.
@@ -1683,28 +1721,27 @@
             >>>     print(subtomo.getCoordinate3D().getX(SCIPION))
             >>>     Error: Tomogram associated to Coordinate3D is NoneType (pointer lost)
             >>> for subtomo in subtomos.iterSubtomos()
             >>>     print(subtomo.getCoordinate3D().getX(SCIPION))
             >>>     330 retrieved correctly
 
         """
+        # Iterate over all Subtomograms if tomoId is None,
+        # otherwise use tomoId to filter the where selection
         if volume is None:
-            volId = None
+            subtomoWhere = '1'
         elif isinstance(volume, int):
-            volId = volume
-        elif isinstance(volume, data.Volume):
-            volId = volume.getObjId()
+            logger.warning("FOR DEVELOPERS: Do not use volId, use volName or tsId")
+            subtomoWhere = '_volId=%d' % volume
+        elif isinstance(volume, Tomogram):
+            subtomoWhere = '%s="%s"' % (SubTomogram.VOL_NAME_FIELD, volume.getTsId())
         else:
             raise Exception('Invalid input tomogram of type %s'
                             % type(volume))
 
-        # Iterate over all coordinates if tomoId is None,
-        # otherwise use tomoId to filter the where selection
-        subtomoWhere = '1' if volId is None else '_volId=%d' % int(volId)
-
         for subtomo in self.iterItems(where=subtomoWhere, orderBy=orderBy):
             if subtomo.hasCoordinate3D():
                 subtomo.getCoordinate3D().setVolume(self.getTomogram(subtomo))
             yield subtomo
 
     def getTomogram(self, subtomo):
         """ returns and caches the tomogram related with a subtomogram.
@@ -1720,18 +1757,16 @@
         # Else, there are coordinates
         volId = coord.getVolId()
         tsId = coord.getTomoId()
 
         self.initTomos()
 
         # If tsId is not cached, save both identifiers.
-        # NOTE: In streaming cases this may have to be different.
-        # We might not use volId at all and query precedents by tsId.
         if tsId not in self._tomos:
-            tomo = self.getCoordinates3D().getPrecedents()[volId]
+            tomo = self.getCoordinates3D().getPrecedents()[{Tomogram.TS_ID_FIELD: tsId}]
             self._tomos[volId] = tomo
             self._tomos[tsId] = tomo
             return tomo
         else:
             return self._tomos[tsId]
 
     def initTomos(self):
@@ -1739,15 +1774,15 @@
         if self._tomos is None:
             self._tomos = dict()
 
     def getTomograms(self):
         """ Returns a list  with only the tomograms involved in the subtomograms. May differ when
         subsets are done."""
 
-        tomoId_attr = "_coordinate." + Coordinate3D.TOMO_ID_ATTR
+        tomoId_attr = SubTomogram.COORD_VOL_NAME_FIELD
         if self._tomos is None:
 
             self.initTomos()
 
             uniqueTomos = self.aggregate(['count'], tomoId_attr, [tomoId_attr])
 
             for row in uniqueTomos:
@@ -1984,24 +2019,24 @@
         else:
             self._setOfTiltSeriesPointer.set(setOfTiltSeries)
 
 
 class MeshPoint(Coordinate3D):
     """Mesh object: it stores the coordinates of the points (specified by the user) needed to define
     the triangulation of a volume.
-    A Mesh object can be consider as a point cloud in 3D containing the coordinates needed to divide a given region of
+    A Mesh object can be considered as a point cloud in 3D containing the coordinates needed to divide a given region of
     space into planar triangles interconnected that will result in a closed surface."""
 
     def __init__(self, **kwargs):
         Coordinate3D.__init__(self, **kwargs)
         self._volumeName = String()
         self._description = None  # Algebraic description of fitted mesh
 
     def getVolumeName(self):
-        return self._volumeName
+        return self._volumeName.get()
 
     def setVolumeName(self, volName):
         self._volumeName.set(volName)
 
     def getDescription(self):
         return self._description
 
@@ -2364,15 +2399,15 @@
         data.EMSet.__init__(self, **kwargs)
         self._tiltSeriesPointer = Pointer(kwargs.get('tiltSeriesPointer', None))
         self._tsId = String(kwargs.get('tsId', None))
         self._isDefocusUDeviationInRange = Boolean(True)
         self._isDefocusVDeviationInRange = Boolean(True)
 
         # CtfModels will always be used inside a SetOfTiltSeries
-        # so, let's do no store the mapper path by default
+        # so, let's do not store the mapper path by default
         self._mapperPath.setStore(False)
 
     def clone(self, ignoreAttrs=('_mapperPath', '_size')):
         clone = self.getClass()()
         clone.copy(self, ignoreAttrs=ignoreAttrs)
         clone.setEnabled(self.isEnabled())
         return clone
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/__init__.py` & `scipion-em-tomo-3.1.6/tomo/protocols/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,7 +44,8 @@
 from .protocol_ctf_validate import ProtCTFTomoSeriesValidate
 from .protocol_particles_to_subtomograms import Prot2DParticlesToSubtomograms
 from .protocol_rotate_astigmatism import ProtRotateAstigmatism
 from .protocol_tomo_to_mics import ProtTomoToMics, Prot2DcoordsTo3DCoords
 from .protocol_ts_convert_coords3d import ProtTsConvertCoordinates3d
 from .protocol_compose_TS import ProtComposeTS
 from .protocol_misalignTS import ProtTomoMisalignTiltSeries
+from .protocol_fit_ellipsoid import TomoProtFitEllipsoid, XmippProtFitEllipsoid
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_alignment_assign.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_assignTransformationTS.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assignTransformationTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_assign_tomo2subtomo.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_assign_tomo2tomoMask.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2tomoMask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_base.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_compose_TS.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_compose_TS.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     _devStatus = pw.BETA
     _label = 'Compose Tilt Serie'
 
     def __init__(self, **args):
         ProtImport.__init__(self, **args)
         self.stepsExecutionMode = STEPS_PARALLEL  # Defining that the protocol contain parallel steps
         self.newSteps = []
+        self.listMdocsRead = []
         self.TiltSeries = None
+        self.waitingMdoc = True
         self.time4NextTS_current = time.time()
 
     # -------------------------- DEFINES AND STEPS -----------------------
     def _defineParams(self, form):
         form.addSection(label='Import')
 
         form.addParam('inputMicrographs', params.PointerParam,
@@ -107,18 +109,17 @@
                            "The default value is  high (30 min) to "
                            "avoid the protocol finishes during the acq of the "
                            "microscope. You can also stop it from right click "
                            "and press STOP_STREAMING.\n")
         form.addParallelSection(threads=3, mpi=1)
 
     def _initialize(self):
-        self.listMdocsRead = []
+
         self.time4NextTS_current = time.time()
         self.ih = ImageHandler()
-        self.waitingMdoc = True
 
     def _insertAllSteps(self):
         self._insertFunctionStep(self._initialize)
         self.CloseStep_ID = self._insertFunctionStep('closeSet',
                                                      prerequisites=[],
                                                      wait=True)
         self.newSteps.append(self.CloseStep_ID)
@@ -268,15 +269,17 @@
         list_mics_matched = []
         for x, mic in enumerate(self.listOfMics):
             if mic.getMicName() in list_mdoc_files:
                 list_mics_matched.append(mic)
         self.listOfMics = list_mics_matched
 
         if len(self.listOfMics) != len(mdoc_order_angle_list):
-            self.error('Micrographs doesnt match with mdoc read')
+            self.error('Micrographs doesnt match with mdoc read.\n'
+                      'number of mics: {}, number of mics on mdoc: {}'.format(
+                len(self.listOfMics), len(mdoc_order_angle_list)))
             return False
         else:
             self.info('Micrographs matched for the mdoc file: {}'.format(
                 len(self.listOfMics)))
             return True
 
     def _loadInputList(self):
@@ -328,14 +331,16 @@
         ts_obj = tomoObj.TiltSeries()
         len_ac = Integer(len(file_ordered_angle_list))
         ts_obj.setAnglesCount(len_ac)
         ts_obj.setTsId(mdoc_obj.getTsId())
         acq = ts_obj.getAcquisition()
         acq.setVoltage(mdoc_obj.getVoltage())
         acq.setMagnification(mdoc_obj.getMagnification())
+        acq.setSphericalAberration(self.listOfMics[0].getAcquisition().getSphericalAberration())
+        acq.setAmplitudeContrast(self.listOfMics[0].getAcquisition().getAmplitudeContrast())
         ts_obj.getAcquisition().setTiltAxisAngle(mdoc_obj.getTiltAxisAngle())
         origin = Transform()
         ts_obj.setOrigin(origin)
         SOTS.append(ts_obj)
 
         self.setingTS(SOTS, ts_obj, file_ordered_angle_list,
                       incoming_dose_list, accumulated_dose_list)
@@ -358,14 +363,21 @@
         :param incoming_dose_list: list of dose
         :param accumulated_dose_list: list of accumulated dose
         :return:
         """
         ts_fn = self._getOutputTiltSeriesPath(ts_obj)
         ts_fn_dw = self._getOutputTiltSeriesPath(ts_obj, '_DW')
         counter_ti = 0
+
+        TSAngleFile = self._getPath("{}.rawtlt".format(ts_obj.getTsId()))
+        TSAngleFile = open(TSAngleFile, "a")
+        for n in file_ordered_angle_list:
+            TSAngleFile.write('{}\n'.format(str(n[2])))
+        TSAngleFile.close()
+
         for f, to, ta in file_ordered_angle_list:
             try:
                 for mic in self.listOfMics:
                     if ts_obj.getSamplingRate() is None:
                         ts_obj.setSamplingRate(mic.getSamplingRate())
                     if SOTS.getSamplingRate() is None:
                         SOTS.setSamplingRate(mic.getSamplingRate())
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_consensus_classes_subtomo.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_consensus_classes_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ctf_validate.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ctf_validate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_extract_coordinates.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_coordinates.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_coordinates_from_scipion.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates_from_scipion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_subtomograms.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_tomograms.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomograms.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,33 +22,36 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from os.path import abspath, basename
 
+from pwem import Ccp4Header
 from pwem.emlib.image import ImageHandler
 from pwem.objects import Transform
 from pyworkflow import BETA
 from pyworkflow.utils.path import createAbsLink, removeExt
 import pyworkflow.protocol.params as params
 
 from .protocol_base import ProtTomoImportFiles, ProtTomoImportAcquisition
-from ..objects import Tomogram
+from ..objects import Tomogram, SetOfTomograms
 from ..utils import _getUniqueFileName
 
 
+OUTPUT_NAME = 'Tomograms'
 class ProtImportTomograms(ProtTomoImportFiles, ProtTomoImportAcquisition):
     """Protocol to import a set of tomograms to the project"""
     _outputClassName = 'SetOfTomograms'
     _label = 'import tomograms'
     _devStatus = BETA
-
+    _possibleOutputs = {OUTPUT_NAME: SetOfTomograms}
     def __init__(self, **args):
         ProtTomoImportFiles.__init__(self, **args)
+        self.Tomograms = None
 
     def _defineParams(self, form):
         ProtTomoImportFiles._defineParams(self, form)
         ProtTomoImportAcquisition._defineParams(self, form)
         form.addSection('Origin Info')
         form.addParam('setOrigCoord', params.BooleanParam,
                       condition='importFrom == IMPORT_FROM_FILES',
@@ -75,32 +78,37 @@
                            "symmetry regarding the origin of coordinates, "
                            "for example the protocol extract unit "
                            "cell, check carefully that the coordinates of the "
                            "origin preserve the symmetry of the whole volume. "
                            "This is particularly relevant for loading "
                            "fragments/subunits of the whole volume.\n",
                       default=False)
-        line = form.addLine('Offset',
+
+        form.addBooleanParam('fromMrcHeader', label='From mrc header',
+                        help='Use origin information in mrc headers of the tomograms.',
+                        default=False, condition='setOrigCoord', )
+
+        line = form.addLine('Manual offset',
                             help="A wizard will suggest you possible "
                                  "coordinates for the ORIGIN. In MRC volume "
                                  "files, the ORIGIN coordinates will be "
                                  "obtained from the file header.\n "
                                  "In case you prefer set your own ORIGIN "
                                  "coordinates, write them here. You have to "
                                  "provide the map center coordinates in "
                                  "Angstroms (pixels x sampling).\n",
-                            condition='setOrigCoord')
+                            condition='setOrigCoord and not fromMrcHeader')
         # line.addParam would produce a nicer looking form
         # but them the wizard icon is drawn outside the visible
         # window. Until this bug is fixed form is a better option
-        form.addParam('x', params.FloatParam, condition='setOrigCoord',
+        form.addParam('x', params.FloatParam, condition='setOrigCoord and not fromMrcHeader',
                       label="x", help="offset along x axis (Angstroms)")
-        form.addParam('y', params.FloatParam, condition='setOrigCoord',
+        form.addParam('y', params.FloatParam, condition='setOrigCoord and not fromMrcHeader',
                       label="y", help="offset along y axis (Angstroms)")
-        form.addParam('z', params.FloatParam, condition='setOrigCoord',
+        form.addParam('z', params.FloatParam, condition='setOrigCoord and not fromMrcHeader',
                       label="z", help="offset along z axis (Angstroms)")
 
     def _getImportChoices(self):
         """ Return a list of possible choices
         from which the import can be done.
         """
         return ['eman']
@@ -125,27 +133,42 @@
         imgh = ImageHandler()
 
         tomoSet = self._createSetOfTomograms()
         tomoSet.setSamplingRate(samplingRate)
 
         self._parseAcquisitionData()
         fileNameList = []
+
         for fileName, fileId in self.iterFiles():
-            x, y, z, n = imgh.getDimensions(fileName)
 
             origin = Transform()
 
-            if self.setOrigCoord.get():
-                origin.setShiftsTuple(self._getOrigCoord())
-            else:
+            def setDefaultOrigin():
+                x, y, z, n = imgh.getDimensions(fileName)
+
                 origin.setShifts(x / -2. * samplingRate,
                                  y / -2. * samplingRate,
                                  z / -2. * samplingRate)
 
-            tomo.setOrigin(origin)  # read origin from form
+            if self.setOrigCoord.get():
+
+                if self.fromMrcHeader.get():
+
+                    if Ccp4Header.isCompatible(fileName):
+                        ccp4Header = Ccp4Header(fileName, readHeader=True)
+                        origin.setShiftsTuple(ccp4Header.getOrigin())
+                    else:
+                        self.info("File %s not compatible with mrc format. Setting default origin: geometrical center of it." % fileName)
+                        setDefaultOrigin()
+                else:
+                    origin.setShiftsTuple(self._getOrigCoord())
+            else:
+                setDefaultOrigin()
+
+            tomo.setOrigin(origin)
 
             newFileName = basename(fileName).split(':')[0]
             if newFileName in fileNameList:
                 newFileName = _getUniqueFileName(self.getPattern(),
                                                  fileName.split(':')[0])
 
             fileNameList.append(newFileName)
@@ -154,53 +177,45 @@
             tomo.setTsId(tsId)
 
             if fileName.endswith(':mrc'):
                 fileName = fileName[:-4]
             createAbsLink(abspath(fileName), abspath(self._getExtraPath(newFileName)))
             tomo.setAcquisition(self._extractAcquisitionParameters(fileName))
 
-            if n == 1:  # One volume per file
-                tomo.cleanObjId()
-                tomo.setFileName(self._getExtraPath(newFileName))
-                tomoSet.append(tomo)
-            else:  # A stack of volumes per file (not common)
-                for index in range(1, n+1):
-                    tomo.cleanObjId()
-                    tomo.setLocation(index, self._getExtraPath(newFileName))
-                    tomoSet.append(tomo)
+            tomo.cleanObjId()
+            tomo.setFileName(self._getExtraPath(newFileName))
+            tomoSet.append(tomo)
 
-        self._defineOutputs(outputTomograms=tomoSet)
+        self._defineOutputs(**{OUTPUT_NAME:tomoSet})
 
     # --------------------------- UTILS functions ------------------------------
     def _getOrigCoord(self):
         return -1. * self.x.get(), -1. * self.y.get(), -1. * self.z.get()
 
     # --------------------------- INFO functions ------------------------------
     def _hasOutput(self):
-        return self.hasAttribute('outputTomograms')
+        return self.Tomograms is not None
 
     def _getTomMessage(self):
-        return "Tomograms %s" % self.getObjectTag('outputTomograms')
+        return "Tomograms %s" % self.getObjectTag(OUTPUT_NAME)
 
     def _summary(self):
 
         try:
             summary = []
             if self._hasOutput():
                 summary.append("%s imported from:\n%s"
                                % (self._getTomMessage(), self.getPattern()))
 
                 if self.samplingRate.get():
                     summary.append(u"Sampling rate: *%0.2f* (Å/px)" % self.samplingRate.get())
 
-                outputTomograms = getattr(self, 'outputTomograms')
-
-                ProtTomoImportAcquisition._summary(self, summary, outputTomograms)
+                ProtTomoImportAcquisition._summary(self, summary, self.Tomograms)
 
-                x, y, z = self.outputTomograms.getFirstItem().getShiftsFromOrigin()
+                x, y, z = self.Tomograms.getFirstItem().getShiftsFromOrigin()
                 summary.append(u"Tomograms Origin (x,y,z):\n"
                                u"    x: *%0.2f* (Å/px)\n"
                                u"    y: *%0.2f* (Å/px)\n"
                                u"    z: *%0.2f* (Å/px)" % (x, y, z))
 
         except Exception as e:
             print(e)
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_import_tomomasks.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomomasks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_misalignTS.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_misalignTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_particles_to_subtomograms.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_particles_to_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_rotate_astigmatism.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_rotate_astigmatism.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_split_evenodd_subtomos.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_split_evenodd_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_tomo_to_mics.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_tomo_to_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_base.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_consensus_alignment.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_consensus_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_convert_coords3d.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_convert_coords3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_correct_motion.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_correct_motion.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         line.addParam('cropDimX', params.IntParam, default=0, label='X')
         line.addParam('cropDimY', params.IntParam, default=0, label='Y')
 
         if self.evenOddCapable and addEvenOddParam:
             form.addParam('splitEvenOdd', params.BooleanParam,
                           default=False,
                           label='Split & sum odd/even frames?',
-                          expertLevel=params.LEVEL_ADVANCED,
                           help='(Used for denoising data preparation). If set to Yes, 2 additional movies/tilt '
                                'series will be generated, one generated from the even frames and the other from the '
                                'odd ones using the same alignment for the whole stack of frames.')
 
         form.addParallelSection(threads=4, mpi=1)
 
     # --------------------------- STEPS functions ----------------------------
@@ -221,18 +220,19 @@
 
         tsFn = self._getOutputTiltSeriesPath(ts)
         tsFnDW = self._getOutputTiltSeriesPath(ts, '_DW')
 
         # Merge all micrographs from the same tilt images in a single "mrcs" stack file
         for i, ti in enumerate(tiList):
             tiFn, tiFnDW = self._getOutputTiltImagePaths(ti)
-            newLocation = (i+1, tsFn)
-            ih.convert(tiFn, newLocation)
-            ti.setLocation(newLocation)
-            pw.utils.cleanPath(tiFn)
+            if os.path.exists(tiFn):
+                newLocation = (i+1, tsFn)
+                ih.convert(tiFn, newLocation)
+                ti.setLocation(newLocation)
+                pw.utils.cleanPath(tiFn)
             if os.path.exists(tiFnDW):
                 ih.convert(tiFnDW, (i+1, tsFnDW))
                 pw.utils.cleanPath(tiFnDW)
 
         self._tsDict.setFinished(tsId)
 
         # Even and odd stuff
@@ -296,15 +296,14 @@
             self.outputSetDW.append(tsObjDW)
 
             for i, ti in enumerate(tiList):
                 tiOut = TiltImage(location=(i+1, tsFnDW))
                 tiOut.copyInfo(ti, copyId=True)
                 tiOut.setAcquisition(ti.getAcquisition())
                 tiOut.setSamplingRate(self._getOutputSampling())
-                tiOut.setIndex(i+1)
                 tiOut.setObjId(ti.getIndex())
                 tsObjDW.append(tiOut)
 
             self.outputSetDW.update(tsObjDW)
 
     def createOutputStep(self):
         """" Overwrites the parent method to allow the creation of odd and even outputs"""
@@ -420,15 +419,14 @@
                 # index after having been sorted by angle previously, in order to avoid tilt image mismatching in
                 # another operations, such as the fiducial alignment, which expects the sqlite to be sorted that way
                 ti = tList[i]
                 tiOut = TiltImage(location=(counter, ti.getFileName()))
                 tiOut.copyInfo(ti, copyId=True)
                 tiOut.setAcquisition(ti.getAcquisition())
                 tiOut.setSamplingRate(self._getOutputSampling())
-                tiOut.setIndex(counter)
                 tiOut.setObjId(ti.getIndex())
                 ts.append(tiOut)
                 counter += 1
 
             outputSet.update(ts)
 
     # --------------------------- INFO functions ------------------------------
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_estimate_ctf.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols/protocol_ts_import.py` & `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -170,48 +170,14 @@
                            "*Absolute symlink*: Create symbolic links to the "
                            "absolute path of the files."
                            "*Relative symlink*: Create symbolic links as "
                            "relative path from the protocol run folder. ")
 
         self._defineAcquisitionParams(form)
 
-        form.addSection('Streaming')
-
-        form.addParam('dataStreaming', params.BooleanParam, default=False,
-                      label="Process data in streaming?",
-                      help="Select this option if you want import data as it "
-                           "is generated and process on the fly by next "
-                           "protocols. In this case the protocol will "
-                           "keep running to check new files and will "
-                           "update the output Set, which can "
-                           "be used right away by next steps.")
-
-        form.addParam('timeout', params.IntParam, default=43200,
-                      condition='dataStreaming',
-                      label="Timeout (secs)",
-                      help="Interval of time (in seconds) after which, "
-                           "if no new file is detected, the protocol will "
-                           "end. When finished, the output Set will be "
-                           "closed and no more data will be "
-                           "added to it. \n"
-                           "Note 1:  The default value is  high (12 hours) to "
-                           "avoid the protocol finishes during the acq of the "
-                           "microscope. You can also stop it from right click "
-                           "and press STOP_STREAMING.\n"
-                           "Note 2: If you're using individual frames when "
-                           "importing movies, the timeout won't be refreshed"
-                           "until a whole movie is stacked.")
-
-        form.addParam('fileTimeout', params.IntParam, default=30,
-                      condition='dataStreaming',
-                      label="File timeout (secs)",
-                      help="Interval of time (in seconds) after which, if a "
-                           "file has not changed, we consider it as a new "
-                           "file.\n")
-
         self._defineBlacklistParams(form)
 
     def _defineAngleParam(self, form):
         """ Used in subclasses to define the option to fetch tilt angles. """
         pass
 
     def _defineAcquisitionParams(self, form):
@@ -295,175 +261,123 @@
             for ts in outputSet:
                 self._existingTs.add(ts.getTsId())
 
         self._fillAcquisitionInfo(outputSet)
         tsClass = outputSet.ITEM_TYPE
         tiClass = tsClass.ITEM_TYPE
 
-        finished = False
-        lastDetectedChange = datetime.now()
+        if self._existingTs:
+            outputSet.enableAppend()
 
-        # Ignore the timeout variables if we are not really in streaming mode
-        if self.dataStreaming:
-            timeout = timedelta(seconds=self.timeout.get())
-            fileTimeout = timedelta(seconds=self.fileTimeout.get())
-        else:
-            timeout = timedelta(seconds=5)
-            fileTimeout = timedelta(seconds=5)
+        # Get files that matches the pattern via mdoc or not
+        matchingFiles = self.getMatchingFiles()
+
+        # Go through all of them
+        for ts, tiltSeriesList in matchingFiles.items():
 
-        while not finished:
-            time.sleep(3)  # wait 3 seconds before check for new files
-            someNew = False  # Check if some new TS has been found
-            someAdded = False  # Check if some new were added
-            # incompleteTs = False  # Check if there are incomplete TS
-
-            matchingFiles = self.getMatchingFiles(fileTimeOut=fileTimeout)
-
-            if self._existingTs:
-                outputSet.enableAppend()
-
-            for ts, tiltSeriesList in matchingFiles.items():
-                someNew = True
-                tsObj = tsClass(tsId=ts)
-                # Form value has higher priority than the mdoc values
-                samplingRate = \
-                    float(samplingRate if samplingRate else self.sRates[ts])
-
-                origin = Transform()
-                tsObj.setOrigin(origin)
-                tsObj.setAnglesCount(len(tiltSeriesList))
-                self.setItemExtraAttributes(tsObj)
-
-                # we need this to set mapper before adding any item
-                outputSet.append(tsObj)
-
-                if self.MDOC_DATA_SOURCE:
-                    accumDoseList = self.accumDoses[ts]
-                    # tsObj.getAcquisition().setAccumDose(accumDoseList[-1])
-                    incomingDoseList = self.incomingDose[ts]
-                    counter = 0
-
-                tiltSeriesObjList = []
-                toList = [ti[1] for ti in tiltSeriesList]
-                # Add tilt images to the tiltSeries
-                for f, to, ta in tiltSeriesList:
-                    try:
-                        # Link/move to extra
-                        if type(f) == tuple:
-                            imageFile = f[1]
-                        else:
-                            imageFile = f
-
-                        finalDestination = \
-                            self._getExtraPath(os.path.basename(imageFile))
-                        self.copyOrLink(imageFile, finalDestination)
-
-                        if type(f) == tuple:
-                            f = f[0], finalDestination
-                        else:
-                            f = finalDestination
-
-                        ti = tiClass(location=f,
-                                     acquisitionOrder=to,
-                                     tiltAngle=ta)
-
-                        ti.setAcquisition(tsObj.getAcquisition().clone())
-                        if self.MDOC_DATA_SOURCE:
-                            dosePerFrame = incomingDoseList[counter]
-                            accumDose = accumDoseList[counter]
-                        else:
-                            # Check if there are doses as a second column in the tlt file
-                            dosePerFrame = self.dosePerFrame.get()
-                            doses = []
-                            anglesFrom = self.getEnumText('anglesFrom')
-                            if anglesFrom == self.ANGLES_FROM_TLT:
-                                _, doses = self.getFromTlt(imageFile)
-                            if doses:
-                                accumDose = doses[counter]
-                            else:
-                                accumDose = \
-                                    self.dosePerFrame.get() * \
-                                    int(to if min(toList) == 1 else (int(to) + 1))
-
-                        # Incoming dose in current ti
-                        ti.getAcquisition().setDosePerFrame(dosePerFrame)
-                        # Accumulated dose in current ti
-                        ti.getAcquisition().setAccumDose(accumDose)
-                        tiltSeriesObjList.append(ti)
-                        counter += 1
-                    except OperationalError:
-                        raise Exception("%s is an invalid {TS} tag. "
-                                        "It must be an alpha-numeric sequence "
-                                        "(avoid symbols like -) that can not "
-                                        "start with a number." % ts)
-
-                # Sort tilt image metadata if importing tilt series
-                if not self._isImportingTsMovies():
-                    tiltSeriesObjList.sort(key=lambda x: x.getTiltAngle(),
-                                           reverse=False)
-
-                for ti in tiltSeriesObjList:
-                    tsObj.append(ti)
-
-                tsObjFirstItem = tsObj.getFirstItem()
-                origin.setShifts(-tsObjFirstItem.getXDim() / 2 * samplingRate,
-                                 -tsObjFirstItem.getYDim() / 2 * samplingRate,
-                                 0)
-
-                if self.MDOC_DATA_SOURCE:
-                    tsObj.getAcquisition().setAccumDose(accumDoseList[-1])
-                    # Tilt series object dose per frame has been updated each
-                    # time the tilt image dose per frame has
-                    # been updated before, so the mean value is used to be the
-                    # reference in the acquisition of the
-                    # whole tilt series movie
-                    tsObj.getAcquisition().setDosePerFrame(
-                        mean(incomingDoseList))
-                else:
-                    tsObj.getAcquisition().setDosePerFrame(
-                        self.dosePerFrame.get())
-                    tsObj.getAcquisition().setAccumDose(
-                        self.dosePerFrame.get() * len(tiltSeriesList))
-                    tsObj.getAcquisition().setTiltAxisAngle(
-                        self.tiltAxisAngle.get())
-
-                outputSet.update(tsObj)  # update items and size info
-                self._existingTs.add(ts)
-                someAdded = True
-
-            if someAdded:
-                self.debug('Updating output...')
-                self._updateOutputSet(self._outputName, outputSet,
-                                      state=outputSet.STREAM_OPEN)
-                self.debug('Update Done.')
-
-            self.debug('Checking if finished...someNew: %s' % someNew)
-
-            now = datetime.now()
-
-            if not someNew:
-                # If there are no new detected files, we should check the
-                # inactivity time elapsed (from last event to now) and
-                # if it is greater than the defined timeout, we conclude
-                # the import and close the output set
-                # Another option is to check if the protocol have some
-                # special stop condition, this can be used to manually stop
-                # some protocols such as import movies
-                finished = (now - lastDetectedChange > timeout
-                            or self.streamingHasFinished())
-                self.debug("Checking if finished:")
-                self.debug("   Now - Last Change: %s"
-                           % pwutils.prettyDelta(now - lastDetectedChange))
+            self.info("Tilt series found: %s" % ts)
+            someNew = True
+            tsObj = tsClass(tsId=ts)
+            # Form value has higher priority than the mdoc values
+            samplingRate = \
+                float(samplingRate if samplingRate else self.sRates[ts])
+
+            origin = Transform()
+            tsObj.setOrigin(origin)
+            tsObj.setAnglesCount(len(tiltSeriesList))
+            self.setItemExtraAttributes(tsObj)
+
+            # we need this to set mapper before adding any item
+            outputSet.append(tsObj)
+
+            if self.MDOC_DATA_SOURCE:
+                accumDoseList = self.accumDoses[ts]
+                incomingDoseList = self.incomingDose[ts]
+                counter = 0
+
+            tiltSeriesObjList = []
+
+            # Add each tilt images to the tiltSeries
+            for f, to, ta, dose in tiltSeriesList:
+                try:
+                    # Link/move to extra
+                    imageFile = f[1] if type(f) == tuple else f
+
+                    finalDestination = self._getExtraPath(os.path.basename(imageFile))
+                    self.copyOrLink(imageFile, finalDestination)
+
+                    f = (f[0], finalDestination) if type(f) == tuple else finalDestination
+
+                    ti = tiClass(location=f,
+                                 acquisitionOrder=to,
+                                 tiltAngle=ta)
+
+                    ti.setAcquisition(tsObj.getAcquisition().clone())
+
+                    # Calculate the dose
+                    if self.MDOC_DATA_SOURCE:
+                        dosePerFrame = incomingDoseList[counter]
+                        dose = accumDoseList[counter]
+                    else:
+                        dosePerFrame = self.dosePerFrame.get()
+
+                    # Incoming dose in current ti
+                    ti.getAcquisition().setDosePerFrame(dosePerFrame)
+                    # Accumulated dose in current ti
+                    ti.getAcquisition().setAccumDose(dose)
+                    tiltSeriesObjList.append(ti)
+                    counter += 1
+
+                except OperationalError:
+                    raise Exception("%s is an invalid {TS} tag. "
+                                    "It must be an alpha-numeric sequence "
+                                    "(avoid symbols like -) that can not "
+                                    "start with a number." % ts)
+
+            # Sort tilt image metadata if importing tilt series
+            if not self._isImportingTsMovies():
+                tiltSeriesObjList.sort(key=lambda x: x.getTiltAngle(),
+                                       reverse=False)
+
+            for ti in tiltSeriesObjList:
+                tsObj.append(ti)
+
+            tsObjFirstItem = tsObj.getFirstItem()
+            origin.setShifts(-tsObjFirstItem.getXDim() / 2 * samplingRate,
+                             -tsObjFirstItem.getYDim() / 2 * samplingRate,
+                             0)
+
+            if self.MDOC_DATA_SOURCE:
+                tsObj.getAcquisition().setAccumDose(accumDoseList[-1])
+                # Tilt series object dose per frame has been updated each
+                # time the tilt image dose per frame has
+                # been updated before, so the mean value is used to be the
+                # reference in the acquisition of the
+                # whole tilt series movie
+                tsObj.getAcquisition().setDosePerFrame(
+                    mean(incomingDoseList))
             else:
-                # If we have detected some files, we should update
-                # the timestamp of the last event
-                lastDetectedChange = now
-                finished = not self.isInStreaming()
+                tsObj.getAcquisition().setDosePerFrame(
+                    self.dosePerFrame.get())
+                tsObj.getAcquisition().setAccumDose(
+                    self.dosePerFrame.get() * len(tiltSeriesList))
+                tsObj.getAcquisition().setTiltAxisAngle(
+                    self.tiltAxisAngle.get())
+
+            outputSet.update(tsObj)  # update items and size info
+            self._existingTs.add(ts)
+            someAdded = True
+
+        if someAdded:
+            self.debug('Updating output...')
+            self._updateOutputSet(self._outputName, outputSet,
+                                  state=outputSet.STREAM_OPEN)
+            self.debug('Update Done.')
 
-            self.debug("Finished: %s" % finished)
+        self.debug('Checking if finished...someNew: %s' % someNew)
 
         # Close the output set
         self._updateOutputSet(self._outputName, outputSet,
                               state=outputSet.STREAM_CLOSED)
 
     # -------------------------- INFO functions -------------------------------
     def _summary(self):
@@ -645,14 +559,15 @@
             accumulatedDoseList = []
             incomingDoseList = []
             for tiltMetadata in mdocObj.getTiltsMetadata():
                 fileOrderAngleList.append((
                     tiltMetadata.getAngleMovieFile(),             # Filename
                     '{:03d}'.format(tiltMetadata.getAcqOrder()),  # Acquisition order
                     tiltMetadata.getTiltAngle(),                  # Tilt angle
+                    tiltMetadata.getAccumDose()                   # Accumulated dose
                 ))
                 accumulatedDoseList.append(tiltMetadata.getAccumDose())
                 incomingDoseList.append(tiltMetadata.getIncomingDose())
 
             # self._getTsIdFromMdocData(fileList)
             matchingFiles[tsId] = fileOrderAngleList
             self.acquisitions[tsId] = acquisition
@@ -661,15 +576,15 @@
             self.incomingDose[tsId] = incomingDoseList
 
         if isValidation:
             if matchingFiles:
                 if warningDetailedMsg:
                     self.skippedMdocs.set(skippedMdocs)
                     self._store(self.skippedMdocs)
-                    print(warningHeadMsg + ' '.join(warningDetailedMsg))
+                    self.info(warningHeadMsg + ' '.join(warningDetailedMsg))
                 return matchingFiles
             else:
                 raise Exception(warningHeadMsg + ' '.join(warningDetailedMsg))
         else:
             return matchingFiles
 
     def _isImportingTsMovies(self):
@@ -705,68 +620,73 @@
                 print("%s excluded. Contains any of %s" %
                       (file, exclusionWords))
                 continue
             allowedFiles.append(file)
 
         return allowedFiles
 
-    def getMatchingFiles(self, fileTimeOut=None, isValidation=False):
+    def getMatchingFiles(self, isValidation=False):
         """ Return an ordered dict with TiltSeries found in the files as key
         and a list of all tilt images of that series as value.
         """
         if self.MDOC_DATA_SOURCE:
             return self._getMatchingFilesFromMdoc(isValidation=isValidation)
         else:
-            return self._getMatchingFilesFromRegExPattern(
-                fileTimeOut=fileTimeOut)
+            return self._getMatchingFilesFromRegExPattern()
 
-    def _getMatchingFilesFromRegExPattern(self, fileTimeOut):
+    def _getMatchingFilesFromRegExPattern(self):
         filePaths = glob(self._globPattern)
 
         filePaths = self._excludeByWords(filePaths)
 
         filePaths.sort(key=lambda fn: os.path.getmtime(fn))
-        fileTimeOut = fileTimeOut or timedelta(seconds=5)
 
         matchingFiles = OrderedDict()
 
         def _getTsId(match):
             """ Retrieve the TiltSerie ID from the matching object.
             We need to have tsId that starts with character, so
             let's add a prefix if it is not the case
             """
             tsId = match.group('TS')
             return normalizeTSId(tsId)
 
         def _addOne(fileList, file, match):
             """ Add one file matching to the list. """
-            fileList.append((file, int(match.group('TO')),
-                             float(match.group('TA'))))
+
+            order = int(match.group('TO'))
+            dose = int(self.dosePerFrame.get()) * order
+            angle = float(match.group('TA'))
+            fileList.append((file, order, angle, dose))
 
         def _addMany(fileList, file, match):
             """ Add many 'files' (when angles in header or mdoc)
                 to the list. """
             anglesFrom = self.getEnumText('anglesFrom')
+            doses = []
+            tiltorders = []
 
             if anglesFrom == self.ANGLES_FROM_HEADER:
                 angles = getAnglesFromHeader(file)
             elif anglesFrom == self.ANGLES_FROM_MDOC:
                 mdocFn = os.path.splitext(file)[0] + '.mdoc'
                 if not os.path.exists(mdocFn):
                     raise Exception("Missing angles file: %s" % mdocFn)
                 angles = getAnglesFromMdoc(mdocFn)
             elif anglesFrom == self.ANGLES_FROM_TLT:
-                angles, _ = self.getFromTlt(file)
+                angles, doses, tiltorders = self.getFromTlt(file)
             elif anglesFrom == self.ANGLES_FROM_RANGE:
                 angles = self._getTiltAngleRange()
             else:
                 raise Exception('Invalid angles option: %s' % anglesFrom)
 
             for i, a in enumerate(angles):
-                fileList.append(((i + 1, file), i + 1, a))
+                order = i+1 if not tiltorders else tiltorders[i]
+                dose = doses[i] if doses else int(self.dosePerFrame.get()) * order
+                fileList.append(((i + 1, file), order, a, dose))
 
         addFunc = _addOne if self._anglesInPattern() else _addMany
 
         # Handle special case of just one TiltSeries, to avoid
         # the user the need to specify {TS}
         if len(filePaths) == 1 and not self.isInStreaming():
             f = filePaths[0]
@@ -775,16 +695,14 @@
             self.info("Raw tilt series id is %s." % ts)
             ts = normalizeTSId(ts)
             self.info("Normalized tilt series id is %s." % ts)
             matchingFiles[ts] = []
             _addMany(matchingFiles[ts], f, None)
         else:
             for f in filePaths:
-                if self.fileModified(f, fileTimeOut):
-                    continue
                 m = self._regex.match(f)
                 if m is not None:
                     ts = _getTsId(m)
                     # Only report files of new tilt-series
                     if ts not in self._existingTs:
                         if ts not in matchingFiles:
                             matchingFiles[ts] = []
@@ -829,25 +747,26 @@
         return False
 
     def getFromTlt(self, file):
         """ Gets angles and doses from a tlt or rawtlt file """
         tltFn = os.path.splitext(file)[0] + '.tlt'
         rawtltFn = tltFn.replace(".tlt", ".rawtlt")
         if os.path.exists(tltFn):
-            angles, doses = getAnglesAndDosesFromTlt(tltFn)
+            angles, doses, tiltorders = getAnglesAndDosesFromTlt(tltFn)
         elif os.path.exists(rawtltFn):
-            angles, doses = getAnglesAndDosesFromTlt(rawtltFn)
+            angles, doses, tiltorders = getAnglesAndDosesFromTlt(rawtltFn)
         else:
             raise Exception("Missing angles file: %s or %s" % (tltFn, rawtltFn))
-        return angles, doses
+
+        return angles, doses, tiltorders
 
     @classmethod
     def worksInStreaming(cls):
-        # Import protocols always work in streaming
-        return True
+        # Streaming is done through SPA + tilt series composer
+        return False
 
     def _fillAcquisitionInfo(self, inputTs):
         # TODO Acquisition is historically expected as
         # one per set of tilt series movies,
         # so the first one is the one used, at least for now
         if self.MDOC_DATA_SOURCE:
             firstTsId = list(self.acquisitions.keys())[0]
@@ -880,46 +799,14 @@
 
     def _sameTiltAngleRange(self, tiltAngleRange, tiltSeriesList):
         # allow some tolerance when comparing tilt-angles
         return np.allclose(tiltAngleRange,
                            self._getSortedAngles(tiltSeriesList),
                            atol=0.1)
 
-    # --------------- Streaming special functions -----------------------
-    def _getStopStreamingFilename(self):
-        return self._getExtraPath("STOP_STREAMING.TXT")
-
-    def getActions(self):
-        """ This method will allow that the 'Stop import' action to appears
-        in the GUI when the user right-click in the protocol import box.
-        It will allow a user to manually stop the streaming.
-        """
-        # Only allow to stop if running and in streaming mode
-        if self.dataStreaming and self.isRunning():
-            return [('STOP STREAMING', self.stopImport)]
-        else:
-            return []
-
-    def stopImport(self):
-        """ Since the actual protocol that is running is in a different
-        process that the one that this method will be invoked from the GUI,
-        we will use a simple mechanism to place an special file to stop
-        the streaming.
-        """
-        # Just place an special file into the run folder
-        f = open(self._getStopStreamingFilename(), 'w')
-        f.close()
-
-    def streamingHasFinished(self):
-        return (not self.isInStreaming() or
-                os.path.exists(self._getStopStreamingFilename()))
-
-    def isInStreaming(self):
-        return self.dataStreaming.get()
-
     def setItemExtraAttributes(self, tsObj):
         """
         To set extra possible attributes of the TiltSerie or TiltSerieM that may have been defined in the form
         :param tsObj:
         :return: None
         """
         pass
```

### Comparing `scipion-em-tomo-3.1.5/tomo/protocols.conf` & `scipion-em-tomo-3.1.6/tomo/protocols.conf`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,22 @@
 		{"tag": "protocol_group", "text": "Preprocess", "openItem": "False", "children": []},
 		{"tag": "protocol_group", "text": "Tomogram Reconstruction", "openItem": "False", "children": []},
 		{"tag": "protocol_group", "text": "Quality Analysis", "openItem": "False", "children": []},
 		{"tag": "protocol_group", "text": "Denoise", "openItem": "False", "children": []},
 		{"tag": "protocol_group", "text": "Segmentation", "openItem": "False", "children": []}
 	]},
 	{"tag": "section", "text": "Particles", "children": [
-	    {"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": [
-            {"tag": "protocol", "value": "ProtTomoExtractCoords",   "text": "default"}]}
+	    {"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": []
+        },
+        {"tag": "protocol_group", "text": "Extract", "openItem": "False", "children": [
+            {"tag": "protocol", "value": "ProtTomoExtractCoords",   "text": "default"}]
+        },
+        {"tag": "protocol_group", "text": "Others", "openItem": "False", "children": [
+            {"tag": "protocol", "value": "TomoProtFitEllipsoid",   "text": "default"}]
+        }
 	]},
 	{"tag": "section", "text": "Subtomogram averaging", "children": [
 		{"tag": "section", "text": "Preprocessing", "children": [
 		    {"tag": "protocol", "value": "ProtAssignTomo2Subtomo",   "text": "default"},
 	   	    {"tag": "protocol", "value": "ProtAssignTransformationMatrixTiltSeries", "text": "default"},
         	    {"tag": "protocol", "value": "ProtSplitEvenOddTomoSet", "text": "default"},
 		    {"tag": "protocol", "value": "ProtAlignmentAssignSubtomo",      "text": "default"}
```

### Comparing `scipion-em-tomo-3.1.5/tomo/templates/HIV-Picking-with-Dynamo.json.template` & `scipion-em-tomo-3.1.6/tomo/templates/HIV-Picking-with-Dynamo.json.template`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         "runMode": 0,
         "tomoSource": 1,
         "boxSize": 64.0,
         "downFactor": 1.0,
         "doInvert": false,
         "doNormalize": false,
         "normproc": 0,
-        "inputTomograms": "2.outputTomograms",
+        "inputTomograms": "2.Tomograms",
         "inputCoordinates": "1287.output3DCoordinates"
     },
     {
         "object.className": "EmanProtTomoConvNet",
         "object.id": "653",
         "object.label": "emantomo - tomo boxer convnet",
         "object.comment": "",
@@ -106,15 +106,15 @@
         "method": 0,
         "SigmaGaussian": 0.5,
         "nIter": 10,
         "Lambda": -1.0,
         "TimeStep": 0.1,
         "hostName": "localhost",
         "numberOfThreads": 12,
-        "inputSetTomograms": "2.outputTomograms"
+        "inputSetTomograms": "2.Tomograms"
     },
     {
         "object.className": "DynamoModelWorkflow",
         "object.id": "1287",
         "object.label": "dynamo - model workflow",
         "object.comment": "",
         "_useQueue": false,
```

### Comparing `scipion-em-tomo-3.1.5/tomo/templates/HIV-Reconstruction.json.template` & `scipion-em-tomo-3.1.6/tomo/templates/HIV-Reconstruction.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/templates/HIV-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.6/tomo/templates/HIV-Subtomogram-averaging.json.template`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
         "object.label": "tomo - import tilt-series",
         "object.comment": "Registers the tiltseries TS_03 to use in this project. Run scipion3 testdata --download relion40_sta_tutorial_data to get the data.",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "filesPath": "~Path to HIV folder dataset|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/tomograms/TS_03/|2|datasetpath~",
-        "filesPattern": "{TS}*.mrc",
-        "exclusionWords": "output",
+        "filesPath": "~Path to HIV folder dataset|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/tomograms/|2|datasetpath~",
+        "filesPattern": "*/*.mrc",
+        "exclusionWords": "~Exlusion list|output 01 43 45 54|0|exclusion~",
         "mdocInfo": null,
         "anglesFrom": 2,
         "minAngle": -60.0,
         "maxAngle": 60.0,
         "stepAngle": 3.0,
         "ctfCorrected": false,
         "interpolated": false,
@@ -52,24 +52,24 @@
         "binningTM": 1,
         "binningTS": 1,
         "inputSetOfTiltSeries": "2.outputTiltSeries"
     },
     {
         "object.className": "CistemProtTsImportCtf",
         "object.id": "113",
-        "object.label": "cistem - import tomo CTFs (copy)",
+        "object.label": "cistem - import tomo CTFs",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "importFrom": 0,
-        "filesPath": "~Path to folder with  .defocus files|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/tomograms/TS_03/|2|ctffolder~",
-        "filesPattern": "*.defocus",
+        "filesPath": "~Path to folder with  .defocus files|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/tomograms/|2|ctffolder~",
+        "filesPattern": "*/*.defocus",
         "copyFiles": false,
         "exclusionWords": null,
         "inputSetOfTiltSeries": "2.outputTiltSeries"
     },
     {
         "object.className": "ProtImportTomograms",
         "object.id": "156",
@@ -88,33 +88,65 @@
         "importAcquisitionFrom": 0,
         "acquisitionData": null,
         "acquisitionAngleMax": 60.0,
         "acquisitionAngleMin": -60.0,
         "step": null,
         "angleAxis1": null,
         "angleAxis2": null,
-        "setOrigCoord": false,
+        "setOrigCoord": true,
+        "fromMrcHeader": true,
         "x": null,
         "y": null,
         "z": null
     },
     {
+        "object.className": "DynamoBoxing",
+        "object.id": "3995",
+        "object.label": "dynamo - vectorial picking",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 0,
+        "boxSize": 48,
+        "deleteGenMFiles": true,
+        "inputTomograms": "156.Tomograms"
+    },
+    {
+        "object.className": "DynamoModelWorkflow",
+        "object.id": "4039",
+        "object.label": "dynamo - model workflow",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 0,
+        "boxSize": 48,
+        "meshParameter": 5,
+        "maxTr": 100000,
+        "cropping": 10,
+        "subDivision": 2,
+        "inputMeshes": "3995.meshes"
+    },
+    {
         "object.className": "ProtImportCoordinates3DFromStar",
         "object.id": "227",
         "object.label": "reliontomo - import coordinates 3D from a star file",
         "object.comment": "Imports relion4 tutorial 3D coordinates.",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "starFile": "~Path to coords.star file|%(SCIPION_TESTS)s/relion40_sta_tutorial_data/input/coords_5tomos.star|2|coordspath~",
         "samplingRate": 1.35,
         "boxSize": 20,
-        "inTomos": "156.outputTomograms"
+        "inTomos": "156.Tomograms"
     },
     {
         "object.className": "ProtSubSet",
         "object.id": "3355",
         "object.label": "Subset for dynamo",
         "object.comment": "We make a small subset of first 200 coordinates to use dynamo STA",
         "_useQueue": false,
@@ -176,15 +208,15 @@
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "useGpu": true,
-        "gpuList": "2",
+        "gpuList": "0",
         "numberOfIters": "2 2 2",
         "dim": "0",
         "useDynamoGui": false,
         "cr": "60 30 10",
         "cs": "10 5 2",
         "cf": "0",
         "inplane_range": "45 15 4",
@@ -200,15 +232,15 @@
         "threshold2": "0.2",
         "thresholdMode2": "0",
         "high": "2",
         "low": "32",
         "sym": "c6 c6 c6",
         "ccmatrixBatch": 128,
         "hostName": "localhost",
-        "numberOfThreads": 10,
+        "numberOfThreads": 4,
         "inputVolumes": "2160.subtomograms",
         "templateRef": "2262.average"
     },
     {
         "object.className": "ProtRelionPrepareData",
         "object.id": "270",
         "object.label": "reliontomo - Prepare data for Relion 4",
@@ -495,15 +527,15 @@
         "numberOfMpi": 1,
         "boxSize": 256,
         "croppedBoxSize": 128,
         "binningFactor": 2.0,
         "applyConeWeight": false,
         "coneAngle": 10.0,
         "applyOffsets": false,
-        "outputInFloat16": true,
+        "outputInFloat16": false,
         "inReParticles": "924.relionParticles"
     },
     {
         "object.className": "ProtRelion3DClassifySubtomograms",
         "object.id": "1343",
         "object.label": "reliontomo - 3D Classification of subtomograms (copy 2)",
         "object.comment": "",
@@ -548,70 +580,29 @@
         "numberOfThreads": 1,
         "numberOfMpi": 3,
         "solventMask": "994.outputMask",
         "referenceVolume": "1116.average",
         "inReParticles": "1155.relionParticles"
     },
     {
-        "object.className": "EmanProtTomoExtraction",
-        "object.id": "1194",
-        "object.label": "emantomo - extraction from tomogram",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "tomoSource": 0,
-        "boxSize": 96.0,
-        "downFactor": 1.0,
-        "doInvert": true,
-        "doNormalize": true,
-        "normproc": 0,
-        "inputCoordinates": "1343.relionParticles"
-    },
-    {
-        "object.className": "ProtRelionSubTomoReconstructAvg",
-        "object.id": "1413",
-        "object.label": "reliontomo - Rec. particle averaging subtomograms",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "symmetryGroup": "c6",
-        "maxRes": -1.0,
-        "pad": 2.0,
-        "subset": 0,
-        "classNum": -1,
-        "extraParams": "",
-        "doCTF": false,
-        "ctfIntactFirstPeak": false,
-        "hostName": "localhost",
-        "numberOfMpi": 1,
-        "inputSubtomos": "1194.subtomograms"
-    },
-    {
         "object.className": "XmippProtSubtomoMapBack",
         "object.id": "1461",
         "object.label": "xmipptomo - map back subtomos",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "selection": 1,
         "invertContrast": false,
-        "paintingType": 0,
+        "paintingType": 2,
         "removeBackground": true,
         "threshold": 0.5,
         "constant": 100000.0,
         "hostName": "localhost",
         "numberOfThreads": 1,
         "numberOfMpi": 1,
-        "inputTomograms": "156.outputTomograms",
-        "inputSubtomos": "1076.coordinates",
-        "inputRef": "1413.average"
+        "inputSubtomos": "227.coordinates",
+        "inputRef": "1116.average"
     }
 ]
```

### Comparing `scipion-em-tomo-3.1.5/tomo/templates/Membrane picking-with-PySeg.json.template` & `scipion-em-tomo-3.1.6/tomo/templates/Membrane picking-with-PySeg.json.template`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         "scaleRangeMin": 0.0,
         "antialias": 5,
         "meanSdToggle": 1,
         "scaleMean": 0.0,
         "scaleSd": 1.0,
         "scaleMax": 255.0,
         "scaleMin": 0.0,
-        "inputSetOfTomograms": "3.outputTomograms"
+        "inputSetOfTomograms": "3.Tomograms"
     },
     {
         "object.className": "ProtJjsoftProtDenoiseTomogram",
         "object.id": "142",
         "object.label": "tomo3d - denoise tomogram",
         "object.comment": "",
         "_useQueue": false,
@@ -122,15 +122,15 @@
         "mbThkPix": 1,
         "mbScaleFactor": 8,
         "blackOverWhite": true,
         "mbStrengthTh": 0.01,
         "sigmaS": 0.5,
         "sigmaP": 0.0,
         "keepAllFiles": true,
-        "inTomograms": "142.outputTomograms"
+        "inTomograms": "142.tomograms"
     },
     {
         "object.className": "ProtPySegPreSegParticles",
         "object.id": "687",
         "object.label": "pyseg - preseg membranes",
         "object.comment": "",
         "_useQueue": false,
@@ -152,15 +152,15 @@
         "object.label": "tomosegmemtv - Resize segmented or annotated volume",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "inTomos": "3.outputTomograms",
+        "inTomos": "3.Tomograms",
         "inTomoMasks": "268.tomoMasks"
     },
     {
         "object.className": "ProtPySegGraphs",
         "object.id": "840",
         "object.label": "pyseg - graphs",
         "object.comment": "",
@@ -238,15 +238,15 @@
         "side": 2,
         "cont": 1,
         "peakTh": 0.0,
         "peakNs": 0.5,
         "hostName": "localhost",
         "numberOfThreads": 3,
         "numberOfMpi": 1,
-        "inTomoSet": "3.outputTomograms",
+        "inTomoSet": "3.Tomograms",
         "inFilsProt": "878."
     },
     {
         "object.className": "ProtTomoPickingRemoveDuplicates",
         "object.id": "987",
         "object.label": "tomoviz - remove duplicates",
         "object.comment": "",
@@ -264,15 +264,15 @@
         "object.label": "xmipptomo - fit vesicles",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
-        "inputTomos": "3.outputTomograms",
+        "inputTomos": "3.Tomograms",
         "input": "987.outputCoordinates"
     },
     {
         "object.className": "XmippProtFilterbyNormal",
         "object.id": "1071",
         "object.label": "tomoviz - filter by normal",
         "object.comment": "",
@@ -374,30 +374,10 @@
         "symmetry": "c1",
         "doMorphological": false,
         "morphologicalOperation": 0,
         "elementSize": 1,
         "doInvert": false,
         "doSmooth": true,
         "sigmaConvolution": 2.0
-    },
-    {
-        "object.className": "ProtPySegGraphs",
-        "object.id": "1623",
-        "object.label": "pyseg - graphs (copy)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "vesiclePkgSize": 3,
-        "keepOnlyReqFiles": true,
-        "sSig": 3.0,
-        "vDen": 0.0035,
-        "vRatio": 4.0,
-        "maxLen": 330.0,
-        "hostName": "localhost",
-        "numberOfThreads": 3,
-        "inSegProt": "687."
     }
 ]
```

### Comparing `scipion-em-tomo-3.1.5/tomo/templates/Ribosomes-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.6/tomo/templates/Ribosomes-Subtomogram-averaging.json.template`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         "max_box_per_image": 600,
         "batchSize": 1,
         "useGpu": true,
         "gpuList": "0",
         "hostName": "localhost",
         "numberOfThreads": 10,
         "numberOfMpi": 1,
-        "inputTomograms": "2.outputTomograms"
+        "inputTomograms": "2.Tomograms"
     },
     {
         "object.className": "EmanProtTomoExtraction",
         "object.id": "137",
         "object.label": "emantomo - extraction from tomogram",
         "object.comment": "",
         "_useQueue": false,
```

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/__init__.py` & `scipion-em-tomo-3.1.6/tomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_base_centralized_layer.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_base_centralized_layer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_compose_TS.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_compose_TS.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,17 @@
                                            objLabel='Import movies (SPA)',
                                            importFrom=emprot.ProtImportMovies.IMPORT_FROM_FILES,
                                            filesPath=self.partFolderPath,
                                            filesPattern=self.pattern,
                                            voltage=300)
         self.launchProtocol(protMovieImport)
         self.assertIsNotNone(protMovieImport.outputMovies, 'Movies not imported')
-
         # Align movies and create a set of micrographs
         xmipp3 = Domain.importFromPlugin('xmipp3.protocols', doRaise=True)
-        protAlign = self.newProtocol(xmipp3.XmippProtMovieCorr,
+        protAlign = self.newProtocol(xmipp3.XmippProtFlexAlign,
                                      objLabel='Movie Alignment (SPA)',
                                      alignFrame0=1, alignFrameN=0,
                                      useAlignToSum=True,
                                      doLocalAlignment=False)
         protAlign.inputMovies.set(protMovieImport.outputMovies)
         self.launchProtocol(protAlign)
         self.assertIsNotNone(protAlign.outputMicrographs, 'Micrograph not generated')
@@ -102,17 +101,17 @@
                                        filesPath=self.partFolderPath,
                                        time4NextTilt=20,
                                        time4NextMic=12,
                                        time4NextTS=30)
         # self.proj.scheduleProtocol(protCompose)
         # checkOutputs(protCompose, 20)#timeout
         self.launchProtocol(protCompose)
-        self.assertIsNotNone(protCompose.TiltSeries, 'TiltSeries dont composed')
+        self.assertIsNotNone(protCompose.TiltSeries, 'TiltSeries not composed')
 
-        # xcor prealigment
+        # xcor prealignment
         imod = Domain.importFromPlugin('imod.protocols', doRaise=True)
         prealigment = self.newProtocol(imod.ProtImodXcorrPrealignment,
                                        objLabel='Xcor preAlignment',
                                        computeAlignment=0,
                                        binning=2)
         prealigment.inputSetOfTiltSeries.set(protCompose.TiltSeries)
         # self.proj.scheduleProtocol(prealigment)
```

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_import.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # **************************************************************************
 import glob
 import os
 from os.path import join, exists, abspath
 
 import numpy
 
+from tomo.convert import getOrderFromList
 from pyworkflow.tests import BaseTest, setupTestProject
 from pyworkflow.utils import magentaStr, createLink
 from pyworkflow.object import Pointer
 from pwem.protocols import ProtSplitSet, ProtSetFilter, ProtSetEditor
 
 from tomo.protocols.protocol_ts_import import MDoc
 from . import DataSet
@@ -159,18 +160,18 @@
     def _importTomograms(self, filesPath, samplingRate, pattern=None):
         protImportTomogram = self.newProtocol(tomo.protocols.ProtImportTomograms,
                                               filesPath=filesPath,
                                               filesPattern=pattern,
                                               samplingRate=samplingRate)
 
         self.launchProtocol(protImportTomogram)
-        outputTomos = getattr(protImportTomogram, 'outputTomograms', None)
-        self.assertIsNotNone(outputTomos, 'No tomograms were genetated.')
 
-        return outputTomos
+        self.assertSetSize(protImportTomogram.Tomograms, size=1, msg='No tomograms were generated.')
+
+        return protImportTomogram.Tomograms
 
     def _runTomoImportSetOfCoordinates(self, pattern, program, ext):
         sRate = 5.5
         protImportCoordinates3d = self.newProtocol(ProtImportCoordinates3D,
                                                    objLabel='Import from %s - %s' % (program, ext),
                                                    auto=IMPORT_FROM_AUTO,
                                                    filesPath=self.tomoDs.getPath(),
@@ -318,75 +319,72 @@
         self.assertSetSize(coordSet, size=size)
         self.assertTrue(coordSet.getBoxSize() == boxSize)
         self.assertTrue(coordSet.getSamplingRate() == samplingRate)
 
         self.assertIsNotNone(coordSet.getPrecedents(), "Tomograms not associated in the output set")
 
         for coord in coordSet.iterCoordinates():
-            # Access the coordinate, this should work if tomograms are assocciated
-            Y = coord.getY(BOTTOM_LEFT_CORNER)
+            # Access the coordinate, this should work if tomograms are associated
+            X = coord.getY(BOTTOM_LEFT_CORNER)
             Y = coord.getY(TOP_LEFT_CORNER)
 
             break
 
 
 class TestTomoImportTomograms(BaseTest):
     """This class check if the protocol to import tomograms works properly."""
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('tomo-em')
         cls.tomogram = cls.dataset.getFile('*.em')
 
-    def _runImportTomograms(self):
+    def _runImportTomograms(self)-> tomo.protocols.ProtImportTomograms:
         protImport = self.newProtocol(
             tomo.protocols.ProtImportTomograms,
             filesPath=self.tomogram,
             filesPattern='',
             acquisitionAngleMax=40,
             acquisitionAngleMin=-40,
             samplingRate=1.35)
         self.launchProtocol(protImport)
         return protImport
 
-    def _runImportTomograms2(self):
+    def _runImportTomograms2(self)->tomo.protocols.ProtImportTomograms:
         protImport = self.newProtocol(
             tomo.protocols.ProtImportTomograms,
             filesPath=self.tomogram,
             filesPattern='',
             samplingRate=1.35)
         self.launchProtocol(protImport)
         return protImport
 
     def test_importTomograms(self):
         protImport = self._runImportTomograms()
-        output = getattr(protImport, 'outputTomograms', None)
-        self.assertIsNotNone(output,
-                             "There was a problem with Import Tomograms protocol")
+        self.assertSetSize(protImport.Tomograms, size=2, msg="There was a problem with Import Tomograms protocol")
 
-        for tomogram in protImport.outputTomograms.iterItems():
+        for tomogram in protImport.Tomograms.iterItems():
             self.assertTrue(tomogram.getXDim() == 1024,
                             "There was a problem with Import Tomograms protocol")
             self.assertIsNotNone(tomogram.getYDim() == 1024,
                                  "There was a problem with Import Tomograms protocol")
 
             self.assertTrue(tomogram.getAcquisition().getAngleMax() == 40,
                             "There was a problem with the acquisition angle max")
             self.assertTrue(tomogram.getAcquisition().getAngleMin() == -40,
                             "There was a problem with the acquisition angle min")
 
             break
 
         protImport2 = self._runImportTomograms2()
-        output2 = getattr(protImport2, 'outputTomograms', None)
-        self.assertIsNotNone(output2,
+        self.assertSetSize(protImport.Tomograms, size=2, msg=
                              "There was a problem with Import Tomograms protocol")
 
-        for tomogram in protImport2.outputTomograms.iterItems():
+        for tomogram in protImport2.Tomograms.iterItems():
             self.assertTrue(tomogram.getXDim() == 1024,
                             "There was a problem with Import Tomograms protocol")
             self.assertIsNotNone(tomogram.getYDim() == 1024,
                                  "There was a problem with Import Tomograms protocol")
 
             self.assertTrue(tomogram.getAcquisition().getAngleMax() == 60,
                             "There was a problem with the acquisition angle max")
@@ -419,15 +417,15 @@
             tiltAxisAngle=84.1
         )
         self.launchProtocol(protImport)
         return protImport
 
     def test_importTiltSeriesM(self):
         protImport = self._runImportTiltSeriesM()
-        self.assertSetSize(protImport.outputTiltSeriesM, 2)
+        self.assertSetSize(protImport.outputTiltSeriesM, size=2, msg="Importing tilt series movies is failing")
 
         return protImport
 
     def test_motioncorTiltSeriesM(self):
         protImport = self.test_importTiltSeriesM()
 
         # --------- Motion correction with motioncor2 for Tilt-series ------
@@ -831,43 +829,41 @@
     def _importTomograms(cls, filesPath):
         print(magentaStr("\n==> Importing data - tomograms:"))
         protImportTomogram = cls.newProtocol(ProtImportTomograms,
                                              filesPath=filesPath,
                                              samplingRate=cls.samplingRate)
 
         cls.launchProtocol(protImportTomogram)
-        outputTomos = getattr(protImportTomogram, 'outputTomograms', None)
-        cls.assertIsNotNone(outputTomos, 'No tomograms were genetated.')
+        cls.assertIsNotNone(protImportTomogram.Tomograms, 'No tomograms were generated importing %s.' % filesPath)
 
-        return outputTomos
+        return protImportTomogram.Tomograms
 
     @classmethod
     def _normalizeTomo(cls):
         print(magentaStr("\n==> Tomogram normalization:"))
         protTomoNormalization = cls.newProtocol(ProtImodTomoNormalization,
                                                 inputSetOfTomograms=cls.inTomoSet,
                                                 binning=2)
 
         cls.launchProtocol(protTomoNormalization)
         outputTomos = getattr(protTomoNormalization, 'Tomograms', None)
-        cls.assertIsNotNone(outputTomos, 'No tomograms were genetated in tomo normalization.')
+        cls.assertIsNotNone(outputTomos, 'No tomograms were generated in tomo normalization.')
 
         return outputTomos
 
     def testImportTomoMasksAllGood(self):
         print(magentaStr("\n==> Importing data - tomoMasks:"))
         protImportTomomasks = self.newProtocol(ProtImportTomomasks,
                                                filesPath=self.ds.getFile('tomoMaskAnnotated'),
                                                inputTomos=self.inTomoSetBinned)
 
         self.launchProtocol(protImportTomomasks)
         tomoMaskSet = getattr(protImportTomomasks, 'outputTomoMasks', None)
 
-        self.assertIsNotNone(tomoMaskSet, 'No tomograms were genetated.')
-        self.assertSetSize(tomoMaskSet, 1)
+        self.assertSetSize(tomoMaskSet, size=1, msg="Importing tomoMasks failed.")
         self.assertEqual(tomoMaskSet.getDimensions(), (464, 464, 250))
         self.assertEqual(tomoMaskSet.getSamplingRate(), 2 * self.samplingRate)
         self.assertFalse(protImportTomomasks.warnMsg)
 
     # The tomogram and the tomomask have different sizes
     def testImportTomoMasksDiffSize(self):
         print(magentaStr("\n==> Importing data - tomoMasks:"))
@@ -885,7 +881,27 @@
         protImportTomomasks = self.newProtocol(ProtImportTomomasks,
                                                filesPath=self.ds.getFile('tomoMaskAnnotated'),
                                                inputTomos=self.inNotMatchingTomoSet)
 
         with self.assertRaises(Exception) as eType:
             self.launchProtocol(protImportTomomasks)
             self.assertEqual(str(eType.exception), ERR_NON_MATCHING_TOMOS)
+
+class TestConvert(BaseTest):
+
+    def test_list_order(self):
+
+        myList = [20,40,50,10,30]
+        orders = getOrderFromList(myList)
+        self.assertEqual(orders, [2,4,5,1,3])
+
+        myList = [20, 40, 50, 10, 30]
+        orders = getOrderFromList(myList)
+        self.assertEqual(orders, [2, 4, 5, 1, 3])
+
+        # Simulate dose list in symmetric dose scheme
+        myList = [24,21,12,9,3,6,15,18,27]
+        orders = getOrderFromList(myList)
+        self.assertEqual(orders, [8,7,4,3,1,2,5,6,9])
+
+
+
```

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_objects.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_tomo_base.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_tomo_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('tomo-em')
         cls.tomogram = cls.dataset.getFile('*.em')
 
-    def _runImportTomograms(self):
+    def _runImportTomograms(self)->tomo.protocols.ProtImportTomograms:
         protImport = self.newProtocol(
             tomo.protocols.ProtImportTomograms,
             filesPath=self.tomogram,
             filesPattern='',
             acquisitionAngleMax=40,
             acquisitionAngleMin=-40,
             samplingRate=1.35)
@@ -321,15 +321,15 @@
             yield output
 
     def test_createSubSetOfTomogram(self):
         print(pwutils.magentaStr("\n==> Importing a Set of Tomograms..."))
         protImport = self._runImportTomograms()
 
         # Check importing
-        for tomo in protImport.outputTomograms.iterItems():
+        for tomo in protImport.Tomograms.iterItems():
             self.assertTrue(tomo.getXDim() == 1024,
                             "There was a problem with Import Tomograms protocol")
             self.assertIsNotNone(tomo.getYDim() == 1024,
                                  "There was a problem with Import Tomograms "
                                  "protocol")
 
             self.assertTrue(tomo.getAcquisition().getAngleMax() == 40,
@@ -340,37 +340,37 @@
         # Create a subset with 1 tomograms
         print(pwutils.magentaStr("\n==> Create the subset 1 of Tomograms"))
         tomoSubset1 = self.newProtocol(emprot.ProtSubSet,
                                        objLabel='subset 1',
                                        chooseAtRandom=True,
                                        nElements=1)
 
-        tomoSubset1.inputFullSet.set(protImport.outputTomograms)
+        tomoSubset1.inputFullSet.set(protImport.Tomograms)
         self.launchProtocol(tomoSubset1)
 
         # Create a subset with 2 tomograms
         print(pwutils.magentaStr("\n==> Create the subset 2 of Tomograms"))
         tomoSubset2 = self.newProtocol(emprot.ProtSubSet,
                                        objLabel='subset 2',
                                        chooseAtRandom=False,
                                        inputSubSet=tomoSubset1.outputTomograms,
                                        setOperation=1,
                                        nElements=1)
 
-        tomoSubset2.inputFullSet.set(protImport.outputTomograms)
+        tomoSubset2.inputFullSet.set(protImport.Tomograms)
         self.launchProtocol(tomoSubset2)
 
         # Create a subset with 3 tomograms
         print(pwutils.magentaStr("\n==> Create the subset 3 of Tomograms"))
         tomoSubset3 = self.newProtocol(emprot.ProtSubSet,
                                        objLabel='subset 3',
                                        chooseAtRandom=True,
                                        nElements=2)
 
-        tomoSubset3.inputFullSet.set(protImport.outputTomograms)
+        tomoSubset3.inputFullSet.set(protImport.Tomograms)
         self.launchProtocol(tomoSubset3)
 
         # create merge protocol
         print(pwutils.magentaStr("\n==> Join subsets 1 and 2 "))
         joinTomoSet = self.newProtocol(emprot.ProtUnionSet,
                                        objLabel='join Tomograms sets',
                                        ignoreExtraAttributes=True)
@@ -430,25 +430,25 @@
         cls.tomogram = cls.dataset.getFile('tomo1')
         cls.coords3D = cls.dataset.getFile('overview_wbp.txt')
         cls.table = cls.dataset.getFile('initial.tbl')
         cls.path = cls.dataset.getPath()
 
     def _runImportSubTomograms(self):
 
-        protImportSubTomogram = self.newProtocol(
+        protImportTomogram = self.newProtocol(
             tomo.protocols.ProtImportTomograms,
             filesPath=self.tomogram,
             samplingRate=5)
-        self.launchProtocol(protImportSubTomogram)
+        self.launchProtocol(protImportTomogram)
 
         protImportCoordinates3d = self.newProtocol(
             tomo.protocols.ProtImportCoordinates3D,
             auto=tomo.protocols.ProtImportCoordinates3D.IMPORT_FROM_FILES,
             filesPath=self.coords3D,
-            importTomograms=protImportSubTomogram.outputTomograms,
+            importTomograms=protImportTomogram.Tomograms,
             filesPattern='', boxSize=32,
             samplingRate=5)
         self.launchProtocol(protImportCoordinates3d)
 
         protImport = self.newProtocol(tomo.protocols.ProtImportSubTomograms,
                                       filesPath=self.path,
                                       filesPattern='base*.hdf',
@@ -701,15 +701,15 @@
         self.launchProtocol(protImportSubtomo)
         return protImportTomo, protImportSubtomo
 
     def _assignTomos2subtomos(self):
         protImportTomo, protImportSubtomo = self._runPreviousProtocols()
         tomo2subtomo = self.newProtocol(tomo.protocols.ProtAssignTomo2Subtomo,
                                         inputSubtomos=protImportSubtomo.outputSubTomograms,
-                                        inputTomos=protImportTomo.outputTomograms)
+                                        inputTomos=protImportTomo.Tomograms)
         self.launchProtocol(tomo2subtomo)
         self.assertIsNotNone(tomo2subtomo.outputSubtomograms,
                              "There was a problem with subtomograms output")
         return tomo2subtomo
 
     def test_assignTomos2subtomos(self):
         tomo2subtomo = self._assignTomos2subtomos()
@@ -826,15 +826,15 @@
                                           filesPath=self.setOfTomograms,
                                           filesPattern='',
                                           acquisitionAngleMax=40,
                                           acquisitionAngleMin=-40,
                                           samplingRate=1.35)
         self.launchProtocol(protImportTomo)
         split = self.newProtocol(tomo.protocols.ProtSplitEvenOddTomoSet,
-                                 inputSet=protImportTomo.outputTomograms)
+                                 inputSet=protImportTomo.Tomograms)
         self.launchProtocol(split)
         self.assertIsNotNone(split.outputset_even,
                              "There was a problem with even tomograms output")
         self.assertIsNotNone(split.outputset_odd,
                              "There was a problem with odd tomograms output")
         return split
```

### Comparing `scipion-em-tomo-3.1.5/tomo/tests/test_transformations.py` & `scipion-em-tomo-3.1.6/tomo/tests/test_transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                                                 boxSize=protPhantom.coordinates3D.getBoxSize(),
                                                 doInvert=True
                                                 )
 
                 self.launchProtocol(stExtraction)
 
                 # Add the averagers
-                addAveragers(self, stExtraction, EmanProtTomoExtraction._possibleOutputs.subtomograms.name)
+                addAveragers(self, stExtraction, EmanProtTomoExtraction._possibleOutputs.subtomograms.name, label=label)
 
 
     # Define the class inside so only the test is available if xmipptomo is.
     class TestTiltSeriesTransformations(BaseTest):
         """ This class generates a phantom based workflow with contrlolled
         tilt series information from a phantom tomogram."""
```

### Comparing `scipion-em-tomo-3.1.5/tomo/utils.py` & `scipion-em-tomo-3.1.6/tomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/viewers/__init__.py` & `scipion-em-tomo-3.1.6/tomo/viewers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .viewers_data import (TomoDataViewer, TSMotionCorrectionViewer,
                            CtfEstimationTomoViewer)
-from .viewer_tomograms import ViewerProtImportTomograms
 from .viewer_split_evenodd import SplitEvenOddViewer
```

### Comparing `scipion-em-tomo-3.1.5/tomo/viewers/viewer_split_evenodd.py` & `scipion-em-tomo-3.1.6/tomo/viewers/viewer_split_evenodd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/viewers/viewers_data.py` & `scipion-em-tomo-3.1.6/tomo/viewers/viewers_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,7 +234,13 @@
                           config={MODE: MODE_MD,
                                   VISIBLE: 'id _tomoId _x _y _z _groupId _eulerMatrix._matrix '})
 
 DataViewer.registerConfig(tomo.objects.SetOfTiltSeriesCoordinates)
 DataViewer.registerConfig(tomo.objects.SetOfMeshes)
 DataViewer.registerConfig(tomo.objects.SetOfLandmarkModels)
 DataViewer.registerConfig(tomo.objects.SetOfCTFTomoSeries)
+DataViewer.registerConfig(tomo.objects.SetOfTomograms,
+                          config={MODE:MODE_MD,
+                                  VISIBLE:'id _filename %s %s' %
+                                          (tomo.objects.Tomogram.TS_ID_FIELD,
+                                           tomo.objects.Tomogram.ORIGIN_MATRIX_FIELD)})
+
```

### Comparing `scipion-em-tomo-3.1.5/tomo/viewers/views.py` & `scipion-em-tomo-3.1.6/tomo/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/viewers/views_tkinter_tree.py` & `scipion-em-tomo-3.1.6/tomo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.5/tomo/wizards.py` & `scipion-em-tomo-3.1.6/tomo/wizards.py`

 * *Files identical despite different names*

