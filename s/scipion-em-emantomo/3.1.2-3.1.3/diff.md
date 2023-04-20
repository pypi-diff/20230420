# Comparing `tmp/scipion-em-emantomo-3.1.2.tar.gz` & `tmp/scipion-em-emantomo-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-emantomo-3.1.2.tar", last modified: Thu Mar 30 13:24:56 2023, max compression
+gzip compressed data, was "scipion-em-emantomo-3.1.3.tar", last modified: Thu Apr 20 07:46:23 2023, max compression
```

## Comparing `scipion-em-emantomo-3.1.2.tar` & `scipion-em-emantomo-3.1.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.391367 scipion-em-emantomo-3.1.2/emantomo/
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.391367 scipion-em-emantomo-3.1.2/emantomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/e2converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2602 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/e2ih.py
--rw-r--r--   0 runner    (1001) docker     (123)    38295 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/eman2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/emantomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_align_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_average_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_mra_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_pca_kmeans_classify_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_boxing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_boxing_convnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_extraction_from_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_extraction_from_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_fill_mw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_subtomogram_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_template_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_tilt_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/emantomo/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20482 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/requirements/Conda_EmanCB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/requirements/Missing_Dependencies
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/emantomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/tests/test_eman_sta_classic_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/tests/test_protocols_sta_classic_emantomoextraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/tests/test_protocols_sta_classic_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/emantomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39691 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/viewers/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/emantomo/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 13:24:56.000000 scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 13:24:56.395367 scipion-em-emantomo-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-03-30 13:23:08.000000 scipion-em-emantomo-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.222027 scipion-em-emantomo-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-20 07:46:23.222027 scipion-em-emantomo-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.214027 scipion-em-emantomo-3.1.3/emantomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.214027 scipion-em-emantomo-3.1.3/emantomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/e2converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2602 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/e2ih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38295 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/eman2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.218027 scipion-em-emantomo-3.1.3/emantomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_align_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_average_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_mra_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_pca_kmeans_classify_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_boxing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_boxing_convnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_extraction_from_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_extraction_from_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_fill_mw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_subtomogram_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_template_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_tilt_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.218027 scipion-em-emantomo-3.1.3/emantomo/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20482 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/requirements/Conda_EmanCB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/requirements/Missing_Dependencies
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.218027 scipion-em-emantomo-3.1.3/emantomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/tests/test_eman_sta_classic_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/tests/test_protocols_sta_classic_emantomoextraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/tests/test_protocols_sta_classic_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.218027 scipion-em-emantomo-3.1.3/emantomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39691 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/viewers/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/emantomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:23.218027 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 07:46:23.000000 scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:46:23.222027 scipion-em-emantomo-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-20 07:44:00.000000 scipion-em-emantomo-3.1.3/setup.py
```

### Comparing `scipion-em-emantomo-3.1.2/LICENSE` & `scipion-em-emantomo-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/PKG-INFO` & `scipion-em-emantomo-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-emantomo
-Version: 3.1.2
+Version: 3.1.3
 Summary: Plugin to use EMAN2 tomography programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-emantomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-emantomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-emantomo/
```

### Comparing `scipion-em-emantomo-3.1.2/README.rst` & `scipion-em-emantomo-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/__init__.py` & `scipion-em-emantomo-3.1.3/emantomo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 from scipion.install.funcs import VOID_TGZ
 
 import emantomo.constants as emanConst
 
-__version__ = "3.1.2"
+__version__ = "3.1.3"
 _logo = "eman2_logo.png"
 _references = ['GALAZMONTOYA2015279', 'BELL201625']
 _url = "https://github.com/scipion-em/scipion-em-emantomo"
 
 
 SCRATCHDIR = pwutils.getEnvVariable('EMANTOMOSCRATCHDIR', default='/tmp/')
