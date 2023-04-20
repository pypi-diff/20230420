# Comparing `tmp/ebilab-2.2.1.tar.gz` & `tmp/ebilab-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebilab-2.2.1.tar", last modified: Mon Jan 30 06:41:14 2023, max compression
+gzip compressed data, was "ebilab-2.3.0.tar", last modified: Thu Apr 20 10:22:58 2023, max compression
```

## Comparing `ebilab-2.2.1.tar` & `ebilab-2.3.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-30 06:41:04.000000 ebilab-2.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-30 06:41:04.000000 ebilab-2.2.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-01-30 06:41:04.000000 ebilab-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-30 06:41:04.000000 ebilab-2.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-30 06:41:04.000000 ebilab-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-30 06:41:04.000000 ebilab-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-30 06:41:04.000000 ebilab-2.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-30 06:41:14.319361 ebilab-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-30 06:41:04.000000 ebilab-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.experiment.devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.experiment.devices.visa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/ebilab.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/changelog-v2.0.0-pre.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/docs/source/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/docs/source/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/installation.po
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/modules.po
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/tutorial.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/tutorial/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/tutorial/experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/tutorial/experiment_device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-30 06:41:04.000000 ebilab-2.2.1/docs/source/tutorial/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/analysis/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/analysis/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/analysis/_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/ebilab/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/data/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/ebilab/data/project-template/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/data/project-template/data/input/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/data/input/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/data/project-template/data/original/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/data/original/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/data/project-template/data/output/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/data/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/data/project-template/data/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/data/plot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/ebilab.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/data/project-template/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/_experiment_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/_ui_tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab/experiment/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/ebilab/experiment/devices/_visa/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/_visa/A707.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/_visa/E4980.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/_visa/K34411A.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/_visa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/devices/visa.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/experiment/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-01-30 06:41:04.000000 ebilab-2.2.1/ebilab/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.315361 ebilab-2.2.1/ebilab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-30 06:41:14.000000 ebilab-2.2.1/ebilab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 06:41:04.000000 ebilab-2.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/sample/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/cont_r.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/multimeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/random-walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-30 06:41:04.000000 ebilab-2.2.1/sample/voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 06:41:14.319361 ebilab-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-30 06:41:04.000000 ebilab-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.311360 ebilab-2.2.1/tests/sample/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/sample/data/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/sample/data/input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/sample/data/original/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/sample/data/original/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/sample/data/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/sample/data/output/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/sample/ebilab.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:14.319361 ebilab-2.2.1/tests/sample/other_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/sample/other_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-30 06:41:04.000000 ebilab-2.2.1/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 10:22:43.000000 ebilab-2.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 10:22:43.000000 ebilab-2.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-20 10:22:43.000000 ebilab-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 10:22:43.000000 ebilab-2.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 10:22:43.000000 ebilab-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 10:22:43.000000 ebilab-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 10:22:43.000000 ebilab-2.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 10:22:58.893872 ebilab-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 10:22:43.000000 ebilab-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.devices.visa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/ebilab.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/changelog-v2.0.0-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/docs/source/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/docs/source/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/installation.po
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/modules.po
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/experiment_device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-20 10:22:43.000000 ebilab-2.3.0/docs/source/tutorial/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/ebilab/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/analysis/_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/ebilab/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.885872 ebilab-2.3.0/ebilab/data/project-template/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/input/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/original/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/original/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/data/project-template/data/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/data/plot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/ebilab.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/data/project-template/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/_experiment_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/_ui_tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab/experiment/devices/_visa/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/A707.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/E4980.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/K34411A.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/_visa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/devices/visa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/experiment/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 10:22:43.000000 ebilab-2.3.0/ebilab/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/ebilab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 10:22:58.000000 ebilab-2.3.0/ebilab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 10:22:43.000000 ebilab-2.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/cont_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/multimeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/random-walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 10:22:43.000000 ebilab-2.3.0/sample/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:22:58.893872 ebilab-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-20 10:22:43.000000 ebilab-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.889872 ebilab-2.3.0/tests/sample/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/original/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/original/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/data/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/data/output/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/ebilab.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:58.893872 ebilab-2.3.0/tests/sample/other_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/sample/other_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 10:22:43.000000 ebilab-2.3.0/tests/test_paths.py
```

### Comparing `ebilab-2.2.1/.gitignore` & `ebilab-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/LICENSE` & `ebilab-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/README.md` & `ebilab-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/Makefile` & `ebilab-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/make.bat` & `ebilab-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/api/ebilab.analysis.rst` & `ebilab-2.3.0/docs/source/api/ebilab.analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/changelog-v2.0.0-pre.rst` & `ebilab-2.3.0/docs/source/changelog-v2.0.0-pre.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/changelog.rst` & `ebilab-2.3.0/docs/source/changelog.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 ####################
 更新履歴
 ####################
 
 **************************
+v2.3.0 (Apr 20, 2023)
+**************************
+
+Features
+=====================
+
+* ebilab.experimentのOptionFieldにおいて、 `IntField` と `StrField` を追加しました。 (`#7 <https://github.com/ebiyuu1121/ebilab/pull/7/>`_)
+
+
+Contributors
+=====================
+
+* `@halphy <https://github.com/halphy>`_ が最初のコントリビューションを行いました。ありがとうございます！
+
+**************************
 v2.2.1 (Jan 30, 2023)
 **************************
 
 Changes (unstable)
 =====================
 
 * ebilab.analysisにおいて、生成されるプロジェクトのgitignoreファイルを変更しました。
