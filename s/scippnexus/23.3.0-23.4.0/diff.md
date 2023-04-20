# Comparing `tmp/scippnexus-23.3.0.tar.gz` & `tmp/scippnexus-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippnexus-23.3.0.tar", last modified: Tue Mar  7 09:27:33 2023, max compression
+gzip compressed data, was "scippnexus-23.4.0.tar", last modified: Thu Apr 20 09:02:14 2023, max compression
```

## Comparing `scippnexus-23.3.0.tar` & `scippnexus-23.4.0.tar`

### file list

```diff
@@ -1,103 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3590 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-03-07 09:27:20.000000 scippnexus-23.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-03-07 09:27:20.000000 scippnexus-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-07 09:27:20.000000 scippnexus-23.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-03-07 09:27:33.654810 scippnexus-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-03-07 09:27:20.000000 scippnexus-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-03-07 09:27:20.000000 scippnexus-23.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/_static/logo-2022.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6200 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/about/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/getting-started/quick-start-guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.646810 scippnexus-23.3.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/user-guide/application-definitions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/user-guide/classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/user-guide/functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11150 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/user-guide/nexus-classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-03-07 09:27:20.000000 scippnexus-23.3.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-07 09:27:20.000000 scippnexus-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.650810 scippnexus-23.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-07 09:27:20.000000 scippnexus-23.3.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.650810 scippnexus-23.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-03-07 09:27:20.000000 scippnexus-23.3.0/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-03-07 09:27:33.654810 scippnexus-23.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.642810 scippnexus-23.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/src/scippnexus/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/_hdf5_nexus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/src/scippnexus/data/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/src/scippnexus/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/definitions/nxcansas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/src/scippnexus/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/leaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxdetector.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxdisk_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxfermi_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxlog.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxmonitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxsource.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/nxtransformations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-03-07 09:27:20.000000 scippnexus-23.3.0/src/scippnexus/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/src/scippnexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-03-07 09:27:33.000000 scippnexus-23.3.0/src/scippnexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-03-07 09:27:33.000000 scippnexus-23.3.0/src/scippnexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 09:27:33.000000 scippnexus-23.3.0/src/scippnexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-07 09:27:33.000000 scippnexus-23.3.0/src/scippnexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-07 09:27:33.000000 scippnexus-23.3.0/src/scippnexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:27:33.654810 scippnexus-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/application_definition_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/externalfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/load_files_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxcylindrical_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    19235 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxdata_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    21838 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxmonitor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxoff_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    13679 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tests/nxtransformations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-03-07 09:27:20.000000 scippnexus-23.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-20 09:02:00.000000 scippnexus-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-20 09:02:00.000000 scippnexus-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-20 09:02:14.796720 scippnexus-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-20 09:02:00.000000 scippnexus-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-20 09:02:00.000000 scippnexus-23.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_static/logo-2022.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6546 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/getting-started/quick-start-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/application-definitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/nexus-classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-20 09:02:00.000000 scippnexus-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-04-20 09:02:00.000000 scippnexus-23.4.0/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 09:02:14.796720 scippnexus-23.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/_hdf5_nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/definitions/nxcansas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdetector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdisk_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxfermi_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxlog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxsource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/src/scippnexus/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18014 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxtransformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2805 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/application_definition_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/externalfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/load_files_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23629 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxcylindrical_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25349 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxevent_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxmonitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxoff_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxtransformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tox.ini
```

### Comparing `scippnexus-23.3.0/.github/workflows/ci.yml` & `scippnexus-23.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/.github/workflows/docs.yml` & `scippnexus-23.4.0/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       - uses: actions/setup-python@v3
         with:
           python-version: 3.8
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
           tox --skip-pkg-install -e docs -- scippnexus==${VERSION}
-          echo "target=$(python docs/version.py --repo=scippnexus --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
+          echo "target=$(python docs/version.py --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
         if: ${{ !inputs.publish }}
       - uses: actions/upload-artifact@v3
         with:
           name: html
           path: html/
```

### Comparing `scippnexus-23.3.0/.github/workflows/release.yml` & `scippnexus-23.4.0/.github/workflows/release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     needs: [build_wheels, build_conda]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v2
       - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   upload_conda:
     name: Deploy Conda Forge
     needs: [build_wheels, build_conda]
@@ -92,16 +92,16 @@
         with:
           python-version: 3.8
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
         run: |
-          echo "new=$(python docs/version.py --repo=scippnexus --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
-          echo "replaced=$(python docs/version.py --repo=scippnexus --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
+          echo "new=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
+          echo "replaced=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
 
   docs:
     needs: [upload_conda, upload_pypi, manage-versions]
     uses: ./.github/workflows/docs.yml
     with:
       publish: ${{ github.event_name == 'release' && github.event.action == 'published' }}
       version: ${{ github.ref_name }}
```

### Comparing `scippnexus-23.3.0/.pre-commit-config.yaml` & `scippnexus-23.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/LICENSE` & `scippnexus-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/PKG-INFO` & `scippnexus-23.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.3.0
+Version: 23.4.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.3.0/README.md` & `scippnexus-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/_static/favicon.ico` & `scippnexus-23.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/_static/logo-2022.svg` & `scippnexus-23.4.0/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/_templates/scipp-class-template.rst` & `scippnexus-23.4.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/_templates/scipp-module-template.rst` & `scippnexus-23.4.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/_templates/sections/header-article.html` & `scippnexus-23.4.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/about/about.rst` & `scippnexus-23.4.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/about/release-notes.rst` & `scippnexus-23.4.0/docs/about/release-notes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,25 @@
    Contributors
    ~~~~~~~~~~~~
 
    Simon Heybrock :sup:`a`\ ,
    Neil Vaytet :sup:`a`\ ,
    and Jan-Lukas Wynen :sup:`a`
 
+v23.04.0
+--------
+
+Features
+~~~~~~~~
+
+* Added the future API of ``scippnexus`` as ``scippnexus.v2``.
+  For many users the API changes will be minor.
+  The old API will be deprecated soon and users should try to migrate to the new API.
+  Note that ``v2`` is not fully stable yet and in particular the behavior in edge cases is subject to change.
+
 v23.03.0
 --------
 
 Features
 ~~~~~~~~
 
 * Improve handling of files with legacy ``signal`` and ``axis`` attributes, yielding better dim labels `#108 <https://github.com/scipp/scippnexus/pull/108>`_.
```

### Comparing `scippnexus-23.3.0/docs/conf.py` & `scippnexus-23.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/getting-started/installation.rst` & `scippnexus-23.4.0/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/docs/getting-started/quick-start-guide.ipynb` & `scippnexus-23.4.0/docs/getting-started/quick-start-guide.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882848972922502%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, '# To use the legacy interface, use:\\n'), (1, '# import "*

 * *            "scippnexus as snx\\n'), (2, 'import scippnexus.v2 as snx\\n')], delete: [0]}}, 9: "*

 * *            '{\'source\': {insert: [(0, "entry = f[\'entry\']\\n")], delete: [0]}}, 13: '*

 * *            '{\'source\': ["f[\'entry/instrument\'][snx.NXdetector]"]}, delete: [10, 9, 8]}'}*

```diff
@@ -60,15 +60,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cbbeaf94-fc7b-4043-9583-0df33c879f39",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import scippnexus as snx\n",
+                "# To use the legacy interface, use:\n",
+                "# import scippnexus as snx\n",
+                "import scippnexus.v2 as snx\n",
                 "\n",
                 "with snx.File(filename) as f:\n",
                 "    print(list(f.keys()))"
             ]
         },
         {
             "cell_type": "markdown",
@@ -94,51 +96,14 @@
             "metadata": {},
             "source": [
                 "## Navigating files"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "067bfa30-b0b6-4c1d-bccd-438ab2789f6c",
-            "metadata": {},
-            "source": [
-                "### `NX_class`-based access\n",
-                "\n",
-                "When there is a unique child group with a specific `NX_class` attribute then this child can be accessed using a special property.\n",
-                "This avoids the need to know about and inspect the keys recursively.\n",
-                "For example, our file contains a single `NXentry`, which in turn contains a single `NXmonitor`.\n",
-                "We can access it using:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "b253b90d-269b-42ae-a236-e91d91ee1b8b",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "f.entry.monitor"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "1e673371-09a2-4f97-8797-44f13e884a3a",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-info\">\n",
-                "    <b>Note:</b>\n",
-                "\n",
-                "The property names are based on the value of `NX_class` attribute (without the \"NX\" prefix), *not* the HDF5 group name.\n",
-                "For example, above we used `f.entry.monitor` to access the monitor named `monitor1`.\n",
-                "\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "a14fa902-5eae-4530-a8b4-3648da9ffea0",
             "metadata": {},
             "source": [
                 "### Name-based access\n",
                 "\n",
                 "If there are multiple children with a specific `NX_class` attribute then the aforementioned properties cannot be used.\n",
                 "Above we saw that the file contains a single key, `'entry'` (the name could be anything, it just happens to match the class name here).\n",
@@ -148,15 +113,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "62b99b27-0f80-4217-a41f-ba40bef7e877",
             "metadata": {},
             "outputs": [],
             "source": [
-                "entry = f['entry']  # equivalent to f.entry, since f contains only a single NXentry\n",
+                "entry = f['entry']\n",
                 "entry"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9ff94b4a-490e-42d6-a9b9-07f372de5be0",
             "metadata": {},
@@ -190,17 +155,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "32c0f1f4-84ee-4258-8cb1-999b06f00ba0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from scippnexus import NXdetector\n",
-                "\n",
-                "f.entry.instrument[NXdetector]"
+                "f['entry/instrument'][snx.NXdetector]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "134beaeb-eee6-4c04-a05c-318974aec1a9",
             "metadata": {},
             "source": [
```

### Comparing `scippnexus-23.3.0/docs/index.rst` & `scippnexus-23.4.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 - **Labeled dimension** can be used to selectively load slices of an entire NeXus class.
   This is modelled after h5py's support for loading slices of datasets but provides the same convenience and safety as `scipp's slicing <https://scipp.github.io/user-guide/slicing.html>`_ by requiring specification of the dimension to slice by its name, rather than plain axis order.
 - **Physical units** are stored with most datasets in a NeXus class and are loaded as unit of the :class:`scipp.DataArray` values or coordinates.
 
 News
 ----
 
+- [April 2023] scippnexus-23.04.0 has been released.
+  This adds ``scippnexus.v2``, which provides the future API of ``scippnexus``.
+  The new API avoids performance bottlenecks when working with small files that contain many groups and datasets.
+  The new behavior is also more faithful to the file content.
+  ``v2`` will become the default in the near future.
 - [March 2023] scippnexus-23.03.0 has been released.
   This brings a number of improvements, including handling of legacy files and loading of geometry information.
 - [January 2023] scippnexus-23.01.0 has been released.
   This brings support for loading arbitrary groups as :class:`scipp.DataGroup`.
   Furthermore, errors are handled in a more transparent way:
   ScippNexus will now fall back to returning group contents as a :class:`scipp.DataGroup` instead of silently skipping loading certain fields.
 - [November 2022] scippnexus-0.4.0 has been released.
