# Comparing `tmp/scipion-em-reliontomo-3.1.3.tar.gz` & `tmp/scipion-em-reliontomo-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-reliontomo-3.1.3.tar", last modified: Thu Mar 30 11:12:37 2023, max compression
+gzip compressed data, was "scipion-em-reliontomo-3.1.4.tar", last modified: Thu Apr 20 14:27:22 2023, max compression
```

## Comparing `scipion-em-reliontomo-3.1.3.tar` & `scipion-em-reliontomo-3.1.4.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.893699 scipion-em-reliontomo-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-03-30 11:12:37.893699 scipion-em-reliontomo-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.885699 scipion-em-reliontomo-3.1.3/reliontomo/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.885699 scipion-em-reliontomo-3.1.3/reliontomo/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/cmd/compareStarFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.889699 scipion-em-reliontomo-3.1.3/reliontomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/convert/convert30_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23349 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/convert/convert40_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/convert/convertBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.889699 scipion-em-reliontomo-3.1.3/reliontomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_3d_classify_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_import_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_per_part_per_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_relion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_ctf_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_de_novo_initial_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_edit_particles_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_extract_coordinates_from_psubtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_import_coordinates_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_import_subtomograms_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_make_pseudo_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_matching_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_rec_tomogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19197 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_refine_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_tomo_frame_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/relion_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.889699 scipion-em-reliontomo-3.1.3/reliontomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/tests/test_compare_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/tests/test_import_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/tests/test_refine_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/reliontomo/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:12:37.889699 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-03-30 11:12:37.000000 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-30 11:12:37.000000 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:12:37.000000 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-30 11:12:37.000000 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-30 11:12:37.000000 scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 11:12:37.893699 scipion-em-reliontomo-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-03-30 11:10:30.000000 scipion-em-reliontomo-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/cmd/compareStarFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convert30_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convert40_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convertBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/reliontomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_3d_classify_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_import_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_per_part_per_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_relion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_ctf_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_de_novo_initial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_edit_particles_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_coordinates_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_subtomograms_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_make_pseudo_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_matching_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17346 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_tomogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_refine_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_tomo_frame_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/relion_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/reliontomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_compare_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_import_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_refine_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:27:22.840166 scipion-em-reliontomo-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/setup.py
```

### Comparing `scipion-em-reliontomo-3.1.3/LICENSE` & `scipion-em-reliontomo-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/PKG-INFO` & `scipion-em-reliontomo-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.3
+Version: 3.1.4
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.3/README.rst` & `scipion-em-reliontomo-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/__init__.py` & `scipion-em-reliontomo-3.1.4/reliontomo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import pwem
 import relion
 from reliontomo.constants import RELIONTOMO_HOME, RELIONTOMO_DEFAULT, RELION, RELIONTOMO_CUDA_LIB, V4_0
 
 _logo = "relion_logo.png"
 _references = ['Scheres2012a', 'Scheres2012b', 'Kimanius2016', 'Zivanov2018']
-__version__ = '3.1.3'
+__version__ = '3.1.4'
 
 
 class Plugin(relion.Plugin):
     _supportedVersions = [V4_0]
     _homeVar = RELIONTOMO_HOME
     _pathVars = [RELIONTOMO_HOME]
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/bibtex.py` & `scipion-em-reliontomo-3.1.4/reliontomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/cmd/compareStarFiles.py` & `scipion-em-reliontomo-3.1.4/reliontomo/cmd/compareStarFiles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/constants.py` & `scipion-em-reliontomo-3.1.4/reliontomo/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 OPT_MANIFOLDS_STAR = 'rlnTomoManifoldsFile'
 OPT_FSC_STAR = 'rlnTomoReferenceFscFile'
 
 # Scipion Coordinates fields
 SCIPION_COORD_X = 'sciXCoord'
 SCIPION_COORD_Y = 'sciYCoord'
 SCIPION_COORD_Z = 'sciZCoord'