```

### Comparing `ebilab-2.2.1/docs/source/conf.py` & `ebilab-2.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/index.rst` & `ebilab-2.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/installation.rst` & `ebilab-2.3.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/api.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/changelog.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/changelog.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/index.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/installation.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/modules.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/modules.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/locale/en/LC_MESSAGES/tutorial.po` & `ebilab-2.3.0/docs/source/locale/en/LC_MESSAGES/tutorial.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/tutorial/analysis.rst` & `ebilab-2.3.0/docs/source/tutorial/analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/tutorial/experiment.rst` & `ebilab-2.3.0/docs/source/tutorial/experiment.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/tutorial/experiment_device.rst` & `ebilab-2.3.0/docs/source/tutorial/experiment_device.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/docs/source/tutorial/version.rst` & `ebilab-2.3.0/docs/source/tutorial/version.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/__init__.py` & `ebilab-2.3.0/ebilab/__init__.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/_cli.py` & `ebilab-2.3.0/ebilab/_cli.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/analysis/_actions.py` & `ebilab-2.3.0/ebilab/analysis/_actions.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/analysis/_preprocess.py` & `ebilab-2.3.0/ebilab/analysis/_preprocess.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/analysis/_process.py` & `ebilab-2.3.0/ebilab/analysis/_process.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/data/project-template/.gitignore` & `ebilab-2.3.0/ebilab/data/project-template/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/experiment/_experiment_controller.py` & `ebilab-2.3.0/ebilab/experiment/_experiment_controller.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/experiment/_ui_tkinter.py` & `ebilab-2.3.0/ebilab/experiment/_ui_tkinter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tkinter.font as tkf
 
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 from ._experiment_controller import ExperimentPlotter, IExperimentUI, ExperimentProtocol, PlotterContext
-from .options import OptionField, FloatField, SelectField
+from .options import OptionField, FloatField, SelectField, IntField, StrField
 
 logger = getLogger(__name__)
 
 # windows dpi workaround
 try:
     import ctypes
     ctypes.windll.shcore.SetProcessDpiAwareness(2) 
@@ -71,14 +71,38 @@
                 var.trace("w", self._on_update)
                 widget = ttk.Combobox(self, textvariable=var, state="readonly", values=field.choices)
                 widget.grid(row=i + 1, column=1, sticky=tk.EW + tk.N)
 
                 self._options_textvars.append(var)
                 self._options_widget.append(widget)
                 continue
+            elif isinstance(field, IntField):
+                label = tk.Label(self, text=key)
+                label.grid(row=i + 1, column=0, sticky=tk.W + tk.N)
+
+                var = tk.StringVar(value=str(field.default))
+                var.trace("w", self._on_update)
+                widget = tk.Entry(self, textvariable=var)
+                widget.grid(row=i + 1, column=1, sticky=tk.EW + tk.N)
+
+                self._options_textvars.append(var)
+                self._options_widget.append(widget)
+                continue
+            elif isinstance(field, StrField):
+                label = tk.Label(self, text=key)
+                label.grid(row=i + 1, column=0, sticky=tk.W + tk.N)
+
+                var = tk.StringVar(value=str(field.default))
+                var.trace("w", self._on_update)
+                widget = tk.Entry(self, textvariable=var)
+                widget.grid(row=i + 1, column=1, sticky=tk.EW + tk.N)
+
+                self._options_textvars.append(var)
+                self._options_widget.append(widget)
+                continue
             raise TypeError("Unknown field type.")
 
         opt = self._get_options()
         if opt is None:
             raise RuntimeError("Unexpected invalid value")
         self.__options = opt
         self.__is_valid = True
@@ -126,14 +150,35 @@
                     val = int(var.get())
                 elif isinstance(field.choices[0], float):
                     val = float(var.get())
                 else:
                     val = var.get()
                 ret[key] = val
                 continue
+            elif isinstance(field, IntField):
+                try:
+                    val = int(var.get())
+                except ValueError:
+                    logger.debug(f"Validation failed: {key} = {var.get()} is not int.")
+                    return None
+                if field.min is not None and val < field.min:
+                    logger.debug(f"Validation failed: {key} = {val} < {field.min}.")
+                    return None
+                if field.max is not None and val > field.max:
+                    logger.debug(f"Validation failed: {key} = {val} > {field.max}.")
+                    return None
+                ret[key] = val
+                continue
+            elif isinstance(field, StrField):
+                val = var.get()
+                if (not field.allow_blank) and len(val) == 0:
+                    logger.debug(f"Validation failed: {key} is blank.")
+                    return None
+                ret[key] = val
+                continue
             raise TypeError("Unknown field type.")
         return ret
 
     @property
     def options(self) -> dict:
         assert self.__options is not None
         return self.__options
```

### Comparing `ebilab-2.2.1/ebilab/experiment/devices/_visa/A707.py` & `ebilab-2.3.0/ebilab/experiment/devices/_visa/A707.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/experiment/devices/_visa/E4980.py` & `ebilab-2.3.0/ebilab/experiment/devices/_visa/E4980.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/experiment/devices/_visa/K34411A.py` & `ebilab-2.3.0/ebilab/experiment/devices/_visa/K34411A.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/experiment/devices/visa.py` & `ebilab-2.3.0/ebilab/experiment/devices/visa.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab/project.py` & `ebilab-2.3.0/ebilab/project.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/ebilab.egg-info/SOURCES.txt` & `ebilab-2.3.0/ebilab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/sample/cont_r.py` & `ebilab-2.3.0/sample/cont_r.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/sample/random-walk.py` & `ebilab-2.3.0/sample/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/sample/voltage.py` & `ebilab-2.3.0/sample/voltage.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/setup.py` & `ebilab-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.2.1/tests/test_paths.py` & `ebilab-2.3.0/tests/test_paths.py`

 * *Files identical despite different names*

