# Comparing `tmp/pyhectiqlab-2.1.6.tar.gz` & `tmp/pyhectiqlab-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hectiq-lab/hectiq-lab/python-client/dist/.tmp-w7uoxhue/pyhectiqlab-2.1.6.tar", last modified: Thu Apr  6 18:59:59 2023, max compression
+gzip compressed data, was "/home/runner/work/hectiq-lab/hectiq-lab/python-client/dist/.tmp-97xk7y4q/pyhectiqlab-2.1.7.tar", last modified: Thu Apr 20 19:29:33 2023, max compression
```

## Comparing `pyhectiqlab-2.1.6.tar` & `pyhectiqlab-2.1.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab/callbacks/
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/callbacks/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/config_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/events_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/mlmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/notebooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15602 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/pulse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29886 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyhectiqlab/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:59:39.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/artifacts/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/artifacts/test_img2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/create_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/dataset/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/dataset/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/dataset/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/mlmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/mlmodel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/mlmodel/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/mlmodel/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/mlmodel/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:59:59.000000 pyhectiqlab-2.1.6/tests/step_artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)   158372 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   165197 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   726799 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   172506 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step4.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   165748 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step8.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   153112 2023-04-06 18:59:35.000000 pyhectiqlab-2.1.6/tests/step_artifacts/step9.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/config_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/events_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/mlmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/notebooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15922 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/pulse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30465 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:29:13.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/artifacts/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/artifacts/test_img2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/create_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/test_img2.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/mlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img2.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/step_artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)   158372 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   165197 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   726799 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   172506 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step4.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   165748 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step8.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   153112 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step9.jpeg
```

### Comparing `pyhectiqlab-2.1.6/LICENSE` & `pyhectiqlab-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/PKG-INFO` & `pyhectiqlab-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python client to use the Hectiq Lab
 Home-page: https://lab.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/apps.py` & `pyhectiqlab-2.1.7/pyhectiqlab/apps.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/auth.py` & `pyhectiqlab-2.1.7/pyhectiqlab/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/buffer.py` & `pyhectiqlab-2.1.7/pyhectiqlab/buffer.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/callbacks/keras.py` & `pyhectiqlab-2.1.7/pyhectiqlab/callbacks/keras.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/cli/auth.py` & `pyhectiqlab-2.1.7/pyhectiqlab/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/config.py` & `pyhectiqlab-2.1.7/pyhectiqlab/config.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/config_template.py` & `pyhectiqlab-2.1.7/pyhectiqlab/config_template.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/datasets.py` & `pyhectiqlab-2.1.7/pyhectiqlab/datasets.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/decorators.py` & `pyhectiqlab-2.1.7/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/events_manager.py` & `pyhectiqlab-2.1.7/pyhectiqlab/events_manager.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/metrics.py` & `pyhectiqlab-2.1.7/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/mlmodels.py` & `pyhectiqlab-2.1.7/pyhectiqlab/mlmodels.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/notebooks.py` & `pyhectiqlab-2.1.7/pyhectiqlab/notebooks.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/ops.py` & `pyhectiqlab-2.1.7/pyhectiqlab/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,21 @@
             logger.info(f'Uploading {filename}')
             if filename is None:
                 continue
 
             upload_file(full_paths[filename], policy)
     return mlmodel
 
+def update_mlmodel_readme(project_path, mlmodel_name, version, readme, token):
+    res = lab_request(path=f"/{project_path}/mlmodels/{mlmodel_name}/{version}/edit/README.md",
+                     request_type="POST",
+                     body_args=dict(content=readme),
+                     token=token)
+    return res
+
 def add_dataset(run_path, 
                 project_path,
                 filenames: List[str], 
                 full_paths: List[str], 
                 num_bytes: List[int], 
                 name: str, 
                 short_description: str,
```

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/paper.py` & `pyhectiqlab-2.1.7/pyhectiqlab/paper.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/pulse.py` & `pyhectiqlab-2.1.7/pyhectiqlab/pulse.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/run.py` & `pyhectiqlab-2.1.7/pyhectiqlab/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,28 @@
              push_dir=push_dir,
              resume_upload=resume_upload)
         if mlmodel is not None:
             self.add_mlmodel_usage(mlmodel.get('name'), version=mlmodel.get('version'))
 
     @write_method
     @action_method
+    def set_mlmodel_readme(self, source_path: str, name: str, version: str):
+        """Set the readme of a mlmodel.
+
+        Args:
+            source_path: Path to the directory/file of the README.md
+            name: Name of the model without spaces and backslash (e.g., 'text-model')
+            version: Specific version of the model. 
+        """
+        with open(source_path, 'r') as file:
+            content = file.read()
+        self.events_manager.add_event("update_mlmodel_readme", ( self._project_path, name, version, content))
+
+    @write_method
+    @action_method
     def download_mlmodel(self, mlmodel_name: str, version: str = None, save_path: str = './', overwrite:bool = False):
         """Download an existing mlmodel from the run's project.
 
         source_path: Path to the directory/file of the mlmodel
         mlmodel_name: Name of the model without spaces and backslash (e.g., 'text-model')
         version: Specific version of the model. If None, the latest version is fetched.
         save_path: Path to where the model is saved.
```

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/stream.py` & `pyhectiqlab-2.1.7/pyhectiqlab/stream.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/upload.py` & `pyhectiqlab-2.1.7/pyhectiqlab/upload.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/utils.py` & `pyhectiqlab-2.1.7/pyhectiqlab/utils.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab/watermark.py` & `pyhectiqlab-2.1.7/pyhectiqlab/watermark.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-2.1.7/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python client to use the Hectiq Lab
 Home-page: https://lab.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhectiqlab-2.1.6/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-2.1.7/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/setup.py` & `pyhectiqlab-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
-__version__ = '2.1.6'
+__version__ = '2.1.7'
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
     "requests",
     "tqdm",
```

### Comparing `pyhectiqlab-2.1.6/tests/artifacts/test_img1.jpeg` & `pyhectiqlab-2.1.7/tests/artifacts/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/artifacts/test_img2.jpeg` & `pyhectiqlab-2.1.7/tests/artifacts/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/create_run.py` & `pyhectiqlab-2.1.7/tests/create_run.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/dataset/imgs/test_img1.jpeg` & `pyhectiqlab-2.1.7/tests/dataset/imgs/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/dataset/imgs/test_img2.jpeg` & `pyhectiqlab-2.1.7/tests/dataset/imgs/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/mlmodel/imgs/test_img1.jpeg` & `pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/mlmodel/imgs/test_img2.jpeg` & `pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step1.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step2.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step3.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step3.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step4.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step4.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step8.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step8.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.6/tests/step_artifacts/step9.jpeg` & `pyhectiqlab-2.1.7/tests/step_artifacts/step9.jpeg`

 * *Files identical despite different names*