```

### Comparing `scippnexus-23.3.0/docs/user-guide/application-definitions.ipynb` & `scippnexus-23.4.0/docs/user-guide/application-definitions.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9750560747399233%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(7, '2. defines the `__write_to_nexus_group__` method that "*

 * *            "takes a `h5py.Group`, i.e., an open HDF5 group, as its single argument.\\n'), (10, "*

 * *            "'This can (and should) make use of ScippNexus features for writing Nexus fields (HDF5 "*

 * *            'datasets) from a `scipp.Variable` via `snx.create_field`, such as automatic writing '*

 * *            "of the `units` attribute, or writing `datetime64` data.\\n')], delete: [10, 7]}}, 5: "*

 * *            "{' […]*

```diff
@@ -32,51 +32,68 @@
                 "ScippNexus' support for application definitions is currently experimental and the API is still subject to changes.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "7fc1d425-4a31-4b75-87d4-f0398b88c090",
+            "metadata": {},
+            "source": [
+                "Definitions provide customization points, e.g., for how ScippNexus can find required information in the HDF5 group, and how contents are mapped to aspects of the returned data (typically a `scipp.DataArray` or `scipp.DataGroup`).\n",
+                "\n",
+                "Definitions in ScippNexus are subclasses of [NXobject](classes.rst#NXobject).\n",
+                "A `definitions` mapping passed to `snx.File` serves as a repository of definitions that `snx.Group` will use when opening a group in a file.\n",
+                "`snx.base_definitions()` is used by default.\n",
+                "The `NX_class` attribute of the HDF5 group is used as a key into the `definitions` mapping.\n",
+                "It provides subclasses such as `NXlog`, `NXdata`, and `NXdetector`.\n",
+                "\n",
+                "Users can implement their application definition (or any definition) by subclassing `NXobject`, or one of the existing base-class definitions."
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "c4164b2f-6e64-4a9f-8204-daf6ef8025fc",
             "metadata": {},
             "source": [
                 "## Writing files\n",
                 "\n",
                 "Skip ahead to [Reading files](#Reading-files) if you simply want to customize how data is read from existing files.\n",
                 "ScippNexus provides a customization point for writing content to NeXus files with `__setitem__`.\n",
                 "The requirements are that the value\n",
                 "\n",
                 "1. provides an `nx_class` attribute that returns a valid NeXus class name such as `'NXdata'` or `scippnexus.NXdata` and\n",
-                "2. defines the `__write_to_nexus_group__` method that takes a `scippnexus.NXobject`, i.e., an open NeXus group, as its single argument.\n",
+                "2. defines the `__write_to_nexus_group__` method that takes a `h5py.Group`, i.e., an open HDF5 group, as its single argument.\n",
                 "\n",
                 "`__write_to_nexus_group__` may then write its content to this group.\n",
-                "This can (and should) make use of ScippNexus features for writing Nexus fields (HDF5 datasets), such as automatic writing of the `units` attribute, or writing `datetime64` data.\n",
+                "This can (and should) make use of ScippNexus features for writing Nexus fields (HDF5 datasets) from a `scipp.Variable` via `snx.create_field`, such as automatic writing of the `units` attribute, or writing `datetime64` data.\n",
                 "Consider the following example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3da8519f-4295-4c94-9850-92020a37ebfd",
             "metadata": {},
             "outputs": [],
             "source": [
+                "import h5py\n",
                 "import scipp as sc\n",
-                "import scippnexus as snx\n",
+                "import scippnexus.v2 as snx\n",
                 "\n",
                 "\n",
                 "class MyData:\n",
                 "    nx_class = snx.NXdata  # required\n",
                 "\n",
                 "    def __init__(self, data: sc.DataArray):\n",
                 "        self._data = data\n",
                 "\n",
-                "    def __write_to_nexus_group__(self, group: snx.NXobject):  # required\n",
+                "    def __write_to_nexus_group__(self, group: h5py.Group):  # required\n",
                 "        group.attrs['axes'] = self._data.dims  # NeXus way of defining dim labels\n",
-                "        group['mysignal'] = self._data.data"
+                "        snx.create_field(group, 'mysignal', self._data.data)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "11c5073d-7231-429c-a461-61b31a03c284",
             "metadata": {},
             "source": [
@@ -108,155 +125,128 @@
                 "\n",
                 "### Overview\n",
                 "\n",
                 "For some application definitions &mdash; or classes within application definitions &mdash; the default ScippNexus mechanisms for reading are sufficient.\n",
                 "This is the case when the application definition follows the NeXus standard and, e.g., introduces no new attributes.\n",
                 "\n",
                 "In other cases we require customization of how ScippNexus reads class contents.\n",
-                "On the lowest level, this is handled using *strategies* that can be passed to `scippnexus.NXobject` and its subclasses such as `scippnexus.NXdata`.\n",
-                "Handling of strategies is usually encapsulated by a *definition* that can be passed to `scippnexus.File`.\n",
+                "This is handled using *definitions* that can be passed to `snx.File` or `snx.Group`.\n",
                 "\n",
-                "As an example, consider the following simple strategy for loading data with a custom signal name, which the file failed to specify.\n",
-                "We also subclass `scippnexus.ApplicationDefinition`:"
+                "As an example, consider the following simple definition for loading data with a custom signal name, which the file failed to specify.\n",
+                "In this particular case we subclass `snx.NXdata`, and pass a custom argument to its `__init__`.\n",
+                "In general this is rarely sufficient, and in practice a definition may need to implement other parts of the `snx.NXobject` interface:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ac9ad742-ea04-4ebf-9f5d-ee68f98983d6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "class MyDataStrategy(snx.NXdataStrategy):\n",
-                "    @staticmethod\n",
-                "    def signal(group: snx.NXobject) -> str:\n",
-                "        return 'mysignal'\n",
+                "class MyDataDefinition(snx.NXdata):\n",
+                "    def __init__(self, attrs, children):\n",
+                "        super().__init__(attrs=attrs, children=children, fallback_signal_name='mysignal')\n",
                 "\n",
                 "\n",
-                "class MyDefinition(snx.ApplicationDefinition):\n",
-                "    def make_strategy(self, group: snx.NXobject):\n",
-                "        if group.nx_class == snx.NXdata:\n",
-                "            return MyDataStrategy"
+                "my_definitions = snx.base_definitions()\n",
+                "my_definitions['NXdata'] = MyDataDefinition"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ef933561-9e32-4549-acd1-1b574b585742",
             "metadata": {},
             "source": [
-                "We can then load our file (created above in [Writing files](#Writing-files)) by passing an instance of our custom definition to `scippnexus.File`:"
+                "We can then load our file (created above in [Writing files](#Writing-files)) by our custom definitions to `snx.File`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "460c1f65-623e-4129-b5dc-50811681d3aa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with snx.File('test.nxs', 'r', definition=MyDefinition()) as f:\n",
+                "with snx.File('test.nxs', 'r', definitions=my_definitions) as f:\n",
                 "    loaded = f['data'][...]\n",
                 "loaded"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f5d55a73-53ce-412a-90d2-18a826ec3c95",
             "metadata": {},
             "source": [
                 "ScippNexus does currently not ship with a library of application definitions.\n",
-                "Custom definitions can be provided by a user as outlined above.\n",
-                "The *definition* passed to ScippNexus serves as a factory for strategies &mdash; in the above example the only custom definition is the one used for `NXdata`.\n",
-                "For a given group in a NeXus tree, ScippNexus calls `definition.make_strategy(group)` to request a strategy for the group.\n",
-                "This may return `None` and ScippNexus will then use its default strategy for loading the group.\n",
-                "\n",
-                "Strategies provide customization points, e.g., for how ScippNexus can find required information in the HDF5 group, and how contents are mapped to aspects of the returned data (typically a `scipp.DataArray`).\n",
-                "For example, the default `scippnexus.NXdataStrategy` provides a static `axes` method that returns the name of the axes in the group, i.e., the dimension labels.\n",
-                "Users can either subclass `NXdataStrategy`, or provide a class with equivalent interfaces.\n",
-                "A full list of available base strategies can be found in [Strategies](classes.rst#Strategies)."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "69a0c1b7-2dc3-47c3-88d1-23cfc1ee77ac",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-info\">\n",
-                "    <b>Note:</b>\n",
-                "\n",
-                "Support for strategies is very new and the number of customization points is currently very limited.\n",
-                "If you encounter the need for more customization, please [open an issue](https://github.com/scipp/scippnexus/issues/new) so we can consider how to extent the base strategy.\n",
-                "\n",
-                "</div>"
+                "Custom definitions can be provided by a user as outlined above."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2371d6ef-8ad3-4a2c-bc63-939d1a29950f",
             "metadata": {},
             "source": [
-                "### Using strategies for filtering\n",
+                "### Using definitions for filtering\n",
                 "\n",
                 "The application-definition mechanism can be used for filtering or selecting which children from a group should be loaded.\n",
                 "For example, we may wish to exclude certain NeXus classes from loading.\n",
-                "We define a strategy as follows:"
+                "We define a custom definition as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a73b4dc8-98a3-40b6-bb03-d1efd666d3aa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import scippnexus as snx\n",
+                "import scippnexus.v2 as snx\n",
+                "\n",
+                "\n",
+                "def skip(name, obj):\n",
+                "    skip_classes = (snx.NXevent_data, snx.NXinstrument)\n",
+                "    return isinstance(obj, snx.Group) and (\n",
+                "        (obj.nx_class in skip_classes) or (name == 'DASlogs')\n",
+                "    )\n",
+                "\n",
                 "\n",
+                "class FilteredEntry(snx.NXobject):\n",
+                "    def __init__(self, attrs, children):\n",
+                "        children = {\n",
+                "            name: child for name, child in children.items() if not skip(name, child)\n",
+                "        }\n",
+                "        super().__init__(attrs=attrs, children=children)\n",
                 "\n",
-                "class FilterStrategy(snx.NXobjectStrategy):\n",
-                "    @staticmethod\n",
-                "    def include_child(group: snx.NXobject) -> bool:\n",
-                "        \"\"\"\n",
-                "        Skip all NXevent_data, the NXinstrument, and the group named \"DASlogs\".\n",
-                "        \"\"\"\n",
-                "        skip_classes = (snx.NXevent_data, snx.NXinstrument)\n",
-                "        if isinstance(group, skip_classes):\n",
-                "            return False\n",
-                "        return not group.name.endswith('DASlogs')"
+                "\n",
+                "my_definitions = snx.base_definitions()\n",
+                "my_definitions['NXentry'] = FilteredEntry"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b95829c7-8d32-4731-9a99-361cdf8017cc",
             "metadata": {},
             "source": [
-                "We can use this strategy with a custom application definition as follows:"
+                "We can use these definitions as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "91614592-0c2f-4575-a07f-aa2fba00ce7c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scippnexus import data\n",
                 "\n",
                 "filename = data.get_path('PG3_4844_event.nxs')\n",
-                "definition = snx.make_definition({snx.NXentry: FilterStrategy})\n",
-                "f = snx.File(filename, definition=definition)\n",
+                "f = snx.File(filename, definitions=my_definitions)\n",
                 "f['entry'][...]"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "e054874a-df45-450d-9cb4-9b5b5ccff309",
-            "metadata": {},
-            "source": [
-                "Above we used the helper [snx.make_definition](../generated/functions/make_definition.rst) which can be used instead of manually subclassing `ApplicationDefinition` in such simple cases."
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `scippnexus-23.3.0/docs/user-guide/classes.rst` & `scippnexus-23.4.0/docs/user-guide/classes.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.. currentmodule:: scippnexus
+.. currentmodule:: scippnexus.v2
 
 Classes
 =======
 
 Data Structures
 ---------------
 
 .. autosummary::
    :toctree: ../generated/classes
    :template: scipp-class-template.rst
    :recursive:
 
-   ApplicationDefinition
    Attrs
    Field
    File
+   Group
    NXaperture
    NXattenuator
    NXbeam
    NXbeam_stop
    NXbending_magnet
    NXcapillary
    NXcite
@@ -69,39 +69,29 @@
    NXsubentry
    NXtransformations
    NXtranslation
    NXuser
    NXvelocity_selector
    NXxraylens
 
-Strategies
-----------
-
-.. autosummary::
-   :toctree: ../generated/classes
-   :template: scipp-class-template.rst
-   :recursive:
-
-   NXdataStrategy
-   NXdetectorStrategy
-   NXlogStrategy
-
 Exceptions
 ----------
 
 .. autosummary::
    :toctree: ../generated/classes
    :template: scipp-class-template.rst
    :recursive:
 
    NexusStructureError
 
 Typing
 ------
 
+.. currentmodule:: scippnexus
+
 .. autosummary::
    :toctree: ../generated/classes
    :template: scipp-class-template.rst
    :recursive:
 
    typing.H5Dataset
    typing.H5Group
```

### Comparing `scippnexus-23.3.0/docs/user-guide/nexus-classes.ipynb` & `scippnexus-23.4.0/docs/user-guide/nexus-classes.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984700520833334%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'import scippnexus.v2 as snx\\n')], delete: [2]}}, 12: "*

 * *            "{'source': {insert: [(0, 'If the underlying data is event data, the underlying event "*

 * *            "data can be selected using the special `event_time_zero` dimension.\\n'), (1, 'This "*

 * *            'dimension is present in the underlying `NXevent_data` group, but not preserved after '*

 * *            "loading and binning by pixels due to the prohibitive size.\\n')], delete: [0]}}, 13: "*

 * *            '{ […]*

```diff
@@ -58,15 +58,15 @@
             "execution_count": null,
             "id": "62027f15-d168-40fd-a8eb-39ac62d2b4ff",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scippnexus import data\n",
                 "filename = data.get_path('PG3_4844_event.nxs')\n",
-                "import scippnexus as snx\n",
+                "import scippnexus.v2 as snx\n",
                 "f = snx.File(filename)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "32c5c15c-e8bd-41fb-9379-e678389c7f38",
             "metadata": {
@@ -170,26 +170,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "de532afe-6382-420b-bda4-4297172ffec5",
             "metadata": {},
             "source": [
-                "If the underlying data is event data, the underlying event data can be selected using the special `select_events` property.\n",
+                "If the underlying data is event data, the underlying event data can be selected using the special `event_time_zero` dimension.\n",
+                "This dimension is present in the underlying `NXevent_data` group, but not preserved after loading and binning by pixels due to the prohibitive size.\n",
                 "For example, we can select the first 1000 pulses and load data for all pixels:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "25b20528-63bb-46a2-b4bf-2106b5ae9ab1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "detector.select_events['pulse', :1000][...]"
+                "detector['event_time_zero', :1000]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a17cf9bf-fe20-4d51-87c9-63ad660efa67",
             "metadata": {},
             "source": [
@@ -242,15 +243,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "36730d49-56e8-45a1-9071-1827050daf18",
             "metadata": {},
             "outputs": [],
             "source": [
-                "f['entry/instrument/bank102'].events[...]"
+                "f['entry/instrument/bank102']['events'][...]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a2a7f817-0b47-47ba-9da7-bcd19819b087",
             "metadata": {
                 "tags": []
```

### Comparing `scippnexus-23.3.0/docs/version.py` & `scippnexus-23.4.0/docs/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import git
 from packaging.version import InvalidVersion, Version, parse
 
 
 def _get_releases() -> List[Version]:
     """Return reversed sorted list of release tag names."""
-    tags = git.Repo('..').tags
+    tags = git.Repo(search_parent_directories=True).tags
     versions = []
     for t in tags:
         try:
             versions.append(parse(t.name))
         except InvalidVersion:
             pass
     return sorted(versions, reverse=True)
@@ -73,30 +73,29 @@
         version = self._to_version(version)
         # If we release 1.2 we want to find 1.1
         for release in self._releases:
             if (release.major, release.minor) < (version.major, version.minor):
                 return release
 
 
-def main(repo: str, action: str, version: str) -> int:
-    info = VersionInfo(repo=repo)
+def main(action: str, version: str) -> int:
+    info = VersionInfo()
     if action == 'is-latest':
         print(info.is_latest(version))
     elif action == 'is-new':
         print(info.is_new(version))
     elif action == 'get-replaced':
         print(info.replaced(version))
     elif action == 'get-target':
         print(info.target(version))
     return 0
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Process some integers.')
-    parser.add_argument('--repo', dest='repo', required=True, help='Repository name')
     parser.add_argument('--action',
                         choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
                         required=True,
                         help='Action to perform: Check whether this major or minor '
                         'release exists or is new (is-latest), check whether this is a '
                         'new major or minor release (is-new), get the version this is '
                         'replacing (get-replaced), get the target folder for '
```

### Comparing `scippnexus-23.3.0/pyproject.toml` & `scippnexus-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/requirements/ci.txt` & `scippnexus-23.4.0/requirements/ci.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,56 @@
-# SHA1:082a95ae14987b5db9a325534ae9b82bd47d1615
+# SHA1:6344d52635ea11dca331a3bc6eb1833c4c64d585
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 cachetools==5.3.0
     # via tox
 certifi==2022.12.7
     # via requests
 chardet==5.1.0
     # via tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.11.0
     # via
     #   tox
     #   virtualenv
+gitdb==4.0.10
+    # via gitpython
+gitpython==3.1.31
+    # via -r ci.in
 idna==3.4
     # via requests
-packaging==23.0
+packaging==23.1
     # via
     #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
-pyproject-api==1.5.0
+pyproject-api==1.5.1
     # via tox
 requests==2.28.2
     # via -r ci.in
+smmap==5.0.0
+    # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.4.2
+tox==4.4.12
     # via -r ci.in
-urllib3==1.26.14
+urllib3==1.26.15
     # via requests
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via tox
```

### Comparing `scippnexus-23.3.0/requirements/docs.txt` & `scippnexus-23.4.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/requirements/static.txt` & `scippnexus-23.4.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/resources/logo-2022.svg` & `scippnexus-23.4.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/setup.cfg` & `scippnexus-23.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	python-dateutil
-	scipp>=23.01.1
+	scipp>=23.03.1
 	scipy  # we use scipp.interpolate which depends on this
 	h5py
 python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
 where = src
```

### Comparing `scippnexus-23.3.0/src/scippnexus/__init__.py` & `scippnexus-23.4.0/src/scippnexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/_common.py` & `scippnexus-23.4.0/src/scippnexus/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                                     "but multiple indices {select} were specified.")
         return {dims[0]: select[0]}
     elif isinstance(select, int) or isinstance(select, slice):
         check_1d()
         return {dims[0]: select}
     if not isinstance(select, dict):
         raise IndexError(f"Cannot process index {select}.")