```

### Comparing `scipion-em-emantomo-3.1.2/emantomo/bibtex.py` & `scipion-em-emantomo-3.1.3/emantomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/constants.py` & `scipion-em-emantomo-3.1.3/emantomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/convert/__init__.py` & `scipion-em-emantomo-3.1.3/emantomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/convert/convert.py` & `scipion-em-emantomo-3.1.3/emantomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/convert/dataimport.py` & `scipion-em-emantomo-3.1.3/emantomo/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/e2converter.py` & `scipion-em-emantomo-3.1.3/emantomo/e2converter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/e2ih.py` & `scipion-em-emantomo-3.1.3/emantomo/e2ih.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/eman2_logo.png` & `scipion-em-emantomo-3.1.3/emantomo/eman2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/__init__.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_align_ts.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_align_ts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_average_subtomos.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_average_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_estimate_ctf.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_mra_refinement.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_mra_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_pca_kmeans_classify_subtomos.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_pca_kmeans_classify_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_resize_tomograms.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_resize_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_boxing.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_boxing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_boxing_convnet.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_boxing_convnet.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_extraction_from_tomo.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_extraction_from_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_extraction_from_ts.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_extraction_from_ts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_fill_mw.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_fill_mw.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_initialmodel.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_reconstruction.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_subtomogram_refinement.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_subtomogram_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_template_match.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_template_match.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols/protocol_tomo_tilt_refine.py` & `scipion-em-emantomo-3.1.3/emantomo/protocols/protocol_tomo_tilt_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/protocols.conf` & `scipion-em-emantomo-3.1.3/emantomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/requirements/Conda_EmanCB.txt` & `scipion-em-emantomo-3.1.3/emantomo/requirements/Conda_EmanCB.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/tests/test_eman_sta_classic_base.py` & `scipion-em-emantomo-3.1.3/emantomo/tests/test_eman_sta_classic_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         # Import tomograms
         print(magentaStr("\n==> Importing the tomograms:"))
         protImportTomogram = cls.newProtocol(ProtImportTomograms,
                                              filesPath=cls.ds.getFile(DataSetEmd10439.tomoEmd10439.name),
                                              samplingRate=cls.origSRate, )
 
         cls.launchProtocol(protImportTomogram)
-        tomoImported = protImportTomogram.outputTomograms
+        tomoImported = protImportTomogram.Tomograms
         cls.assertIsNotNone(tomoImported, "There was a problem with tomogram output")
         return tomoImported
 
     @classmethod
     def runImport3dCoords(cls, tomoImported):
         # Import coordinates
         print(magentaStr("\n==> Importing the 3D coordinates:"))
```

### Comparing `scipion-em-emantomo-3.1.2/emantomo/tests/test_protocols_sta_classic_emantomoextraction.py` & `scipion-em-emantomo-3.1.3/emantomo/tests/test_protocols_sta_classic_emantomoextraction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/tests/test_protocols_sta_classic_workflow.py` & `scipion-em-emantomo-3.1.3/emantomo/tests/test_protocols_sta_classic_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/viewers/__init__.py` & `scipion-em-emantomo-3.1.3/emantomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/viewers/viewers.py` & `scipion-em-emantomo-3.1.3/emantomo/viewers/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/viewers/viewers_data.py` & `scipion-em-emantomo-3.1.3/emantomo/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/viewers/views_tkinter_tree.py` & `scipion-em-emantomo-3.1.3/emantomo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/emantomo/wizards.py` & `scipion-em-emantomo-3.1.3/emantomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/PKG-INFO` & `scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-emantomo
-Version: 3.1.2
+Version: 3.1.3
 Summary: Plugin to use EMAN2 tomography programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-emantomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-emantomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-emantomo/
```

### Comparing `scipion-em-emantomo-3.1.2/scipion_em_emantomo.egg-info/SOURCES.txt` & `scipion-em-emantomo-3.1.3/scipion_em_emantomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-emantomo-3.1.2/setup.py` & `scipion-em-emantomo-3.1.3/setup.py`

 * *Files identical despite different names*