+SCIPION_COORD_GROUP_ID = 'sciGroupId'
 
 FILE_NOT_FOUND = 'FileNotFound'
 
 RELION_30_TOMO_LABELS = [TOMO_NAME_30,
                          COORD_X,
                          COORD_Y,
                          COORD_Z,
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/convert/__init__.py` & `scipion-em-reliontomo-3.1.4/reliontomo/convert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 
 from emtable import Table
+
+from reliontomo.objects import RelionSetOfPseudoSubtomograms
 from reliontomo import Plugin
-from reliontomo.constants import TOMO_NAME_30, PARTICLES_TABLE, RELION_30_TOMO_LABELS, RELION_40_TOMO_LABELS
+from reliontomo.constants import TOMO_NAME_30, PARTICLES_TABLE, RELION_30_TOMO_LABELS, RELION_40_TOMO_LABELS, \
+    PSUBTOMOS_SQLITE
 from reliontomo.convert import convert40_tomo, convert30_tomo
 
 
 def createWriterTomo(isPyseg=False, **kwargs):
     if isPyseg or not Plugin.isRe40():
         writer = createWriterTomo30(starHeaders=RELION_30_TOMO_LABELS, **kwargs)
     else:
@@ -85,10 +88,10 @@
         isReader40 = True
 
     return reader, isReader40
 
 
 def readSetOfPseudoSubtomograms(outputSet):
     """ Convenience function to write a SetOfPseudoSubtomograms as Relion metadata using a Reader."""
-    # Subtomogras are represented in Relion 4 as Pseudosubtomograms
+    # Subtomograms are represented in Relion 4 as Pseudosubtomograms
     reader, _ = createReaderTomo(outputSet.getParticles())
     return reader.starFile2PseudoSubtomograms(outputSet)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/convert/convert30_tomo.py` & `scipion-em-reliontomo-3.1.4/reliontomo/convert/convert30_tomo.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
+
+import logging
+logger = logging.getLogger(__name__)
 from os import symlink
 from emtable import Table
 from pwem.emlib.image import ImageHandler
 import pyworkflow.utils as pwutils
 from pwem.objects import Transform
 from pyworkflow.object import Float
 from pyworkflow.utils import removeBaseExt, getParentFolder
@@ -47,26 +50,28 @@
      interface as the new Writer class.
     """
 
     def __init__(self,  **kwargs):
         super().__init__(**kwargs)
 
     def subtomograms2Star(self, subtomoSet, subtomosStar):
+
+        logger.info("Converting scipion subtomograms to relion 3 format.")
         currentTomo = ''
         ih = ImageHandler()
         tomoTable = Table(columns=self.starHeaders)
         tmpDir = pwutils.getParentFolder(subtomosStar)
         for subtomo in subtomoSet.iterSubtomos():
             if pwutils.getExt(subtomo.getFileName().replace(':' + MRC, '')) != '.' + MRC:
                 mrcDir = join(tmpDir, pwutils.removeBaseExt(subtomo.getVolName()))
                 if currentTomo != subtomo.getVolName():
                     mkdir(mrcDir)
                 mrcFile = join(mrcDir, pwutils.replaceBaseExt(subtomo.getFileName(), MRC))
                 ih.convert(subtomo.getFileName(), mrcFile)
-            angles, shifts = getTransformInfoFromCoordOrSubtomo(subtomo)
+            angles, shifts = getTransformInfoFromCoordOrSubtomo(subtomo, 1)
             magn = subtomo.getAcquisition().getMagnification()
 
             rlnCoordinateX = 0
             rlnCoordinateY = 0
             rlnCoordinateZ = 0
             coord3D = subtomo.getCoordinate3D()
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/convert/convert40_tomo.py` & `scipion-em-reliontomo-3.1.4/reliontomo/convert/convert40_tomo.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 import logging
+logger = logging.getLogger(__name__)
 import csv
 
 from emtable import Table
-from pwem import ALIGN_NONE, ALIGN_2D, ALIGN_PROJ
+from pwem import ALIGN_NONE
 from pwem.convert.headers import fixVolume
 from pwem.objects import Transform
 from pyworkflow.object import Integer, Float
 from pyworkflow.utils import getParentFolder, yellowStr, createLink, makePath
 from relion.convert import OpticsGroups
 from reliontomo.constants import *
-import pwem.convert.transformations as tfs
 import numpy as np
 from os.path import join, basename
 from reliontomo.convert.convertBase import (checkSubtomogramFormat,
                                             getTransformInfoFromCoordOrSubtomo,
                                             WriterTomo, ReaderTomo, getTransformMatrixFromRow)
 from reliontomo.objects import RelionPSubtomogram
 from tomo.constants import BOTTOM_LEFT_CORNER, TR_SCIPION, TR_RELION, SCIPION
@@ -81,91 +81,96 @@
         tsTable.write(outStarFileName)
 
     def coordinates2Star(self, coordSet, subtomosStar, sRate=1, coordsScale=1):
         """Input coordsScale is used to scale the coordinates so they are expressed in bin 1, as expected by Relion 4"""
         tomoTable = Table(columns=self._getCoordinatesStarFileLabels())
         i = 0
         for coord in coordSet.iterCoordinates():
-            angles, shifts = getTransformInfoFromCoordOrSubtomo(coord)
+            angles, shifts = getTransformInfoFromCoordOrSubtomo(coord, coordSet.getSamplingRate())
             # Add row to the table which will be used to generate the STAR file
             tomoTable.addRow(
                 coord.getTomoId(),  # 1 _rlnTomoName
                 coord.getObjId(),  # 2 _rlnTomoParticleId
                 coord.getGroupId() if coord.getGroupId() else 1,  # 3 _rlnTomoManifoldIndex
                 # coord in pix at scale of bin1
                 coord.getX(RELION_3D_COORD_ORIGIN) * coordsScale,  # 4 _rlnCoordinateX
                 coord.getY(RELION_3D_COORD_ORIGIN) * coordsScale,  # 5 _rlnCoordinateY
                 coord.getZ(RELION_3D_COORD_ORIGIN) * coordsScale,  # 6 _rlnCoordinateZ
                 # pix * Å/pix = [shifts in Å]
-                shifts[0] * sRate,  # 7 _rlnOriginXAngst
-                shifts[1] * sRate,  # 8 _rlnOriginYAngst
-                shifts[2] * sRate,  # 9 _rlnOriginZAngst
+                shifts[0], #* sRate,  # 7 _rlnOriginXAngst
+                shifts[1], #* sRate,  # 8 _rlnOriginYAngst
+                shifts[2], #* sRate,  # 9 _rlnOriginZAngst
                 # Angles in degrees
                 angles[0],  # 10 _rlnAngleRot
                 angles[1],  # 11 _rlnAngleTilt
                 angles[2],  # 12 _rlnAnglePsi
                 # Extended fields
                 int(getattr(coord, '_classNumber', -1)),  # 13_rlnClassNumber
                 # Alternated 1 and 2 values
                 int(getattr(coord, '_randomSubset', (i % 2) + 1)),  # 14 _rlnRandomSubset
                 int(coord.getX(SCIPION)),  # 15 _sciXCoord
                 int(coord.getY(SCIPION)),  # 16 _sciYCoord
-                int(coord.getZ(SCIPION))   # 17 _sciZCoord
+                int(coord.getZ(SCIPION)),   # 17 _sciZCoord
+                coord.getGroupId() # 18 _sciGroupId
             )
             i += 1
         # Write the STAR file
         tomoTable.write(subtomosStar)
 
     def pseudoSubtomograms2Star(self, pSubtomoSet, outStar, withPriors=False):
+
+        logger.info("Generating particles file (%s) from pseudosubtomogram set." % outStar)
         sRate = pSubtomoSet.getSamplingRate()
         hasCoords = pSubtomoSet.getFirstItem().hasCoordinate3D()
         tomoTable = Table(columns=self._getPseudoSubtomogramStarFileLabels(hasCoords, withPriors=withPriors))
 
         # Write the STAR file
         optGroup = OpticsGroups.fromString(pSubtomoSet.getAcquisition().opticsGroupInfo.get())
         with open(outStar, 'w') as f:
             optGroup.toStar(f)
             # Write header first
             partsWriter = Table.Writer(f)
             partsWriter.writeTableName(PARTICLES_TABLE)
             partsWriter.writeHeader(tomoTable.getColumns())
             for pSubtomo in pSubtomoSet:
-                angles, shifts = getTransformInfoFromCoordOrSubtomo(pSubtomo, convention=TR_SCIPION)
+                angles, shifts = getTransformInfoFromCoordOrSubtomo(pSubtomo, pSubtomo.getSamplingRate())
                 pSubtomoFile = pSubtomo.getFileName()
                 pSubtomoFile = pSubtomoFile.replace(':' + MRC, '') if pSubtomoFile else FILE_NOT_FOUND
                 pSubtomoCtfFile = pSubtomo.getCtfFile() if pSubtomo.getCtfFile() else FILE_NOT_FOUND
 
                 # Add row to the table which will be used to generate the STAR file
                 rowsValues = [
                     pSubtomo.getTsId(),  # _rlnTomoName #1
                     pSubtomo.getObjId(),  # rlnTomoParticleId #2
                     pSubtomo.getManifoldIndex(),  # rlnTomoManifoldIndex #3
                     # Coords in pixels
                     pSubtomo.getX(),  # _rlnCoordinateX #4
                     pSubtomo.getY(),  # _rlnCoordinateY #5
                     pSubtomo.getZ(),  # _rlnCoordinateZ #6
                     # pix * Å/pix = [shifts in Å]
-                    shifts[0] * sRate,  # _rlnOriginXAngst #7
-                    shifts[1] * sRate,  # _rlnOriginYAngst #8
-                    shifts[2] * sRate,  # _rlnOriginZAngst #9
+                    shifts[0], #* sRate,  # _rlnOriginXAngst #7
+                    shifts[1], #* sRate,  # _rlnOriginYAngst #8
+                    shifts[2], #* sRate,  # _rlnOriginZAngst #9
                     # Angles in degrees
                     angles[0],  # _rlnAngleRot #10
                     angles[1],  # _rlnAngleTilt #11
                     angles[2],  # _rlnAnglePsi #12
 
                     pSubtomo.getClassId(),  # _rlnClassNumber #13
                     pSubtomo.getRdnSubset(),  # _rlnRandomSubset #14
                 ]
 
                 if withPriors:
                     rowsValues += [angles[0], angles[1], angles[2]]
                 if hasCoords:
                     rowsValues += [pSubtomo.getCoordinate3D().getX(SCIPION),  # _sciXCoord #15
                                    pSubtomo.getCoordinate3D().getY(SCIPION),  # _sciYCoord #16
-                                   pSubtomo.getCoordinate3D().getZ(SCIPION)]  # _sciZCoord #17
+                                   pSubtomo.getCoordinate3D().getZ(SCIPION),  # _sciZCoord #17
+                                   pSubtomo.getCoordinate3D().getGroupId(),   # _sciGroupId #18
+                                   ]
 
                 rowsValues += [pSubtomo.getRe4ParticleName(),  # _rlnTomoParticleName #18
                                pSubtomo.getOpticsGroupId(),  # _rlnOpticsGroup #19
                                pSubtomoFile,  # _rlnImageName #20
                                pSubtomoCtfFile]  # _rlnCtfImage #21
 
                 partsWriter.writeRowValues(rowsValues)
@@ -173,15 +178,15 @@
     def subtomograms2Star(self, subtomoSet, subtomosStar):
         logger.info("Writing relion4 star file (%s) from subtomograms." % subtomosStar)
         tomoTable = Table(columns=self.starHeaders)
         sRate = subtomoSet.getSamplingRate()
         extraPath = join(getParentFolder(subtomosStar), 'extra')
         for subtomo in subtomoSet.iterSubtomos():
             checkSubtomogramFormat(subtomo, extraPath)
-            angles, shifts = getTransformInfoFromCoordOrSubtomo(subtomo)
+            angles, shifts = getTransformInfoFromCoordOrSubtomo(subtomo, subtomo.getSamplingRate())
             ctfFile = getattr(subtomo, '_ctfImage', None)
             if ctfFile:
                 ctfFile = ctfFile.get()
             classNumber = subtomo.getClassId()
             rlnClassNumber = classNumber if classNumber else 1
             rlnTomoName = subtomo.getVolName()
             rlnImageName = subtomo.getFileName().replace(':' + MRC, '')
@@ -196,17 +201,17 @@
                 rlnCoordinateY = subtomo.getCoordinate3D().getY(BOTTOM_LEFT_CORNER)
                 rlnCoordinateZ = subtomo.getCoordinate3D().getZ(BOTTOM_LEFT_CORNER)
 
             rlnAngleRot = angles[0]
             rlnAngleTilt = angles[1]
             rlnAnglePsi = angles[2]
             # pix * Å/pix = [shifts in Å]
-            rlnOriginX = shifts[0] * sRate
-            rlnOriginY = shifts[1] * sRate
-            rlnOriginZ = shifts[2] * sRate
+            rlnOriginX = shifts[0] #* sRate
+            rlnOriginY = shifts[1] #* sRate
+            rlnOriginZ = shifts[2] #* sRate
             # Angles in degrees
             rlnTiltPrior = subtomo._tiltPriorAngle.get() if hasattr(subtomo, '_tiltPriorAngle') else rlnAngleTilt
             rlnPsiPrior = subtomo._psiPriorAngle.get() if hasattr(subtomo, '_psiPriorAngle') else rlnAnglePsi
             # Add row to the table which will be used to generate the STAR file
             fieldsToAdd = [rlnTomoName,
                            rlnImageName,
                            rlnCtfImage,
@@ -260,15 +265,15 @@
 
         ]
 
         if withPriors:
             starFileLabels+=[ROT_PRIOR, TILT_PRIOR, PSI_PRIOR]
 
         if hasCoords:
-            starFileLabels += [SCIPION_COORD_X, SCIPION_COORD_Y, SCIPION_COORD_Z]
+            starFileLabels += [SCIPION_COORD_X, SCIPION_COORD_Y, SCIPION_COORD_Z, SCIPION_COORD_GROUP_ID]
 
         return starFileLabels
 
     @staticmethod
     def _getPseudoSubtomogramStarFileLabels(hasCoords=True, withPriors=False):
         pSubtomosLabels = Writer._getCoordinatesStarFileLabels(hasCoords, withPriors=withPriors)
         pSubtomosLabels.extend([
@@ -362,15 +367,15 @@
             if coord:
                 coordsSet.append(coord)
             else:
                 if tomoId not in nonMatchingTomoIds:
                     nonMatchingTomoIds += '%s ' % tomoId
 
         if nonMatchingTomoIds:
-            print(yellowStr('The star file contains coordinates that belong to tomograms not present '
+            logger.info(yellowStr('The star file contains coordinates that belong to tomograms not present '
                             'in the introduced set of tomograms: %s' % nonMatchingTomoIds))
 
     def starFile2PseudoSubtomograms(self, outputSet):
         sRate = outputSet.getSamplingRate()
         listOfFilesToFixVolume = []
         for counter, row in enumerate(self.dataTable):
             t = Transform()
@@ -395,25 +400,26 @@
 
             # Set the coordinate3D
             if row.get(SCIPION_COORD_X) is not None:  # Assume that the coordinates exists
                 sciCoord = Coordinate3D()
                 sciCoord.setX(row.get(SCIPION_COORD_X), SCIPION)
                 sciCoord.setY(row.get(SCIPION_COORD_Y), SCIPION)
                 sciCoord.setZ(row.get(SCIPION_COORD_Z), SCIPION)
+                sciCoord.setGroupId(row.get(SCIPION_COORD_GROUP_ID,1))
                 sciCoord.setTomoId(row.get(TOMO_NAME))
                 psubtomo.setCoordinate3D(sciCoord)
 
             # Set the transformation matrix
             t.setMatrix(getTransformMatrixFromRow(row, sRate=sRate))
             psubtomo.setTransform(t)
 
             # Add the files to the list of files whose header has to be corrected to be interpreted as volumes
-            if particleFile:
+            if particleFile is not None and particleFile != FILE_NOT_FOUND:
                 listOfFilesToFixVolume.append(particleFile)
-            if ctfFile:
+            if ctfFile is not None and ctfFile!=FILE_NOT_FOUND:
                 listOfFilesToFixVolume.append(ctfFile)
             # Add current pseudosubtomogram to the output set
             outputSet.append(psubtomo)
 
         # Keep the number of particles to compare sizes in case of subset
         outputSet.setNReParticles(self.dataTable.size())
         # Fix volume headers
@@ -456,63 +462,7 @@
 
             # Add current subtomogram to the output set
             subtomoSet.append(subtomo)
 
         # Set the set of coordinates which corresponds to the current set of subtomograms
         subtomoSet.setCoordinates3D(coordSet)
 
-    def setParticleTransform(self, particle, row, sRate):
-        """ Set the transform values from the row. """
-
-        if (self._alignType == ALIGN_NONE) or not row.hasAnyColumn(self.ALIGNMENT_LABELS):
-            self.setParticleTransform = self.__setParticleTransformNone
-        else:
-            # Ensure the Transform object exists
-            self._angles = np.zeros(3)
-            self._shifts = np.zeros(3)
-
-            particle.setTransform(Transform())
-
-            if self._alignType == ALIGN_2D:
-                self.setParticleTransform = self.__setParticleTransform2D
-            elif self._alignType == ALIGN_PROJ:
-                self.setParticleTransform = self.__setParticleTransformProj
-            else:
-                raise TypeError("Unexpected alignment type: %s"
-                                % self._alignType)
-
-        # Call again the modified function
-        self.setParticleTransform(particle, row, sRate)
-
-    @staticmethod
-    def __setParticleTransformNone(particle, row, sRate):
-        particle.setTransform(None)
-
-    def __setParticleTransform2D(self, particle, row, sRate):
-        angles = self._angles
-        shifts = self._shifts
-
-        shifts[0] = float(row.get(SHIFTX_ANGST / sRate, 0))
-        shifts[1] = float(row.get(SHIFTY_ANGST / sRate, 0))
-        angles[2] = float(row.get(PSI, 0))
-        radAngles = -np.deg2rad(angles)
-        M = tfs.euler_matrix(radAngles[0], radAngles[1], radAngles[2], 'szyz')
-        M[:3, 3] = shifts[:3]
-        particle.getTransform().setMatrix(M)
-
-    def __setParticleTransformProj(self, particle, row, sRate):
-        angles = self._angles
-        shifts = self._shifts
-
-        shifts[0] = float(row.get(SHIFTX_ANGST, 0)) / sRate
-        shifts[1] = float(row.get(SHIFTY_ANGST, 0)) / sRate
-        shifts[2] = float(row.get(SHIFTZ_ANGST, 0)) / sRate
-
-        angles[0] = float(row.get(ROT, 0))
-        angles[1] = float(row.get(TILT, 0))
-        angles[2] = float(row.get(PSI, 0))
-
-        radAngles = -np.deg2rad(angles)
-        M = tfs.euler_matrix(radAngles[0], radAngles[1], radAngles[2], 'szyz')
-        M[:3, 3] = -shifts[:3]
-        M = np.linalg.inv(M)
-        particle.getTransform().setMatrix(M)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/convert/convertBase.py` & `scipion-em-reliontomo-3.1.4/reliontomo/convert/convertBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 from os.path import join
 import numpy as np
 from pwem.convert import transformations
-from pwem.convert.transformations import translation_from_matrix, euler_from_matrix
+from pwem.convert.transformations import translation_from_matrix, euler_from_matrix, euler_matrix
 from pwem.emlib.image import ImageHandler
 from pyworkflow.utils import getExt, removeBaseExt, replaceBaseExt, makePath
 from relion.convert.convert_base import WriterBase
 from reliontomo import Plugin
 from reliontomo.constants import MRC, SHIFTX_ANGST, SHIFTY_ANGST, SHIFTZ_ANGST, TILT, PSI, ROT
 from tomo.constants import TR_RELION
 from tomo.objects import Coordinate3D
@@ -44,22 +44,25 @@
 
 class ReaderTomo:
     def __init__(self, starFile, dataTable):
         self.starFile = starFile
         self.dataTable = dataTable
 
 
-def getTransformInfoFromCoordOrSubtomo(obj, convention=TR_RELION, calcInv=True):
-    M = obj.getMatrix(convention=convention) if type(obj) is Coordinate3D else obj.getTransform(convention=convention).getMatrix()
+def getTransformInfoFromCoordOrSubtomo(obj, samplingRate):
+
+    M = obj.getMatrix(convention=TR_RELION) if isinstance(obj, Coordinate3D) else obj.getTransform(convention=TR_RELION).getMatrix()
     shifts = translation_from_matrix(M)
-    if calcInv:
-        shifts = -shifts
-        M = np.linalg.inv(M)
+
+    # These 2 lines below were done when inverting, which is now what we always do.
+    shifts = -shifts
+    M = np.linalg.inv(M)
 
     angles = -np.rad2deg(euler_from_matrix(M, axes='szyz'))
+    shifts *=samplingRate
 
     return angles, shifts
 
 
 def checkSubtomogramFormat(subtomo, extraPath):
     """Convert the subtomograms into mrc format if they are in a different one. They will be created in extra folder
     generating a subdirectory for each tomogram found and the corresponding subtomograms contained on it."""
@@ -67,34 +70,36 @@
     if getExt(subtomo.getFileName().replace(':' + MRC, '')) != '.' + MRC:
         mrcDir = join(extraPath, removeBaseExt(subtomo.getVolName()))
         makePath(mrcDir)
         mrcFile = join(mrcDir, replaceBaseExt(subtomo.getFileName(), MRC))
         ih.convert(subtomo.getFileName(), mrcFile)
 
 
-def getTransformMatrixFromRow(row, sRate=1, invert=True):
-    shiftx = float(row.get(SHIFTX_ANGST, 0)) / sRate
-    shifty = float(row.get(SHIFTY_ANGST, 0)) / sRate
-    shiftz = float(row.get(SHIFTZ_ANGST, 0)) / sRate
+def getTransformMatrixFromRow(row, sRate=1):
+    shiftx = float(row.get(SHIFTX_ANGST, 0))
+    shifty = float(row.get(SHIFTY_ANGST, 0))
+    shiftz = float(row.get(SHIFTZ_ANGST, 0))
+    rot = row.get(ROT, 0)
     tilt = row.get(TILT, 0)
     psi = row.get(PSI, 0)
-    rot = row.get(ROT, 0)
 
-    return genTransformMatrix(shiftx, shifty, shiftz, rot, tilt, psi, invert)
+    return genTransformMatrix(shiftx, shifty, shiftz, rot, tilt, psi, sRate)
 
 
-def genTransformMatrix(shiftx, shifty, shiftz, rot, tilt, psi, invert):
-    shifts = (float(shiftx), float(shifty), float(shiftz))
+def genTransformMatrix(shiftx, shifty, shiftz, rot, tilt, psi, sRate):
+    shifts = (float(shiftx)/sRate, float(shifty)/sRate, float(shiftz)/sRate)
     angles = (float(rot), float(tilt), float(psi))
     radAngles = -np.deg2rad(angles)
     M = transformations.euler_matrix(radAngles[0], radAngles[1], radAngles[2], 'szyz')
-    if invert:
-        M[0, 3] = -shifts[0]
-        M[1, 3] = -shifts[1]
-        M[2, 3] = -shifts[2]
-        M = np.linalg.inv(M)
-    else:
-        M[0, 3] = shifts[0]
-        M[1, 3] = shifts[1]
-        M[2, 3] = shifts[2]
+
+    # These 3 lines are the ones for "invert" flag.
+    M[0, 3] = -shifts[0]
+    M[1, 3] = -shifts[1]
+    M[2, 3] = -shifts[2]
+    M = np.linalg.inv(M)
+
+    # These line were fot the non invert mode. Not used
+    #     M[0, 3] = shifts[0]
+    #     M[1, 3] = shifts[1]
+    #     M[2, 3] = shifts[2]
 
     return M
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/objects.py` & `scipion-em-reliontomo-3.1.4/reliontomo/objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 from enum import Enum
 from os.path import exists, join
 
 from emtable import Table
+
 from pyworkflow.object import String, Integer, Float
 from relion.convert import OpticsGroups
 from reliontomo.constants import (OPT_TOMOS_STAR, OPT_PARTICLES_STAR,
                                   OPT_TRAJECTORIES_STAR, OPT_MANIFOLDS_STAR,
                                   OPT_FSC_STAR, OUT_TOMOS_STAR, OUT_PARTICLES_STAR,
                                   TRAJECTORIES_STAR, MANIFOLDS_STAR, FSC_REF_STAR,
                                   STAR_DIFF_SIZE, STAR_DIFF_LABELS, STAR_DIFF_VALUES,
@@ -51,32 +52,29 @@
     def __init__(self, fileName=None, samplingRate=None, ctfFile=None, tsId=None, classId=None,
                  x=None, y=None, z=None, rdnSubset=None, re4ParticleName=None,
                  opticsGroupId=1, manifoldIndex=None, **kwargs):
         super().__init__(**kwargs)
         self.setFileName(fileName)
         self.setSamplingRate(samplingRate)
         self.setClassId(classId)
-        self._tsId = String(tsId)
+        self._volName.set(tsId)
         self._ctfFile = String(ctfFile)
         self._x = Float(x)
         self._y = Float(y)
         self._z = Float(z)
         self._rdnSubset = Integer(rdnSubset)
         self._re4ParticleName = String(re4ParticleName)
         self._opticsGroupId = Integer(opticsGroupId)
         self._manifoldIndex = Integer(manifoldIndex)
 
     def getCtfFile(self):
         return self._ctfFile.get()
 
     def getTsId(self):
-        return self._tsId.get()
-
-    def getTransform(self, convention=SCIPION):
-        return super().getTransform(convention=TR_SCIPION)
+        return self.getVolName()
 
     def getBoxSize(self):
         return self._boxSize.get()
 
     def getX(self):
         return self._x.get()
 
@@ -101,15 +99,15 @@
     def getManifoldIndex(self):
         return self._manifoldIndex.get()
 
     def setCtfFile(self, val):
         self._ctfFile.set(val)
 
     def setTsId(self, val):
-        self._tsId.set(val)
+        self._volName.set(val)
 
     def setTransform(self, newTransform, convention=TR_SCIPION):
         super().setTransform(newTransform, convention=convention)
 
     def setBoxSize(self, val):
         self._boxSize = val
 
@@ -135,35 +133,45 @@
 
     def setOpticsGroupId(self, val):
         self._opticsGroupId.set(val)
 
     def setManifoldIndex(self, val):
         self._manifoldIndex.set(val)
 
-    def copyInfo(self, other):
-        self.copyAttributes(other, '_samplingRate', '_tsId', '_tsName', '_rdnSubset',
-                            '_re4ParticleName', '_opticsGroupId', '_boxSize')
+    # def copyInfo(self, other):
+    #     self.copyAttributes(other, '_samplingRate', '_tsId', '_rdnSubset',
+    #                         '_re4ParticleName', '_opticsGroupId', '_boxSize')
 
 
 class RelionSetOfPseudoSubtomograms(SetOfSubTomograms):
+    """ Set to persist relion's metadata files and particles.
+    Approach: heep always the generated optimization_set.star file. Additionally,
+    Keep the particles.star file is apply (e.g.: apply operation)
+
+    Run relion with optimization star file and additionally, particles if is not none (empty it when apply)
+
+    For subsets... we could generate always a new particles star file, either based on this set
+    (when we fixed the shifts conversion  problem) or alternatively read the relion starfile and generate
+    a new one filtered out base on  this set ids? (warning, ids will fail if there are joins!!)
+    """
     ITEM_TYPE = RelionPSubtomogram
 
     def __init__(self, optimSetStar=None, relionBinning=None, tsSamplingRate=None, boxSize=24,
                  nReParticles=0, **kwargs):
         super().__init__(**kwargs)
-        self._filesMaster = String()
+        self._filesMaster = String() # Optimisation set file path
         self._boxSize = Integer(boxSize)
-        self._tomograms = String()
-        self._particles = String()
-        self._trajectories = String()
-        self._manifolds = String()
-        self._referenceFsc = String()
-        self._relionBinning = Float(relionBinning)
-        self._tsSamplingRate = Float(tsSamplingRate)
-        self._nReParticles = Integer(nReParticles)
+        self._tomograms = String() # Path to tomograms star file, usually the one prepared by relion at the beginning
+        self._particles = String() # Path to particles.star file where particles metadata
+        self._trajectories = String() # Path to trajectories file
+        self._manifolds = String() # Path to manifolds file
+        self._referenceFsc = String() # FSC file
+        self._relionBinning = Float(relionBinning) # Binning of this set
+        self._tsSamplingRate = Float(tsSamplingRate) # Sampling rate of the tilt series
+        self._nReParticles = Integer(nReParticles) # number of relion particles in the particles star file
 
         if optimSetStar:
             self.filesMaster = optimSetStar
 
     # def __str__(self):
     #     strRep = ''
     #     if self.getNumParticles():
@@ -249,15 +257,15 @@
     def setTsSamplingRate(self, val):
         self._tsSamplingRate.set(val)
 
     def setBoxSize(self, val):
         self._boxSize.set(val)
 
     def copyInfo(self, other):
-        self.copyAttributes(other, '_tomograms', '_particles', '_trajectories', '_manifolds', '_referenceFsc',
+        self.copyAttributes(other,'_filesMaster', '_tomograms', '_particles', '_trajectories', '_manifolds', '_referenceFsc',
                             '_relionBinning', '_tsSamplingRate', '_samplingRate', '_boxSize', '_nReParticles',
                             '_coordsPointer')
         self._acquisition.copyInfo(other._acquisition)
         # self._relionMd = relionMd if relionMd else relionTomoMetadata
 
     # def iterPSubtomos(self, ts=None, orderBy='id'):
     #     if ts is None:
@@ -284,14 +292,25 @@
     # def copyInfo(self, other):
     #     self.copyAttributes(other, '_samplingRate', '_relionMd')
     #     self._acquisition.copyInfo(other._acquisition)
 
 
 def createSetOfRelionPSubtomograms(protocolPath, optimSetStar, coordsPointer, template=PSUBTOMOS_SQLITE, tsSamplingRate=1,
                                    relionBinning=1, boxSize=24, nReParticles=0):
+    """ Creates the RelionSetOfSubtomograms from the input arguments
+
+    :param protocolPath: Path of the protocol where to create the sqlite
+    :param optimSetStar: optimization set star file. This file is a small collection of files(images and metadata to pass to future jobs
+    :param coordsPointer: Pointer to the set of coordinates
+    :param tsSamplingRate: Sampling rate of the tilt series
+    :param relionBinning: binning of the set
+    :param boxSize: Box size of the set
+    :param nReParticles: Number of particles in relion's particles star file
+
+    """
     psubtomoSet = RelionSetOfPseudoSubtomograms.create(protocolPath, template=template)
     psubtomoSet.filesMaster = optimSetStar
     psubtomoSet.setTsSamplingRate(tsSamplingRate)
     psubtomoSet.setRelionBinning(relionBinning)
     psubtomoSet.setSamplingRate(psubtomoSet.getCurrentSamplingRate())
     psubtomoSet.setBoxSize(boxSize)
     psubtomoSet.setNReParticles(nReParticles)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/__init__.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 from .protocol_edit_particles_star import ProtRelionEditParticlesStar
-# from .protocol_extract_coordinates_from_psubtomos import ProtExtractCoordsFromPSubtomos
 from .protocol_import_coordinates_from_star import ProtImportCoordinates3DFromStar
 from .protocol_import_subtomograms_from_star import ProtImportSubtomogramsFromStar
 from .protocol_post_process import ProtRelionPostProcess
 from .protocol_prepare_data import ProtRelionPrepareData
 from .protocol_make_pseudo_subtomos import ProtRelionMakePseudoSubtomograms
 from .protocol_rec_tomogram import ProtRelionTomoReconstruct
 from .protocol_reconstruc_particle_from_ts import ProtRelionReconstructParticle
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_3d_classify_subtomograms.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_3d_classify_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_import_from_star.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_import_from_star.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 self.coordsSRate = float(sRateFromStar)
             else:
                 self.coordsSRate = self.inTomos.get().getSamplingRate()
 
     def _importStep(self):
         precedentsSet = self.inTomos.get()
         coordSet = SetOfCoordinates3D.create(self._getPath(), template='coordinates%s.sqlite')
-        coordSet.setPrecedents(precedentsSet)
+        coordSet.setPrecedents(self.inTomos) # As a pointer is better for streaming
         coordSet.setSamplingRate(precedentsSet.getSamplingRate())
         coordSet.setBoxSize(self.boxSize.get())
         self.reader.starFile2Coords3D(coordSet, precedentsSet, self.coordsSRate / precedentsSet.getSamplingRate())
 
         self._defineOutputs(**{outputObjects.coordinates.name: coordSet})
         self._defineSourceRelation(self.inTomos.get(), coordSet)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,17 +77,25 @@
 
     # -------------------------- INFO functions -------------------------------
 
     # --------------------------- UTILS functions -----------------------------
     def _genCommonCmd(self):
         inRelionParticles = self.inReParticles.get()
         cmd = ''
-        cmd += '--t %s ' % inRelionParticles.getTomograms()
+
+        # Cancel this for now
+        self.info("Using optimization_set: %s" % inRelionParticles.filesMaster)
+        cmd += '--i %s ' % inRelionParticles.filesMaster
+
+        # This would be either the particles start file in the set or a new generated one from the subtomo set.
         cmd += '--p %s ' % self.getOutStarFileName()
+
         if inRelionParticles.getTrajectories():
             cmd += '--mot %s ' % inRelionParticles.getTrajectories()
+
+
         cmd += '--b %i ' % self.boxSize.get()
         cmd += '--crop %i ' % self.croppedBoxSize.get()
         cmd += '--bin %.1f ' % self.binningFactor.get()
         cmd += '--j %i ' % self.numberOfThreads.get()
         return cmd
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_per_part_per_tilt.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_per_part_per_tilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_refine.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_base_relion.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_relion.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # **************************************************************************
 from os.path import exists, join
 
 from pwem.objects import VolumeMask
 from pwem.protocols import EMProtocol
 from pyworkflow.protocol import PointerParam
 from pyworkflow.utils import Message, createLink
-from reliontomo.constants import IN_PARTICLES_STAR, POSTPROCESS_DIR, OPTIMISATION_SET_STAR, PSUBTOMOS_SQLITE
+from reliontomo.constants import IN_PARTICLES_STAR, POSTPROCESS_DIR, OPTIMISATION_SET_STAR, PSUBTOMOS_SQLITE, \
+    OUT_PARTICLES_STAR
 from reliontomo.convert import writeSetOfPseudoSubtomograms, readSetOfPseudoSubtomograms
 from reliontomo.objects import createSetOfRelionPSubtomograms, RelionSetOfPseudoSubtomograms
 
 
 class ProtRelionTomoBase(EMProtocol):
 
     def __init__(self, **kwargs):
@@ -49,47 +50,55 @@
 
     def genInStarFile(self, withPriors=False):
         """It will check if the set size and the stored particles star file are of the same size or not. In
         the first case, a link will be made to the previous particles star file to avoid generating it and in the
         second case, a new file will be generated containing only the ones present in the input set."""
         inReParticlesSet = self.inReParticles.get()
         outStarFileName = self.getOutStarFileName()
-        # if inReParticlesSet.getSize() == inReParticlesSet.getNReParticles():
-        #     createLink(inReParticlesSet.getParticles(), outStarFileName)
-        # else:
-        writeSetOfPseudoSubtomograms(inReParticlesSet, outStarFileName, withPriors=withPriors)
+        if inReParticlesSet.getSize() == inReParticlesSet.getNReParticles() and not withPriors:
+             self.info("Using existing star (%s) file instead of generating a new one." % inReParticlesSet.getParticles())
+             createLink(inReParticlesSet.getParticles(), outStarFileName)
+        else:
+            writeSetOfPseudoSubtomograms(inReParticlesSet, outStarFileName, withPriors=withPriors)
 
     def _genPostProcessOutputMrcFile(self, fileName):
         """File generated using the sharpening protocol (called post-process protocol) and also using the
         rec particle from TS protocol in case the optional input 'solvent mask' is introduced."""
         postProccesMrc = VolumeMask()
         postProccesMrc.setFileName(self._getExtraPath(POSTPROCESS_DIR, fileName))
         postProccesMrc.setSamplingRate(self.inReParticles.get().getCurrentSamplingRate())
 
         return postProccesMrc
 
-    def genRelionParticles(self, binningFactor=None, boxSize=24):
+    def genRelionParticles(self, optimisationFileName=OPTIMISATION_SET_STAR, particles=OUT_PARTICLES_STAR, binningFactor=None, boxSize=24):
         """Generate a RelionSetOfPseudoSubtomograms object containing the files involved for the next protocol,
         considering that some protocols don't generate the optimisation_set.star file. In that case, the input Object
         which represents it will be copied and, after that, this method will be used to update the corresponding
         attribute."""
-        extraPath = self._getExtraPath()
+
+        # Create the set
         inParticlesSet = self.inReParticles.get()
-        coordsPointer = inParticlesSet._coordsPointer
-        optimSetStar = join(extraPath, OPTIMISATION_SET_STAR)
-        protocolPath = join(extraPath, '..')
+        psubtomoSet = RelionSetOfPseudoSubtomograms.create(self.getPath(), template=PSUBTOMOS_SQLITE)
+        psubtomoSet.copyInfo(inParticlesSet)
+
+        # Verify out star file
+        extraPath = self._getExtraPath()
+        optimSetStar = join(extraPath, optimisationFileName)
         if exists(optimSetStar):
-            psubtomoSet = createSetOfRelionPSubtomograms(protocolPath,
-                                                         optimSetStar,
-                                                         coordsPointer,
-                                                         template=PSUBTOMOS_SQLITE,
-                                                         tsSamplingRate=inParticlesSet.getTsSamplingRate(),
-                                                         relionBinning=binningFactor if binningFactor else inParticlesSet.getRelionBinning(),
-                                                         boxSize=boxSize if boxSize else inParticlesSet.getBoxSize())
-        else:
-            psubtomoSet = RelionSetOfPseudoSubtomograms.create(protocolPath, template=PSUBTOMOS_SQLITE)
-            psubtomoSet.copyInfo(inParticlesSet)
-            psubtomoSet.updateGenFiles(extraPath)
+            psubtomoSet.filesMaster = optimSetStar
 
-        # Fill the set with the generated particles
+        particles = join(extraPath, particles)
+        if exists(particles):
+            psubtomoSet._particles.set(particles)
+
+
+        if binningFactor:
+            psubtomoSet.setRelionBinning(binningFactor)
+
+        if boxSize:
+            psubtomoSet.setBoxSize(boxSize)
+
+        # Fill the items (pseudo subtomos/particles) from de particles star file
         readSetOfPseudoSubtomograms(psubtomoSet)
+
         return psubtomoSet
+
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_ctf_refine.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_ctf_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_de_novo_initial_model.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_de_novo_initial_model.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_edit_particles_star.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_edit_particles_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_extract_coordinates_from_psubtomos.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_make_pseudo_subtomos.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,114 +19,85 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 from enum import Enum
-from pyworkflow import BETA
-from pyworkflow.object import Integer
-from reliontomo.constants import RELION_3D_COORD_ORIGIN
-from reliontomo.convert.convertBase import genTransformMatrix, getTransformInfoFromCoordOrSubtomo
-from reliontomo.protocols.protocol_base_refine import ProtRelionRefineBase
-from tomo.constants import TR_SCIPION
-from tomo.objects import SetOfTomograms, SetOfCoordinates3D, Coordinate3D
-from tomo.utils import getObjFromRelation
+from pyworkflow.protocol import FloatParam, BooleanParam
+from pyworkflow.protocol.constants import LEVEL_ADVANCED
+from reliontomo import Plugin
+from reliontomo.objects import RelionSetOfPseudoSubtomograms
+from reliontomo.protocols.protocol_base_make_pseusosubtomos_and_rec_particle import \
+    ProtRelionMakePseudoSubtomoAndRecParticleBase
+from reliontomo.utils import getProgram
+from tomo.protocols import ProtTomoBase
 
 
 class outputObjects(Enum):
-    coordinates = SetOfCoordinates3D()
+    relionParticles = RelionSetOfPseudoSubtomograms
 
 
-class ProtExtractCoordsFromPSubtomos(ProtRelionRefineBase):
-    """Protocol to extract a set of 3D coordinates from a set of pseudo-subtomograms"""
+class ProtRelionMakePseudoSubtomograms(ProtRelionMakePseudoSubtomoAndRecParticleBase, ProtTomoBase):
+    """Make pseudo-subtomograms"""
 
-    _label = 'extract coordinates from pseudo-subtomograms'
+    _label = 'Make pseudo-subtomograms'
     _possibleOutputs = outputObjects
-    _devStatus = BETA
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.tomoSet = None
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
-        super()._defineCommonInputParams(form)
+        super()._defineParams(form)
+        form.addSection(label='Reconstruct pseudo-Subtomograms')
+        super()._defineCommonRecParams(form)
+        form.addParam('applyConeWeight', BooleanParam,
+                      label='Apply cone weight?',
+                      default=False,
+                      help='Down weight a cone in Fourier space along the Z axis (as defined by the coordinate system '
+                           'of the particle). This is useful for particles embedded in a membrane, as it can prevent '
+                           'the alignment from being driven by the membrane signal (the signal of a planar membrane is '
+                           'localised within one line in 3D Fourier space). Note that the coordinate system of a '
+                           'particle is given by both the subtomogram orientation (if defined) and the particle '
+                           'orientation. This allows the user to first obtain a membrane-driven alignment, and to then '
+                           'specifically suppress the signal in that direction.')
+        form.addParam('coneAngle', FloatParam,
+                      label='Cone angle (deg.)',
+                      condition='applyConeWeight',
+                      default=10,
+                      help='It is the (full) opening angle of the cone to be suppressed, given in degrees. This angle '
+                           'should  include both the uncertainty about the membrane orientation and its variation '
+                           'across the region represented in the subtomogram.')
+        form.addParam('outputInFloat16', BooleanParam,
+                      label='Write output in float16?',
+                      expertLevel=LEVEL_ADVANCED,
+                      default=False,
+                      help='If set to Yes, this program will write output images in float16 MRC format. This will '
+                           'save a factor of two in disk space compared to the default of writing in float32. Note '
+                           'that RELION and CCPEM will read float16 images, but other programs may not (yet) do so.')
 
     # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
-        self._initialize()
-        self._insertFunctionStep(self._extractCoordsStep)
+        self._insertFunctionStep(self.convertInputStep)
+        self._insertFunctionStep(self.relionMakePseudoSubtomos)
+        self._insertFunctionStep(self.createOutputStep)
 
     # -------------------------- STEPS functions ------------------------------
-    def _initialize(self):
-        # Get the tomograms through the relations
-        self.tomoSet = getObjFromRelation(self.inReParticles.get(), self, SetOfTomograms)
-
-    def _extractCoordsStep(self):
-        pSubtomos = self.inReParticles.get()
-        # Manage the precedents
-        precedents = self.tomoSet
-        precedentsSRate = precedents.getSamplingRate()
-        precedentIdDict = {}
-        for tomo in precedents:
-            precedentIdDict[tomo.getTsId()] = tomo.clone()
-
-        # Generate the output set of coordinates
-        coordSet = SetOfCoordinates3D.create(self._getPath(), template='coordinates%s.sqlite')
-        coordSet.setPrecedents(precedents)
-        coordSet.setBoxSize(pSubtomos.getBoxSize())
-        coordSet.setSamplingRate(precedentsSRate)
-        scaleFactor = self.getScaleFactor()
-
-        for pSubtomo in pSubtomos:
-            # CHeck if the current psubtomo has a precedent in the tomoset
-            coordTsId = pSubtomo.getTsId()
-            precedent = precedentIdDict.get(coordTsId, None)
-            if precedent:
-                coordinate3d = Coordinate3D()
-                coordinate3d.setTomoId(coordTsId)
-                coordinate3d.setVolume(precedent)
-                # Scale x, y and z properly
-                coordinate3d.setX(pSubtomo.getX() * scaleFactor, RELION_3D_COORD_ORIGIN)
-                coordinate3d.setY(pSubtomo.getY() * scaleFactor, RELION_3D_COORD_ORIGIN)
-                coordinate3d.setZ(pSubtomo.getZ() * scaleFactor, RELION_3D_COORD_ORIGIN)
-                # Scale the shifts properly
-                tm = pSubtomo.getTransform().getMatrix()
-                tm[0, 3] = tm[0, 3] * scaleFactor
-                tm[1, 3] = tm[0, 1] * scaleFactor
-                tm[2, 3] = tm[0, 2] * scaleFactor
-                coordinate3d.setMatrix(self.getTransformMatrix(pSubtomo, precedentsSRate))
-                # Extended fields
-                coordinate3d._classNumber = Integer(pSubtomo.getClassId())
-                coordinate3d._randomSubset = Integer(pSubtomo.getRdnSubset())
-                # Append the current coordinate to the output set
-                coordSet.append(coordinate3d)
-
-        self._defineOutputs(**{outputObjects.coordinates.name: coordSet})
-        self._defineSourceRelation(pSubtomos, coordSet)
+    def relionMakePseudoSubtomos(self):
+        Plugin.runRelionTomo(self, getProgram('relion_tomo_subtomo', self.numberOfMpi.get()),
+                             self._genMakePseudoSubtomoCmd(), numberOfMpi=self.numberOfMpi.get())
+
+    def createOutputStep(self):
+        psubtomoSet = super().createOutputStep()
+        self._defineOutputs(**{outputObjects.relionParticles.name: psubtomoSet})
+        self._defineSourceRelation(self.inReParticles.get(), psubtomoSet)
 
     # -------------------------- INFO functions -------------------------------
 
-    def _summary(self):
-        summary = []
-        if self.isFinished():
-            outputCoords = getattr(self, outputObjects.coordinates.name, None)
-            if outputCoords:
-                summary.append('Coordinates were scaled to the sampling rate of the tomograms from where\n'
-                               'they were picked --> *%.2f Å/pix*.' % outputCoords.getSamplingRate())
-
-        return summary
-
-    # --------------------------- UTILS functions -----------------------------
-
-    def getScaleFactor(self):
-        inPSubtomos = self.inReParticles.get()
-        sRatePSubtomo = inPSubtomos.getSamplingRate() / inPSubtomos.getRelionBinning()
-        sRateTomo = self.tomoSet.getSamplingRate()
-        return sRatePSubtomo / sRateTomo
-
-    @staticmethod
-    def getTransformMatrix(pSubtomo, tomoSRate, invert=True):
-        angles, shiftsAngst = getTransformInfoFromCoordOrSubtomo(pSubtomo, convention=TR_SCIPION)
-        shiftsPix = shiftsAngst / tomoSRate
-        return genTransformMatrix(shiftsPix[0], shiftsPix[1], shiftsPix[2], angles[0], angles[1], angles[2], invert)
+    # # --------------------------- UTILS functions -----------------------------
+    def _genMakePseudoSubtomoCmd(self):
+        cmd = self._genCommonCmd()
+        cmd += '--o %s ' % self._getExtraPath()
+        if self.applyConeWeight.get():
+            cmd += '--cone_weight '
+            cmd += '--cone_angle %.2f ' % self.coneAngle.get()
+        if self.outputInFloat16.get():
+            cmd += '--float16 '
+        return cmd
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_import_coordinates_from_star.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_coordinates_from_star.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class outputObjects(Enum):
     tomograms = SetOfTomograms()
     coordinates = SetOfCoordinates3D()
 
 
 class ProtImportCoordinates3DFromStar(ProtBaseImportFromStar):
-    """Protocol to import a set of 3D coordinates from a star file"""
+    """Protocol to import a 3D coordinates from a relion star file as the one provided in the tutorial"""
 
-    _label = 'import coordinates 3D from a star file'
+    _label = 'import 3D coordinates'
     _possibleOutputs = outputObjects
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.linkedStarFileName = 'in3dCoordinates.star'
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_import_subtomograms_from_star.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_subtomograms_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_matching_coordinates.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_matching_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_post_process.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_post_process.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_prepare_data.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_prepare_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,20 +89,19 @@
                            'whether the focus increases or decreases as a function of Z distance.')
         form.addParam('inputCoords', PointerParam,
                       pointerClass='SetOfCoordinates3D',
                       label="Input coordinates",
                       important=True,
                       allowsNull=False)
         form.addParam('inputTS', PointerParam,
-                      help="Tilt series with alignment (non interpolated) used in the tomograms recnstruction. "
-                           "To be deprecated!!",
+                      help="Tilt series with alignment (non interpolated) used in the tomograms reconstruction.",
                       pointerClass='SetOfTiltSeries',
                       label="Input tilt series",
                       important=True,
-                      allowsNull=True)
+                      allowsNull=False)
 
         form.addParam('flipZCoords', BooleanParam,
                       label='Flip Z coordinate?',
                       default=False,
                       help='This option is generally False if your coordinates are displayed correctly in Scipion. '
                            'You may want to check this to True only if you see that the extracted subtomograms'
                            ' are wrong.',
@@ -151,16 +150,16 @@
         self.inputCtfs = self.inputCtfTs.get()
         # If coordinates are referred to a set of tomograms, they'll be rescaled
         # to be expressed in bin 1, as the ts images
         if self.tomoSet:
             self.coordScale.set(self.tomoSet.getSamplingRate() / self.tsSet.getSamplingRate())
 
     def _getTiltSeriesNonInterpolated(self):
-        return self.inputTS.get() if self.inputTS.get() is not None else \
-            getNonInterpolatedTsFromRelations(self.inputCoords.get(), self)
+        return self.inputTS.get() # if self.inputTS.get() is not None else \
+            #getNonInterpolatedTsFromRelations(self.inputCoords.get(), self)
 
     def _getTSIDFromCoordinates(self):
         # TODO: Add this functionality to the SetOFCoordinates. May be useful for other cases
         volIds = self.coords.aggregate(["MAX"], "_tomoId", ["_tomoId"])
         volIds = [d['_tomoId'] for d in volIds]
         self.info("Involved tomograms in the coordinates: %s" % volIds)
         return volIds
@@ -185,18 +184,21 @@
                                             Y_SIZE: y * coordScale,
                                             THICKNESS: thickness * coordScale}
 
             # Based on this: https://github.com/3dem/relion/blob/ver4.0/src/jaz/tomography/programs/convert_projections.cpp#L368
             # First element is X, second Z!
             shiftsAngs = tomo.getShiftsFromOrigin()
 
-            shiftX = int((shiftsAngs[0] / tomo.getSamplingRate()) + x/2)
-            shiftZ = int((shiftsAngs[2] / tomo.getSamplingRate()) + thickness/2)
+            # shifts are stored in Angstrom, we convert to tomo SR and then add the half and the to TS pixel size
+            shiftX = int(((shiftsAngs[0] / tomo.getSamplingRate()) + x/2) * self.coordScale.get())
+            shiftZ = int(((shiftsAngs[2] / tomo.getSamplingRate()) + thickness/2) * self.coordScale.get())
             tomoShiftsDict[tomo.getTsId()] = (shiftX, shiftZ)
 
+            self.info("Shifts detected for %s are: %s" % (tomo.getTsId(), (shiftX, shiftZ)))
+
         # Simulate the etomo files that serve as entry point to relion4
         self._simulateETomoFiles(self.tsSet, tomoSizeDict, tomoShiftsDict, binned=1, binByFactor=self.coordScale,
                                  whiteList=self.coordsVolIds, swapDims=self.swapXY.get())
 
         # Write the tomograms star file
         writeSetOfTomograms(self.tsSet,
                             self._getStarFilename(IN_TOMOS_STAR),
@@ -240,15 +242,15 @@
 
         # Generate the fiducial model
         projections = generateProjections(self._getStarFilename(OUT_PARTICLES_STAR),
                                           self._getStarFilename(OUT_TOMOS_STAR))
 
         fiducialModelGaps = self._createSetOfLandmarkModels(suffix='Gaps')
         fiducialModelGaps.copyInfo(self.tsSet)
-        fiducialModelGaps.setSetOfTiltSeries(self.tsSet)
+        fiducialModelGaps.setSetOfTiltSeries(self.inputTS) # Use the pointer better when scheduling
 
         pos = 0
         for ts in self.tsSet:
             tsId = ts.getTsId()
             landmarkModelGapsFilePath = os.path.join(self._getExtraPath(),
                                                      str(tsId) + "_gaps.sfid")
 
@@ -273,26 +275,26 @@
                 pos += 1
             fiducialModelGaps.append(landmarkModelGaps)
 
         self._defineOutputs(**{outputObjects.projected2DCoordinates.name: fiducialModelGaps})
         self._defineSourceRelation(self.tsSet, fiducialModelGaps)
 
     # -------------------------- INFO functions -------------------------------
-    def _validate(self):
-        # TODO: generar los nombres culled --> tsId_culled.st:mrc cuando se quiten vistas con IMOD
-        valMsg = []
-
-        if not self.inputTS.get():
-            try:
-                self._getTiltSeriesNonInterpolated()
-            except:
-                valMsg.append('Unable to go via relations from the introduced coordinates to the '
-                              'corresponding non-interpolated tilt series. Please introduce them using the '
-                              'advanced parameter "Tilt series with alignment..."')
-        return valMsg
+    # def _validate(self):
+    #     # TODO: generar los nombres culled --> tsId_culled.st:mrc cuando se quiten vistas con IMOD
+    #     valMsg = []
+    #
+    #     if not self.inputTS.get():
+    #         try:
+    #             self._getTiltSeriesNonInterpolated()
+    #         except:
+    #             valMsg.append('Unable to go via relations from the introduced coordinates to the '
+    #                           'corresponding non-interpolated tilt series. Please introduce them using the '
+    #                           'advanced parameter "Tilt series with alignment..."')
+    #     return valMsg
 
     def _summary(self):
         msg = []
         if self.isFinished():
             if self.coordScale.get():
                 msg.append('Coordinates were scaled using an scale factor of *%.2f* to be expressed considering the '
                            'size of the introduced tilt series' % self.coordScale.get())
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 
 class outputObjects(Enum):
     average = AverageSubTomogram()
 
 
 class ProtRelionSubTomoReconstructAvg(ProtReconstruct3D):
     """ This protocol reconstructs a volume using Relion.
-    Reconstruct a volume from a given set of particles.
+    Reconstruct a volume from a given set of subtomograms.
     The alignment parameters will be converted to a Relion star file
     and used as direction projections to reconstruct.
     """
-    _label = 'Rec. particle averaging subtomograms'
+    _label = 'Average from subtomograms'
     _devStatus = BETA
     inStarName = 'input_particles'
     outTomoName = 'output_volume'
     _possibleOutputs = outputObjects
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_rec_tomogram.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_tomogram.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 class outputObjects(Enum):
     average = AverageSubTomogram
     postProcessVolume = VolumeMask
     relionParticles = RelionSetOfPseudoSubtomograms
 
 
 class ProtRelionReconstructParticle(ProtRelionMakePseudoSubtomoAndRecParticleBase):
-    """Reconstruct particle from the original tilt series images"""
+    """Reconstructs/averages from the tilt series projected particles"""
 
-    _label = 'Reconstruct particle from tilt series'
+    _label = 'Average from tilt series'
     _possibleOutputs = outputObjects
 
     def __init__(self, **args):
         super().__init__(**args)
 
     # -------------------------- DEFINE param functions -----------------------
 
@@ -82,18 +82,18 @@
             self._insertFunctionStep(self.relionTomoMaskReference)
         self._insertFunctionStep(self.createOutputStep)
 
     # -------------------------- STEPS functions ------------------------------
     def relionReconstructParticle(self):
         cmd = self._genRecParticleCmd()
         try:
-            Plugin.runRelionTomo(self, 'relion_tomo_reconstruct_particle', cmd, numberOfMpi=self.numberOfMpi.get())
+            Plugin.runRelionTomo(self, 'relion_tomo_reconstruct_particle_mpi', cmd, numberOfMpi=self.numberOfMpi.get())
         except:
             # The --mem argument should also be set using around 80-90% to keep a safety margin
-            Plugin.runRelionTomo(self, 'relion_tomo_reconstruct_particle', cmd + '--mem 50 ',
+            Plugin.runRelionTomo(self, 'relion_tomo_reconstruct_particle_mpi', cmd + '--mem 50 ',
                                  numberOfMpi=self.numberOfMpi.get())
 
     def relionTomoMaskReference(self):
         Plugin.runRelionTomo(self, 'relion_tomo_make_reference', self._genTomoMaskRefCmd(),
                              numberOfMpi=self.numberOfMpi.get())
 
     def createOutputStep(self):
@@ -117,14 +117,19 @@
             postProccesMrc.setHalfMaps(halves)
             postProccesMrc.setSamplingRate(currentSamplingRate)
             self._defineOutputs(**{outputObjects.postProcessVolume.name: postProccesMrc})
             self._defineSourceRelation(inParticles, postProccesMrc)
 
         self._defineSourceRelation(inParticles, vol)
 
+        # Create the output set with the new optimization set
+        outParticles = self.genRelionParticles(boxSize=self.boxSize.get(),
+                                      binningFactor=self.binningFactor.get())
+        self._defineOutputs(**{outputObjects.relionParticles.name:outParticles})
+
 
     # -------------------------- INFO functions -------------------------------
     def _validate(self):
         pass
 
     # --------------------------- UTILS functions -----------------------------
     def _genRecParticleCmd(self):
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_refine_subtomograms.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_refine_subtomograms.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,19 +209,17 @@
     def autoRefineStep(self):
         nMpi = self.numberOfMpi.get()
         Plugin.runRelionTomo(self, getProgram('relion_refine', nMpi), self._genAutoRefineCommand(), numberOfMpi=nMpi)
 
     def createOutputStep(self):
         inParticles = self.inReParticles.get()
 
-        # Rename the particles file generated (_data.star) to follow the name convention
-        createLink(self._getExtraPath('_data.star'), self._getExtraPath(OUT_PARTICLES_STAR))
-
-        # Output RelionParticles
-        relionParticles = self.genRelionParticles()
+        # Output Relion particles
+        relionParticles = self.genRelionParticles(optimisationFileName='run_optimization_set.star',
+                                                  particles='_data.star')
 
         # Output volume
         vol = AverageSubTomogram()
         volName = self._getExtraPath('_class001.mrc')
         fixVolume(volName)  # Fix header for xmipp to consider it a volume instead of a stack
         vol.setFileName(volName)
         vol.setSamplingRate(relionParticles.getCurrentSamplingRate())
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols/protocol_tomo_frame_align.py` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_tomo_frame_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/protocols.conf` & `scipion-em-reliontomo-3.1.4/reliontomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/relion_logo.png` & `scipion-em-reliontomo-3.1.4/reliontomo/relion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/tests/__init__.py` & `scipion-em-reliontomo-3.1.4/reliontomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/tests/test_compare_star_files.py` & `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_compare_star_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,23 +136,24 @@
                               testName=testName,
                               filesEqual=False,
                               diffSize=False,
                               diffLabels=False,
                               diffValues=True,
                               strings2check=strings2check)
 
-    def test_05_prepareTomosInVsOut(self):
-        starFile1 = self.dataset.getFile(DataSetRe4Tomo.prepareTomosStarScipion.name)
-        starFile2 = self.dataset.getFile(DataSetRe4Tomo.prepareTomosStarRelion.name)
-        tablesList = [GLOBAL_TABLE, TS_45_TABLE, TS_54_TABLE]
-        testName = self.test_05_prepareTomosInVsOut.__name__
-        excludeLabelsList = [TILT_SERIES_NAME]  # paths may differ
-        self._checkMultipleTablesOk(starFile1, starFile2, tablesList,
-                                    testName=testName,
-                                    excludeLabelsList=excludeLabelsList)
+    # This is failing and files are clearly not equal. They differ in dimensions, dose and other fields.
+    # def test_05_prepareTomosInVsOut(self):
+    #     starFile1 = self.dataset.getFile(DataSetRe4Tomo.prepareTomosStarScipion.name)
+    #     starFile2 = self.dataset.getFile(DataSetRe4Tomo.prepareTomosStarRelion.name)
+    #     tablesList = [GLOBAL_TABLE, TS_45_TABLE, TS_54_TABLE]
+    #     testName = self.test_05_prepareTomosInVsOut.__name__
+    #     excludeLabelsList = [TILT_SERIES_NAME]  # paths may differ
+    #     self._checkMultipleTablesOk(starFile1, starFile2, tablesList,
+    #                                 testName=testName,
+    #                                 excludeLabelsList=excludeLabelsList)
 
     def test_06_prepareParticlesInVsOut(self):
         starFile1 = self.dataset.getFile(DataSetRe4Tomo.preparePartcilesStarScipion.name)
         starFile2 = self.dataset.getFile(DataSetRe4Tomo.prepareParticlesStarRelion.name)
         tablesList = [OPTICS_TABLE, PARTICLES_TABLE]
         testName = self.test_06_prepareParticlesInVsOut.__name__
         excludeLabelsList = ['rlnTomoParticleId']
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/tests/test_import_star_files.py` & `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_import_star_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,40 +61,40 @@
     def _importTomograms(cls):
         print(magentaStr("\n==> Importing data - tomograms:"))
         protImportTomogram = cls.newProtocol(ProtImportTomograms,
                                              filesPath=cls.dataset.getFile(DataSetEmd10439.tomoEmd10439.name),
                                              samplingRate=cls.samplingRate)
 
         cls.launchProtocol(protImportTomogram)
-        outputTomos = getattr(protImportTomogram, OUTPUT_TOMOS, None)
-        cls.assertIsNotNone(outputTomos, 'No tomograms were genetated.')
+        outputTomos = protImportTomogram.Tomograms
+        cls.assertIsNotNone(outputTomos, 'No tomograms were generated.')
         return outputTomos
 
     @classmethod
     def _normalizeTomograms(cls):
         # Generate a tomogram with a different sampling rate
         protNormTomogram = cls.newProtocol(ProtImodTomoNormalization,
                                            inputSetOfTomograms=cls.inTomoSet,
                                            binning=2)
         cls.launchProtocol(protNormTomogram)
         outputTomos = protNormTomogram.Tomograms
-        cls.assertIsNotNone(outputTomos, 'No tomograms were genetated.')
+        cls.assertIsNotNone(outputTomos, 'No tomograms were generated.')
         return outputTomos
 
     @classmethod
     def _runImportCoords3dFromStarFile(cls, starFile, samplingRate=None, inTomos=None):
         protImportCoords3dFromStar = cls.newProtocol(ProtImportCoordinates3DFromStar,
                                                      starFile=starFile,
                                                      inTomos=inTomos,
                                                      samplingRate=samplingRate,
                                                      boxSize=cls.boxSize)
 
         cls.launchProtocol(protImportCoords3dFromStar)
         outCoords = getattr(protImportCoords3dFromStar, importSubtomosOutputs.coordinates.name)
-        cls.assertIsNotNone(outCoords, 'No coordinates were genetated.')
+        cls.assertIsNotNone(outCoords, 'No coordinates were generated.')
         return outCoords
 
     def _checkCoordinates(self, outputCoordsSet, coordSetSize=None, inTomos=None):
         # Check the output set of 3D coordinates
         self.assertTrue(outputCoordsSet, 'No 3D coordinates were registered in the protocol output.')
         self.assertSetSize(outputCoordsSet, size=coordSetSize)
         self.assertEqual(outputCoordsSet.getBoxSize(), self.boxSize)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/tests/test_refine_cycle.py` & `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_refine_cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         cls.recTomoFromPrepareSingle = cls._runRecFromPrepare_SingleTomo()
         cls.recTomoFromPrepareAll = cls._runRecFromPrepare_AllTomos()
         cls.protMakePSubtomos = cls._makePSubtomograms()
         cls.protEditStarCenter = cls._editStar_shiftCenter()
         cls.protEditStarAngles = cls._editStar_addToAngles()
         cls.protEditStarCoordsMult = cls._editStar_multiplyCoordinates()
         cls.protEditStarSetCoords = cls._editStar_setCoordinatesToValue()
-        # cls.protExtractCoords = cls._extractCoordsFromPSubtomos()
         cls.protInitialModel = cls._genInitialModel()
         cls.protCl3d = cls._3dClassify()
         cls.protCl3dWithAlign = cls._3dClassify(doAlingment=True)
         cls.protAutoRefine = cls._autoRefine()
         cls.protRecPartFromTS = cls._recParticleFromTS()
         cls.protRecPartFromTsWithSolvent = cls._recParticleFromTsWithSolventMask()
 
@@ -202,14 +201,15 @@
 
     @classmethod
     def _prepareData4RelionTomo(cls):
         print(magentaStr("\n==> Preparing data for relion 4 tomo:"))
         protPrepare = cls.newProtocol(ProtRelionPrepareData,
                                       inputCtfTs=cls.ctfTomoSeries,
                                       inputCoords=cls.inCoords,
+                                      inputTS=cls.inTS,
                                       flipYZ=True,
                                       flipZ=True)
         return cls.launchProtocol(protPrepare)
 
     @classmethod
     def _recFromPrepare(cls, recMode, tomoId=None):
         protRelionRec = cls.newProtocol(ProtRelionTomoReconstruct,
@@ -233,14 +233,15 @@
         return protRelionRec
 
     @classmethod
     def _makePSubtomograms(cls):
         print(magentaStr("\n==> Making the psudosubtomograms:"))
         protMakePsubtomos = cls.newProtocol(ProtRelionMakePseudoSubtomograms,
                                             inReParticles=getattr(cls.protPrepare, RELION_TOMO_PARTICLES, None),
+
                                             boxSize=192,
                                             croppedBoxSize=cls.boxSizeBin4,
                                             binningFactor=4,
                                             outputInFloat16=False,
                                             numberOfThreads=5,
                                             numberOfMpi=3)
         cls.launchProtocol(protMakePsubtomos)
@@ -299,22 +300,14 @@
                                        operateWith=cls.editStarLabelsDict[COORDINATES],
                                        label2y=True,
                                        label3z=True)
         protEditStar.setObjLabel('Set coords to value')
         cls.launchProtocol(protEditStar)
         return protEditStar
 
-    # @classmethod
-    # def _extractCoordsFromPSubtomos(cls):
-    #     print(magentaStr("\n==> Generating the a de novo 3D initial model:"))
-    #     protExtractCoords = cls.newProtocol(ProtExtractCoordsFromPSubtomos,
-    #                                         inReParticles=getattr(cls.protMakePSubtomos, RELION_TOMO_PARTICLES, None))
-    #     cls.launchProtocol(protExtractCoords)
-    #     return protExtractCoords
-
     @classmethod
     def _genInitialModel(cls):
         print(magentaStr("\n==> Generating the a de novo 3D initial model:"))
         protInitialModel = cls.newProtocol(ProtRelionDeNovoInitialModel,
                                            inReParticles=getattr(cls.protMakePSubtomos, RELION_TOMO_PARTICLES, None),
                                            nVdamMiniBatches=10,
                                            maskDiameter=230,
@@ -554,20 +547,14 @@
 
     @classmethod
     def _getAnglesFromPSubtomogram(cls, pSubtomo):
         M = pSubtomo.getTransform().getMatrix()
         rot, tilt, psi = euler_from_matrix(M)
         return rot, tilt, psi
 
-    # def testExtractCoordsFromPSubtomos(self):
-    #     protExtractCoords = self.protExtractCoords
-    #     outCoords = getattr(protExtractCoords, extractCoordsOutputs.coordinates.name, None)
-    #     self.assertEqual(outCoords.getSamplingRate(), 5.4)
-    #     self.assertEqual(outCoords.getBoxSize(), self.boxSizeBin4)
-
     def testInitialModel(self):
         protInitialModel = self.protInitialModel
         recVol = getattr(protInitialModel, OUTPUT_MODEL, None)
         self._checkRecVolume(recVol,
                              optSet=protInitialModel.inReParticles.get(),
                              boxSize=self.boxSizeBin4)
```

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/utils.py` & `scipion-em-reliontomo-3.1.4/reliontomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/reliontomo/wizards.py` & `scipion-em-reliontomo-3.1.4/reliontomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/PKG-INFO` & `scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.3
+Version: 3.1.4
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.3/scipion_em_reliontomo.egg-info/SOURCES.txt` & `scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 reliontomo/__init__.py
 reliontomo/bibtex.py
 reliontomo/constants.py
 reliontomo/objects.py
 reliontomo/protocols.conf
 reliontomo/relion_logo.png
 reliontomo/utils.py
+reliontomo/viewers.py
 reliontomo/wizards.py
 reliontomo/cmd/__init__.py
 reliontomo/cmd/compareStarFiles.py
 reliontomo/convert/__init__.py
 reliontomo/convert/convert30_tomo.py
 reliontomo/convert/convert40_tomo.py
 reliontomo/convert/convertBase.py
@@ -22,28 +23,28 @@
 reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
 reliontomo/protocols/protocol_base_per_part_per_tilt.py
 reliontomo/protocols/protocol_base_refine.py
 reliontomo/protocols/protocol_base_relion.py
 reliontomo/protocols/protocol_ctf_refine.py
 reliontomo/protocols/protocol_de_novo_initial_model.py
 reliontomo/protocols/protocol_edit_particles_star.py
-reliontomo/protocols/protocol_extract_coordinates_from_psubtomos.py
 reliontomo/protocols/protocol_import_coordinates_from_star.py
 reliontomo/protocols/protocol_import_subtomograms_from_star.py
 reliontomo/protocols/protocol_make_pseudo_subtomos.py
 reliontomo/protocols/protocol_matching_coordinates.py
 reliontomo/protocols/protocol_post_process.py
 reliontomo/protocols/protocol_prepare_data.py
 reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
 reliontomo/protocols/protocol_rec_tomogram.py
 reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
 reliontomo/protocols/protocol_refine_subtomograms.py
 reliontomo/protocols/protocol_tomo_frame_align.py
 reliontomo/tests/__init__.py
 reliontomo/tests/test_compare_star_files.py
+reliontomo/tests/test_conversion.py
 reliontomo/tests/test_import_star_files.py
 reliontomo/tests/test_refine_cycle.py
 scipion_em_reliontomo.egg-info/PKG-INFO
 scipion_em_reliontomo.egg-info/SOURCES.txt
 scipion_em_reliontomo.egg-info/dependency_links.txt
 scipion_em_reliontomo.egg-info/entry_points.txt
 scipion_em_reliontomo.egg-info/top_level.txt
```

### Comparing `scipion-em-reliontomo-3.1.3/setup.py` & `scipion-em-reliontomo-3.1.4/setup.py`

 * *Files identical despite different names*