-    return select
+    return select.copy()
 
 
 def to_plain_index(dims: List[str], select: ScippIndex) -> Union[int, slice, tuple]:
     """
     Given a valid "scipp" index 'select', return an equivalent plain numpy-style index.
     """
     select = _to_canonical_select(dims, select)
```

### Comparing `scippnexus-23.3.0/src/scippnexus/_hdf5_nexus.py` & `scippnexus-23.4.0/src/scippnexus/_hdf5_nexus.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/data/__init__.py` & `scippnexus-23.4.0/src/scippnexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/definition.py` & `scippnexus-23.4.0/src/scippnexus/definition.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/definitions/nxcansas.py` & `scippnexus-23.4.0/src/scippnexus/definitions/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md` & `scippnexus-23.4.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/file.py` & `scippnexus-23.4.0/src/scippnexus/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/leaf.py` & `scippnexus-23.4.0/src/scippnexus/leaf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nexus_classes.py` & `scippnexus-23.4.0/src/scippnexus/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxcylindrical_geometry.py` & `scippnexus-23.4.0/src/scippnexus/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxdata.py` & `scippnexus-23.4.0/src/scippnexus/nxdata.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxdetector.py` & `scippnexus-23.4.0/src/scippnexus/nxdetector.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxevent_data.py` & `scippnexus-23.4.0/src/scippnexus/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxlog.py` & `scippnexus-23.4.0/src/scippnexus/nxlog.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxmonitor.py` & `scippnexus-23.4.0/src/scippnexus/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxobject.py` & `scippnexus-23.4.0/src/scippnexus/nxobject.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxoff_geometry.py` & `scippnexus-23.4.0/src/scippnexus/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxsample.py` & `scippnexus-23.4.0/src/scippnexus/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/nxtransformations.py` & `scippnexus-23.4.0/src/scippnexus/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus/typing.py` & `scippnexus-23.4.0/src/scippnexus/typing.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.3.0/src/scippnexus.egg-info/PKG-INFO` & `scippnexus-23.4.0/src/scippnexus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.3.0
+Version: 23.4.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.3.0/tests/nexus_test.py` & `scippnexus-23.4.0/tests/nexus_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import h5py
 import numpy as np
 import pytest
 import scipp as sc
+from scipp.testing import assert_identical
 
-from scippnexus import (
-    Field,
+import scippnexus.v2 as snx
+from scippnexus.v2 import (
     NexusStructureError,
     NXdetector,
     NXentry,
     NXevent_data,
     NXlog,
     NXmonitor,
     NXroot,
@@ -23,18 +24,25 @@
     "∮ E⋅da = Q,  n → ∞, ∑ f(i) = ∏ g(i), ∀x∈ℝ: ⌈x⌉ = −⌊−x⌋, α ∧ ¬β = ¬(¬α ∨ β)",
     "2H₂ + O₂ ⇌ 2H₂O, R = 4.7 kΩ, ⌀ 200 mm",
     "Σὲ γνωρίζω ἀπὸ τὴν κόψη",
 )
 
 
 @pytest.fixture()
-def nxroot(request):
+def h5root():
+    """Yield h5py root group (file)"""
+    with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
+        yield f
+
+
+@pytest.fixture()
+def nxroot():
     """Yield NXroot containing a single NXentry named 'entry'"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
+        root = snx.Group(f, definitions=snx.base_definitions())
         root.create_class('entry', NXentry)
         yield root
 
 
 def test_nxobject_root(nxroot):
     assert nxroot.nx_class == NXroot
     assert set(nxroot.keys()) == {'entry'}
@@ -49,15 +57,15 @@
     nxroot.create_class('log', 'NXlog')
     assert set(nxroot.keys()) == {'entry', 'log'}
 
 
 def test_nxobject_items(nxroot):
     items = nxroot.items()
     assert len(items) == 1
-    name, entry = items[0]
+    name, entry = next(iter(items))
     assert name == 'entry'
     entry.create_class('monitor', NXmonitor)
     entry.create_class('log', NXlog)
     assert {k: v.nx_class
             for k, v in entry.items()} == {
                 'log': NXlog,
                 'monitor': NXmonitor
@@ -78,90 +86,94 @@
     assert entry.nx_class == NXentry
     entry.create_class('events_0', NXevent_data)
     entry.create_class('events_1', NXevent_data)
     entry.create_class('log', NXlog)
     assert set(entry.keys()) == {'events_0', 'events_1', 'log'}
 
 
-def test_nxobject_log(nxroot):
+def test_nx_class_can_be_bytes(h5root):
+    log = h5root.create_group('log')
+    attr = np.chararray((), itemsize=5)
+    attr[()] = b'NXlog'
+    log.attrs['NX_class'] = attr
+    group = snx.Group(log, definitions=snx.base_definitions())
+    assert group.nx_class == NXlog
+
+
+def test_nxobject_log(h5root):
     da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
                       coords={
                           'time':
                           sc.epoch(unit='ns') +
                           sc.array(dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(
                               unit='ns', dtype='int64')
                       })
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = da.data
-    log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    assert log.nx_class == NXlog
+    log = snx.create_class(h5root, 'log', NXlog)
+    snx.create_field(log, 'value', da.data)
+    snx.create_field(log, 'time', da.coords['time'] - sc.epoch(unit='ns'))
+    log = snx.Group(log, definitions=snx.base_definitions())
     assert sc.identical(log[...], da)
 
 
 def test_nxlog_with_missing_value_triggers_fallback(nxroot):
     time = sc.epoch(unit='ns') + sc.array(
         dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(unit='ns', dtype='int64')
     log = nxroot['entry'].create_class('log', NXlog)
     log['time'] = time - sc.epoch(unit='ns')
     loaded = log[()]
-    assert sc.identical(loaded, sc.DataGroup(time=time.rename(time='dim_0')))
+    # Fallback to DataGroup, but we still have partial info from NXlog: dim is time
+    assert_identical(loaded, sc.DataGroup(time=time))
 
 
-def test_nxlog_length_1(nxroot):
+def test_nxlog_length_1(h5root):
+    nxroot = snx.Group(h5root, definitions=snx.base_definitions())
     da = sc.DataArray(
         sc.array(dims=['time'], values=[1.1]),
         coords={
             'time':
             sc.epoch(unit='ns') +
             sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
         })
-    log = nxroot['entry'].create_class('log', NXlog)
+    log = nxroot.create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    assert log.nx_class == NXlog
     assert sc.identical(log[...], da)
 
 
-def test_nxlog_length_1_two_dims_no_time_squeezes_all_dims(nxroot):
-    da = sc.DataArray(
-        sc.array(dims=['time', 'ignored'], values=[[1.1]]),
-        coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
+def test_nxlog_length_1_two_dims_no_time_defaults_inner_dim_name(nxroot):
+    var = sc.array(dims=['time', 'ignored'], values=[[1.1]])
     log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = da.data
-    assert sc.identical(log[...], sc.DataArray(sc.scalar(1.1)))
+    log['value'] = var
+    assert_identical(log[...], sc.DataArray(var.rename(ignored='dim_1')))
 
 
-def test_nxlog_length_1_two_dims_with_time_squeezes_inner_dim(nxroot):
+def test_nxlog_length_1_two_dims_with_time_defaults_inner_dim_name(nxroot):
     da = sc.DataArray(
         sc.array(dims=['time', 'ignored'], values=[[1.1]]),
         coords={
             'time':
             sc.epoch(unit='ns') +
             sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
         })
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    assert sc.identical(log[...], da['ignored', 0])
+    assert sc.identical(log[...], da.rename(ignored='dim_1'))
 
 
 def test_nxlog_axes_replaces_time_dim(nxroot):
     da = sc.DataArray(
         sc.array(dims=['time', 'ignored'], values=[[1.1]]),
         coords={
             'time':
             sc.epoch(unit='ns') +
             sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
         })
     log = nxroot['entry'].create_class('log', NXlog)
-    log.attrs['axes'] = ['yy', 'xx']
+    log._group.attrs['axes'] = ['yy', 'xx']
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
     expected = sc.DataArray(sc.array(dims=['yy', 'xx'], values=[[1.1]]),
                             coords={'time': da.coords['time'].squeeze()})
     assert sc.identical(log[...], expected)
 
 
@@ -173,27 +185,28 @@
             sc.epoch(unit='ns') +
             sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
         })
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time'] - sc.epoch(unit='ns')
     loaded = log[...]
-    assert sc.identical(
+    assert_identical(
         loaded.data,
         sc.array(dims=['time', 'dim_1', 'dim_2'], values=np.arange(9.).reshape(1, 3,
                                                                                3)))
 
 
 def test_nxlog_with_shape_0(nxroot):
     da = sc.DataArray(sc.ones(dims=['time', 'ignored'], shape=(0, 1)),
                       coords={'time': sc.ones(dims=['time'], shape=(0, ), unit='s')})
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = da.data
     log['time'] = da.coords['time']
-    assert sc.identical(log[...], da['ignored', 0])
+    da.coords['time'] = sc.datetimes(dims=['time'], values=[], unit='ns')
+    assert_identical(log[...], da.rename(ignored='dim_1'))
 
 
 def test_nxobject_event_data(nxroot):
     event_data = nxroot['entry'].create_class('events_0', NXevent_data)
     assert event_data.nx_class == NXevent_data
 
 
@@ -233,33 +246,33 @@
 
 
 def test_nxobject_getitem_by_class_get_fields(nxroot):
     nxroot['entry'].create_class('log', NXlog)
     nxroot['entry'].create_class('events_0', NXevent_data)
     nxroot['entry']['field1'] = sc.arange('event', 4.0, unit='ns')
     nxroot['entry']['field2'] = sc.arange('event', 2.0, unit='ns')
-    assert list(nxroot[Field]) == []
-    assert set(nxroot['entry'][Field]) == {'field1', 'field2'}
+    assert list(nxroot[snx.Field]) == []
+    assert set(nxroot['entry'][snx.Field]) == {'field1', 'field2'}
 
 
 def test_nxobject_getitem_by_class_list(nxroot):
     nxroot['entry'].create_class('log', NXlog)
     nxroot['entry'].create_class('events_0', NXevent_data)
     nxroot['entry'].create_class('events_1', NXevent_data)
     nxroot['entry']['field1'] = sc.arange('event', 4.0, unit='ns')
     assert set(nxroot['entry'][[NXlog,
                                 NXevent_data]]) == {'log', 'events_0', 'events_1'}
-    assert set(nxroot['entry'][[NXlog, Field]]) == {'log', 'field1'}
+    assert set(nxroot['entry'][[NXlog, snx.Field]]) == {'log', 'field1'}
 
 
 def test_nxobject_dataset_items_are_returned_as_Field(nxroot):
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('event', 5)
     field = nxroot['entry/events_0/event_time_offset']
-    assert isinstance(field, Field)
+    assert isinstance(field, snx.Field)
 
 
 def test_field_properties(nxroot):
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('event', 6, dtype='int64', unit='ns')
     field = nxroot['entry/events_0/event_time_offset']
     assert field.dtype == 'int64'
@@ -272,16 +285,16 @@
     events = nxroot['entry'].create_class('events_0', NXevent_data)
     events['event_time_offset'] = sc.arange('ignored', 2)
     events['event_time_zero'] = sc.arange('ignored', 2)
     events['event_index'] = sc.arange('ignored', 2)
     events['event_id'] = sc.arange('ignored', 2)
     event_data = nxroot['entry/events_0']
     assert event_data['event_time_offset'].dims == ('event', )
-    assert event_data['event_time_zero'].dims == ('pulse', )
-    assert event_data['event_index'].dims == ('pulse', )
+    assert event_data['event_time_zero'].dims == ('event_time_zero', )
+    assert event_data['event_index'].dims == ('event_time_zero', )
     assert event_data['event_id'].dims == ('event', )
     log = nxroot['entry'].create_class('log', NXlog)
     log['value'] = sc.arange('ignored', 2)
     log['time'] = sc.arange('ignored', 2)
     assert log['time'].dims == ('time', )
     assert log['value'].dims == ('time', )
 
@@ -291,14 +304,33 @@
     log['value'] = sc.arange('ignored', 2, unit=None)
     log['time'] = sc.arange('ignored', 2)
     assert log.unit is None
     field = log['value']
     assert field.unit is None
 
 
+def test_field_errors_with_same_unit_handles_them_with_value(nxroot):
+    entry = nxroot.create_class('group', snx.NXentry)
+    entry['value'] = sc.array(dims=['ignored'], values=[10.0], unit='m')
+    entry['value_errors'] = sc.array(dims=['ignored'], values=[2.0], unit='m')
+    value = nxroot['group']['value'][()]
+    assert_identical(value, sc.scalar(value=10.0, variance=4.0, unit='m'))
+
+
+def test_field_errors_with_different_unit_handles_them_individually(nxroot):
+    entry = nxroot.create_class('group', snx.NXentry)
+    entry['value'] = sc.array(dims=['ignored'], values=[10.0], unit='m')
+    entry['value_errors'] = sc.array(dims=['ignored'], values=[200.0], unit='cm')
+    value = nxroot['group']['value'][()]
+    assert_identical(value, sc.scalar(value=10.0, unit='m'))
+    assert 'value_errors' in nxroot['group']
+    errors = nxroot['group']['value_errors'][()]
+    assert_identical(errors, sc.scalar(value=200.0, unit='cm'))
+
+
 @pytest.mark.parametrize('value,type_', [(1.2, np.float32), (123, np.int32),
                                          ('abc', str), (True, bool)])
 def test_field_is_returned_as_python_object_if_shape_empty_and_no_unit(
         nxroot, value, type_):
     nxroot['field1'] = sc.scalar(value, unit=None, dtype=type_)
     field = nxroot['field1'][()]
     assert isinstance(field, type_)
@@ -337,142 +369,100 @@
 
 def test_field_of_extended_ascii_in_ascii_encoded_dataset_is_loaded_correctly():
     # When writing, if we use bytes h5py will write as ascii encoding
     # 0xb0 = degrees symbol in latin-1 encoding.
     string = b"run at rot=90" + bytes([0xb0])
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
         f['title'] = np.array([string, string + b'x'])
-        title = NXroot(f)['title']
+        title = snx.Group(f)['title']
         assert sc.identical(
             title[...],
             sc.array(dims=['dim_0'], values=["run at rot=90°", "run at rot=90°x"]))
 
 
 def test_ms_field_with_second_datetime_attribute_loaded_as_ms_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='ms')
-    nxroot['mytime'].attrs['start_time'] = '2022-12-12T12:13:14'
+    nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:14'
     assert sc.identical(
         nxroot['mytime'][...],
         sc.datetimes(dims=['dim_0'],
                      unit='ms',
                      values=['2022-12-12T12:13:14.000', '2022-12-12T12:13:14.001']))
 
 
 def test_ns_field_with_second_datetime_attribute_loaded_as_ns_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='ns')
-    nxroot['mytime'].attrs['start_time'] = '1970-01-01T00:00:00'
+    nxroot['mytime'].dataset.attrs['start_time'] = '1970-01-01T00:00:00'
     assert sc.identical(
         nxroot['mytime'][...],
         sc.datetimes(
             dims=['dim_0'],
             unit='ns',
             values=['1970-01-01T00:00:00.000000000', '1970-01-01T00:00:00.000000001']))
 
 
 def test_second_field_with_ns_datetime_attribute_loaded_as_ns_datetime(nxroot):
     nxroot['mytime'] = sc.arange('ignored', 2, unit='s')
-    nxroot['mytime'].attrs['start_time'] = '1984-01-01T00:00:00.000000000'
+    nxroot['mytime'].dataset.attrs['start_time'] = '1984-01-01T00:00:00.000000000'
     assert sc.identical(
         nxroot['mytime'][...],
         sc.datetimes(dims=['dim_0'],
                      unit='ns',
                      values=['1984-01-01T00:00:00', '1984-01-01T00:00:01']))
 
 
 @pytest.mark.parametrize('timezone,hhmm', [('Z', '12:00'), ('+04', '08:00'),
                                            ('+00', '12:00'), ('-02', '14:00'),
                                            ('+1130', '00:30'), ('-0930', '21:30'),
                                            ('+11:30', '00:30'), ('-09:30', '21:30')])
 def test_timezone_information_in_datetime_attribute_is_applied(nxroot, timezone, hhmm):
     nxroot['mytime'] = sc.scalar(value=3, unit='s')
-    nxroot['mytime'].attrs['start_time'] = f'1984-01-01T12:00:00{timezone}'
+    nxroot['mytime'].dataset.attrs['start_time'] = f'1984-01-01T12:00:00{timezone}'
     assert sc.identical(nxroot['mytime'][...],
                         sc.datetime(unit='s', value=f'1984-01-01T{hhmm}:03'))
 
 
 def test_timezone_information_in_datetime_attribute_preserves_ns_precision(nxroot):
     nxroot['mytime'] = sc.scalar(value=3, unit='s')
-    nxroot['mytime'].attrs['start_time'] = '1984-01-01T12:00:00.123456789+0200'
+    nxroot['mytime'].dataset.attrs['start_time'] = '1984-01-01T12:00:00.123456789+0200'
     assert sc.identical(nxroot['mytime'][...],
                         sc.datetime(unit='ns', value='1984-01-01T10:00:03.123456789'))
 
 
 def test_loads_bare_timestamps_if_multiple_candidate_datetime_offsets_found(nxroot):
     offsets = sc.arange('ignored', 2, unit='ms')
     nxroot['mytime'] = offsets
-    nxroot['mytime'].attrs['offset'] = '2022-12-12T12:13:14'
-    nxroot['mytime'].attrs['start_time'] = '2022-12-12T12:13:15'
+    nxroot['mytime'].dataset.attrs['offset'] = '2022-12-12T12:13:14'
+    nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:15'
     assert sc.identical(nxroot['mytime'][...], offsets.rename(ignored='dim_0'))
 
 
-def create_event_data_ids_1234(group):
-    group['event_id'] = sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2, 2])
-    group['event_time_offset'] = sc.array(dims=[''],
-                                          unit='s',
-                                          values=[456, 7, 3, 345, 632, 23])
-    group['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
-    group['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, -1000])
-
-
-def test_negative_event_index_converted_to_num_event(nxroot):
-    event_data = nxroot['entry'].create_class('events_0', NXevent_data)
-    create_event_data_ids_1234(event_data)
-    events = nxroot['entry/events_0'][...]
-    assert events.bins.size().values[2] == 3
-    assert events.bins.size().values[3] == 0
-
-
-def test_bad_event_index_causes_load_as_DataGroup(nxroot):
-    event_data = nxroot['entry'].create_class('events_0', NXevent_data)
-    event_data['event_id'] = sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2])
-    event_data['event_time_offset'] = sc.array(dims=[''], unit='s', values=[0, 0, 0, 0])
-    event_data['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
-    event_data['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, 666])
-    dg = nxroot['entry/events_0'][...]
-    assert isinstance(dg, sc.DataGroup)
-
-
-def create_event_data_without_event_id(group):
-    group['event_time_offset'] = sc.array(dims=[''],
-                                          unit='s',
-                                          values=[456, 7, 3, 345, 632, 23])
-    group['event_time_zero'] = sc.array(dims=[''], unit='s', values=[1, 2, 3, 4])
-    group['event_index'] = sc.array(dims=[''], unit=None, values=[0, 3, 3, 5])
-
-
-def test_event_data_without_event_id_can_be_loaded(nxroot):
-    event_data = nxroot['entry'].create_class('events_0', NXevent_data)
-    create_event_data_without_event_id(event_data)
-    da = event_data[...]
-    assert len(da.bins.coords) == 1
-    assert 'event_time_offset' in da.bins.coords
-
-
-def test_event_mode_monitor_without_event_id_can_be_loaded(nxroot):
-    monitor = nxroot['entry'].create_class('monitor', NXmonitor)
-    create_event_data_without_event_id(monitor)
-    da = monitor[...]
-    assert len(da.bins.coords) == 1
-    assert 'event_time_offset' in da.bins.coords
+def test_length_0_field_with_datetime_attribute_loaded_as_datetime(nxroot):
+    nxroot['mytime'] = sc.arange('ignored', 0, unit='ms')
+    nxroot['mytime'].dataset.attrs['start_time'] = '2022-12-12T12:13:14'
+    assert_identical(nxroot['mytime'][...],
+                     sc.datetimes(dims=['dim_0'], unit='ms', values=[]))
 
 
+@pytest.mark.skip(reason='Special attributes disabled for now. Do we keep them?')
 def test___getattr__for_unique_child_groups(nxroot):
     entry = nxroot['entry']
     with pytest.raises(NexusStructureError):
         entry.log
     entry.create_class('log1', NXlog)
     log = entry.log
     assert log.nx_class == NXlog
     assert log.name == '/entry/log1'
     assert isinstance(log, NXlog)
     entry.create_class('log2', NXlog)
     with pytest.raises(NexusStructureError):
         entry.log
 
 
+@pytest.mark.skip(reason='Special attributes disabled for now. Do we keep them?')
 def test___dir__(nxroot):
     entry = nxroot['entry']
     assert 'log' not in entry.__dir__()
     entry.create_class('log1', NXlog)
     assert 'log' in entry.__dir__()
     entry.create_class('log2', NXlog)
     assert 'log' not in entry.__dir__()
@@ -480,7 +470,125 @@
 
 def test___dir__includes_non_dynamic_properties(nxroot):
     entry = nxroot['entry']
     det = entry.create_class('det', NXdetector)
     det.create_class('events', NXevent_data)
     # Ensure we are not replacing __dir__ but adding to it
     assert 'unit' in det.__dir__()
+
+
+def test_read_recursive(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data['signal'] = np.arange(4)
+    data['signal'].attrs['units'] = 'm'
+    data['time'] = np.arange(5)
+    data['time'].attrs['units'] = 's'
+    obj = snx.Group(entry)
+    dg = obj[()]
+    assert obj.sizes == {'dim_0': None}
+    assert 'data' in dg
+
+
+def test_errors_read_as_variances(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data['signal'] = np.arange(4.0)
+    data['signal'].attrs['units'] = 'm'
+    data['signal_errors'] = np.arange(4.0)
+    data['signal_errors'].attrs['units'] = 'm'
+    data['time'] = np.arange(5.0)
+    data['time'].attrs['units'] = 's'
+    data['time_errors'] = np.arange(5.0)
+    data['time_errors'].attrs['units'] = 's'
+    obj = snx.Group(data)
+    assert set(obj._children.keys()) == {'signal', 'time'}
+    dg = obj[()]
+    assert dg['signal'].variances is not None
+    assert dg['time'].variances is not None
+    assert np.array_equal(dg['signal'].variances, np.arange(4.0)**2)
+    assert np.array_equal(dg['time'].variances, np.arange(5.0)**2)
+
+
+def test_read_field(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data['signal'] = np.arange(4)
+    data['signal'].attrs['units'] = 'm'
+    obj = snx.Group(data)
+    var = obj['signal'][()]
+    assert sc.identical(var, sc.array(dims=['dim_0'], values=np.arange(4), unit='m'))
+
+
+def test_nxdata_with_signal_axes_indices_reads_as_data_array(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data.attrs['NX_class'] = 'NXdata'
+    data.attrs['signal'] = 'signal'
+    data.attrs['axes'] = ['time', 'temperature']
+    data.attrs['time_indices'] = [0]
+    data.attrs['temperature_indices'] = [1]
+    ref = sc.DataArray(
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+    ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
+    ref.coords['temperature'] = sc.array(dims=['temperature'],
+                                         values=np.arange(4),
+                                         unit='K')
+    data['signal'] = ref.values
+    data['signal'].attrs['units'] = str(ref.unit)
+    data['time'] = ref.coords['time'].values
+    data['time'].attrs['units'] = str(ref.coords['time'].unit)
+    data['temperature'] = ref.coords['temperature'].values
+    data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
+    obj = snx.Group(data, definitions=snx.base_definitions())
+    da = obj[()]
+    assert sc.identical(da, ref)
+
+
+def test_nxdata_positional_indexing_returns_correct_slice(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data.attrs['NX_class'] = 'NXdata'
+    data.attrs['signal'] = 'signal'
+    data.attrs['axes'] = ['time', 'temperature']
+    data.attrs['time_indices'] = [0]
+    data.attrs['temperature_indices'] = [1]
+    ref = sc.DataArray(
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+    ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
+    ref.coords['temperature'] = sc.array(dims=['temperature'],
+                                         values=np.arange(4),
+                                         unit='K')
+    data['signal'] = ref.values
+    data['signal'].attrs['units'] = str(ref.unit)
+    data['time'] = ref.coords['time'].values
+    data['time'].attrs['units'] = str(ref.coords['time'].unit)
+    data['temperature'] = ref.coords['temperature'].values
+    data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
+    obj = snx.Group(data, definitions=snx.base_definitions())
+    da = obj['time', 0:2]
+    assert sc.identical(da, ref['time', 0:2])
+
+
+def test_nxdata_with_bin_edges_positional_indexing_returns_correct_slice(h5root):
+    entry = h5root.create_group('entry')
+    data = entry.create_group('data')
+    data.attrs['NX_class'] = 'NXdata'
+    data.attrs['signal'] = 'signal'
+    data.attrs['axes'] = ['time', 'temperature']
+    data.attrs['time_indices'] = [0]
+    data.attrs['temperature_indices'] = [1]
+    ref = sc.DataArray(
+        data=sc.ones(dims=['time', 'temperature'], shape=[3, 4], unit='m'))
+    ref.coords['time'] = sc.array(dims=['time'], values=np.arange(3), unit='s')
+    ref.coords['temperature'] = sc.array(dims=['temperature'],
+                                         values=np.arange(5),
+                                         unit='K')
+    data['signal'] = ref.values
+    data['signal'].attrs['units'] = str(ref.unit)
+    data['time'] = ref.coords['time'].values
+    data['time'].attrs['units'] = str(ref.coords['time'].unit)
+    data['temperature'] = ref.coords['temperature'].values
+    data['temperature'].attrs['units'] = str(ref.coords['temperature'].unit)
+    obj = snx.Group(data, definitions=snx.base_definitions())
+    da = obj['temperature', 0:2]
+    assert sc.identical(da, ref['temperature', 0:2])
```

### Comparing `scippnexus-23.3.0/tests/nxcylindrical_geometry_test.py` & `scippnexus-23.4.0/tests/nxcylindrical_geometry_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import h5py
 import pytest
 import scipp as sc
 
-from scippnexus import NXcylindrical_geometry, NXentry, NXroot
+import scippnexus.v2 as snx
 
 
 @pytest.fixture()
-def nxroot(request):
+def nxroot():
     """Yield NXroot containing a single NXentry named 'entry'"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
-        root.create_class('entry', NXentry)
+        root = snx.Group(f, snx.base_definitions())
+        root.create_class('entry', snx.NXentry)
         yield root
 
 
 def test_vertices_loaded_as_vector3(nxroot):
-    shape = nxroot['entry'].create_class('shape', NXcylindrical_geometry)
+    shape = nxroot['entry'].create_class('shape', snx.NXcylindrical_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='mm')
     loaded = shape[()]
     assert sc.identical(loaded['vertices'],
                         sc.vectors(dims=['vertex'], values=values, unit='mm'))
 
 
 def test_field_properties(nxroot):
-    shape = nxroot['entry'].create_class('shape', NXcylindrical_geometry)
+    shape = nxroot['entry'].create_class('shape', snx.NXcylindrical_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='m')
     shape['cylinders'] = sc.array(dims=['ignored', 'index'],
                                   values=[[0, 1, 2]],
                                   unit=None)
     shape['detector_number'] = sc.array(dims=['ignored'], values=[], unit=None)
     loaded = shape[()]
```

### Comparing `scippnexus-23.3.0/tests/nxdetector_test.py` & `scippnexus-23.4.0/tests/nxdetector_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,467 +1,521 @@
 import h5py
 import numpy as np
 import pytest
 import scipp as sc
+from scipp.testing import assert_identical
 
-import scippnexus as snx
-from scippnexus import (
-    NexusStructureError,
-    NXdetector,
-    NXentry,
-    NXevent_data,
-    NXobject,
-    NXoff_geometry,
-    NXroot,
-)
+import scippnexus.v2 as snx
+from scippnexus.v2 import NXdetector, NXentry, NXoff_geometry
+
+
+def make_group(group: h5py.Group) -> snx.Group:
+    return snx.Group(group, definitions=snx.base_definitions())
+
+
+@pytest.fixture()
+def h5root():
+    """Yield h5py root group (file)"""
+    with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
+        yield f
 
 
 @pytest.fixture()
-def nxroot(request):
+def nxroot():
     """Yield NXroot containing a single NXentry named 'entry'"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
+        root = make_group(f)
         root.create_class('entry', NXentry)
         yield root
 
 
-def test_warns_if_no_data_found(nxroot):
+def test_returns_as_datagroup_if_no_signal_found(nxroot):
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_numbers', detector_numbers)
-    with pytest.warns(UserWarning, match="Failed to load "):
-        dg = detector[...]
+    dg = detector[...]
     assert isinstance(dg, sc.DataGroup)
 
 
-def test_can_load_fields_if_no_data_found(nxroot):
+def test_can_load_fields_if_no_data_found(h5root):
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', detector_numbers)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, 'detector_numbers', detector_numbers)
     detector['detector_numbers'][...]
 
 
-def test_finds_data_from_group_attr(nxroot):
+def test_finds_data_from_group_attr(h5root):
     da = sc.DataArray(
         sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', da.coords['detector_numbers'])
-    detector.create_field('custom', da.data)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
+    snx.create_field(detector, 'custom', da.data)
     detector.attrs['signal'] = 'custom'
+    detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
 
 
-def test_loads_events_when_data_and_events_found(nxroot):
+def test_loads_signal_and_events_when_both_found(nxroot):
     detector_number = sc.array(dims=[''], unit=None, values=np.array([1, 2]))
-    data = sc.ones(dims=['xx'], shape=[2])
+    data = sc.ones(dims=['detector_number'], shape=[2])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_number)
     detector.create_field('data', data)
-    assert detector[...].bins is None
+    events = detector.create_class('events', snx.NXevent_data)
+    events.create_field('event_id', sc.array(dims=[''], unit=None, values=[1]))
+    events.create_field('event_time_offset', sc.array(dims=[''], unit='s', values=[1]))
+    events.create_field('event_time_zero', sc.array(dims=[''], unit='s', values=[1]))
+    events.create_field('event_index', sc.array(dims=[''], unit='None', values=[0]))
+    assert detector.sizes == {'detector_number': 2, 'event_time_zero': 1}
+    loaded = detector[...]
+    assert isinstance(loaded, sc.Dataset)
+    assert_identical(loaded['data'].data, data)
+    assert loaded['events'].bins is not None
+
+
+def test_loads_as_data_array_with_embedded_events(nxroot):
+    detector_number = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3]))
+    detector = nxroot.create_class('detector0', NXdetector)
+    detector.create_field('detector_number', detector_number)
     detector.create_field('event_id', sc.array(dims=[''], unit=None, values=[1]))
     detector.create_field('event_time_offset', sc.array(dims=[''], unit='s',
                                                         values=[1]))
     detector.create_field('event_time_zero', sc.array(dims=[''], unit='s', values=[1]))
     detector.create_field('event_index', sc.array(dims=[''], unit='None', values=[0]))
-    loaded = detector[...]
-    assert loaded.bins is not None
-    assert loaded.values[0].variances is None
+    assert detector.dims == ('detector_number', 'event_time_zero')
+    da = detector[...]
+    assert da.bins is not None
+    assert_identical(
+        da.bins.size(),
+        sc.DataArray(
+            data=sc.array(dims=['detector_number'], unit=None, values=[1, 0, 0]),
+            coords={'detector_number': detector_number.rename({'':
+                                                               'detector_number'})}))
 
 
 def detector_numbers_xx_yy_1234():
     return sc.array(dims=['xx', 'yy'], unit=None, values=np.array([[1, 2], [3, 4]]))
 
 
-def test_loads_data_without_coords(nxroot):
+def test_loads_data_without_coords(h5root):
     da = sc.DataArray(sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', da.coords['detector_numbers'])
-    detector.create_field('data', da.data)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
+    snx.create_field(detector, 'data', da.data)
+    detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
 
 
 @pytest.mark.parametrize('detector_number_key',
                          ['detector_number', 'pixel_id', 'spectrum_index'])
-def test_detector_number_key_alias(nxroot, detector_number_key):
+def test_detector_number_key_alias(h5root, detector_number_key):
     da = sc.DataArray(sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords[detector_number_key] = detector_numbers_xx_yy_1234()
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field(detector_number_key, da.coords[detector_number_key])
-    detector.create_field('data', da.data)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, detector_number_key, da.coords[detector_number_key])
+    snx.create_field(detector, 'data', da.data)
+    detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'xx': 'dim_0', 'yy': 'dim_1'}))
 
 
-def test_select_events_raises_if_detector_contains_data(nxroot):
-    da = sc.DataArray(sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]]))
-    da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', da.coords['detector_numbers'])
-    detector.create_field('data', da.data)
-    with pytest.raises(NexusStructureError):
-        detector.select_events
-
-
-def test_loads_data_with_coords(nxroot):
+def test_loads_data_with_coords(h5root):
     da = sc.DataArray(
         sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords['detector_numbers'] = detector_numbers_xx_yy_1234()
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', da.coords['detector_numbers'])
-    detector.create_field('xx', da.coords['xx'])
-    detector.create_field('data', da.data)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
+    snx.create_field(detector, 'xx', da.coords['xx'])
+    snx.create_field(detector, 'data', da.data)
     detector.attrs['axes'] = ['xx', '.']
+    detector = make_group(detector)
     assert sc.identical(detector[...], da.rename_dims({'yy': 'dim_1'}))
 
 
-def test_slicing_works_as_in_scipp(nxroot):
+def test_slicing_works_as_in_scipp(h5root):
     da = sc.DataArray(
         sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2, 3.3], [3.3, 4.4,
                                                                         5.5]]))
     da.coords['detector_numbers'] = sc.array(dims=['xx', 'yy'],
                                              unit=None,
                                              values=np.array([[1, 2, 3], [4, 5, 6]]))
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
     da.coords['xx2'] = sc.array(dims=['xx'], unit='m', values=[0.3, 0.4])
     da.coords['yy'] = sc.array(dims=['yy'], unit='m', values=[0.1, 0.2, 0.3])
     da.coords['2d_edges'] = sc.array(dims=['yy', 'xx'],
                                      unit='m',
                                      values=[[1, 2, 3], [4, 5, 6], [7, 8, 9]])
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_numbers', da.coords['detector_numbers'])
-    detector.create_field('xx', da.coords['xx'])
-    detector.create_field('xx2', da.coords['xx2'])
-    detector.create_field('yy', da.coords['yy'])
-    detector.create_field('2d_edges', da.coords['2d_edges'])
-    detector.create_field('data', da.data)
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    snx.create_field(detector, 'detector_numbers', da.coords['detector_numbers'])
+    snx.create_field(detector, 'xx', da.coords['xx'])
+    snx.create_field(detector, 'xx2', da.coords['xx2'])
+    snx.create_field(detector, 'yy', da.coords['yy'])
+    snx.create_field(detector, '2d_edges', da.coords['2d_edges'])
+    snx.create_field(detector, 'data', da.data)
     detector.attrs['axes'] = ['xx', 'yy']
     detector.attrs['2d_edges_indices'] = [1, 0]
-    assert sc.identical(detector[...], da)
-    assert sc.identical(detector['xx', 0], da['xx', 0])
-    assert sc.identical(detector['xx', 1], da['xx', 1])
-    assert sc.identical(detector['xx', 0:1], da['xx', 0:1])
-    assert sc.identical(detector['yy', 0], da['yy', 0])
-    assert sc.identical(detector['yy', 1], da['yy', 1])
-    assert sc.identical(detector['yy', 0:1], da['yy', 0:1])
-    assert sc.identical(detector['yy', 1:1], da['yy', 1:1])  # empty slice
+    detector = make_group(detector)
+    assert_identical(detector[...], da)
+    assert_identical(detector['xx', 0], da['xx', 0])
+    assert_identical(detector['xx', 1], da['xx', 1])
+    assert_identical(detector['xx', 0:1], da['xx', 0:1])
+    assert_identical(detector['yy', 0], da['yy', 0])
+    assert_identical(detector['yy', 1], da['yy', 1])
+    assert_identical(detector['yy', 0:1], da['yy', 0:1])
+    assert_identical(detector['yy', 1:1], da['yy', 1:1])  # empty slice
 
 
 def create_event_data_ids_1234(group):
     group.create_field('event_id',
                        sc.array(dims=[''], unit=None, values=[1, 2, 4, 1, 2, 2]))
     group.create_field('event_time_offset',
                        sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]))
     group.create_field('event_time_zero',
                        sc.array(dims=[''], unit='s', values=[1, 2, 3, 4]))
     group.create_field('event_index',
                        sc.array(dims=[''], unit='None', values=[0, 3, 3, 5]))
 
 
 def test_loads_event_data_mapped_to_detector_numbers_based_on_their_event_id(nxroot):
-    detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
+    detector_numbers = sc.array(dims=[''],
+                                unit=None,
+                                values=np.array([1, 2, 3, 4, 5, 6]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ('detector_number', )
-    assert detector.shape == (4, )
-    loaded = detector[...]
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.sizes == {'detector_number': 6, 'event_time_zero': 4}
+    da = detector[...]
     assert sc.identical(
-        loaded.bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['detector_number'],
                  unit=None,
                  dtype='int64',
-                 values=[2, 3, 0, 1]))
-    assert 'event_time_offset' in loaded.bins.coords
-    assert 'event_time_zero' in loaded.bins.coords
+                 values=[2, 3, 0, 1, 0, 0]))
+    assert 'event_time_offset' in da.bins.coords
+    assert 'event_time_zero' in da.bins.coords
+
+
+def test_detector_number_fallback_dims_determines_dims_with_event_data(nxroot):
+    detector_numbers = sc.array(dims=['detector_number'],
+                                unit=None,
+                                values=np.array([1, 2, 3, 4, 5, 6]))
+    detector = nxroot.create_class('detector0', NXdetector)
+    detector.create_field('detector_number', detector_numbers)
+    detector.create_field('pixel_offset', detector_numbers)
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    da = detector[()]
+    assert da.sizes == {'detector_number': 6}
+    assert_identical(da.coords['pixel_offset'], detector_numbers)
 
 
 def test_loads_event_data_with_0d_detector_numbers(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', sc.index(1, dtype='int64'))
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ()
-    assert detector.shape == ()
-    loaded = detector[...]
-    assert sc.identical(loaded.bins.size().data, sc.index(2, dtype='int64'))
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.dims == ('event_time_zero', )
+    assert detector.shape == (4, )
+    da = detector[...]
+    assert sc.identical(da.bins.size().data, sc.index(2, dtype='int64'))
 
 
 def test_loads_event_data_with_2d_detector_numbers(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ('dim_0', 'dim_1')
-    assert detector.shape == (2, 2)
-    loaded = detector[...]
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
+    da = detector[...]
     assert sc.identical(
-        loaded.bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['dim_0', 'dim_1'],
                  unit=None,
                  dtype='int64',
                  values=[[2, 3], [0, 1]]))
 
 
+def test_selecting_pixels_works_with_event_signal(nxroot):
+    detector = nxroot.create_class('detector0', NXdetector)
+    detector.create_field('detector_number', detector_numbers_xx_yy_1234())
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
+    da = detector['dim_0', 0]
+    assert_identical(da.bins.size().data,
+                     sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]))
+
+
+def test_selecting_pixels_works_with_embedded_event_signal(nxroot):
+    detector = nxroot.create_class('detector0', NXdetector)
+    detector.create_field('detector_number', detector_numbers_xx_yy_1234())
+    create_event_data_ids_1234(detector)
+    assert detector.sizes == {'dim_0': 2, 'dim_1': 2, 'event_time_zero': 4}
+    da = detector['dim_0', 0]
+    assert_identical(da.bins.size().data,
+                     sc.array(dims=['dim_1'], unit=None, dtype='int64', values=[2, 3]))
+
+
 def test_select_events_slices_underlying_event_data(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers_xx_yy_1234())
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    da = detector['event_time_zero', :2]
     assert sc.identical(
-        detector.select_events['pulse', :2][...].bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['dim_0', 'dim_1'],
                  unit=None,
                  dtype='int64',
                  values=[[1, 1], [0, 1]]))
+    da = detector['event_time_zero', :3]
     assert sc.identical(
-        detector.select_events['pulse', :3][...].bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['dim_0', 'dim_1'],
                  unit=None,
                  dtype='int64',
                  values=[[2, 2], [0, 1]]))
+    da = detector['event_time_zero', 3]
     assert sc.identical(
-        detector.select_events['pulse', 3][...].bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['dim_0', 'dim_1'],
                  unit=None,
                  dtype='int64',
                  values=[[0, 1], [0, 0]]))
+    da = detector[()]
     assert sc.identical(
-        detector.select_events[...][...].bins.size().data,
-        sc.array(dims=['dim_0', 'dim_1'],
-                 unit=None,
-                 dtype='int64',
-                 values=[[2, 3], [0, 1]]))
-
-
-def test_select_events_slice_does_not_affect_original_detector(nxroot):
-    detector = nxroot.create_class('detector0', NXdetector)
-    detector.create_field('detector_number', detector_numbers_xx_yy_1234())
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    detector.select_events['pulse', 0][...]
-    assert sc.identical(
-        detector[...].bins.size().data,
+        da.bins.size().data,
         sc.array(dims=['dim_0', 'dim_1'],
                  unit=None,
                  dtype='int64',
                  values=[[2, 3], [0, 1]]))
 
 
-def test_loading_event_data_creates_automatic_detector_numbers_if_not_present_in_file(
-        nxroot):
+def test_loading_event_data_without_detector_numbers_does_not_group_events(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ['detector_number']
-    with pytest.raises(NexusStructureError):
-        detector.shape
-    loaded = detector[...]
-    assert sc.identical(
-        loaded.bins.size().data,
-        sc.array(dims=['detector_number'],
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.dims == ('event_time_zero', )
+    da = detector[...]
+    assert_identical(
+        da.bins.size().data,
+        sc.array(dims=['event_time_zero'],
                  unit=None,
                  dtype='int64',
-                 values=[2, 3, 0, 1]))
+                 values=[3, 0, 2, 1]))
 
 
-def test_loading_event_data_with_selection_and_automatic_detector_numbers_raises(
+def test_loading_event_data_with_det_selection_and_automatic_detector_numbers_raises(
         nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ['detector_number']
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.dims == ('event_time_zero', )
     with pytest.raises(sc.DimensionError):
         detector['detector_number', 0]
 
 
 def test_loading_event_data_with_full_selection_and_automatic_detector_numbers_works(
         nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
-    assert detector.dims == ['detector_number']
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+    assert detector.dims == ('event_time_zero', )
     assert tuple(detector[...].shape) == (4, )
     assert tuple(detector[()].shape) == (4, )
 
 
 def test_event_data_field_dims_labels(nxroot):
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     assert detector['detector_number'].dims == ('detector_number', )
 
 
 def test_nxevent_data_selection_yields_correct_pulses(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
-    create_event_data_ids_1234(detector.create_class('events', NXevent_data))
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
 
     class Load:
 
         def __getitem__(self, select=...):
             da = detector['events'][select]
             return da.bins.size().values
 
     assert np.array_equal(Load()[...], [3, 0, 2, 1])
-    assert np.array_equal(Load()['pulse', 0], 3)
-    assert np.array_equal(Load()['pulse', 1], 0)
-    assert np.array_equal(Load()['pulse', 3], 1)
-    assert np.array_equal(Load()['pulse', -1], 1)
-    assert np.array_equal(Load()['pulse', -2], 2)
-    assert np.array_equal(Load()['pulse', 0:0], [])
-    assert np.array_equal(Load()['pulse', 1:1], [])
-    assert np.array_equal(Load()['pulse', 1:-3], [])
-    assert np.array_equal(Load()['pulse', 3:3], [])
-    assert np.array_equal(Load()['pulse', -1:-1], [])
-    assert np.array_equal(Load()['pulse', 0:1], [3])
-    assert np.array_equal(Load()['pulse', 0:-3], [3])
-    assert np.array_equal(Load()['pulse', -1:], [1])
-    assert np.array_equal(Load()['pulse', -2:-1], [2])
-    assert np.array_equal(Load()['pulse', -2:], [2, 1])
-    assert np.array_equal(Load()['pulse', :-2], [3, 0])
+    assert np.array_equal(Load()['event_time_zero', 0], 3)
+    assert np.array_equal(Load()['event_time_zero', 1], 0)
+    assert np.array_equal(Load()['event_time_zero', 3], 1)
+    assert np.array_equal(Load()['event_time_zero', -1], 1)
+    assert np.array_equal(Load()['event_time_zero', -2], 2)
+    assert np.array_equal(Load()['event_time_zero', 0:0], [])
+    assert np.array_equal(Load()['event_time_zero', 1:1], [])
+    assert np.array_equal(Load()['event_time_zero', 1:-3], [])
+    assert np.array_equal(Load()['event_time_zero', 3:3], [])
+    assert np.array_equal(Load()['event_time_zero', -1:-1], [])
+    assert np.array_equal(Load()['event_time_zero', 0:1], [3])
+    assert np.array_equal(Load()['event_time_zero', 0:-3], [3])
+    assert np.array_equal(Load()['event_time_zero', -1:], [1])
+    assert np.array_equal(Load()['event_time_zero', -2:-1], [2])
+    assert np.array_equal(Load()['event_time_zero', -2:], [2, 1])
+    assert np.array_equal(Load()['event_time_zero', :-2], [3, 0])
 
 
-def create_off_geometry_detector_numbers_1234(group: NXobject,
+def create_off_geometry_detector_numbers_1234(group: snx.Group,
                                               name: str,
-                                              detector_faces: bool = True):
+                                              detector_faces: bool = True
+                                              ) -> sc.DataGroup:
+    dg = sc.DataGroup()
     off = group.create_class(name, NXoff_geometry)
     # square with point in center
     values = np.array([[0, 0, 0], [0, 1, 0], [1, 0, 0], [1, 1, 0], [0.5, 0.5, 0]])
-    off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
+    dg['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     # triangles
-    off['winding_order'] = sc.array(dims=['_'],
-                                    values=[0, 1, 4, 1, 2, 4, 2, 3, 4, 3, 0, 4],
-                                    unit=None)
-    off['faces'] = sc.array(dims=['_'], values=[0, 3, 6, 9], unit=None)
+    dg['winding_order'] = sc.array(dims=['winding_order'],
+                                   values=[0, 1, 4, 1, 2, 4, 2, 3, 4, 3, 0, 4],
+                                   unit=None)
+    dg['faces'] = sc.array(dims=['face'], values=[0, 3, 6, 9], unit=None)
     if detector_faces:
-        off['detector_faces'] = sc.array(dims=['_', 'dummy'],
-                                         values=[[0, 1], [1, 2], [2, 3], [3, 4]],
-                                         unit=None)
+        dg['detector_faces'] = sc.array(dims=['face', 'face_index|detector_number'],
+                                        values=[[0, 1], [1, 2], [2, 3], [3, 4]],
+                                        unit=None)
+    for name, var in dg.items():
+        off[name] = var
+    dg['vertices'] = sc.vectors(dims=['vertex'], values=values, unit='m')
+    return dg
 
 
 @pytest.mark.parametrize('detid_name',
                          ['detector_number', 'pixel_id', 'spectrum_index'])
 def test_loads_data_with_coords_and_off_geometry(nxroot, detid_name):
     da = sc.DataArray(
         sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]]))
     da.coords['detector_number'] = detector_numbers_xx_yy_1234()
     da.coords['xx'] = sc.array(dims=['xx'], unit='m', values=[0.1, 0.2])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field(detid_name, da.coords['detector_number'])
     detector.create_field('xx', da.coords['xx'])
     detector.create_field('data', da.data)
-    detector.attrs['axes'] = ['xx', 'yy']
-    create_off_geometry_detector_numbers_1234(detector, name='shape')
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    expected = create_off_geometry_detector_numbers_1234(detector, name='shape')
     loaded = detector[...]
-    expected = snx.nxoff_geometry.off_to_shape(
-        **detector['shape'][()], detector_number=da.coords['detector_number'])
-    assert sc.identical(loaded.coords['shape'].bins.size(),
-                        sc.array(dims=da.dims, values=[[1, 1], [1, 1]], unit=None))
-    assert sc.identical(loaded.coords['shape'], expected)
+    assert_identical(loaded.coords['shape'].value, expected)
 
 
-def test_missing_detector_numbers_triggers_fallback_given_off_geometry_with_det_faces(
+def test_missing_detector_numbers_given_off_geometry_with_det_faces_loads_as_usual(
         nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
-    create_off_geometry_detector_numbers_1234(detector, name='shape')
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    expected = create_off_geometry_detector_numbers_1234(detector, name='shape')
     loaded = detector[...]
-    assert isinstance(loaded, sc.DataGroup)
-    assert sc.identical(loaded['shape'], detector['shape'][()])
+    assert_identical(loaded.coords['shape'].value, expected)
 
 
 def test_off_geometry_without_detector_faces_loaded_as_0d_with_multiple_faces(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
-    create_off_geometry_detector_numbers_1234(detector,
-                                              name='shape',
-                                              detector_faces=False)
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    expected = create_off_geometry_detector_numbers_1234(detector,
+                                                         name='shape',
+                                                         detector_faces=False)
     loaded = detector[...]
-    assert loaded.coords['shape'].dims == ()
-    assert sc.identical(loaded.coords['shape'].bins.size(), sc.index(4))
+    assert_identical(loaded.coords['shape'].value, expected)
+    shape = snx.NXoff_geometry.assemble_as_child(loaded.coords['shape'].value)
+    assert sc.identical(shape.bins.size(), sc.index(4))
 
 
-def create_cylindrical_geometry_detector_numbers_1234(group: snx.NXobject,
+def create_cylindrical_geometry_detector_numbers_1234(group: snx.Group,
                                                       name: str,
-                                                      detector_numbers: bool = True):
+                                                      detector_numbers: bool = True
+                                                      ) -> sc.DataGroup:
     shape = group.create_class(name, snx.NXcylindrical_geometry)
     values = np.array([[0, 0, 0], [0, 1, 0], [3, 0, 0]])
-    shape['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
-    shape['cylinders'] = sc.array(dims=['_', 'vertex'],
-                                  values=[[0, 1, 2], [2, 1, 0]],
-                                  unit=None)
+    dg = sc.DataGroup()
+    dg['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
+    dg['cylinders'] = sc.array(dims=['cylinder', 'vertex_index'],
+                               values=[[0, 1, 2], [2, 1, 0]],
+                               unit=None)
     if detector_numbers:
-        shape['detector_number'] = sc.array(dims=['_'], values=[0, 1, 1, 0], unit=None)
+        dg['detector_number'] = sc.array(dims=['detector_number'],
+                                         values=[0, 1, 1, 0],
+                                         unit=None)
+    for name, var in dg.items():
+        shape[name] = var
+    dg['vertices'] = sc.vectors(dims=['vertex'], values=values, unit='m')
+    return dg
 
 
 def test_cylindrical_geometry_without_detector_numbers_loaded_as_0d(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
-    create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                      name='shape',
-                                                      detector_numbers=False)
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
+                                                                 name='shape',
+                                                                 detector_numbers=False)
     loaded = detector[...]
-    shape = loaded.coords['shape']
+    assert_identical(loaded.coords['shape'].value, expected)
+    shape = snx.NXcylindrical_geometry.assemble_as_child(loaded.coords['shape'].value)
     assert shape.dims == ()
     assert sc.identical(shape.bins.size(), sc.index(2))
     assert sc.identical(
         shape.value,
         sc.Dataset({
             'face1_center':
             sc.vectors(dims=['cylinder'], values=[[0, 0, 0], [3, 0, 0]], unit='m'),
             'face1_edge':
             sc.vectors(dims=['cylinder'], values=[[0, 1, 0], [0, 1, 0]], unit='m'),
             'face2_center':
             sc.vectors(dims=['cylinder'], values=[[3, 0, 0], [0, 0, 0]], unit='m'),
         }))
 
 
-def test_cylindrical_geometry_with_missing_parent_detector_numbers_triggers_fallback(
+def test_cylindrical_geometry_with_missing_parent_detector_numbers_loads_as_usual(
         nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
-    create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                      name='shape',
-                                                      detector_numbers=True)
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
+                                                                 name='shape',
+                                                                 detector_numbers=True)
     loaded = detector[...]
-    assert isinstance(loaded, sc.DataGroup)
-    assert isinstance(loaded['shape'], sc.DataGroup)
+    assert_identical(loaded.coords['shape'].value, expected)
 
 
-def test_cylindrical_geometry_with_inconsistent_detector_numbers_triggers_fallback(
-        nxroot):
+def test_cylindrical_geometry_with_inconsistent_detector_numbers_loads_as_usual(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1], [3.3]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
-    detector.create_field('detector_numbers',
+    detector._group.attrs['axes'] = ['xx', 'yy']
+    detector.create_field('detector_number',
                           sc.array(dims=var.dims, values=[[1], [2]], unit=None))
-    create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                      name='shape',
-                                                      detector_numbers=True)
-    loaded = detector[...]
-    assert isinstance(loaded, sc.DataGroup)
-    assert isinstance(loaded['shape'], sc.DataGroup)
+    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
+                                                                 name='shape',
+                                                                 detector_numbers=True)
+    loaded = detector[...]
+    assert_identical(loaded.coords['shape'].value, expected)
+    detector_number = loaded.coords['detector_number']
+    with pytest.raises(snx.NexusStructureError):
+        snx.NXcylindrical_geometry.assemble_as_child(loaded.coords['shape'].value,
+                                                     detector_number=detector_number)
 
 
 def test_cylindrical_geometry_with_detector_numbers(nxroot):
     var = sc.array(dims=['xx', 'yy'], unit='K', values=[[1.1, 2.2], [3.3, 4.4]])
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('data', var)
-    detector.attrs['axes'] = ['xx', 'yy']
+    detector._group.attrs['axes'] = ['xx', 'yy']
     detector_number = sc.array(dims=var.dims, values=[[1, 2], [3, 4]], unit=None)
     detector.create_field('detector_number', detector_number)
-    create_cylindrical_geometry_detector_numbers_1234(detector,
-                                                      name='shape',
-                                                      detector_numbers=True)
-    loaded = detector[...]
-    shape = loaded.coords['shape']
+    expected = create_cylindrical_geometry_detector_numbers_1234(detector,
+                                                                 name='shape',
+                                                                 detector_numbers=True)
+    loaded = detector[...]
+    assert_identical(loaded.coords['shape'].value, expected)
+    shape = snx.NXcylindrical_geometry.assemble_as_child(
+        loaded.coords['shape'].value, detector_number=loaded.coords['detector_number'])
     assert shape.dims == detector_number.dims
     for i in [0, 3]:
         assert sc.identical(
             shape.values[i],
             sc.Dataset({
                 'face1_center':
                 sc.vectors(dims=['cylinder'], values=[[0, 0, 0]], unit='m'),
```

### Comparing `scippnexus-23.3.0/tests/nxmonitor_test.py` & `scippnexus-23.4.0/tests/nxmonitor_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,75 @@
 import h5py
 import pytest
 import scipp as sc
+from scipp.testing import assert_identical
 
-from scippnexus import NXentry, NXevent_data, NXmonitor, NXroot
+import scippnexus.v2 as snx
 
 
 @pytest.fixture()
-def nxroot(request):
+def h5root():
+    """Yield h5py root group (file)"""
+    with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
+        yield f
+
+
+def make_group(group: h5py.Group) -> snx.Group:
+    return snx.Group(group, definitions=snx.base_definitions())
+
+
+@pytest.fixture()
+def group():
     """Yield NXroot containing a single NXentry named 'entry'"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
-        root.create_class('entry', NXentry)
-        yield root
+        yield snx.Group(f, definitions=snx.base_definitions())
 
 
-def test_dense_monitor(nxroot):
-    monitor = nxroot['entry'].create_class('monitor', NXmonitor)
-    assert monitor.nx_class == NXmonitor
+def test_dense_monitor(h5root):
+    monitor = snx.create_class(h5root, 'monitor', snx.NXmonitor)
     da = sc.DataArray(
         sc.array(dims=['time_of_flight'], values=[1.0]),
         coords={'time_of_flight': sc.array(dims=['time_of_flight'], values=[1.0])})
-    monitor['data'] = da.data
-    monitor['data'].attrs['axes'] = 'time_of_flight'
-    monitor['time_of_flight'] = da.coords['time_of_flight']
+    data = snx.create_field(monitor, 'data', da.data)
+    data.attrs['axes'] = 'time_of_flight'
+    snx.create_field(monitor, 'time_of_flight', da.coords['time_of_flight'])
+    monitor = make_group(monitor)
     assert sc.identical(monitor[...], da)
 
 
 def create_event_data_no_ids(group):
     group.create_field('event_time_offset',
                        sc.array(dims=[''], unit='s', values=[456, 7, 3, 345, 632, 23]))
     group.create_field('event_time_zero',
                        sc.array(dims=[''], unit='s', values=[1, 2, 3, 4]))
     group.create_field('event_index', sc.array(dims=[''],
                                                unit=None,
                                                values=[0, 3, 3, 5]))
 
 
-def test_loads_event_data_in_current_group(nxroot):
-    monitor = nxroot.create_class('monitor1', NXmonitor)
+def test_loads_event_data_in_current_group_as_data_array(group):
+    monitor = group.create_class('monitor1', snx.NXmonitor)
     create_event_data_no_ids(monitor)
-    assert monitor.dims == ('pulse', )
+    assert monitor.dims == ('event_time_zero', )
     assert monitor.shape == (4, )
     loaded = monitor[...]
-    assert sc.identical(
+    assert_identical(
         loaded.bins.size().data,
-        sc.array(dims=['pulse'], unit=None, dtype='int64', values=[3, 0, 2, 1]))
+        sc.array(dims=['event_time_zero'],
+                 unit=None,
+                 dtype='int64',
+                 values=[3, 0, 2, 1]))
 
 
-def test_loads_event_data_in_child_group(nxroot):
-    monitor = nxroot.create_class('monitor1', NXmonitor)
-    create_event_data_no_ids(monitor.create_class('events', NXevent_data))
-    assert monitor.dims == ('pulse', )
+def test_loads_event_data_in_child_group_as_data_array(group):
+    monitor = group.create_class('monitor1', snx.NXmonitor)
+    create_event_data_no_ids(monitor.create_class('events', snx.NXevent_data))
+    assert monitor.dims == ('event_time_zero', )
     assert monitor.shape == (4, )
     loaded = monitor[...]
+    assert isinstance(loaded, sc.DataArray)
     assert sc.identical(
         loaded.bins.size().data,
-        sc.array(dims=['pulse'], unit=None, dtype='int64', values=[3, 0, 2, 1]))
+        sc.array(dims=['event_time_zero'],
+                 unit=None,
+                 dtype='int64',
+                 values=[3, 0, 2, 1]))
```

### Comparing `scippnexus-23.3.0/tests/nxoff_geometry_test.py` & `scippnexus-23.4.0/tests/nxoff_geometry_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,76 @@
 import h5py
 import numpy as np
 import pytest
 import scipp as sc
 
-from scippnexus import NexusStructureError, NXentry, NXoff_geometry, NXroot
-from scippnexus.nxoff_geometry import off_to_shape
+import scippnexus.v2 as snx
+from scippnexus.v2.nxoff_geometry import NXoff_geometry, off_to_shape
 
 
 @pytest.fixture()
-def nxroot(request):
+def group():
     """Yield NXroot containing a single NXentry named 'entry'"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
-        root.create_class('entry', NXentry)
-        yield root
+        yield snx.Group(f, definitions=snx.base_definitions())
 
 
-def test_vertices_loaded_as_vector3(nxroot):
-    shape = nxroot['entry'].create_class('shape', NXoff_geometry)
+def test_vertices_loaded_as_vector3(group):
+    shape = group.create_class('shape', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='mm')
     loaded = shape[()]
     assert sc.identical(loaded['vertices'],
                         sc.vectors(dims=['vertex'], values=values, unit='mm'))
 
 
-def test_field_properties(nxroot):
-    shape = nxroot['entry'].create_class('shape', NXoff_geometry)
+def test_field_properties(group):
+    shape = group.create_class('shape', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6]]
     shape['vertices'] = sc.array(dims=['ignored', 'comp'], values=values, unit='m')
     shape['winding_order'] = sc.array(dims=['ignored'], values=[], unit=None)
     shape['faces'] = sc.array(dims=['ignored'], values=[], unit=None)
     loaded = shape[()]
     assert loaded['vertices'].dims == ('vertex', )
     assert loaded['winding_order'].dims == ('winding_order', )
     assert loaded['winding_order'].unit is None
     assert loaded['faces'].dims == ('face', )
     assert loaded['faces'].unit is None
 
 
-def test_off_to_shape_without_detector_faces_yields_scalar_shape_with_all_faces(nxroot):
-    off = nxroot['entry'].create_class('off', NXoff_geometry)
+def test_off_to_shape_without_detector_faces_yields_scalar_shape_with_all_faces(group):
+    off = group.create_class('off', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     loaded = off[()]
     shape = off_to_shape(**loaded)
     assert shape.ndim == 0
     assert sc.identical(shape.bins.size(), sc.index(2))
 
 
-def test_off_to_shape_raises_if_detector_faces_but_not_detector_numbers_given(nxroot):
-    off = nxroot['entry'].create_class('off', NXoff_geometry)
+def test_off_to_shape_raises_if_detector_faces_but_not_detector_numbers_given(group):
+    off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
     off['detector_faces'] = sc.array(dims=['_', 'dummy'],
                                      values=[[0, det_num2], [1, det_num1]],
                                      unit=None)
     loaded = off[()]
-    with pytest.raises(NexusStructureError):
+    with pytest.raises(snx.NexusStructureError):
         off_to_shape(**loaded)
 
 
-def test_off_to_shape_with_single_detector_yields_1d_shape(nxroot):
-    off = nxroot['entry'].create_class('off', NXoff_geometry)
+def test_off_to_shape_with_single_detector_yields_1d_shape(group):
+    off = group.create_class('off', NXoff_geometry)
     values = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 7
     off['detector_faces'] = sc.array(dims=['_', 'dummy'],
                                      values=[[0, det_num1], [1, det_num1]],
@@ -89,16 +87,16 @@
 
     detector_number = sc.array(dims=['detector_number'], values=[det_num1], unit=None)
     shape = off_to_shape(**loaded, detector_number=detector_number)
     assert sc.identical(shape.bins.size(),
                         sc.array(dims=['detector_number'], values=[2], unit=None))
 
 
-def test_off_to_shape_with_two_detectors_yields_1d_shape(nxroot):
-    off = nxroot['entry'].create_class('off', NXoff_geometry)
+def test_off_to_shape_with_two_detectors_yields_1d_shape(group):
+    off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
     off['detector_faces'] = sc.array(dims=['_', 'dummy'],
@@ -115,16 +113,16 @@
     assert sc.identical(
         shape[0].value,
         sc.vectors(dims=['face', 'vertex'], values=[values[[0, 2, 1]]], unit='m'))
     assert sc.identical(shape[1].value,
                         sc.vectors(dims=['face', 'vertex'], values=[values], unit='m'))
 
 
-def test_off_to_shape_uses_order_of_provided_detector_number_param(nxroot):
-    off = nxroot['entry'].create_class('off', NXoff_geometry)
+def test_off_to_shape_uses_order_of_provided_detector_number_param(group):
+    off = group.create_class('off', NXoff_geometry)
     values = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     off['vertices'] = sc.array(dims=['_', 'comp'], values=values, unit='m')
     off['winding_order'] = sc.array(dims=['_'], values=[0, 1, 2, 0, 2, 1], unit=None)
     off['faces'] = sc.array(dims=['_'], values=[0, 3], unit=None)
     det_num1 = 1
     det_num2 = 3
     off['detector_faces'] = sc.array(dims=['_', 'dummy'],
```

### Comparing `scippnexus-23.3.0/tests/nxtransformations_test.py` & `scippnexus-23.4.0/tests/nxtransformations_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,306 +1,411 @@
 import h5py
 import numpy as np
 import pytest
 import scipp as sc
+from scipp.testing import assert_identical
 
-from scippnexus import (
-    NXdetector,
-    NXentry,
-    NXlog,
-    NXroot,
-    NXtransformations,
-    nxtransformations,
-)
+import scippnexus.v2 as snx
+from scippnexus.v2.nxtransformations import NXtransformations
+
+
+def make_group(group: h5py.Group) -> snx.Group:
+    return snx.Group(group, definitions=snx.base_definitions())
 
 
 @pytest.fixture()
-def nxroot():
-    """Yield NXroot containing a single NXentry named 'entry'"""
+def h5root():
+    """Yield h5py root group (file)"""
     with h5py.File('dummy.nxs', mode='w', driver="core", backing_store=False) as f:
-        root = NXroot(f)
-        root.create_class('entry', NXentry)
-        yield root
+        yield f
 
 
 def create_detector(group):
     data = sc.array(dims=['xx', 'yy'], values=[[1.1, 2.2], [3.3, 4.4]])
     detector_numbers = sc.array(dims=['xx', 'yy'],
                                 unit=None,
                                 values=np.array([[1, 2], [3, 4]]))
-    detector = group.create_class('detector_0', NXdetector)
-    detector.create_field('detector_number', detector_numbers)
-    detector.create_field('data', data)
+    detector = snx.create_class(group, 'detector_0', snx.NXdetector)
+    snx.create_field(detector, 'detector_number', detector_numbers)
+    snx.create_field(detector, 'data', data)
     return detector
 
 
-def test_Transformation_with_single_value(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+def test_Transformation_with_single_value(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     value = sc.scalar(6.5, unit='mm')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
     vector = sc.vector(value=[0, 0, 1])
-    t = value.to(unit='m') * vector
+    t = value * vector
     expected = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    expected = expected * sc.spatial.translation(value=[0.001, 0.002, 0.003], unit='m')
-    value = transformations.create_field('t1', value)
+    expected = expected * offset
+    value = snx.create_field(transformations, 't1', value)
     value.attrs['depends_on'] = '.'
     value.attrs['transformation_type'] = 'translation'
     value.attrs['offset'] = offset.values
     value.attrs['offset_units'] = str(offset.unit)
     value.attrs['vector'] = vector.value
 
+    expected = sc.DataArray(data=expected, attrs={'depends_on': sc.scalar('.')})
+    detector = make_group(detector)
     depends_on = detector['depends_on'][()]
-    t = nxtransformations.Transformation(nxroot[depends_on])
-    assert t.depends_on is None
-    assert sc.identical(t.offset, offset)
-    assert sc.identical(t.vector, vector)
-    assert sc.identical(t[()], expected)
+    assert depends_on == 'transformations/t1'
+    t = detector[depends_on][()]
+    assert_identical(t, expected)
+
+
+def test_time_independent_Transformation_with_length_0(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
+    value = sc.array(dims=['dim_0'], values=[], unit='mm')
+    offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
+    vector = sc.vector(value=[0, 0, 1])
+    t = value * vector
+    expected = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
+    expected = expected * offset
+    value = snx.create_field(transformations, 't1', value)
+    value.attrs['depends_on'] = '.'
+    value.attrs['transformation_type'] = 'translation'
+    value.attrs['offset'] = offset.values
+    value.attrs['offset_units'] = str(offset.unit)
+    value.attrs['vector'] = vector.value
+
+    expected = sc.DataArray(data=expected, attrs={'depends_on': sc.scalar('.')})
+    detector = make_group(detector)
+    depends_on = detector['depends_on'][()]
+    assert depends_on == 'transformations/t1'
+    t = detector[depends_on][()]
+    assert_identical(t, expected)
+
+
+def test_depends_on_absolute_path_to_sibling_group_resolved_to_relative_path(h5root):
+    det1 = snx.create_class(h5root, 'det1', NXtransformations)
+    snx.create_field(det1, 'depends_on', sc.scalar('/det2/transformations/t1'))
+
+    depends_on = make_group(det1)['depends_on'][()]
+    assert depends_on == '../det2/transformations/t1'
 
 
-def test_chain_with_single_values_and_different_unit(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+def test_depends_on_relative_path_unchanged(h5root):
+    det1 = snx.create_class(h5root, 'det1', NXtransformations)
+    snx.create_field(det1, 'depends_on', sc.scalar('transformations/t1'))
+
+    depends_on = make_group(det1)['depends_on'][()]
+    assert depends_on == 'transformations/t1'
+
+
+def test_depends_on_attr_absolute_path_to_sibling_group_resolved_to_relative_path(
+        h5root):
+    det1 = snx.create_class(h5root, 'det1', NXtransformations)
+    transformations = snx.create_class(det1, 'transformations', NXtransformations)
+    t1 = snx.create_field(transformations, 't1', sc.scalar(0.1, unit='cm'))
+    t1.attrs['depends_on'] = '/det2/transformations/t2'
+    t1.attrs['transformation_type'] = 'translation'
+    t1.attrs['vector'] = [0, 0, 1]
+
+    loaded = make_group(det1)['transformations/t1'][()]
+    assert loaded.attrs['depends_on'].value == '../../det2/transformations/t2'
+
+
+def test_depends_on_attr_relative_path_unchanged(h5root):
+    det = snx.create_class(h5root, 'det', NXtransformations)
+    transformations = snx.create_class(det, 'transformations', NXtransformations)
+    t1 = snx.create_field(transformations, 't1', sc.scalar(0.1, unit='cm'))
+    t1.attrs['depends_on'] = '.'
+    t1.attrs['transformation_type'] = 'translation'
+    t1.attrs['vector'] = [0, 0, 1]
+
+    loaded = make_group(det)['transformations/t1'][()]
+    assert loaded.attrs['depends_on'].value == '.'
+    t1.attrs['depends_on'] = 't2'
+    loaded = make_group(det)['transformations/t1'][()]
+    assert loaded.attrs['depends_on'].value == 't2'
+
+
+def test_chain_with_single_values_and_different_unit(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     value = sc.scalar(6.5, unit='mm')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='mm')
     vector = sc.vector(value=[0, 0, 1])
-    t = value.to(unit='m') * vector
-    value1 = transformations.create_field('t1', value)
+    t = value * vector
+    value1 = snx.create_field(transformations, 't1', value)
     value1.attrs['depends_on'] = 't2'
     value1.attrs['transformation_type'] = 'translation'
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
-    value2 = transformations.create_field('t2', value.to(unit='cm'))
+    value2 = snx.create_field(transformations, 't2', value.to(unit='cm'))
     value2.attrs['depends_on'] = '.'
     value2.attrs['transformation_type'] = 'translation'
     value2.attrs['vector'] = vector.value
 
-    expected = (sc.spatial.translations(dims=t.dims, values=2 * t.values, unit=t.unit) *
-                sc.spatial.translation(value=[0.001, 0.002, 0.003], unit='m'))
-    assert sc.identical(detector[...].coords['depends_on'], expected)
+    t1 = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) * offset
+    t2 = sc.spatial.translations(dims=t.dims, values=t.values,
+                                 unit=t.unit).to(unit='cm')
+    detector = make_group(h5root['detector_0'])
+    loaded = detector[()]
+    depends_on = loaded.coords['depends_on']
+    assert depends_on.value == 'transformations/t1'
+    transforms = loaded.coords['transformations'].value
+    assert_identical(transforms['t1'].data, t1)
+    assert transforms['t1'].attrs['depends_on'].value == 't2'
+    assert_identical(transforms['t2'].data, t2)
+    assert transforms['t2'].attrs['depends_on'].value == '.'
 
 
-def test_Transformation_with_multiple_values(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+def test_Transformation_with_multiple_values(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
         coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    expected = t * offset
-    value = transformations.create_class('t1', NXlog)
-    value['time'] = log.coords['time'] - sc.epoch(unit='ns')
-    value['value'] = log.data
+    value = snx.create_class(transformations, 't1', snx.NXlog)
+    snx.create_field(value, 'time', log.coords['time'] - sc.epoch(unit='ns'))
+    snx.create_field(value, 'value', log.data)
     value.attrs['depends_on'] = '.'
     value.attrs['transformation_type'] = 'translation'
     value.attrs['offset'] = offset.values
     value.attrs['offset_units'] = str(offset.unit)
     value.attrs['vector'] = vector.value
 
+    expected = t * offset
+    expected.attrs['depends_on'] = sc.scalar('.')
+    detector = make_group(detector)
     depends_on = detector['depends_on'][()]
-    t = nxtransformations.Transformation(nxroot[depends_on])
-    assert t.depends_on is None
-    assert sc.identical(t.offset, offset)
-    assert sc.identical(t.vector, vector)
-    assert sc.identical(t[()], expected)
+    assert depends_on == 'transformations/t1'
+    assert_identical(detector[depends_on][()], expected)
 
 
-def test_chain_with_multiple_values(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+def test_chain_with_multiple_values(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
         coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    value1 = transformations.create_class('t1', NXlog)
-    value1['time'] = log.coords['time'] - sc.epoch(unit='ns')
-    value1['value'] = log.data
+    value1 = snx.create_class(transformations, 't1', snx.NXlog)
+    snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='ns'))
+    snx.create_field(value1, 'value', log.data)
     value1.attrs['depends_on'] = 't2'
     value1.attrs['transformation_type'] = 'translation'
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
-    value2 = transformations.create_class('t2', NXlog)
-    value2['time'] = log.coords['time'] - sc.epoch(unit='ns')
-    value2['value'] = log.data
+    value2 = snx.create_class(transformations, 't2', snx.NXlog)
+    snx.create_field(value2, 'time', log.coords['time'] - sc.epoch(unit='ns'))
+    snx.create_field(value2, 'value', log.data)
     value2.attrs['depends_on'] = '.'
     value2.attrs['transformation_type'] = 'translation'
     value2.attrs['vector'] = vector.value
 
-    expected = t * (t * offset)
-    assert sc.identical(detector[...].coords['depends_on'].value, expected)
-
-
-def test_chain_with_multiple_values_and_different_time_unit(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+    expected1 = t * offset
+    expected1.attrs['depends_on'] = sc.scalar('t2')
+    expected2 = t
+    expected2.attrs['depends_on'] = sc.scalar('.')
+    detector = make_group(detector)[()]
+    depends_on = detector.coords['depends_on']
+    assert depends_on.value == 'transformations/t1'
+    assert_identical(detector.coords['transformations'].value['t1'], expected1)
+    assert_identical(detector.coords['transformations'].value['t2'], expected2)
+
+
+def test_chain_with_multiple_values_and_different_time_unit(h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     # Making sure to not use nanoseconds since that is used internally and may thus
     # mask bugs.
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
         coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
     log.coords['time'] = sc.epoch(unit='us') + log.coords['time'].to(unit='us')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    value1 = transformations.create_class('t1', NXlog)
-    value1['time'] = log.coords['time'] - sc.epoch(unit='us')
-    value1['value'] = log.data
+    value1 = snx.create_class(transformations, 't1', snx.NXlog)
+    snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='us'))
+    snx.create_field(value1, 'value', log.data)
     value1.attrs['depends_on'] = 't2'
     value1.attrs['transformation_type'] = 'translation'
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
-    value2 = transformations.create_class('t2', NXlog)
-    value2['time'] = log.coords['time'].to(unit='ms') - sc.epoch(unit='ms')
-    value2['value'] = log.data
+    value2 = snx.create_class(transformations, 't2', snx.NXlog)
+    snx.create_field(value2, 'time',
+                     log.coords['time'].to(unit='ms') - sc.epoch(unit='ms'))
+    snx.create_field(value2, 'value', log.data)
     value2.attrs['depends_on'] = '.'
     value2.attrs['transformation_type'] = 'translation'
     value2.attrs['vector'] = vector.value
 
-    expected = t * (t * offset)
-    assert sc.identical(detector[...].coords['depends_on'].value, expected)
-
+    expected1 = t * offset
+    expected1.attrs['depends_on'] = sc.scalar('t2')
 
-def test_broken_time_dependent_transformation_returns_path_and_transformations(nxroot):
-    detector = create_detector(nxroot)
-    detector.create_field('depends_on', sc.scalar('/detector_0/transformations/t1'))
-    transformations = detector.create_class('transformations', NXtransformations)
+    t2 = t.copy()
+    t2.coords['time'] = t2.coords['time'].to(unit='ms')
+    expected2 = t2
+    expected2.attrs['depends_on'] = sc.scalar('.')
+
+    detector = make_group(detector)
+    loaded = detector[...]
+    depends_on = loaded.coords['depends_on']
+    assert depends_on.value == 'transformations/t1'
+    assert_identical(loaded.coords['transformations'].value['t1'], expected1)
+    assert_identical(loaded.coords['transformations'].value['t2'], expected2)
+
+
+def test_broken_time_dependent_transformation_returns_datagroup_but_sets_up_depends_on(
+        h5root):
+    detector = create_detector(h5root)
+    snx.create_field(detector, 'depends_on',
+                     sc.scalar('/detector_0/transformations/t1'))
+    transformations = snx.create_class(detector, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2], unit='m'),
         coords={'time': sc.array(dims=['time'], values=[11, 22], unit='s')})
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    value = transformations.create_class('t1', NXlog)
-    value['time'] = log.coords['time'] - sc.epoch(unit='ns')
+    value = snx.create_class(transformations, 't1', snx.NXlog)
+    snx.create_field(value, 'time', log.coords['time'] - sc.epoch(unit='ns'))
     # This makes the transform "broken" since "time" has length 2 but data has length 0.
-    value['value'] = log.data[0:0]
+    snx.create_field(value, 'value', log.data[0:0])
     value.attrs['depends_on'] = '.'
     value.attrs['transformation_type'] = 'translation'
     value.attrs['offset'] = offset.values
     value.attrs['offset_units'] = str(offset.unit)
     value.attrs['vector'] = vector.value
 
+    detector = make_group(detector)
     loaded = detector[()]
-    assert sc.identical(loaded.coords['depends_on'],
-                        sc.scalar('/detector_0/transformations/t1'))
     t = loaded.coords['transformations'].value
     assert isinstance(t, sc.DataGroup)
     # Due to the way NXtransformations works, vital information is stored in the
     # attributes. DataGroup does currently not support attributes, so this information
     # is mostly useless until that is addressed.
-    assert 't1' in t
+    t1 = t['t1']
+    assert isinstance(t1, sc.DataGroup)
+    assert t1.keys() == {'time', 'value'}
+    assert loaded.coords['depends_on'].value == 'transformations/t1'
+    assert_identical(loaded.coords['transformations'].value['t1'], t1)
 
 
 def write_translation(group, name: str, value: sc.Variable, offset: sc.Variable,
                       vector: sc.Variable) -> None:
-    dset = group.create_field(name, value)
+    dset = snx.create_field(group, name, value)
     dset.attrs['transformation_type'] = 'translation'
     dset.attrs['offset'] = offset.values
     dset.attrs['offset_units'] = str(offset.unit)
     dset.attrs['vector'] = vector.value
 
 
-def test_nxtransformations_group_single_item(nxroot):
+def test_nxtransformations_group_single_item(h5root):
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
-    t = value.to(unit='m') * vector
+    t = value * vector
     expected = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                sc.spatial.translation(value=[0.006, 0.002, 0.006], unit='m'))
+                offset)
 
-    transformations = nxroot.create_class('transformations', NXtransformations)
+    transformations = snx.create_class(h5root, 'transformations', NXtransformations)
     write_translation(transformations, 't1', value, offset, vector)
 
-    loaded = nxroot['transformations'][()]
+    loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1'}
     assert sc.identical(loaded['t1'], expected)
 
 
-def test_nxtransformations_group_two_independent_items(nxroot):
-    transformations = nxroot.create_class('transformations', NXtransformations)
+def test_nxtransformations_group_two_independent_items(h5root):
+    transformations = snx.create_class(h5root, 'transformations', NXtransformations)
 
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
-    t = value.to(unit='m') * vector
+    t = value * vector
     write_translation(transformations, 't1', value, offset, vector)
     expected1 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 sc.spatial.translation(value=[0.006, 0.002, 0.006], unit='m'))
+                 offset)
 
     value = value * 0.1
-    t = value.to(unit='m') * vector
+    t = value * vector
     write_translation(transformations, 't2', value, offset, vector)
     expected2 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 sc.spatial.translation(value=[0.006, 0.002, 0.006], unit='m'))
+                 offset)
 
-    loaded = nxroot['transformations'][()]
+    loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1', 't2'}
     assert sc.identical(loaded['t1'], expected1)
     assert sc.identical(loaded['t2'], expected2)
 
 
-def test_nxtransformations_group_single_chain(nxroot):
-    transformations = nxroot.create_class('transformations', NXtransformations)
+def test_nxtransformations_group_single_chain(h5root):
+    transformations = snx.create_class(h5root, 'transformations', NXtransformations)
 
     value = sc.scalar(2.4, unit='mm')
     offset = sc.spatial.translation(value=[6, 2, 6], unit='mm')
     vector = sc.vector(value=[0, 1, 1])
-    t = value.to(unit='m') * vector
+    t = value * vector
     write_translation(transformations, 't1', value, offset, vector)
     expected1 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 sc.spatial.translation(value=[0.006, 0.002, 0.006], unit='m'))
+                 offset)
 
     value = value * 0.1
-    t = value.to(unit='m') * vector
+    t = value * vector
     write_translation(transformations, 't2', value, offset, vector)
     transformations['t2'].attrs['depends_on'] = 't1'
-    expected2 = (expected1 *
-                 sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
-                 sc.spatial.translation(value=[0.006, 0.002, 0.006], unit='m'))
+    expected2 = (sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit) *
+                 offset)
 
-    loaded = nxroot['transformations'][()]
+    loaded = make_group(h5root)['transformations'][()]
     assert set(loaded.keys()) == {'t1', 't2'}
-    assert sc.identical(loaded['t1'], expected1)
-    assert sc.allclose(loaded['t2'], expected2)
+    assert_identical(loaded['t1'], expected1)
+    assert_identical(loaded['t2'].data, expected2)
+    assert loaded['t2'].attrs['depends_on'].value == 't1'
 
 
-def test_slice_transformations(nxroot):
-    transformations = nxroot.create_class('transformations', NXtransformations)
+def test_slice_transformations(h5root):
+    transformations = snx.create_class(h5root, 'transformations', NXtransformations)
     log = sc.DataArray(
         sc.array(dims=['time'], values=[1.1, 2.2, 3.3], unit='m'),
         coords={'time': sc.array(dims=['time'], values=[11, 22, 33], unit='s')})
     log.coords['time'] = sc.epoch(unit='ns') + log.coords['time'].to(unit='ns')
     offset = sc.spatial.translation(value=[1, 2, 3], unit='m')
     vector = sc.vector(value=[0, 0, 1])
     t = log * vector
     t.data = sc.spatial.translations(dims=t.dims, values=t.values, unit=t.unit)
-    value1 = transformations.create_class('t1', NXlog)
-    value1['time'] = log.coords['time'] - sc.epoch(unit='ns')
-    value1['value'] = log.data
+    value1 = snx.create_class(transformations, 't1', snx.NXlog)
+    snx.create_field(value1, 'time', log.coords['time'] - sc.epoch(unit='ns'))
+    snx.create_field(value1, 'value', log.data)
     value1.attrs['transformation_type'] = 'translation'
     value1.attrs['offset'] = offset.values
     value1.attrs['offset_units'] = str(offset.unit)
     value1.attrs['vector'] = vector.value
 
     expected = t * offset
 
-    assert sc.identical(nxroot['transformations']['time', 1:3]['t1'], expected['time',
-                                                                               1:3])
+    assert sc.identical(
+        make_group(h5root)['transformations']['time', 1:3]['t1'], expected['time', 1:3])
```

### Comparing `scippnexus-23.3.0/tox.ini` & `scippnexus-23.4.0/tox.ini`

 * *Files identical despite different names*

