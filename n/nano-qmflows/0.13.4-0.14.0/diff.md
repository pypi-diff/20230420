# Comparing `tmp/nano-qmflows-0.13.4.tar.gz` & `tmp/nano-qmflows-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nano-qmflows-0.13.4.tar", last modified: Thu Jun  2 18:41:26 2022, max compression
+gzip compressed data, was "nano-qmflows-0.14.0.tar", last modified: Wed Apr 19 19:36:39 2023, max compression
```

## Comparing `nano-qmflows-0.13.4.tar` & `nano-qmflows-0.14.0.tar`

### file list

```diff
@@ -1,82 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/doc_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/install_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/libint/
--rw-r--r--   0 runner    (1001) docker     (121)    22202 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/libint/compute_integrals.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/libint/include/
--rw-r--r--   0 runner    (1001) docker     (121)     4325 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/libint/include/namd.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/linting_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nano_qmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-06-02 18:41:25.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-06-02 18:41:26.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 18:41:25.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-02 18:41:26.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-06-02 18:41:26.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-02 18:41:26.000000 nano-qmflows-0.13.4/nano_qmflows.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nanoqm/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/_version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nanoqm/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8209 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/analysis/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nanoqm/basis/
--rw-r--r--   0 runner    (1001) docker     (121)    57514 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/BASIS_ADMM
--rw-r--r--   0 runner    (1001) docker     (121)   189910 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/BASIS_ADMM_MOLOPT
--rw-r--r--   0 runner    (1001) docker     (121)   126074 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/BASIS_MOLOPT
--rw-r--r--   0 runner    (1001) docker     (121)   118443 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/GTH_POTENTIALS
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/aux_fit.json
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/basis/valence_electrons.json
--rw-r--r--   0 runner    (1001) docker     (121)    12512 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/compute_integrals.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nanoqm/integrals/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/integrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/integrals/multipole_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/integrals/nonAdiabaticCoupling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.305700 nano-qmflows-0.13.4/nanoqm/schedule/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12205 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/schedule/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/schedule/scheduleCP2K.py
--rw-r--r--   0 runner    (1001) docker     (121)    17827 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/schedule/scheduleCoupling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/nanoqm/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9467 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/distribute_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/initialization.py
--rw-r--r--   0 runner    (1001) docker     (121)    12365 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/orbitals_type.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1838 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/run_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    11049 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     6231 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/workflow_coop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/workflow_coupling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/workflow_ipr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/workflow_single_points.py
--rw-r--r--   0 runner    (1001) docker     (121)    22317 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/nanoqm/workflows/workflow_stddft_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4371 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/convert_legacy_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/scripts/hamiltonians/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2077 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/hamiltonians/plot_mos_energies.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6103 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/hamiltonians/plot_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/scripts/pyxaid/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3318 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/pyxaid/plot_average_energy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6461 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/pyxaid/plot_cooling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6462 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/pyxaid/plot_spectra_pyxaid.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3673 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/pyxaid/plot_states_pops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/scripts/qmflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/convolution.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1881 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/mergeHDF5.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5075 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/plot_dos.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1308 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/removeHDF5folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/scripts/qmflows/remove_mos_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-06-02 18:41:26.309700 nano-qmflows-0.13.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-06-02 18:41:11.000000 nano-qmflows-0.13.4/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.154359 nano-qmflows-0.14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-19 19:36:39.154359 nano-qmflows-0.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/doc_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/install_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.134358 nano-qmflows-0.14.0/libint/
+-rw-r--r--   0 runner    (1001) docker     (123)    17182 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/libint/compute_integrals.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.134358 nano-qmflows-0.14.0/libint/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/libint/include/compute_integrals.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/libint/include/namd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/libint/py_compute_integrals.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/linting_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.134358 nano-qmflows-0.14.0/nano_qmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 19:36:39.000000 nano-qmflows-0.14.0/nano_qmflows.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.138358 nano-qmflows-0.14.0/nanoqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/_version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.138358 nano-qmflows-0.14.0/nanoqm/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/analysis/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.142358 nano-qmflows-0.14.0/nanoqm/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)    57514 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/BASIS_ADMM
+-rw-r--r--   0 runner    (1001) docker     (123)   189910 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/BASIS_ADMM_MOLOPT
+-rw-r--r--   0 runner    (1001) docker     (123)   126074 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/BASIS_MOLOPT
+-rw-r--r--   0 runner    (1001) docker     (123)   118443 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/GTH_POTENTIALS
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/aux_fit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/basis/valence_electrons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/compute_integrals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.142358 nano-qmflows-0.14.0/nanoqm/integrals/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/integrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/integrals/multipole_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/integrals/nonAdiabaticCoupling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.146359 nano-qmflows-0.14.0/nanoqm/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/schedule/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/schedule/scheduleCP2K.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/schedule/scheduleCoupling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.150359 nano-qmflows-0.14.0/nanoqm/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/distribute_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/orbitals_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/run_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/workflow_coop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/workflow_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/workflow_ipr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/workflow_single_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22520 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/nanoqm/workflows/workflow_stddft_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.150359 nano-qmflows-0.14.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4371 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/convert_legacy_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.150359 nano-qmflows-0.14.0/scripts/hamiltonians/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2077 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/hamiltonians/plot_mos_energies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6069 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/hamiltonians/plot_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.150359 nano-qmflows-0.14.0/scripts/pyxaid/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3266 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/pyxaid/plot_average_energy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6516 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/pyxaid/plot_cooling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6430 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/pyxaid/plot_spectra_pyxaid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/pyxaid/plot_states_pops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:36:39.154359 nano-qmflows-0.14.0/scripts/qmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/convolution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/mergeHDF5.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/plot_dos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/removeHDF5folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/scripts/qmflows/remove_mos_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 19:36:39.154359 nano-qmflows-0.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 19:36:25.000000 nano-qmflows-0.14.0/test_requirements.txt
```

### Comparing `nano-qmflows-0.13.4/LICENSE.txt` & `nano-qmflows-0.14.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/PKG-INFO` & `nano-qmflows-0.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: nano-qmflows
-Version: 0.13.4
+Version: 0.14.0
 Summary: Derivative coupling calculation
 Home-page: https://github.com/SCM-NV/nano-qmflows
 Author: Felipe Zapata & Ivan Infante
 Author-email: f.zapata@esciencecenter.nl
 License: Apache-2.0
 Keywords: chemistry Photochemistry Simulation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: lint
 License-File: LICENSE.txt
 
 .. image:: https://readthedocs.org/projects/qmflows-namd/badge/?version=latest
```

### Comparing `nano-qmflows-0.13.4/README.rst` & `nano-qmflows-0.14.0/README.rst`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/libint/compute_integrals.cc` & `nano-qmflows-0.14.0/libint/compute_integrals.cc`

 * *Files 21% similar despite different names*

```diff
@@ -3,20 +3,14 @@
  * kind of integrals used for non-adiabatic molecular dynamics,
  * including the overlaps integrals between different geometries
  * And the dipoles and quadrupoles to compute absorption spectra.
  * This module is based on libint and Eigen.
  * Copyright (C) 2018-2022 the Netherlands eScience Center.
  */
 
-#define PY_SSIZE_T_CLEAN
-#define Py_LIMITED_API 0x03070000
-#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
-#include <Python.h>
-#include <numpy/arrayobject.h>
-
 #include "namd.hpp"
 
 using HighFive::Attribute;
 using HighFive::DataSet;
 using HighFive::File;
 using HighFive::Group;
 using libint2::Atom;
@@ -543,167 +537,7 @@
     int i = op * matrices[0].rows();
     super_matrix.block(i, 0, matrices[op].rows(), matrices[op].cols()) =
         matrices[op];
   }
 
   return super_matrix;
 }
-
-
-/** \brief Convert python `str` instance into a C++ std::string **/
-int py_obj_to_string(PyObject *py_str, void *ptr) {
-  Py_ssize_t size;
-  char *str;
-
-  // PyUnicode_AsUTF8AndSize is part of the stable ABI ever since Python 3.10.
-  // For older versions we have to use a workaround by first converting the
-  // python str instance into a python bytes instance.
-#if defined(PyUnicode_AsUTF8AndSize)
-  str = PyUnicode_AsUTF8AndSize(py_str, &size);
-  if (str == nullptr) {
-    return 0;
-  }
-#else
-  PyObject *py_bytes = PyUnicode_AsEncodedString(py_str, "utf8", nullptr);
-  if (py_bytes == nullptr) {
-    return 0;
-  }
-
-  const int num = PyBytes_AsStringAndSize(py_bytes, &str, &size);
-  Py_DecRef(py_bytes);
-  if (num == -1) {
-    return 0;
-  }
-#endif
-  *(string *)ptr = std::string(str, size);
-  return 1;
-}
-
-
-/** \brief Convert (copy) an Eigen matrix into a numpy array **/
-PyObject *mat_to_npy_array(Matrix &mat) {
-  PyObject *npy_array;
-  PyObject *ret;
-  const npy_intp shape [2] = {mat.rows(), mat.cols()};
-
-  npy_array = PyArray_SimpleNewFromData(2, shape, NPY_DOUBLE, mat.data());
-  if (npy_array == nullptr) {
-    return nullptr;
-  }
-
-  // TODO: Figure out how to transfer ownership of `mat`s memory to the numpy array.
-  // As a stop-gap measure, simply create a copy to ensure the arrays' memory is
-  // fully managed by numpy.
-  ret = PyArray_SimpleNew(2, shape, NPY_DOUBLE);
-  int res = PyArray_CopyInto((PyArrayObject *)ret, (PyArrayObject *)npy_array);
-  Py_DecRef(npy_array);
-  return (res == -1) ? nullptr : ret;
-}
-
-
-/** \brief Python wrapper for compute_integrals_couplings */
-PyObject *py_compute_integrals_couplings(PyObject *self, PyObject *args) {
-  string path_xyz_1;
-  string path_xyz_2;
-  string path_hdf5;
-  string basis_name;
-  Matrix mat;
-
-  if (!PyArg_ParseTuple(args, "O&O&O&O&:compute_integrals_couplings",
-      py_obj_to_string, &path_xyz_1,
-      py_obj_to_string, &path_xyz_2,
-      py_obj_to_string, &path_hdf5,
-      py_obj_to_string, &basis_name)) {
-    return nullptr;
-  }
-
-  try {
-    mat = compute_integrals_couplings(path_xyz_1, path_xyz_2, path_hdf5, basis_name);
-  } catch (HighFive::Exception &err) {
-    PyErr_SetString(PyExc_RuntimeError, err.what());
-    return nullptr;
-  }
-  return mat_to_npy_array(mat);
-}
-
-
-/** \brief Python wrapper for compute_integrals_multipole */
-PyObject *py_compute_integrals_multipole(PyObject *self, PyObject *args) {
-  string path_xyz;
-  string path_hdf5;
-  string basis_name;
-  string multipole;
-  Matrix mat;
-
-  if (!PyArg_ParseTuple(args, "O&O&O&O&:compute_integrals_multipole",
-      py_obj_to_string, &path_xyz,
-      py_obj_to_string, &path_hdf5,
-      py_obj_to_string, &basis_name,
-      py_obj_to_string, &multipole)) {
-    return nullptr;
-  }
-
-  try {
-    mat = compute_integrals_multipole(path_xyz, path_hdf5, basis_name, multipole);
-  } catch (HighFive::Exception &err) {
-    PyErr_SetString(PyExc_RuntimeError, err.what());
-    return nullptr;
-  }
-  return mat_to_npy_array(mat);
-}
-
-
-/** \brief Get the number of threads */
-PyObject * py_get_thread_count(PyObject *self, PyObject *args) {
-  using libint2::nthreads;
-  return PyLong_FromLong(std::thread::hardware_concurrency());
-}
-
-
-/** \brief Get the type of threads */
-PyObject * py_get_thread_type(PyObject *self, PyObject *args) {
-  PyObject *ret;
-
-#if defined(_OPENMP)
-  ret = PyUnicode_FromString("OpenMP");
-#else
-  ret = PyUnicode_FromString("C++11");
-#endif
-  return ret;
-}
-
-
-PyMethodDef method_defs[] = {
-  {"compute_integrals_couplings", py_compute_integrals_couplings, METH_VARARGS,
-    "Compute the basis-set-specific overlap integrals for the molecule as provided in the xyz file."},
-  {"compute_integrals_multipole", py_compute_integrals_multipole, METH_VARARGS,
-    "Compute the given multipole."},
-  {"get_thread_count", py_get_thread_count, METH_NOARGS, "Get the number of threads."},
-  {"get_thread_type", py_get_thread_type, METH_NOARGS, "Get the type of threads."},
-  {nullptr}  // Sentinel
-};
-
-
-PyModuleDef py_module = {
-  PyModuleDef_HEAD_INIT,
-  "nanoqm.compute_integrals",                                              // m_name
-  "C++ extension module for computing integral overlaps and multipoles.",  // m_doc
-  -1,                                                                      // m_size
-  method_defs                                                              // m_methods
-};
-
-// Workaround to prevent C++ name mangling
-//
-// The `PyMODINIT_FUNC` macro should be able to take care of it, but it doesn't
-// seem to work on python <= 3.8.
-// Possibly related to the "-fvisibility=hidden" flag?
-
-#if defined(WIN32) || defined(_WIN32)
-  #define MODULE_EXPORT __declspec(dllexport)
-#else
-  #define MODULE_EXPORT __attribute__((visibility("default")))
-#endif
-
-extern "C" MODULE_EXPORT PyObject *PyInit_compute_integrals(void) {
-  import_array();
-  return PyModule_Create(&py_module);
-}
```

### Comparing `nano-qmflows-0.13.4/libint/include/namd.hpp` & `nano-qmflows-0.14.0/libint/include/namd.hpp`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nano_qmflows.egg-info/PKG-INFO` & `nano-qmflows-0.14.0/nano_qmflows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: nano-qmflows
-Version: 0.13.4
+Version: 0.14.0
 Summary: Derivative coupling calculation
 Home-page: https://github.com/SCM-NV/nano-qmflows
 Author: Felipe Zapata & Ivan Infante
 Author-email: f.zapata@esciencecenter.nl
 License: Apache-2.0
 Keywords: chemistry Photochemistry Simulation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: lint
 License-File: LICENSE.txt
 
 .. image:: https://readthedocs.org/projects/qmflows-namd/badge/?version=latest
```

### Comparing `nano-qmflows-0.13.4/nano_qmflows.egg-info/SOURCES.txt` & `nano-qmflows-0.14.0/nano_qmflows.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 install_requirements.txt
 linting_requirements.txt
 pyproject.toml
 setup.cfg
 setup.py
 test_requirements.txt
 libint/compute_integrals.cc
+libint/py_compute_integrals.cc
+libint/include/compute_integrals.hpp
 libint/include/namd.hpp
 nano_qmflows.egg-info/PKG-INFO
 nano_qmflows.egg-info/SOURCES.txt
 nano_qmflows.egg-info/dependency_links.txt
 nano_qmflows.egg-info/entry_points.txt
 nano_qmflows.egg-info/requires.txt
 nano_qmflows.egg-info/top_level.txt
 nanoqm/__init__.py
+nanoqm/_data.py
 nanoqm/_logger.py
+nanoqm/_monkey_patch.py
 nanoqm/_version.py
 nanoqm/_version_info.py
 nanoqm/common.py
 nanoqm/compute_integrals.pyi
 nanoqm/py.typed
 nanoqm/analysis/__init__.py
 nanoqm/analysis/tools.py
```

### Comparing `nano-qmflows-0.13.4/nanoqm/__init__.py` & `nano-qmflows-0.14.0/nanoqm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Nano-QMFlows is a generic python library for computing (numerically) electronic properties \
 for nanomaterials like the non-adiabatic coupling vectors (NACV) using several quantum \
 chemical (QM) packages."""
 
+# Monkey patch noodles with support for slots-containing dataclasses
+from . import _monkey_patch
+
 from ._version import __version__ as __version__
 from ._version_info import version_info as version_info
 from ._logger import logger as logger
 
 from .analysis import (
     autocorrelate, dephasing, convolute, func_conv, gauss_function,
     parse_list_of_lists, read_couplings, read_energies,
     read_energies_pyxaid, read_pops_pyxaid, spectral_density
 )
 
-from .integrals import (
-    calculate_couplings_levine, compute_overlaps_for_coupling)
+from .integrals import (calculate_couplings_levine, compute_overlaps_for_coupling)
 
 from .schedule import (calculate_mos, lazy_couplings)
 
-from .workflows import (
-    workflow_derivative_couplings, workflow_stddft)
+from .workflows import (workflow_derivative_couplings, workflow_stddft)
+
+del _monkey_patch
 
 __all__ = [
+    '__version__', 'version_info', 'logger',
     'autocorrelate', 'calculate_couplings_levine', 'calculate_mos',
     'compute_overlaps_for_coupling', 'convolute', 'dephasing',
     'func_conv', 'gauss_function', 'lazy_couplings',
     'parse_list_of_lists', 'read_couplings', 'read_energies',
     'read_energies_pyxaid', 'read_pops_pyxaid', 'spectral_density',
-    'workflow_derivative_couplings', 'workflow_stddft']
+    'workflow_derivative_couplings', 'workflow_stddft',
+]
```

### Comparing `nano-qmflows-0.13.4/nanoqm/_logger.py` & `nano-qmflows-0.14.0/nanoqm/_logger.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/analysis/tools.py` & `nano-qmflows-0.14.0/nanoqm/analysis/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 .. autosummary::
 
 API
 ---
 
 """
 
+from __future__ import annotations
+
 import os
-from typing import List, Tuple
 
 import numpy as np
 import pyparsing as pa
 from scipy.optimize import curve_fit
 
 from ..common import fs_to_cm, h2ev, hbar, r2meV
 
-""" Functions to fit data """
+# Functions to fit data
 
 
 def gauss_function(x: float, sigma: float) -> np.ndarray:
     """Compute a Gaussian function used for fitting data."""
     return np.exp(-0.5 * (-x / sigma) ** 2)
 
 
@@ -70,15 +71,15 @@
     ])
     return y_points
 
 
 """ Useful functions to compute autocorrelation, dephasing, etc. """
 
 
-def autocorrelate(f: np.ndarray) -> Tuple[float, float]:
+def autocorrelate(f: np.ndarray) -> tuple[float, float]:
     """Compute the un-normalized and normalized autocorrelation of a function."""
     d_f = f - f.mean()
     d_f2 = np.append(d_f, d_f, axis=0)
     # Compute the autocorrelation function
     uacf = np.correlate(d_f, d_f2, "valid")[:d_f.size] / d_f.size
     # Compute the normalized autocorrelation function
     nacf = uacf / uacf[0]
@@ -99,26 +100,31 @@
     freq = freq * fs_to_cm
     return f_fft, freq
 
 
 def dephasing(f: np.ndarray, dt: float):
     """Compute the dephasing time of a given function.
 
-        f            = energies, in eV  (if other function/unit: then the line_broadening will not be in eV)
-        dt           = time step, in fs
-
     Use the optical response formalisms:
     S. Mukamel, Principles of Nonlinear Optical Spectroscopy, 1995
     About the implementation we use the 2nd order cumulant expansion.
     See also eq. (2) in : Kilina et al. Phys. Rev. Lett., 110, 180404, (2013)
     To calculate the dephasing time tau we fit the dephasing function to a
     gaussian of the type : exp(-0.5 * (-x / tau) ** 2)
+
+    Parameters
+    ----------
+    f : np.ndarray
+        energies, in eV  (if other function/unit: then the line_broadening will not be in eV).
+    dt : float
+        time step, in fs.
+
     """
     # Conversion of hbar to hartree * fs
-    hbar_au = hbar / h2ev
+    # hbar_au = hbar / h2ev
     ts = np.arange(f.shape[0]) * dt
     cumu_ii = np.asarray([np.trapz(f[0:i + 1], dx=(dt / hbar), axis=0) for i in range(ts.size)])
     cumu_i = np.asarray([np.trapz(cumu_ii[0:i + 1], dx=(dt / hbar), axis=0)
                          for i in range(ts.size)])
     deph = np.exp(-cumu_i)
 
     return deph, ts
@@ -136,75 +142,84 @@
     np.seterr(over='ignore')
 
     if fit_func == 0:
         # fit with Gaussian
         popt, pcov = curve_fit(gauss_function, ts, deph, p0=(t_deph_guess, deph[0]))    # [0]
         ts_fit = np.arange(res * deph.shape[0]) * dt / res
         deph_fit = popt[1] * np.exp(-0.5 * (-ts_fit / popt[0]) ** 2)
-        deph_time = popt[0]                                           # in fs (defined as standard deviation of a Gaussian)
-        e_fwhm = std_to_fwhm * hbar / deph_time                       # FWHM in eV
+        deph_time = popt[0]  # in fs (defined as standard deviation of a Gaussian)
+        e_fwhm = std_to_fwhm * hbar / deph_time  # FWHM in eV
         perr = np.sqrt(np.diag(pcov))
-        deph_time_err = perr[0]                                            # error (standard deviation) for the deph. time
-        e_fwhm_err = deph_time_err * std_to_fwhm * hbar / (deph_time ** 2)  # error (standard deviation) for the FWHM
+
+        # error (standard deviation) for the deph. time
+        deph_time_err = perr[0]
+
+        # error (standard deviation) for the FWHM
+        e_fwhm_err = deph_time_err * std_to_fwhm * hbar / (deph_time ** 2)
     elif fit_func == 1:
         # fit with exponential
         popt, pcov = curve_fit(exp_function, ts, deph, p0=(t_deph_guess, deph[0]))  # [0]
         ts_fit = np.arange(res * deph.shape[0]) * dt / res
         deph_fit = popt[1] * np.exp(-ts_fit / popt[0])
-        deph_time = popt[0]                                           # in fs (defined as the exp. time constant)
-        e_fwhm = 2 * hbar / deph_time                                 # FWHM in eV
+        deph_time = popt[0]  # in fs (defined as the exp. time constant)
+        e_fwhm = 2 * hbar / deph_time  # FWHM in eV
         perr = np.sqrt(np.diag(pcov))
-        deph_time_err = perr[0]                                       # error (standard deviation) for the deph. time
-        e_fwhm_err = deph_time_err * 2 * hbar / (deph_time ** 2)      # error (standard deviation) for the FWHM
+
+        # error (standard deviation) for the deph. time
+        deph_time_err = perr[0]
+
+        # error (standard deviation) for the FWHM
+        e_fwhm_err = deph_time_err * 2 * hbar / (deph_time ** 2)
 
     return ts_fit, deph_fit, deph_time, deph_time_err, e_fwhm, e_fwhm_err
 
 
 def read_couplings(path_hams, ts):
-    """Read the non adiabatic coupling vectors from the files generated for the NAMD simulations."""
-    files_im = [os.path.join(path_hams, f'Ham_{i}_im')
-                for i in range(ts)]
-    xs = np.stack(np.loadtxt(fn) for fn in files_im)
+    """Read the non adiabatic coupling vectors from the files generated \
+    for the NAMD simulations."""
+    files_im = [os.path.join(path_hams, f'Ham_{i}_im') for i in range(ts)]
+    xs = np.stack([np.loadtxt(fn) for fn in files_im])
     return xs * r2meV  # return energies in meV
 
 
 def read_energies(path_hams, ts):
     """Read the molecular orbital energies of each state.
 
     The target files are generated for the NAMD simulations.
     """
     files_re = [os.path.join(path_hams, f'Ham_{i}_re')
                 for i in range(ts)]
-    xs = np.stack(np.diag(np.loadtxt(fn)) for fn in files_re)
+    xs = np.stack([np.diag(np.loadtxt(fn)) for fn in files_re])
     return xs * r2meV / 1000  # return energies in eV
 
 
 def read_energies_pyxaid(path, fn, nstates, nconds):
-    """Read the molecular orbital energies of each state from the output files generated by PYXAID."""
+    """Read the molecular orbital energies of each state from the \
+    output files generated by PYXAID."""
     inpfile = os.path.join(path, fn)
     cols = tuple(range(5, nstates * 2 + 5, 2))
-    xs = np.stack(np.loadtxt(f'{inpfile}{j}', usecols=cols)
-                  for j in range(nconds)).transpose()
+    xs = np.stack([np.loadtxt(f'{inpfile}{j}', usecols=cols)
+                  for j in range(nconds)]).T
     # Rows = timeframes ; Columns = states ; tensor = initial conditions
     xs = xs.swapaxes(0, 1)
     return xs
 
 
 def read_pops_pyxaid(path, fn, nstates, nconds):
     """Read the population of each state from the output files generated by PYXAID."""
     inpfile = os.path.join(path, fn)
     cols = tuple(range(3, nstates * 2 + 3, 2))
-    xs = np.stack(np.loadtxt(f'{inpfile}{j}', usecols=cols)
-                  for j in range(nconds)).transpose()
+    xs = np.stack([np.loadtxt(f'{inpfile}{j}', usecols=cols)
+                  for j in range(nconds)]).T
     # Rows = timeframes ; Columns = states ; tensor = initial conditions
     xs = xs.swapaxes(0, 1)
     return xs
 
 
-def parse_list_of_lists(xs: str) -> List[List[int]]:
+def parse_list_of_lists(xs: str) -> list[list[int]]:
     """Parse a list of list of integers using pyparsing."""
     enclosed = pa.Forward()  # Parser to be defined later
     natural = pa.Word(pa.nums)  # Natural Number
     # Nested Grammar
     nestedBrackets = pa.nestedExpr(pa.Suppress(
         '['), pa.Suppress(']'), content=enclosed)
     enclosed << (natural | pa.Suppress(',') | nestedBrackets)
```

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/BASIS_ADMM` & `nano-qmflows-0.14.0/nanoqm/basis/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/BASIS_ADMM_MOLOPT` & `nano-qmflows-0.14.0/nanoqm/basis/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/BASIS_MOLOPT` & `nano-qmflows-0.14.0/nanoqm/basis/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/GTH_POTENTIALS` & `nano-qmflows-0.14.0/nanoqm/basis/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/aux_fit.json` & `nano-qmflows-0.14.0/nanoqm/basis/aux_fit.json`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/basis/valence_electrons.json` & `nano-qmflows-0.14.0/nanoqm/basis/valence_electrons.json`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/nanoqm/common.py` & `nano-qmflows-0.14.0/nanoqm/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,22 @@
 .. autofunction:: number_spherical_functions_per_atom
 .. autofunction:: store_arrays_in_hdf5
 
 """
 
 from __future__ import annotations
 
-__all__ = ['DictConfig', 'Matrix', 'Tensor3D', 'Vector',
-           'change_mol_units', 'getmass', 'h2ev', 'hardness',
-           'number_spherical_functions_per_atom', 'retrieve_hdf5_data',
-           'is_data_in_hdf5', 'store_arrays_in_hdf5', 'UniqueSafeLoader',
-           'valence_electrons', 'aux_fit']
-
 import os
 import json
 from itertools import chain
 from pathlib import Path
-from typing import (Any, Dict, Iterable, List, Mapping, NamedTuple, Tuple,
-                    Sequence, overload, TypeVar, TYPE_CHECKING, Iterator)
+from collections.abc import Iterable, Sequence
+from typing import (
+    Any, Dict, List, NamedTuple, overload, TypeVar, TYPE_CHECKING, TypedDict, Literal
+)
 
 import h5py
 import mendeleev
 import numpy as np
 from scipy.constants import physical_constants
 from qmflows.common import AtomXYZ
 from qmflows.type_hints import PathLike
@@ -49,14 +45,20 @@
 from . import __path__ as nanoqm_path
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
 _T = TypeVar("_T")
 
+__all__ = ['DictConfig', 'Matrix', 'Tensor3D', 'Vector',
+           'change_mol_units', 'getmass', 'h2ev', 'hardness',
+           'number_spherical_functions_per_atom', 'retrieve_hdf5_data',
+           'is_data_in_hdf5', 'store_arrays_in_hdf5', 'UniqueSafeLoader',
+           'valence_electrons', 'aux_fit']
+
 
 _path_valence_electrons = Path(nanoqm_path[0]) / "basis" / "valence_electrons.json"
 _path_aux_fit = Path(nanoqm_path[0]) / "basis" / "aux_fit.json"
 
 with open(_path_valence_electrons, 'r') as f1, open(_path_aux_fit, 'r') as f2:
     valence_electrons: "dict[str, int]" = json.load(f1)
     aux_fit: "dict[str, list[int]]" = json.load(f2)
@@ -81,15 +83,15 @@
 class BasisFormats(NamedTuple):
     """NamedTuple that contains the name/value for the basis formats."""
 
     name: str
     value: list[npt.NDArray[np.int64]]
 
 
-def concat(xss: Iterable[Iterable[_T]]) -> List[_T]:
+def concat(xss: Iterable[Iterable[_T]]) -> list[_T]:
     """Concatenate of all the elements of a list."""
     return list(chain(*xss))
 
 
 # ================> Constants <================
 
 # Prevent a TypeError whenever scipy is mocked
@@ -107,14 +109,15 @@
     #: conversion from fs to nm
     fs_to_nm = 299.79246
     #: planck constant in eV * fs
     hbar = 1e15 * physical_constants['Planck constant over 2 pi in eV s'][0]
 else:
     angs2au = femtosec2au = h2ev = r2meV = fs_to_cm = fs_to_nm = hbar = 1.0
 
+
 # type hints
 MolXYZ = List[AtomXYZ]
 Vector = np.ndarray
 Matrix = np.ndarray
 Tensor3D = np.ndarray
 
 
@@ -144,45 +147,72 @@
         'at': 2.6528, 'rn': 2.8899, 'fr': 0.9882, 'ra': 1.2819, 'ac': 1.3497, 'th': 1.4175,
         'pa': 1.9368, 'u': 2.2305, 'np': 2.5241, 'pu': 3.0436, 'am': 3.4169, 'cm': 3.4050,
         'bk': 3.9244, 'cf': 4.2181, 'es': 4.5116, 'fm': 4.8051, 'md': 5.0100, 'no': 5.3926,
         'lr': 5.4607}
     return d[s] / 27.211
 
 
-def xc(s: str) -> Dict[str, Any]:
+class _XCDict(TypedDict):
+    type: Literal["pure", "hybrid", "rhs"]
+    alpha1: float
+    alpha2: float
+    ax: float
+    beta1: float
+    beta2: float
+
+
+_XC_DICT: dict[str, _XCDict] = {
+    'pbe': {
+        'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'blyp': {
+        'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'bp': {
+        'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'pbe0': {
+        'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.25, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'b3lyp': {
+        'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.20, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'bhlyp': {
+        'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.50, 'beta1': 0.2, 'beta2': 1.83
+    },
+    'cam-b3lyp': {
+        'type': 'rhs', 'alpha1': 1.86, 'alpha2': 0.00, 'ax': 0.38, 'beta1': 0.90, 'beta2': 0
+    },
+    'lc-blyp': {
+        'type': 'rhs', 'alpha1': 8.0, 'alpha2': 0.00, 'ax': 0.53, 'beta1': 4.50, 'beta2': 0
+    },
+    'wb97': {
+        'type': 'rhs', 'alpha1': 8.0, 'alpha2': 0.00, 'ax': 0.61, 'beta1': 4.41, 'beta2': 0.0
+    },
+}
+
+
+def xc(s: str) -> _XCDict:
     """Return the exchange functional composition."""
-    d = {
-        'pbe': {
-            'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83},
-        'blyp': {
-            'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83},
-        'bp': {
-            'type': 'pure', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0, 'beta1': 0.2, 'beta2': 1.83},
-        'pbe0': {
-            'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.25, 'beta1': 0.2, 'beta2': 1.83},
-        'b3lyp': {
-            'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.20, 'beta1': 0.2, 'beta2': 1.83},
-        'bhlyp': {
-            'type': 'hybrid', 'alpha1': 1.42, 'alpha2': 0.48, 'ax': 0.50, 'beta1': 0.2, 'beta2': 1.83},
-        'cam-b3lyp': {
-            'type': 'rhs', 'alpha1': 1.86, 'alpha2': 0.00, 'ax': 0.38, 'beta1': 0.90, 'beta2': 0},
-        'lc-blyp': {
-            'type': 'rhs', 'alpha1': 8.0, 'alpha2': 0.00, 'ax': 0.53, 'beta1': 4.50, 'beta2': 0},
-        'wb97': {
-            'type': 'rhs', 'alpha1': 8.0, 'alpha2': 0.00, 'ax': 0.61, 'beta1': 4.41, 'beta2': 0.0}}
-    return d[s]
+    return _XC_DICT[s]
 
 
 @overload
-def retrieve_hdf5_data(path_hdf5: str | os.PathLike[str], paths_to_prop: str) -> npt.NDArray[Any]:
+def retrieve_hdf5_data(
+    path_hdf5: str | os.PathLike[str],
+    paths_to_prop: str,
+) -> npt.NDArray[Any]:
     ...
 
 
 @overload
-def retrieve_hdf5_data(path_hdf5: str | os.PathLike[str], paths_to_prop: List[str]) -> List[npt.NDArray[Any]]:
+def retrieve_hdf5_data(
+    path_hdf5: str | os.PathLike[str],
+    paths_to_prop: list[str],
+) -> list[npt.NDArray[Any]]:
     ...
 
 
 def retrieve_hdf5_data(
     path_hdf5: str | os.PathLike[str],
     paths_to_prop: str | list[str],
 ) -> npt.NDArray[Any] | list[npt.NDArray[Any]]:
@@ -205,27 +235,27 @@
     RuntimeError
         The property has not been found
 
     """
     path_hdf5 = os.fspath(path_hdf5)
     try:
         with h5py.File(path_hdf5, 'r') as f5:
-            if isinstance(paths_to_prop, list):
-                return [f5[path][()] for path in paths_to_prop]
-            else:
+            if isinstance(paths_to_prop, str):
                 return f5[paths_to_prop][()]
+            else:
+                return [f5[path][()] for path in paths_to_prop]
     except KeyError:
         msg = f"There is not {paths_to_prop} stored in the HDF5\n"
         raise KeyError(msg)
     except FileNotFoundError:
         msg = "there is not HDF5 file containing the numerical results"
         raise RuntimeError(msg)
 
 
-def is_data_in_hdf5(path_hdf5: str | os.PathLike[str], xs: str | List[str]) -> bool:
+def is_data_in_hdf5(path_hdf5: str | os.PathLike[str], xs: str | Iterable[str]) -> bool:
     """Search if the node exists in the HDF5 file.
 
     Parameters
     ----------
     path_hdf5
         path to the HDF5
     xs
@@ -235,26 +265,26 @@
     -------
     bool
         Whether the data is stored
 
     """
     path_hdf5 = os.fspath(path_hdf5)
     if os.path.exists(path_hdf5):
-        with h5py.File(path_hdf5, 'r+') as f5:
-            if isinstance(xs, list):
-                return all(path in f5 for path in xs)
-            else:
+        with h5py.File(path_hdf5, 'r') as f5:
+            if isinstance(xs, str):
                 return xs in f5
+            else:
+                return all(path in f5 for path in xs)
     else:
         return False
 
 
 def store_arrays_in_hdf5(
     path_hdf5: PathLike,
-    paths: str | List[str],
+    paths: str | list[str],
     tensor: np.ndarray | Sequence[np.ndarray],
     dtype: npt.DTypeLike = np.float32,
     attribute: BasisFormats | None = None,
 ) -> None:
     """Store a tensor in the HDF5.
 
     Parameters
@@ -274,48 +304,48 @@
     path_hdf5 = os.fspath(path_hdf5)
 
     def add_attribute(data_set, k: int = 0):
         if attribute is not None:
             data_set.attrs[attribute.name] = attribute.value[k]
 
     with h5py.File(path_hdf5, 'r+') as f5:
-        if isinstance(paths, list):
+        if isinstance(paths, str):
+            dset = f5.require_dataset(paths, shape=np.shape(
+                tensor), data=tensor, dtype=dtype)
+            add_attribute(dset)
+        else:
             for k, path in enumerate(paths):
                 data = tensor[k]
                 dset = f5.require_dataset(path, shape=np.shape(data),
                                           data=data, dtype=dtype)
                 add_attribute(dset, k)
-        else:
-            dset = f5.require_dataset(paths, shape=np.shape(
-                tensor), data=tensor, dtype=dtype)
-            add_attribute(dset)
 
 
-def change_mol_units(mol: List[AtomXYZ], factor: float = angs2au) -> List[AtomXYZ]:
+def change_mol_units(mol: list[AtomXYZ], factor: float = angs2au) -> list[AtomXYZ]:
     """Change the units of the molecular coordinates."""
     new_molecule = []
     for atom in mol:
         coord = tuple(map(lambda x: x * factor, atom.xyz))
         new_molecule.append(AtomXYZ(atom.symbol, coord))  # type: ignore[arg-type]
     return new_molecule
 
 
-def tuplesXYZ_to_plams(xs: List[AtomXYZ]) -> Molecule:
+def tuplesXYZ_to_plams(xs: list[AtomXYZ]) -> Molecule:
     """Transform a list of namedTuples to a Plams molecule."""
     plams_mol = Molecule()
     for at in xs:
         symb = at.symbol
         cs = at.xyz
         plams_mol.add_atom(Atom(symbol=symb, coords=tuple(cs)))
 
     return plams_mol
 
 
 def number_spherical_functions_per_atom(
-    mol: List[AtomXYZ],
+    mol: list[AtomXYZ],
     package_name: str,
     basis_name: str,
     path_hdf5: PathLike,
 ) -> npt.NDArray[np.int_]:
     """Compute the number of spherical shells per atom."""
     ret = []
     with h5py.File(path_hdf5, 'r') as f:
@@ -357,15 +387,15 @@
 
     """
     return (fss * np.arange(1, 1 + 2 * len(fss), 2)).sum()
 
 
 def read_cell_parameters_as_array(
     file_cell_parameters: str | os.PathLike[str],
-) -> Tuple[str, npt.NDArray[np.float64]]:
+) -> tuple[str, npt.NDArray[np.float64]]:
     """Read the cell parameters as a numpy array."""
     arr = np.loadtxt(file_cell_parameters, skiprows=1)
 
     with open(file_cell_parameters, 'r') as f:
         header = f.readline()
 
     return header, arr
```

### Comparing `nano-qmflows-0.13.4/nanoqm/integrals/multipole_matrices.py` & `nano-qmflows-0.14.0/nanoqm/integrals/multipole_matrices.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,30 +18,33 @@
 
 from __future__ import annotations
 
 import os
 import uuid
 from os.path import join
 from pathlib import Path
-from typing import List, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
-import numpy as np
 from qmflows.common import AtomXYZ
 
 from .. import logger
-from ..common import (DictConfig, is_data_in_hdf5, retrieve_hdf5_data,
-                      store_arrays_in_hdf5, tuplesXYZ_to_plams)
+from ..common import is_data_in_hdf5, retrieve_hdf5_data, store_arrays_in_hdf5, tuplesXYZ_to_plams
 from ..compute_integrals import compute_integrals_multipole, get_thread_count, get_thread_type
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from numpy import float64 as f8
+    from .. import _data
 
 
-def get_multipole_matrix(config: DictConfig, inp: DictConfig, multipole: str) -> NDArray[f8]:
+def get_multipole_matrix(
+    config: _data.AbsorptionSpectrum,
+    inp: _data.AbsorptionData,
+    multipole: Literal["overlap", "dipole", "quadrupole"],
+) -> NDArray[f8]:
     """Retrieve the `multipole` number `i` from the trajectory. Otherwise compute it.
 
     Parameters
     ----------
     config
         Global configuration to run a workflow
     inp
@@ -65,26 +68,32 @@
         matrix_multipole = compute_matrix_multipole(inp.mol, config, multipole)
         store_arrays_in_hdf5(path_hdf5, path_multipole_hdf5, matrix_multipole)
 
     return matrix_multipole
 
 
 def search_multipole_in_hdf5(
-        path_hdf5: Union[str, Path], path_multipole_hdf5: str, multipole: str) -> None | NDArray[f8]:
+    path_hdf5: str | Path,
+    path_multipole_hdf5: str,
+    multipole: str,
+) -> None | NDArray[f8]:
     """Search if the multipole is already store in the HDF5."""
     if is_data_in_hdf5(path_hdf5, path_multipole_hdf5):
         logger.info(f"retrieving multipole: {multipole} from the hdf5")
         return retrieve_hdf5_data(path_hdf5, path_multipole_hdf5)
 
     logger.info(f"computing multipole: {multipole}")
     return None
 
 
 def compute_matrix_multipole(
-        mol: List[AtomXYZ], config: DictConfig, multipole: str) -> NDArray[f8]:
+    mol: list[AtomXYZ],
+    config: _data.GeneralOptions,
+    multipole: Literal["overlap", "dipole", "quadrupole"],
+) -> NDArray[f8]:
     """Compute a `multipole` matrix: overlap, dipole, etc. for a given geometry `mol`.
 
     The multipole is Computed in spherical coordinates.
 
     Note: for the dipole and quadrupole the super_matrix contains all the matrices stack all the
     0-axis.
 
@@ -107,15 +116,15 @@
 
     # Write molecule in temporal file
     path = join(config.scratch_path, f"molecule_{uuid.uuid4()}.xyz")
     mol_plams = tuplesXYZ_to_plams(mol)
     mol_plams.write(path)
 
     # name of the basis set
-    basis_name = config["cp2k_general_settings"]["basis"]
+    basis_name = config.cp2k_general_settings.basis
     thread_count = get_thread_count()
     thread_type = get_thread_type()
     logger.info(f"Will scale over {thread_count} {thread_type} threads")
 
     if multipole == 'overlap':
         matrix_multipole = compute_integrals_multipole(
             path, path_hdf5, basis_name, multipole)
@@ -130,14 +139,15 @@
 
     elif multipole == 'quadrupole':
         # The tensor contains the overlap + {xx, xy, xz, yy, yz, zz} quadrupole matrices
         super_matrix = compute_integrals_multipole(
             path, path_hdf5, basis_name, multipole)
         dim = super_matrix.shape[1]
 
-        # Reshape to 3d tensor containing overlap + {x, y, z} + {xx, xy, xz, yy, yz, zz} quadrupole matrices
+        # Reshape to 3d tensor containing overlap + {x, y, z} + {xx, xy, xz, yy, yz, zz}
+        # quadrupole matrices
         matrix_multipole = super_matrix.reshape(10, dim, dim)
 
     # Delete the tmp molecule file
     os.remove(path)
 
     return matrix_multipole
```

### Comparing `nano-qmflows-0.13.4/nanoqm/integrals/nonAdiabaticCoupling.py` & `nano-qmflows-0.14.0/nanoqm/integrals/nonAdiabaticCoupling.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,34 @@
 ---
 .. autofunction:: calculate_couplings_3points
 .. autofunction:: calculate_couplings_levine
 .. autofunction:: compute_overlaps_for_coupling
 .. autofunction:: correct_phases
 
 """
-__all__ = ['calculate_couplings_3points', 'calculate_couplings_levine',
-           'compute_overlaps_for_coupling', 'correct_phases']
+
+from __future__ import annotations
 
 import os
 import uuid
 from os.path import join
-from typing import List, Tuple
+from typing import TYPE_CHECKING
 
 import numpy as np
 
 from .. import logger
-from ..common import (DictConfig, Matrix, MolXYZ, Tensor3D, retrieve_hdf5_data,
-                      tuplesXYZ_to_plams)
+from ..common import Matrix, MolXYZ, Tensor3D, retrieve_hdf5_data, tuplesXYZ_to_plams
 from ..compute_integrals import compute_integrals_couplings, get_thread_count, get_thread_type
 
+if TYPE_CHECKING:
+    from .. import _data
+
+__all__ = ['calculate_couplings_3points', 'calculate_couplings_levine',
+           'compute_overlaps_for_coupling', 'correct_phases']
+
 
 def calculate_couplings_3points(
         dt: float, mtx_sji_t0: Matrix, mtx_sij_t0: Matrix,
         mtx_sji_t1: Matrix, mtx_sij_t1: Matrix) -> Matrix:
     """Calculate the non-adiabatic interaction matrix using 3 geometries.
 
     see: https://aip.scitation.org/doi/10.1063/1.467455
@@ -168,17 +173,18 @@
         # Update array with the fixed phases
         overlaps[k] *= mtx_phases_Sji_t0_t1
 
     return overlaps
 
 
 def compute_overlaps_for_coupling(
-        config: DictConfig,
-        pair_molecules: Tuple[MolXYZ, MolXYZ],
-        coefficients: Tuple[Matrix, Matrix]) -> Matrix:
+    config: _data.GeneralOptions,
+    pair_molecules: tuple[MolXYZ, MolXYZ],
+    coefficients: tuple[Matrix, Matrix],
+) -> Matrix:
     """Compute the Overlap matrices used to compute the couplings.
 
     Parameters
     ---------
     config
         Configuration of the current task
     pair_molecule
@@ -197,57 +203,55 @@
 
     # Read Orbitals Coefficients
     css0, css1 = coefficients
 
     return np.dot(css0.T, np.dot(suv, css1))
 
 
-def read_overlap_data(config: DictConfig, mo_paths: List[str]) -> Tuple[Matrix, Matrix]:
+def read_overlap_data(config: _data.GeneralOptions, mo_paths: list[str]) -> tuple[Matrix, Matrix]:
     """Read the Molecular orbital coefficients."""
     mos = retrieve_hdf5_data(config.path_hdf5, mo_paths)
 
     # Extract a subset of molecular orbitals to compute the coupling
     lowest, highest = compute_range_orbitals(config)
     css0, css1 = tuple(map(lambda xs: xs[:, lowest: highest], mos))
 
     return css0, css1
 
 
-def compute_range_orbitals(config: DictConfig) -> Tuple[int, int]:
+def compute_range_orbitals(config: _data.GeneralOptions) -> tuple[int, int]:
     """Compute the lowest and highest index used to extract a subset of Columns from the MOs."""
     lowest = config.nHOMO - (config.mo_index_range[0] + config.active_space[0])
     highest = config.nHOMO + config.active_space[1] - config.mo_index_range[0]
 
     return lowest, highest
 
 
-def calcOverlapMtx(config: DictConfig, molecules: Tuple[MolXYZ, MolXYZ]) -> Matrix:
+def calcOverlapMtx(config: _data.GeneralOptions, molecules: tuple[MolXYZ, MolXYZ]) -> Matrix:
     """Compute the overlap matrix between two geometries.
 
     The calculation of the overlap matrix uses the libint2 library
     at two different geometries: R0 and R1.
     """
     mol_i, mol_j = tuple(tuplesXYZ_to_plams(x) for x in molecules)
 
     # unique molecular paths
-    path_i = join(config["scratch_path"],
-                  f"molecule_{uuid.uuid4()}.xyz")
-    path_j = join(config["scratch_path"],
-                  "molecule_{uuid.uuid4()}.xyz")
+    path_i = join(config.scratch_path, f"molecule_{uuid.uuid4()}.xyz")
+    path_j = join(config.scratch_path, f"molecule_{uuid.uuid4()}.xyz")
 
     # Write the molecules in atomic units
     mol_i.write(path_i)
     mol_j.write(path_j)
 
-    basis_name = config["cp2k_general_settings"]["basis"]
+    basis_name = config.cp2k_general_settings.basis
 
     thread_count = get_thread_count()
     thread_type = get_thread_type()
     logger.info(f"Will scale over {thread_count} {thread_type} threads")
     try:
         integrals = compute_integrals_couplings(
-            path_i, path_j, config["path_hdf5"], basis_name)
+            path_i, path_j, config.path_hdf5, basis_name)
     finally:
         os.remove(path_i)
         os.remove(path_j)
 
     return integrals
```

### Comparing `nano-qmflows-0.13.4/nanoqm/schedule/components.py` & `nano-qmflows-0.14.0/nanoqm/schedule/components.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,186 +4,187 @@
 ---
 .. autofunction:: calculate_mos
 
 """
 
 from __future__ import annotations
 
-__all__ = ["calculate_mos", "create_point_folder",
-           "split_file_geometries"]
-
 import fnmatch
 import os
-from collections import defaultdict
 from os.path import join
-from typing import (Any, DefaultDict, Dict, List, NamedTuple, Sequence, Tuple,
-                    Union)
+from typing import NamedTuple, Tuple, Union
 
 import numpy as np
 from noodles import gather, schedule
 from qmflows.common import CP2KInfoMO
 from qmflows.type_hints import PathLike, PromisedObject
 from qmflows.warnings_qmflows import SCF_Convergence_Warning
 
 from .. import logger
-from ..common import (DictConfig, Matrix, is_data_in_hdf5,
-                      read_cell_parameters_as_array, store_arrays_in_hdf5)
+from .. import _data
+from ..common import Matrix, is_data_in_hdf5, read_cell_parameters_as_array, store_arrays_in_hdf5
 from .scheduleCP2K import prepare_job_cp2k
 
+__all__ = ["calculate_mos", "create_point_folder", "split_file_geometries"]
+
 #: Molecular orbitals from both restricted and unrestricted calculations
 OrbitalType = Union[CP2KInfoMO, Tuple[CP2KInfoMO, CP2KInfoMO]]
 
 
 class JobFiles(NamedTuple):
     """Contains the data to compute the molecular orbitals for a given geometry."""
 
     get_xyz: PathLike
     get_inp: PathLike
     get_out: PathLike
     get_MO: PathLike
 
 
-def calculate_mos(config: DictConfig) -> List[str]:
+def calculate_mos(config: _data.GeneralOptions) -> PromisedObject:
     """Look for the MO in the HDF5 file and compute them if they are not present.
 
     The orbitals are computed  by splitting the jobs in batches given by
     the ``restart_chunk`` variables. Only the first job is calculated from scratch
     while the rest of the batch uses as guess the wave function of the first calculation
     inthe batch.
 
     The config dict contains:
         * geometries: list of molecular geometries
         * project_name: Name of the project used as root path for storing data in HDF5.
         * path_hdf5: Path to the HDF5 file that contains the numerical results.
         * folders: path to the directories containing the MO outputs
         * settings_main: Settings for the job to run.
-        * calc_new_wf_guess_on_points: Calculate a new Wave function guess in each of the geometries indicated. By Default only an initial guess is computed.
-        * enumerate_from: Number from where to start enumerating the folders create for each point in the MD
+        * calc_new_wf_guess_on_points: Calculate a new Wave function guess in
+          each of the geometries indicated. By Default only an initial guess is computed.
+        * enumerate_from: Number from where to start enumerating the folders create for
+          each point in the MD
 
     Returns
     -------
         paths to the datasets in the HDF5 file containging both the MO energies and MO coefficients
 
     """
     # Read Cell parameters file
-    general = config['cp2k_general_settings']
-    file_cell_parameters = general["file_cell_parameters"]
+    general = config.cp2k_general_settings
+    file_cell_parameters = general.file_cell_parameters
     if file_cell_parameters is not None:
         array_cell_parameters = read_cell_parameters_as_array(file_cell_parameters)[
             1]
 
     # First calculation has no initial guess
     # calculate the rest of the jobs using the previous point as initial guess
-    orbitals = []  # list to the nodes in the HDF5 containing the MOs
+
+    # list to the nodes in the HDF5 containing the MOs
+    orbitals: list[None | tuple[str, str, str]] = []
     energies = []
     guess_job = None
 
     # orbital type is either an empty string for restricted calculation
     # or alpha/beta for unrestricted calculations
     orbitals_type = config.orbitals_type
 
     for j, gs in enumerate(config.geometries):
 
         # number of the point with respect to all the trajectory
         k = j + config.enumerate_from
 
         # dictionary containing the information of the j-th job
-        dict_input = defaultdict(lambda: None)  # type:  DefaultDict[str, Any]
-        dict_input["geometry"] = gs
-        dict_input["k"] = k
-
-        # Path where the MOs will be store in the HDF5
-        dict_input["node_MOs"] = [
-            join(orbitals_type, "eigenvalues", f"point_{k}"),
-            join(orbitals_type, "coefficients", f"point_{k}"),
-            join(orbitals_type, "occupation", f"point_{k}"),
-        ]
-
-        dict_input["node_energy"] = join(orbitals_type, "energy", f"point_{k}")
+        dict_input = _data.ComponentsData(
+            geometry=gs,
+            k=k,
+            node_MOs=(  # Path where the MOs will be store in the HDF5
+                join(orbitals_type, "eigenvalues", f"point_{k}"),
+                join(orbitals_type, "coefficients", f"point_{k}"),
+                join(orbitals_type, "occupation", f"point_{k}"),
+            ),
+            node_energy=join(orbitals_type, "energy", f"point_{k}"),
+        )
 
         # If the MOs are already store in the HDF5 format return the path
         # to them and skip the calculation
-        if config["compute_orbitals"]:
-            predicate = dict_input["node_MOs"]
+        if config.compute_orbitals:
+            predicate: str | tuple[str, str, str] = dict_input.node_MOs
         else:
-            predicate = dict_input["node_energy"]
+            predicate = dict_input.node_energy
 
         if is_data_in_hdf5(config.path_hdf5, predicate):
             logger.info(f"point_{k} has already been calculated")
-            orbitals.append(dict_input["node_MOs"])
+            orbitals.append(dict_input.node_MOs)
         else:
             logger.info(f"point_{k} has been scheduled")
 
             # Add cell parameters from file if given
             if file_cell_parameters is not None:
                 adjust_cell_parameters(general, array_cell_parameters, j)
             # Path to I/O files
-            dict_input["point_dir"] = config.folders[j]
-            dict_input["job_files"] = create_file_names(
-                dict_input["point_dir"], k)
-            dict_input["job_name"] = f'point_{k}'
+            dict_input.point_dir = config.folders[j]
+            dict_input.job_files = create_file_names(dict_input.point_dir, k)
+            dict_input.job_name = f'point_{k}'
 
             # Compute the MOs and return a new guess
             promise_qm = compute_orbitals(config, dict_input, guess_job)
 
             # Check if the job finishes succesfully
             promise_qm = schedule_check(promise_qm, config, dict_input)
 
             # Store the computation
-            if config["compute_orbitals"]:
+            if config.compute_orbitals:
                 orbitals.append(store_molecular_orbitals(config, dict_input, promise_qm))
             else:
                 orbitals.append(None)
             energies.append(store_enery(config, dict_input, promise_qm))
 
             guess_job = promise_qm
 
     return gather(gather(*orbitals), gather(*energies))
 
 
 @schedule
 def store_molecular_orbitals(
-        config: DictConfig, dict_input: DefaultDict[str, Any], promise_qm: PromisedObject) -> str:
+    config: _data.GeneralOptions,
+    dict_input: _data.ComponentsData,
+    promise_qm: PromisedObject,
+) -> tuple[str, str, str]:
     """Store the MOs in the HDF5.
 
     Returns
     -------
     str
         Node path in the HDF5
 
     """
     # Molecular Orbitals
     mos = promise_qm.orbitals
 
     # Store in the HDF5
     try:
-        save_orbitals_in_hdf5(mos, config, dict_input["job_name"])
+        save_orbitals_in_hdf5(mos, config, dict_input.job_name)
     # Remove the ascii MO file
     finally:
         if config.remove_log_file:
             work_dir = promise_qm.archive['work_dir']
             path_mos = fnmatch.filter(os.listdir(work_dir), 'mo_*MOLog')[0]
             os.remove(join(work_dir, path_mos))
 
-    return dict_input["node_MOs"]
+    return dict_input.node_MOs
 
 
-def save_orbitals_in_hdf5(mos: OrbitalType, config: DictConfig, job_name: str) -> None:
+def save_orbitals_in_hdf5(mos: OrbitalType, config: _data.GeneralOptions, job_name: str) -> None:
     """Store the orbitals from restricted and unrestricted calculations."""
     if isinstance(mos, CP2KInfoMO):
         dump_orbitals_to_hdf5(mos, config, job_name)
     else:
         alphas, betas = mos
         dump_orbitals_to_hdf5(alphas, config, job_name, "alphas")
         dump_orbitals_to_hdf5(betas, config, job_name, "betas")
 
 
 def dump_orbitals_to_hdf5(
     data: CP2KInfoMO,
-    config: DictConfig,
+    config: _data.GeneralOptions,
     job_name: str,
     orbitals_type: str = "",
 ) -> None:
     """Store the result in HDF5 format.
 
     Parameters
     ----------
@@ -206,110 +207,108 @@
     path_property = join(orbitals_type, "occupation", job_name)
     occ_array = np.array(data.get_nocc_nvirt(), dtype=np.int64)
     store_arrays_in_hdf5(config.path_hdf5, path_property, occ_array, dtype=np.int64)
 
 
 @schedule
 def store_enery(
-        config: DictConfig, dict_input: Dict, promise_qm: PromisedObject) -> str:
+    config: _data.GeneralOptions,
+    dict_input: _data.ComponentsData,
+    promise_qm: PromisedObject,
+) -> str:
     """Store the total energy in the HDF5 file.
 
     Returns
     -------
     str
         Node path to the energy in the HDF5
 
     """
-    store_arrays_in_hdf5(
-        config.path_hdf5, dict_input['node_energy'], promise_qm.energy)
-
-    logger.info(
-        f"Total energy of point {dict_input['k']} is: {promise_qm.energy}")
-
-    return dict_input["node_energy"]
+    store_arrays_in_hdf5(config.path_hdf5, dict_input.node_energy, promise_qm.energy)
+    logger.info(f"Total energy of point {dict_input.k} is: {promise_qm.energy}")
+    return dict_input.node_energy
 
 
 def compute_orbitals(
-        config: DictConfig, dict_input: Dict, guess_job: PromisedObject) -> PromisedObject:
+    config: _data.GeneralOptions,
+    dict_input: _data.ComponentsData,
+    guess_job: None | PromisedObject,
+) -> PromisedObject:
     """Call a Quantum chemisty package to compute the MOs.
 
     When finish store the MOs in the HdF5 and returns a new guess.
     """
-    dict_input["job_files"] = create_file_names(
-        dict_input["point_dir"], dict_input["k"])
+    dict_input.job_files = create_file_names(dict_input.point_dir, dict_input.k)
 
     # Calculating initial guess
     compute_guess = config.calc_new_wf_guess_on_points is not None
 
     # A job  is a restart if guess_job is None and the list of
     # wf guesses are not empty
     is_restart = guess_job is None and compute_guess
 
-    pred = (dict_input['k']
-            in config.calc_new_wf_guess_on_points) or is_restart
+    pred = (dict_input.k in config.calc_new_wf_guess_on_points) or is_restart
 
     general = config.cp2k_general_settings
 
     if pred:
-        guess_job = prepare_job_cp2k(
-            general["cp2k_settings_guess"], dict_input, guess_job)
-
-    promise_qm = prepare_job_cp2k(
-        general["cp2k_settings_main"], dict_input, guess_job)
-
-    return promise_qm
+        guess_job = prepare_job_cp2k(general.cp2k_settings_guess, dict_input, guess_job)
+    return prepare_job_cp2k(general.cp2k_settings_main, dict_input, guess_job)
 
 
 @schedule
 def schedule_check(
-        promise_qm: PromisedObject, config: DictConfig, dict_input: DictConfig) -> PromisedObject:
+    promise_qm: PromisedObject,
+    config: _data.GeneralOptions,
+    dict_input: _data.ComponentsData,
+) -> PromisedObject:
     """Check wether a calculation finishes succesfully otherwise run a new guess."""
-    job_name = dict_input["job_name"]
-    point_dir = dict_input["point_dir"]
+    job_name = dict_input.job_name
+    point_dir = dict_input.point_dir
 
     # Warnings of the computation
     warnings = promise_qm.warnings
 
     # Check for SCF convergence errors
     if not config.ignore_warnings and warnings is not None and any(
             w == SCF_Convergence_Warning for msg, w in warnings.items()):
         # Report the failure
         msg = f"Job: {job_name} Finished with Warnings: {warnings}"
         logger.warning(msg)
 
         # recompute a new guess
-        msg1 = "Computing a new wave function guess for job: {job_name}"
+        msg1 = f"Computing a new wave function guess for job: {job_name}"
         logger.warning(msg1)
 
         # Remove the previous ascii file containing the MOs
         msg2 = f"removing file containig the previous failed MOs of {job_name}"
         logger.warning(msg2)
         path = fnmatch.filter(os.listdir(point_dir), 'mo*MOLog')[0]
         os.remove(join(point_dir, path))
 
         # Compute new guess at point k
-        config.calc_new_wf_guess_on_points.append(dict_input["k"])
+        config.calc_new_wf_guess_on_points.append(dict_input.k)
         return compute_orbitals(config, dict_input, None)
     else:
         return promise_qm
 
 
 def create_point_folder(
-        work_dir: str | os.PathLike[str], n: int, enumerate_from: int) -> List[str]:
+        work_dir: str | os.PathLike[str], n: int, enumerate_from: int) -> list[str]:
     """Create a new folder for each point in the MD trajectory."""
     folders = []
     for k in range(enumerate_from, n + enumerate_from):
         new_dir = join(work_dir, f'point_{k}')
         os.makedirs(new_dir, exist_ok=True)
         folders.append(new_dir)
 
     return folders
 
 
-def split_file_geometries(path_xyz: PathLike) -> Sequence[str]:
+def split_file_geometries(path_xyz: PathLike) -> list[str]:
     """Read a set of molecular geometries in xyz format."""
     # Read Cartesian Coordinates
     with open(path_xyz) as f:
         xss = iter(f.readlines())
 
     data = []
     while True:
@@ -330,22 +329,19 @@
     file_out = join(work_dir, f'point_{i}.out')
     file_mo = join(work_dir, f'mo_coeff_{i}.out')
 
     return JobFiles(file_xyz, file_inp, file_out, file_mo)
 
 
 def adjust_cell_parameters(
-        general: DictConfig,
-        array_cell_parameters: Matrix,
-        j: int) -> None:
+    general: _data.CP2KGeneralSetting,
+    array_cell_parameters: Matrix,
+    j: int,
+) -> None:
     """Adjust the cell parameters on the fly.
 
     If the cell parameters change during the MD simulations, adjust them
     for the molecular orbitals computation.
     """
-    for s in (
-        general[p] for p in (
-            'cp2k_settings_main',
-            'cp2k_settings_guess')):
-        s.cell_parameters = array_cell_parameters[j, 2:11].reshape(
-            3, 3).tolist()
+    for s in (general.cp2k_settings_main, general.cp2k_settings_guess):
+        s.cell_parameters = array_cell_parameters[j, 2:11].reshape(3, 3).tolist()
         s.cell_angles = None
```

### Comparing `nano-qmflows-0.13.4/nanoqm/schedule/scheduleCP2K.py` & `nano-qmflows-0.14.0/nanoqm/schedule/scheduleCP2K.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
 from __future__ import annotations
 
 import fnmatch
 import os
 from os.path import join
 from pathlib import Path
-from typing import Any, Dict
+from typing import TYPE_CHECKING
 
 from noodles import schedule  # Workflow Engine
 from qmflows import Settings, cp2k, templates
 from qmflows.packages import CP2K, CP2K_Result
 from qmflows.parsers import string_to_plams_Molecule
 from qmflows.type_hints import PromisedObject
 
 from .. import logger
+if TYPE_CHECKING:
+    from .. import _data
 
 
 def try_to_read_wf(path_dir: str | os.PathLike[str]) -> str:
     """Try to get a wave function file from ``path_dir``.
 
     Returns
     -------
@@ -51,15 +53,18 @@
         msg = f"There are no wave function file in path: {os.fspath(path_dir)!r}\n"
         msg += print_cp2k_error(path_dir, "err")
         msg += print_cp2k_error(path_dir, "out")
         raise RuntimeError(msg)
 
 
 def prepare_cp2k_settings(
-        settings: Settings, dict_input: Dict[str, Any], guess_job: CP2K_Result) -> Settings:
+    settings: Settings,
+    dict_input: _data.ComponentsData,
+    guess_job: None | CP2K_Result,
+) -> Settings:
     """Fill in the parameters for running a single job in CP2K.
 
     Parameters
     ----------
     settings
         Input for CP2K
     dict_input
@@ -70,33 +75,36 @@
     Returns
     .......
     CP2K
         job to run
 
     """
     dft = settings.specific.cp2k.force_eval.dft
-    dft['print']['mo']['filename'] = dict_input["job_files"].get_MO
+    dft['print']['mo']['filename'] = dict_input.job_files.get_MO
 
     # Global parameters for CP2K
-    settings.specific.cp2k['global']['project'] = f'point_{dict_input["k"]}'
+    settings.specific.cp2k['global']['project'] = f'point_{dict_input.k}'
 
     if guess_job is not None:
         plams_dir = guess_job.archive['plams_dir']
         if plams_dir is None:
-            raise RuntimeError(f"There are no wave function file in path: None\n")
+            raise RuntimeError("There are no wave function file in path: None\n")
         dft.wfn_restart_file_name = try_to_read_wf(plams_dir)
 
     input_args = templates.singlepoint.overlay(settings)
 
     return input_args
 
 
 @schedule
 def prepare_job_cp2k(
-        settings: Settings, dict_input: Dict[str, Any], guess_job: PromisedObject) -> CP2K:
+    settings: Settings,
+    dict_input: _data.ComponentsData,
+    guess_job: None | PromisedObject,
+) -> CP2K:
     """Generate a :class:`qmflows.packages.CP2K` job.
 
     Parameters
     ----------
     settings
         Input for CP2K
     dict_input
@@ -114,16 +122,17 @@
 
     # remove keywords not use on the next translation phase
     for x in ('basis', 'potential'):
         if x in job_settings:
             del job_settings[x]
 
     return cp2k(
-        job_settings, string_to_plams_Molecule(dict_input["geometry"]),
-        work_dir=dict_input['point_dir'])
+        job_settings, string_to_plams_Molecule(dict_input.geometry),
+        work_dir=dict_input.point_dir,
+    )
 
 
 def print_cp2k_error(path_dir: str | os.PathLike[str], prefix: str) -> str:
     """Search for error in the CP2K output files."""
     err_file = next(Path(path_dir).glob(f"*{prefix}"), None)
     msg = ""
     if err_file is not None:
```

### Comparing `nano-qmflows-0.13.4/nanoqm/schedule/scheduleCoupling.py` & `nano-qmflows-0.14.0/nanoqm/schedule/scheduleCoupling.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,32 +27,33 @@
 
 import numpy as np
 from noodles import schedule
 from scipy.optimize import linear_sum_assignment
 from qmflows.parsers import parse_string_xyz
 
 from .. import logger
-from ..common import (DictConfig, Matrix, MolXYZ, Tensor3D, Vector, hbar,
+from ..common import (Matrix, MolXYZ, Tensor3D, Vector, hbar,
                       femtosec2au, h2ev, is_data_in_hdf5, retrieve_hdf5_data,
                       store_arrays_in_hdf5)
 from ..integrals import (calculate_couplings_3points,
                          calculate_couplings_levine,
                          compute_overlaps_for_coupling, correct_phases)
 from ..integrals.nonAdiabaticCoupling import (compute_range_orbitals,
                                               read_overlap_data)
 
 if TYPE_CHECKING:
     import numpy.typing as npt
+    from .. import _data
 
 __all__ = ["calculate_overlap", "lazy_couplings", "write_hamiltonians"]
 
 
 @schedule
 def lazy_couplings(
-    config: DictConfig,
+    config: _data.DerivativeCoupling,
     paths_overlaps: List[str],
 ) -> Tuple[npt.NDArray[np.int_], List[str]]:
     """Compute the Nonadibatic coupling.
 
     The coupling is computed sing a either 3-point approximation. See:
     The Journal of Chemical Physics 137, 22A514 (2012); doi: 10.1063/1.4738960
 
@@ -79,16 +80,15 @@
     if config.tracking:
         fixed_phase_overlaps, swaps = compute_the_fixed_phase_overlaps(
             paths_overlaps, config)
     else:
         # Do not track the crossings
         mtx_0 = retrieve_hdf5_data(config.path_hdf5, paths_overlaps[0])
         _, dim = mtx_0.shape
-        overlaps = np.stack(
-            retrieve_hdf5_data(config.path_hdf5, paths_overlaps))
+        overlaps = np.stack(retrieve_hdf5_data(config.path_hdf5, paths_overlaps))
         nOverlaps, nOrbitals, _ = overlaps.shape
         swaps = np.tile(np.arange(nOrbitals), (nOverlaps + 1, 1))
         mtx_phases = compute_phases(overlaps, nOverlaps, dim)
         fixed_phase_overlaps = correct_phases(overlaps, mtx_phases)
 
     # Write the overlaps in text format
     if config.write_overlaps:
@@ -96,28 +96,28 @@
         write_overlaps_in_ascii(fixed_phase_overlaps)
 
     # Compute the couplings using either the levine method
     # or the 3Points approximation
     coupling_algorithms = {'levine': (calculate_couplings_levine, 1),
                            '3points': (calculate_couplings_3points, 2)}
     # Choose an algorithm to compute the couplings
-    fun_coupling, step = coupling_algorithms[config["algorithm"]]
-    config["fun_coupling"] = fun_coupling
+    fun_coupling, step = coupling_algorithms[config.algorithm]
+    config.fun_coupling = fun_coupling
 
     # Number of couplings to compute
     nCouplings = fixed_phase_overlaps.shape[0] - step + 1
     couplings = [calculate_couplings(config, i, fixed_phase_overlaps)
                  for i in range(nCouplings)]
 
     return swaps, couplings
 
 
 def compute_the_fixed_phase_overlaps(
     paths_overlaps: List[str],
-    config: DictConfig,
+    config: _data.DerivativeCoupling,
 ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.int_]]:
     """Fix the phase of the overlaps.
 
     First track the unavoided crossings between Molecular orbitals and
     finally correct the phase for the whole trajectory.
     """
     number_of_frames = len(paths_overlaps)
@@ -169,15 +169,19 @@
         fixed_phase_overlaps = np.stack(
             retrieve_hdf5_data(config.path_hdf5, paths_corrected_overlaps))
         swaps = retrieve_hdf5_data(config.path_hdf5, path_swaps)
 
     return fixed_phase_overlaps, swaps
 
 
-def calculate_couplings(config: DictConfig, i: int, fixed_phase_overlaps: Tensor3D) -> str:
+def calculate_couplings(
+    config: _data.DerivativeCoupling,
+    i: int,
+    fixed_phase_overlaps: Tensor3D,
+) -> str:
     """Compute couplings for the i-th geometry.
 
     Search for the ith Coupling in the HDF5, if it is not available compute it
     using the 3 points approximation and store it in the HDF5.
 
     Returns
     -------
@@ -198,20 +202,20 @@
         return path
     else:
         logger.info(f"Computing coupling: {path}")
         if config.algorithm == 'levine':
             # Extract the overlap matrices involved in the coupling computation
             sji_t0 = fixed_phase_overlaps[i]
             # Compute the couplings with the phase corrected overlaps
-            couplings = config["fun_coupling"](
-                dt_au, sji_t0, sji_t0.transpose())
+            couplings = config.fun_coupling(dt_au, sji_t0, sji_t0.T)
         elif config.algorithm == '3points':
             sji_t0, sji_t1 = fixed_phase_overlaps[i: i + 2]
-            couplings = config["fun_coupling"](dt_au, sji_t0, sji_t0.transpose(), sji_t1,
-                                               sji_t1.transpose())
+            couplings = config.fun_coupling(
+                dt_au, sji_t0, sji_t0.T, sji_t1, sji_t1.T
+            )
 
             # Store the Coupling in the HDF5
         store_arrays_in_hdf5(config.path_hdf5, path, couplings)
 
         return path
 
 
@@ -321,15 +325,18 @@
     for i, mtx in enumerate(np.rollaxis(overlaps, 0)):
         overlaps[i] = mtx[:, swaps][swaps]
 
     return overlaps
 
 
 @schedule
-def calculate_overlap(config: DictConfig, mo_paths_hdf5: List[str]) -> List[str]:
+def calculate_overlap(
+    config: _data.DerivativeCoupling,
+    mo_paths_hdf5: List[str],
+) -> List[str]:
     """Calculate the Overlap matrices.
 
     Parameters
     ----------
     config
         Configuration of the current job
     mo_paths_hdf5
@@ -355,15 +362,18 @@
             p = single_machine_overlaps(config, mo_paths_hdf5, i)
         paths.append(p)
 
     return paths
 
 
 def single_machine_overlaps(
-        config: DictConfig, mo_paths_hdf5: List[str], i: int) -> str:
+    config: _data.DerivativeCoupling,
+    mo_paths_hdf5: List[str],
+    i: int,
+) -> str:
     """Compute the overlaps in the CPUs avaialable on the local machine.
 
     Returns
     -------
     str
         Node path to the overlaps store in the HDF5
 
@@ -382,44 +392,45 @@
     # Store the array in the HDF5
     overlaps_paths_hdf5 = create_overlap_path(config, i)
     store_arrays_in_hdf5(config.path_hdf5, overlaps_paths_hdf5, overlaps)
 
     return overlaps_paths_hdf5
 
 
-def create_overlap_path(config: DictConfig, i: int) -> str:
+def create_overlap_path(config: _data.DerivativeCoupling, i: int) -> str:
     """Create the path inside the HDF5 where the overlap is going to be store."""
     root = join(config.orbitals_type, 'overlaps_{}'.format(
         i + config.enumerate_from))
     return join(root, 'mtx_sji_t0')
 
 
-def select_molecules(config: DictConfig, i: int) -> Tuple[MolXYZ, MolXYZ]:
+def select_molecules(config: _data.DerivativeCoupling, i: int) -> Tuple[MolXYZ, MolXYZ]:
     """Select the pairs of molecules to compute the couplings."""
     k = 0 if config.overlaps_deph else i
     return (
         parse_string_xyz(config.geometries[k]),
         parse_string_xyz(config.geometries[i + 1]),
     )
 
 
-def check_if_overlap_is_done(config: DictConfig, overlaps_paths_hdf5: str) -> bool:
+def check_if_overlap_is_done(config: _data.DerivativeCoupling, overlaps_paths_hdf5: str) -> bool:
     """Search for a given Overlap inside the HDF5."""
     if is_data_in_hdf5(config.path_hdf5, overlaps_paths_hdf5):
         logger.info(f"{overlaps_paths_hdf5} Overlaps are already in the HDF5")
         return True
     else:
         logger.info(f"Computing: {overlaps_paths_hdf5}")
         return False
 
 
 def write_hamiltonians(
-        config: DictConfig,
-        crossing_and_couplings: Tuple[np.ndarray, List[Matrix]],
-        mo_paths_hdf5: List[str]) -> List[Tuple[str, str]]:
+    config: _data.DerivativeCoupling,
+    crossing_and_couplings: Tuple[np.ndarray, List[Matrix]],
+    mo_paths_hdf5: List[str],
+) -> List[Tuple[str, str]]:
     """Write the real and imaginary components of the hamiltonian.
 
     It uses both the orbitals energies and the derivative coupling accoring to:
     http://pubs.acs.org/doi/abs/10.1021/ct400641n
     .. Note::
         **Units are: Rydbergs**.
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/distribute_jobs.py` & `nano-qmflows-0.14.0/nanoqm/workflows/distribute_jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,28 @@
 Otherwise the user can fill the the ``free_format`` property with her
 own configuration in the yaml input file.
 
 """
 
 from __future__ import annotations
 
+import copy
 import argparse
 import os
 import shutil
 import subprocess
 from os.path import join
-from typing import Dict, Tuple
 
 import numpy as np
 import yaml
 
-from qmflows import Settings
-
-from ..common import DictConfig, read_cell_parameters_as_array, UniqueSafeLoader
+from ..common import read_cell_parameters_as_array, UniqueSafeLoader
 from .initialization import split_trajectory
 from .input_validation import process_input
+from .. import _data
 
 
 def read_cmd_line() -> str:
     """Read the input file and the workflow name from the command line."""
     msg = "distribute_jobs.py -i input.yml"
 
     parser = argparse.ArgumentParser(description=msg)
@@ -62,169 +61,179 @@
     input_file = read_cmd_line()
 
     with open(input_file, 'r') as f:
         args = yaml.load(f, Loader=UniqueSafeLoader)
 
     # Read and process input
     workflow_type = args['workflow'].lower()
-    dict_input = process_input(input_file, workflow_type)
+    config = process_input(input_file, workflow_type)
+
     # Write scripts to run calculations
     if workflow_type == "distribute_derivative_couplings":
-        distribute_computations(dict_input, hamiltonians=True)
+        distribute_computations(config, hamiltonians=True)
     else:
-        distribute_computations(dict_input)
+        distribute_computations(config)
 
 
-def distribute_computations(config: DictConfig, hamiltonians: bool = False) -> None:
+def distribute_computations(config: _data.Distribute, hamiltonians: bool = False) -> None:
     """Prepare the computation and write the scripts."""
     # Check if workdir exits otherwise create it
     os.makedirs(config.workdir, exist_ok=True)
 
     # Split the trajectory in Chunks and move each chunk to its corresponding
     # directory.
     chunks_trajectory = split_trajectory(
         config.path_traj_xyz, config.blocks, config.workdir)
     chunks_trajectory.sort()
 
-    file_cell_parameters = config.cp2k_general_settings.get(
-        "file_cell_parameters")
+    file_cell_parameters = config.cp2k_general_settings.file_cell_parameters
     if file_cell_parameters is not None:
         header_array_cell_parameters = read_cell_parameters_as_array(
             file_cell_parameters)
 
     # Scratch for all the chunks
     parent_scratch = config.scratch_path
     accumulated_number_of_geometries = 0
 
     for index, file_xyz in enumerate(chunks_trajectory):
-        copy_config = DictConfig(config.copy())
-        copy_config["scratch_path"] = os.path.join(parent_scratch, f"scratch_chunk_{index}")
+        copy_config = copy.copy(config)
+        copy_config.scratch_path = os.path.join(parent_scratch, f"scratch_chunk_{index}")
 
         folder_path = os.path.abspath(join(copy_config.workdir, f'chunk_{index}'))
 
-        dict_input = DictConfig({
-            'folder_path': folder_path, "file_xyz": file_xyz, 'index': index})
+        dict_input = _data.DistributeData(
+            folder_path=folder_path,
+            file_xyz=file_xyz,
+            index=index,
+            hamiltonians_dir=None,
+        )
 
         create_folders(copy_config, dict_input)
 
         # number of geometries per batch
         dim_batch = compute_number_of_geometries(join(folder_path, file_xyz))
 
         # change the window of molecules to compute
-        copy_config['enumerate_from'] = accumulated_number_of_geometries
+        copy_config.enumerate_from = accumulated_number_of_geometries
 
         # HDF5 file where both the Molecular orbitals and coupling are stored
         copy_config.path_hdf5 = join(copy_config.scratch_path, f'chunk_{index}.hdf5')
 
         # Change hdf5 and trajectory path of each batch
-        copy_config["path_traj_xyz"] = file_xyz
+        copy_config.path_traj_xyz = file_xyz
 
         if file_cell_parameters is not None:
-            add_chunk_cell_parameters(
-                header_array_cell_parameters, copy_config, dict_input)
+            add_chunk_cell_parameters(header_array_cell_parameters, copy_config, dict_input)
 
         # files with PYXAID
         if hamiltonians:
-            path_ham = "hamiltonians" if not config.orbitals_type else f"{config.orbitals_type}_hamiltonians"
-            dict_input.hamiltonians_dir = join(
-                copy_config.scratch_path, path_ham)
+            if not config.orbitals_type:
+                path_ham = "hamiltonians"
+            else:
+                path_ham = f"{config.orbitals_type}_hamiltonians"
+            dict_input.hamiltonians_dir = join(copy_config.scratch_path, path_ham)
 
         # Write input file
         write_input(folder_path, copy_config)
 
         # Slurm executable
-        scheduler = copy_config.job_scheduler["scheduler"].upper()
+        scheduler = copy_config.job_scheduler.scheduler.upper()
         if scheduler == "SLURM":
             write_slurm_script(copy_config, dict_input, dim_batch, accumulated_number_of_geometries)
         else:
             msg = f"The request job_scheduler: {scheduler} it is not implemented"
             raise RuntimeError(msg)
 
         accumulated_number_of_geometries += dim_batch
 
 
-def write_input(folder_path: str | os.PathLike[str], original_config: DictConfig) -> None:
+def write_input(folder_path: str | os.PathLike[str], original_config: _data.Distribute) -> None:
     """Write the python script to compute the PYXAID hamiltonians."""
     file_path = join(folder_path, "input.yml")
 
     # transform settings to standard dictionary
-    config = Settings(original_config).as_dict()
+    config = original_config.asdict()
 
     # basis and potential
     config["cp2k_general_settings"]["path_basis"] = os.path.abspath(
-        config["cp2k_general_settings"]["path_basis"])
+        config["cp2k_general_settings"]["path_basis"]
+    )
 
     # remove unused keys from input
-    for k in ['blocks', 'job_scheduler', 'mo_index_range',
-              'workdir']:
+    for k in ['blocks', 'job_scheduler', 'mo_index_range', 'workdir']:
         del config[k]
 
     # rename the workflow to execute
-    dict_distribute = {"distribute_derivative_couplings": "derivative_couplings",
-                       "distribute_absorption_spectrum": "absorption_spectrum",
-                       "distribute_single_points": "single_points"
-                       }
+    dict_distribute = {
+        "distribute_derivative_couplings": "derivative_couplings",
+        "distribute_absorption_spectrum": "absorption_spectrum",
+        "distribute_single_points": "single_points",
+    }
     workflow_type = config["workflow"].lower()
     config['workflow'] = dict_distribute[workflow_type]
     with open(file_path, "w") as f:
         yaml.dump(config, f, default_flow_style=False, allow_unicode=True)
 
 
-def create_folders(config: DictConfig, dict_input: DictConfig) -> None:
+def create_folders(config: _data.Distribute, dict_input: _data.DistributeData) -> None:
     """Create folder for each batch and copy the xyz."""
     # Move xyz to temporal file
     os.makedirs(dict_input.folder_path, exist_ok=True)
     shutil.move(dict_input.file_xyz, dict_input.folder_path)
 
     # Scratch directory
     batch_dir = join(config.scratch_path, f'batch_{dict_input.index}')
     os.makedirs(batch_dir, exist_ok=True)
 
 
-def write_slurm_script(config: DictConfig, dict_input: DictConfig,
-                       dim_batch: int, acc: int) -> None:
+def write_slurm_script(
+    config: _data.Distribute,
+    dict_input: _data.DistributeData,
+    dim_batch: int,
+    acc: int,
+) -> None:
     """Write an Slurm launch script."""
     index = dict_input.index
     python = "\n\nrun_workflow.py -i input.yml\n"
     results_dir = "results_chunk_" + str(index)
     mkdir = f"\nmkdir -p {results_dir}\n"
     slurm_config = config.job_scheduler
 
     # Copy a subset of Hamiltonians
-    if dict_input.get("hamiltonians_dir") is None:
+    if dict_input.hamiltonians_dir is None:
         copy = ""
     else:
         range_batch = (acc, acc + dim_batch - 1)
         files_hams = f"{dict_input.hamiltonians_dir}/Ham_{{{range_batch[0]}..{range_batch[1]}}}_*"
         copy = f'cp -r {config.path_hdf5} {files_hams} {results_dir}\n'
 
     # Script content
     content = format_slurm_parameters(slurm_config) + python + mkdir + copy
 
     # Write the script
     with open(join(dict_input.folder_path, "launch.sh"), 'w') as f:
         f.write(content)
 
 
-def format_slurm_parameters(slurm: Dict[str, str]) -> str:
+def format_slurm_parameters(slurm: _data.JobScheduler) -> str:
     """Format as a string some SLURM parameters."""
     sbatch = "#SBATCH -{} {}\n".format
 
     header = "#! /bin/bash\n"
-    time = sbatch('t', slurm["wall_time"])
-    nodes = sbatch('N', slurm["nodes"])
-    tasks = sbatch('n', slurm["tasks"])
-    name = sbatch('J', slurm["job_name"])
-    queue = sbatch('p', slurm["queue_name"])
+    time = sbatch('t', slurm.wall_time)
+    nodes = sbatch('N', slurm.nodes)
+    tasks = sbatch('n', slurm.tasks)
+    name = sbatch('J', slurm.job_name)
+    queue = sbatch('p', slurm.queue_name)
 
-    modules = slurm["load_modules"]
+    modules = slurm.load_modules
 
-    if "free_format" in slurm:
+    if slurm.free_format:
         # Remove empty spaces
-        lines = slurm["free_format"].splitlines()
+        lines = slurm.free_format.splitlines()
         return '\n'.join(' '.join(x.split()) for x in lines if x)
     else:
         return ''.join((header, time, nodes, tasks, name, queue, modules))
 
 
 def compute_number_of_geometries(file_name: str | os.PathLike[str]) -> int:
     """Count the number of geometries in XYZ formant in a given file."""
@@ -236,22 +245,23 @@
 
     lines_per_geometry = numat + 2
 
     return int(wc) // lines_per_geometry
 
 
 def add_chunk_cell_parameters(
-        header_array_cell_parameters: Tuple[str, np.ndarray],
-        config: DictConfig, dict_input: DictConfig) -> None:
+    header_array_cell_parameters: tuple[str, np.ndarray],
+    config: _data.Distribute,
+    dict_input: _data.DistributeData,
+) -> None:
     """Add the corresponding set of cell parameters for a given chunk."""
-    path_file_cell_parameters = join(
-        dict_input.folder_path, "cell_parameters.txt")
+    path_file_cell_parameters = join(dict_input.folder_path, "cell_parameters.txt")
 
     # Adjust settings
-    config.cp2k_general_settings["file_cell_parameters"] = path_file_cell_parameters
+    config.cp2k_general_settings.file_cell_parameters = path_file_cell_parameters
 
     # extract cell parameters for a chunk
     header, arr = header_array_cell_parameters
     size = int(np.ceil(arr.shape[0] / config.blocks))
     low = dict_input.index * size
     high = low + size
     step = config.stride
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/initialization.py` & `nano-qmflows-0.14.0/nanoqm/workflows/initialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,106 +11,101 @@
 .. autofunction:: initialize
 .. autofunction:: split_trajectory
 
 """
 
 from __future__ import annotations
 
-__all__ = ['initialize', 'read_swaps', 'split_trajectory']
-
 import re
 import fnmatch
 import getpass
 import os
 import subprocess
 import tempfile
 from os.path import join
 from pathlib import Path
 from subprocess import PIPE, Popen
-from typing import List, Union
+from typing import List, Union, TYPE_CHECKING
 
 import h5py
 import numpy as np
 import qmflows
 from nanoutils import RecursiveItemsView
 from packaging.version import Version
 from qmflows.common import AtomBasisKey
 from qmflows.parsers import parse_string_xyz
 from qmflows.parsers.cp2k import read_cp2k_basis
 from qmflows.type_hints import PathLike
 
 from .. import logger, __version__, __path__ as nanoqm_path
 from .._logger import EnableFileHandler
-from ..common import (BasisFormats, DictConfig, Matrix, change_mol_units,
+from ..common import (BasisFormats, Matrix, change_mol_units,
                       is_data_in_hdf5, retrieve_hdf5_data,
                       store_arrays_in_hdf5)
 from ..schedule.components import create_point_folder, split_file_geometries
 
+if TYPE_CHECKING:
+    from .. import _data
 
-def initialize(config: DictConfig) -> DictConfig:
-    """Initialize all the data required to schedule the workflows.
+__all__ = ['initialize', 'read_swaps', 'split_trajectory']
 
-    Returns
-    -------
-    DictConfig
-        Input to run the workflow.
 
-    """
+def initialize(config: _data.GeneralOptions) -> None:
+    """Initialize all the data required to schedule the workflows."""
     with EnableFileHandler(f'{config.project_name}.log'):
         logger.info(f"Using nano-qmflows version: {qmflows.__version__} ")
         logger.info(f"nano-qmflows path is: {nanoqm_path[0]}")
         logger.info(f"Working directory is: {os.path.abspath('.')}")
         logger.info(f"Data will be stored in HDF5 file: {config.path_hdf5}")
 
         # Scratch folder
-        scratch_path = create_path_option(config["scratch_path"])
+        scratch_path = create_path_option(config.scratch_path)
         if scratch_path is None:
             scratch_path = (
                 Path(tempfile.gettempdir()) / getpass.getuser() / config.project_name
             )
+            config.scratch_path = scratch_path
             logger.warning(f"path to scratch was not defined, using: {scratch_path}")
-        config['workdir'] = scratch_path
+        config.workdir = scratch_path
 
         # If the directory does not exist create it
         if not scratch_path.exists():
             scratch_path.mkdir(parents=True)
 
         # Touch HDF5 if it doesn't exists
-        if not os.path.exists(config.path_hdf5):
-            Path(config.path_hdf5).touch()
+        with h5py.File(config.path_hdf5, "a"):
+            pass
 
         # all_geometries type :: [String]
-        geometries = split_file_geometries(config["path_traj_xyz"])
-        config['geometries'] = geometries
+        geometries = split_file_geometries(config.path_traj_xyz)
+        config.geometries = geometries
 
         # Create a folder for each point the the dynamics
-        enumerate_from = config["enumerate_from"]
+        enumerate_from = config.enumerate_from
         len_geometries = len(geometries)
-        config["folders"] = create_point_folder(
-            scratch_path, len_geometries, enumerate_from)
+        config.folders = create_point_folder(scratch_path, len_geometries, enumerate_from)
 
-        config['calc_new_wf_guess_on_points'] = guesses_to_compute(
-            config['calculate_guesses'], enumerate_from, len_geometries)
+        config.calc_new_wf_guess_on_points = guesses_to_compute(
+            config.calculate_guesses, enumerate_from, len_geometries
+        )
 
         # Generate a list of tuples containing the atomic label
         # and the coordinates to generate the primitive CGFs
         atoms = parse_string_xyz(geometries[0])
-        if 'angstrom' in config["geometry_units"].lower():
+        if 'angstrom' in config.geometry_units.lower():
             atoms = change_mol_units(atoms)
 
         # Save Basis to HDF5
         save_basis_to_hdf5(config)
 
-    return config
-
 
-def save_basis_to_hdf5(config: DictConfig) -> None:
+def save_basis_to_hdf5(config: _data.GeneralOptions) -> None:
     """Store the specification of the basis set in the HDF5 to compute the integrals."""
-    root: str = config['cp2k_general_settings']['path_basis']
-    files: "None | list[str]" = config['cp2k_general_settings']['basis_file_name']
+    root: str = config.cp2k_general_settings.path_basis
+    files: "None | list[str]" = config.cp2k_general_settings.basis_file_name
     if files is not None:
         basis_paths = [os.path.join(root, i) for i in files]
     else:
         basis_paths = [os.path.join(root, "BASIS_MOLOPT")]
 
     for path in basis_paths:
         if not is_data_in_hdf5(config.path_hdf5, path):
@@ -162,15 +157,19 @@
     formats = [np.fromiter(xs.basisFormat, dtype=np.int64) for xs in keys]
 
     store_arrays_in_hdf5(path_hdf5, node_paths_exponents, exponents)
     store_arrays_in_hdf5(path_hdf5, node_paths_coefficients, coefficients,
                          attribute=BasisFormats(name="basisFormat", value=formats))
 
 
-def guesses_to_compute(calculate_guesses: str, enumerate_from: int, len_geometries: int) -> List[int]:
+def guesses_to_compute(
+    calculate_guesses: str,
+    enumerate_from: int,
+    len_geometries: int,
+) -> List[int]:
     """Guess for the wave function."""
     if calculate_guesses is None:
         points_guess = []
     elif calculate_guesses.lower() in 'first':
         # Calculate new Guess in the first geometry
         points_guess = [enumerate_from]
         msg = "An initial Calculation will be computed as guess for the wave function"
@@ -240,10 +239,10 @@
     err = rs[1]
     if err:
         raise RuntimeError(f"Submission Errors: {err.decode()}")
     else:
         return fnmatch.filter(os.listdir(), "chunk_xyz_?")
 
 
-def create_path_option(path: str | os.PathLike[str]) -> Path | None:
+def create_path_option(path: None | str | os.PathLike[str]) -> Path | None:
     """Create a Path object or return None if path is None."""
     return Path(path) if path is not None else None
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/input_validation.py` & `nano-qmflows-0.14.0/nanoqm/workflows/input_validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Functionality to check that the input provided by the user is valid.
 
 Index
 -----
 .. currentmodule:: nanoqm.workflows.input_validation
-.. autosummary:: process_input
+.. autosummary::
+    process_input
 
 API
 ---
 .. autofunction:: process_input
 
 """
 
+from __future__ import annotations
+
 import os
-import warnings
 from os.path import join
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import overload, Literal
 
 import yaml
 from schema import SchemaError
 from scm.plams import Molecule
 
 from qmflows import Settings
 from qmflows.type_hints import PathLike
 
+from .. import _data
 from .. import logger
-from ..common import DictConfig, UniqueSafeLoader, valence_electrons
+from ..common import UniqueSafeLoader, valence_electrons
 from .schemas import (schema_absorption_spectrum, schema_coop,
                       schema_cp2k_general_settings,
                       schema_derivative_couplings,
                       schema_distribute_absorption_spectrum,
                       schema_distribute_derivative_couplings,
                       schema_distribute_single_points, schema_ipr,
                       schema_single_points)
@@ -44,15 +47,35 @@
     'distribute_absorption_spectrum': schema_distribute_absorption_spectrum,
     'distribute_single_points': schema_distribute_single_points,
     'ipr_calculation': schema_ipr,
     'coop_calculation': schema_coop
 }
 
 
-def process_input(input_file: PathLike, workflow_name: str) -> DictConfig:
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["absorption_spectrum"]) -> _data.AbsorptionSpectrum: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["derivative_couplings"]) -> _data.DerivativeCoupling: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["single_points"]) -> _data.SinglePoints: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["cp2k_general_settings"]) -> _data.CP2KGeneralSetting: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["distribute_derivative_couplings"]) -> _data.DistributeDerivativeCoupling: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["distribute_absorption_spectrum"]) -> _data.DistributeAbsorptionSpectrum: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["distribute_single_points"]) -> _data.DistributeSinglePoints: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["ipr_calculation"]) -> _data.IPR: ...
+@overload
+def process_input(input_file: PathLike, workflow_name: Literal["coop_calculation"]) -> _data.COOP: ...
+
+
+def process_input(input_file: PathLike, workflow_name: str) -> _data.GeneralOptions:
     """Read the `input_file` in YAML format and validate it.
 
     Use the corresponding `workflow_name` schema and return a nested
     dictionary with the input.
 
     Parameters
     ----------
@@ -72,73 +95,64 @@
     schema = schema_workflows[workflow_name]
 
     with open(input_file, 'r') as f:
         dict_input = yaml.load(f.read(), Loader=UniqueSafeLoader)
 
     try:
         d = schema.validate(dict_input)
-        return DictConfig(InputSanitizer(d).sanitize())
-
+        return InputSanitizer(d).sanitize()
     except SchemaError as e:
         msg = f"There was an error in the input yaml provided:\n{e}"
         logger.warning(msg)
         raise
 
 
 class InputSanitizer:
     """Class to sanitize the input."""
 
-    def __init__(self, input_dict: Dict):
+    def __init__(self, dataclass: _data.GeneralOptions) -> None:
         """Set the class properties."""
-        self.user_input = input_dict
-        self.general = input_dict["cp2k_general_settings"]
+        self.user_input = dataclass
+        self.general = dataclass.cp2k_general_settings
 
-    def sanitize(self) -> Dict:
+    def sanitize(self) -> _data.GeneralOptions:
         """Apply all the sanity check on the input."""
-        self.create_settings()
         self.apply_templates()
         self.add_missing_keywords()
         self.add_executable()
         self.print_final_input()
-
         return self.user_input
 
-    def create_settings(self) -> None:
-        """Transform the CP2K input dict into :class:`QMFLows.Settings`."""
-        self.general['cp2k_settings_main'] = Settings(self.general['cp2k_settings_main'])
-        self.general['cp2k_settings_guess'] = Settings(self.general['cp2k_settings_guess'])
-
     def apply_templates(self) -> None:
         """Apply a template for CP2K if the user requested it."""
-        for s in [
-                self.general[x] for x in ('cp2k_settings_main', 'cp2k_settings_guess')]:
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
             val = s['specific']
 
             if "template" in val:
                 cp2k_template = create_settings_from_template(
-                    self.general, val['template'], self.user_input["path_traj_xyz"])
+                    self.general, val['template'], self.user_input.path_traj_xyz)
                 # remove template
                 del s['specific']['template']
 
                 # Add other keywords
                 s['specific'] = cp2k_template.overlay(s['specific'])
 
     def add_executable(self) -> None:
         """Add executable to the job settings."""
-        self.general['cp2k_settings_main']['executable'] = self.general['executable']
-        self.general['cp2k_settings_guess']['executable'] = self.general['executable']
+        self.general.cp2k_settings_main.executable = self.general.executable
+        self.general.cp2k_settings_guess.executable = self.general.executable
 
     def add_missing_keywords(self) -> None:
         """Add missing input data using the defaults."""
         # Add the `added_mos` and `mo_index_range` keywords
-        if self.user_input.get('nHOMO') is None:
-            self.user_input["nHOMO"] = self.compute_homo_index()
+        if self.user_input.nHOMO is None:
+            self.user_input.nHOMO = self.compute_homo_index()
 
         # Added_mos keyword
-        if self.user_input.get('compute_orbitals'):
+        if self.user_input.compute_orbitals:
             self.add_mo_index_range()
         else:
             logger.info("Orbitals are neither print nor store!")
 
         # Add restart point provided by the user
         self.add_restart_point()
 
@@ -161,41 +175,41 @@
         self.add_functional_x()
 
         # Add DFT correlation part
         self.add_functional_c()
 
     def compute_homo_index(self) -> int:
         """Compute the index of the (doubly occupied) HOMO."""
-        charge = self.general['charge']
-        multiplicity = self.general['multiplicity']
-        mol = Molecule(self.user_input["path_traj_xyz"], 'xyz')
+        charge = self.general.charge
+        multiplicity = self.general.multiplicity
+        mol = Molecule(self.user_input.path_traj_xyz, 'xyz')
 
         n_paired_electrons = sum(valence_electrons[at.symbol] for at in mol.atoms)
         n_paired_electrons -= charge  # Correct for total charge of the system
         n_paired_electrons -= (multiplicity - 1)  # Correct for the number of SOMOs
 
         assert (n_paired_electrons % 2) == 0
         return n_paired_electrons // 2
 
     def add_basis(self) -> None:
         """Add path to the basis and potential."""
-        setts = [self.general[p] for p in ['cp2k_settings_main', 'cp2k_settings_guess']]
+        setts = (self.general.cp2k_settings_main, self.general.cp2k_settings_guess)
 
-        root = os.path.abspath(self.general['path_basis'])
-        if self.general['potential_file_name'] is not None:
-            names = [join(root, f) for f in self.general["potential_file_name"]]
+        root = os.path.abspath(self.general.path_basis)
+        if self.general.potential_file_name is not None:
+            names = [join(root, f) for f in self.general.potential_file_name]
         else:
             names = [join(root, "GTH_POTENTIALS")]
 
         # add basis and potential path
-        if self.general["path_basis"] is not None:
+        if self.general.path_basis is not None:
             logger.info("path to basis added to cp2k settings")
             for x in setts:
-                x.basis = self.general['basis']
-                x.potential = self.general['potential']
+                x.basis = self.general.basis
+                x.potential = self.general.potential
 
                 # Do not overwrite explicitly specified CP2K settings
                 dft = x.specific.cp2k.force_eval.dft
                 if dft.get("potential_file_name") is None:
                     dft["potential_file_name"] = names
 
                 # Choose the file basis to use
@@ -205,103 +219,88 @@
         """Choose the right basis set based on the potential and basis name."""
         dft = sett.specific.cp2k.force_eval.dft
 
         # Do not overwrite explicitly specified CP2K settings
         if dft.get("basis_set_file_name") is not None:
             return
 
-        root = os.path.abspath(self.general['path_basis'])
-        if self.general['basis_file_name'] is not None:
-            dft["basis_set_file_name"] = [join(root, f) for f in self.general["basis_file_name"]]
+        root = os.path.abspath(self.general.path_basis)
+        if self.general.basis_file_name is not None:
+            dft["basis_set_file_name"] = [join(root, f) for f in self.general.basis_file_name]
         else:
             dft["basis_set_file_name"] = [join(root, "BASIS_MOLOPT")]
             # USE ADMM
             if dft.xc.get("xc_functional pbe") is None:
                 dft["basis_set_file_name"] += [
                     join(root, "BASIS_ADMM_MOLOPT"),
                     join(root, "BASIS_ADMM"),
                 ]
 
     def add_cell_parameters(self) -> None:
         """Add the Unit cell information to both the main and the guess settings."""
         # Search for a file containing the cell parameters
-        for s in (self.general[p] for p in [
-                'cp2k_settings_main',
-                'cp2k_settings_guess']):
-            if self.general["file_cell_parameters"] is None:
-                s.cell_parameters = self.general['cell_parameters']
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+            if self.general.file_cell_parameters is None:
+                s.cell_parameters = self.general.cell_parameters
                 s.cell_angles = None
             else:
                 s.cell_parameters = None
             s.cell_angles = None
 
     def add_periodic(self) -> None:
         """Add the keyword for the periodicity of the system."""
-        for s in (
-            self.general[p] for p in [
-                'cp2k_settings_main',
-                'cp2k_settings_guess']):
-            s.specific.cp2k.force_eval.subsys.cell.periodic = self.general['periodic']
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+            s.specific.cp2k.force_eval.subsys.cell.periodic = self.general.periodic
 
     def add_charge(self) -> None:
         """Add the keyword for the charge of the system."""
-        for s in (
-            self.general[p] for p in [
-                'cp2k_settings_main',
-                'cp2k_settings_guess']):
-            s.specific.cp2k.force_eval.dft.charge = self.general['charge']
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+            s.specific.cp2k.force_eval.dft.charge = self.general.charge
 
     def add_multiplicity(self) -> None:
         """Add the keyword for the multiplicity of the system only if greater than 1."""
-        if self.general['multiplicity'] > 1:
-            for s in (
-                    self.general[p] for p in ('cp2k_settings_main', 'cp2k_settings_guess')):
-                s.specific.cp2k.force_eval.dft.multiplicity = self.general['multiplicity']
+        if self.general.multiplicity > 1:
+            for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+                s.specific.cp2k.force_eval.dft.multiplicity = self.general.multiplicity
                 s.specific.cp2k.force_eval.dft.uks = ""
-        self.user_input["multiplicity"] = self.general["multiplicity"]
+        self.user_input.multiplicity = self.general.multiplicity
 
     def add_functional_x(self) -> None:
         """Add the keyword for the exchange part of the DFT functional: GGA or MGGA."""
-        if self.general['functional_x'] is None:
+        if self.general.functional_x is None:
             return
-        for s in (
-            self.general[p] for p in [
-                'cp2k_settings_main',
-                'cp2k_settings_guess']):
-            s.specific.cp2k.force_eval.dft.xc.xc_functional[self.general['functional_x']] = {}
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+            s.specific.cp2k.force_eval.dft.xc.xc_functional[self.general.functional_x] = {}
 
     def add_functional_c(self) -> None:
         """Add the keyword for the correlation part of the DFT functional: GGA or MGGA."""
-        if self.general['functional_c'] is None:
+        if self.general.functional_c is None:
             return
-        for s in (
-            self.general[p] for p in [
-                'cp2k_settings_main',
-                'cp2k_settings_guess']):
-            s.specific.cp2k.force_eval.dft.xc.xc_functional[self.general['functional_c']] = {}
+        for s in (self.general.cp2k_settings_main, self.general.cp2k_settings_guess):
+            s.specific.cp2k.force_eval.dft.xc.xc_functional[self.general.functional_c] = {}
 
     def add_restart_point(self) -> None:
         """Add a restart file if the user provided it."""
-        guess = self.general['cp2k_settings_guess']
-        wfn = self.general['wfn_restart_file_name']
+        guess = self.general.cp2k_settings_guess
+        wfn = self.general.wfn_restart_file_name
         if wfn is not None and wfn:
             dft = guess.specific.cp2k.force_eval.dft
             dft.wfn_restart_file_name = Path(wfn).absolute().as_posix()
 
     def add_mo_index_range(self) -> None:
         """Compute the MO range to print."""
-        nocc, nvirt = self.user_input["active_space"]
-        nSOMO = self.general["multiplicity"] - 1
-        nHOMO = self.user_input["nHOMO"]
+        nocc, nvirt = self.user_input.active_space
+        nSOMO = self.general.multiplicity - 1
+        nHOMO = self.user_input.nHOMO
 
         mo_index_range = nHOMO - nocc, nHOMO + nSOMO + nvirt
-        self.user_input["mo_index_range"] = mo_index_range
+        self.user_input.mo_index_range = mo_index_range
 
         # mo_index_range keyword
-        cp2k_main = self.general['cp2k_settings_main']
+        cp2k_main = self.general.cp2k_settings_main
         dft_main_print = cp2k_main.specific.cp2k.force_eval.dft.print
         dft_main_print.mo.mo_index_range = f"{mo_index_range[0] + 1} {mo_index_range[1]}"
 
         # added_mos
         dft = cp2k_main.specific.cp2k.force_eval.dft
         if nSOMO == 0:
             dft.scf.added_mos = mo_index_range[1] - nHOMO - nSOMO
@@ -313,25 +312,10 @@
         dft.print.mo.each.qs_scf = 0
         dft.print.mo.eigenvalues = ""
         dft.print.mo.eigenvectors = ""
         dft.print.mo.ndigits = 36
 
     def print_final_input(self) -> None:
         """Print the input after post-processing."""
-        xs = self.user_input.copy()
-
-        for k, v in self.user_input.items():
-            xs[k] = recursive_traverse(v)
-
+        xs = self.user_input.asdict()
         with open("input_parameters.yml", "w") as f:
             yaml.dump(xs, f, indent=4)
-
-
-def recursive_traverse(val: Union[Dict, Settings, Any]) -> Union[Dict, Settings, Any]:
-    """Check if the value of a key is a Settings instance a transform it to plain dict."""
-    if isinstance(val, dict):
-        if isinstance(val, Settings):
-            return val.as_dict()
-        else:
-            return {k: recursive_traverse(v) for k, v in val.items()}
-    else:
-        return val
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/orbitals_type.py` & `nano-qmflows-0.14.0/nanoqm/workflows/orbitals_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 """Module to run restricted and unrestricted calculations."""
 
-from typing import Any, Callable
+from __future__ import annotations
+
+import copy
+from typing import Any, Callable, TypeVar, TYPE_CHECKING
 
 from noodles import gather
 from qmflows import run
 
 from .. import logger
-from ..common import DictConfig
 from .initialization import initialize
 
+if TYPE_CHECKING:
+    from qmflows.type_hints import PromisedObject
+    from .. import _data
+
+    _T = TypeVar("_T", bound=_data.GeneralOptions)
+
+__all__ = ["select_orbitals_type"]
+
 
-def select_orbitals_type(
-        config: DictConfig, workflow: Callable[[DictConfig], Any]) -> Any:
+def select_orbitals_type(config: _T, workflow: Callable[[_T], PromisedObject]) -> Any:
     """Call a workflow using restriced or unrestricted orbitals."""
     # Dictionary containing the general configuration
-    config.update(initialize(config))
+    initialize(config)
 
     if config.orbitals_type != "both":
         logger.info("starting workflow calculation!")
         promises = workflow(config)
         return run(promises, folder=config.workdir, always_cache=False)
     else:
-        config_alphas = DictConfig(config.copy())
-        config_betas = DictConfig(config.copy())
+        config_alphas = copy.copy(config)
+        config_betas = copy.copy(config)
         config_alphas.orbitals_type = "alphas"
         promises_alphas = workflow(config_alphas)
         config_betas.orbitals_type = "betas"
         promises_betas = workflow(config_betas)
         all_promises = gather(promises_alphas, promises_betas)
         alphas, betas = run(all_promises, folder=config.workdir, always_cache=False)
         return alphas, betas
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/run_workflow.py` & `nano-qmflows-0.14.0/nanoqm/workflows/run_workflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,16 +9,20 @@
     * derivative_couplings
     * single_points
     * ipr_calculation
     * coop_calculation
 
 """
 
+from __future__ import annotations
+
 import argparse
 import os
+from collections.abc import Callable
+from typing import Any
 
 import yaml
 
 from .. import logger
 from ..common import UniqueSafeLoader
 from .input_validation import process_input
 from .workflow_coop import workflow_crystal_orbital_overlap_population
@@ -26,30 +30,29 @@
 from .workflow_ipr import workflow_ipr
 from .workflow_single_points import workflow_single_points
 from .workflow_stddft_spectrum import workflow_stddft
 
 msg = "run_workflow.py -i input.yml"
 
 parser = argparse.ArgumentParser(description=msg)
-parser.add_argument('-i', required=True,
-                    help="Input file in YAML format")
-
+parser.add_argument('-i', required=True, help="Input file in YAML format")
 
-dict_workflows = {
+dict_workflows: dict[str, Callable[[Any], object]] = {
     'absorption_spectrum': workflow_stddft,
     'derivative_couplings': workflow_derivative_couplings,
     'single_points': workflow_single_points,
     'ipr_calculation': workflow_ipr,
-    'coop_calculation': workflow_crystal_orbital_overlap_population}
+    'coop_calculation': workflow_crystal_orbital_overlap_population,
+}
 
 
-def main():
+def main() -> None:
     """Parse the command line arguments and run workflow."""
     args = parser.parse_args()
-    input_file = args.i
+    input_file: str = args.i
     with open(input_file, 'r') as f:
         dict_input = yaml.load(f, Loader=UniqueSafeLoader)
     if 'workflow' not in dict_input:
         raise RuntimeError(
             "The name of the workflow is required in the input file")
     else:
         workflow_name = dict_input['workflow']
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/schemas.py` & `nano-qmflows-0.14.0/nanoqm/workflows/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,46 +7,54 @@
     {autosummary}
 
 API
 ---
 {autodata}
 
 """
+
+from __future__ import annotations
+
+import os
+from numbers import Real
+from collections.abc import Iterable
+from typing import Any
+
+import pkg_resources as pkg
+from schema import And, Optional, Or, Regex, Schema, Use
+from qmflows import Settings
+
+from .. import _data
+
 __all__ = [
     'schema_cp2k_general_settings',
     'schema_derivative_couplings',
     'schema_single_points',
     'schema_distribute_absorption_spectrum',
     'schema_distribute_derivative_couplings',
     'schema_distribute_single_points',
     'schema_absorption_spectrum',
     'schema_ipr',
-    'schema_coop']
-
-import os
-from numbers import Real
-from typing import Any, Dict, Iterable
-
-import pkg_resources as pkg
-from schema import And, Optional, Or, Regex, Schema, Use
+    'schema_coop',
+]
 
 
 def equal_lambda(name: str) -> And:
     """Create an schema checking that the keyword matches the expected value."""
     return And(
         str, Use(str.lower), lambda s: s == name)
 
 
 def any_lambda(array: Iterable[str]) -> And:
     """Create an schema checking that the keyword matches one of the expected values."""
     return And(
         str, Use(str.lower), lambda s: s in array)
 
 
-def merge(d1: Dict[str, Any], d2: Dict[str, Any]) -> Dict[str, Any]:
+def merge(d1: dict[str, Any], d2: dict[str, Any]) -> dict[str, Any]:
     """Merge two dictionaries using without modifying the original."""
     x = d1.copy()
 
     x.update(d2)
 
     return x
 
@@ -57,16 +65,36 @@
         return [f]
     elif f is None or (isinstance(f, list) and all(isinstance(i, str) for i in f)):
         return f
     else:
         raise TypeError(type(f).__name__)
 
 
+class _DataSchema(Schema):
+    """Schema subclass that casts the return type into a user-specified dataclass."""
+
+    def __init__(
+        self,
+        *args: Any,
+        data_cls: None | type[Any] = None,
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(*args, **kwargs)
+        self._data_cls = data_cls
+
+    def validate(self, data: Any, **kwargs: Any) -> Any:
+        ret = super().validate(data, **kwargs)
+        if type(self.schema) is dict and self._data_cls is not None:
+            return self._data_cls(**ret)
+        else:
+            return ret
+
+
 #: Schema to validate the CP2K general settings
-schema_cp2k_general_settings = Schema({
+schema_cp2k_general_settings = _DataSchema({
 
     # "Basis set to carry out the quantum chemistry simulation"
     "basis": str,
 
     # "Pseudo-potential to carry out the quantum chemistry simulation"
     "potential": str,
 
@@ -82,15 +110,15 @@
         lambda xs: len(xs) == 3 and isinstance(xs, list),
         lambda xs: len(xs) == 3 and all(len(r) == 3 for r in xs)),
 
     # Type of periodicity
     "periodic": any_lambda(("none", "x", "y", "z", "xy", "xy", "yz", "xyz")),
 
     # Specify the angles between the vectors defining the unit cell
-    Optional("cell_angles"): list,
+    Optional("cell_angles", default=None): list,
 
     # Path to the folder containing the basis set specifications
     Optional("path_basis", default=pkg.resource_filename("nanoqm", "basis")): os.path.isdir,
 
     # Name(s) of the basis set file(s) stored in ``path_basis``
     Optional("basis_file_name", default=None): Use(_parse_filenames),
 
@@ -100,55 +128,56 @@
     # Name(s) of the exchange part of the DFT functional`
     Optional("functional_x", default=None): str,
 
     # Name(s) of the correlation part of the DFT functional`
     Optional("functional_c", default=None): str,
 
     # Settings describing the input of the quantum package
-    "cp2k_settings_main": object,
+    "cp2k_settings_main": Use(Settings),
 
     # Settings describing the input of the quantum package
     # to compute the guess wavefunction"
-    "cp2k_settings_guess": object,
+    "cp2k_settings_guess": Use(Settings),
 
     # Restart File Name
     Optional("wfn_restart_file_name", default=None): Or(str, None),
 
     # File containing the Parameters of the cell if those
     # parameters change during the MD simulation.
     Optional("file_cell_parameters", default=None): Or(str, None),
 
     # Quality of the auxiliar basis cFIT
     Optional("aux_fit", default="verygood"):
         any_lambda(("low", "medium", "good", "verygood", "excellent")),
 
-    # executable name
-    # "sdbg" Serial single core testing and debugging
-    # "sopt" Serial general single core usage
-    # "ssmp" Parallel (only OpenMP), single node, multi core
-    # "pdbg" Parallel (only MPI) multi-node testing and debugging
-    # "popt" Parallel (only MPI) general usage, no threads
-    # "psmp" parallel (MPI + OpenMP) general usage, threading might improve scalability and memory usage
+    # executable name:
+    # * "sdbg" Serial single core testing and debugging
+    # * "sopt" Serial general single core usage
+    # * "ssmp" Parallel (only OpenMP), single node, multi core
+    # * "pdbg" Parallel (only MPI) multi-node testing and debugging
+    # * "popt" Parallel (only MPI) general usage, no threads
+    # * "psmp" parallel (MPI + OpenMP) general usage,
+    #   threading might improve scalability and memory usage
 
     Optional("executable", default="cp2k.psmp"):
         Regex(r'.*cp2k\.(?:popt|psmp|sdbg|sopt|ssmp|pdbg)', flags=2)  # flag 2 == IGNORECASE
-})
+}, data_cls=_data.CP2KGeneralSetting)
 
 
 #: Dictionary with the options common to all workflows
 dict_general_options = {
 
     # Number of occupied/virtual orbitals to use
-    Optional('active_space', default=[10, 10]): And(list, lambda xs: len(xs) == 2),
+    Optional('active_space', default=(10, 10)): And(Use(tuple), lambda xs: len(xs) == 2),
 
     # Index of the HOMO
-    Optional("nHOMO"): int,
+    Optional("nHOMO", default=None): int,
 
     # Index of the orbitals to compute the couplings
-    Optional("mo_index_range"): tuple,
+    Optional("mo_index_range", default=None): tuple,
 
     # "default quantum package used"
     Optional("package_name", default="cp2k"): str,
 
     # project
     Optional("project_name", default="namd"): str,
 
@@ -216,29 +245,29 @@
     Optional("overlaps_deph", default=False): bool
 }
 
 dict_merged_derivative_couplings = merge(
     dict_general_options, dict_derivative_couplings)
 
 #: Schema to validate the input for a derivative coupling calculation
-schema_derivative_couplings = Schema(
-    dict_merged_derivative_couplings)
+schema_derivative_couplings = _DataSchema(
+    dict_merged_derivative_couplings, data_cls=_data.DerivativeCoupling)
 
 #: Schema to validate the input for a job scheduler
-schema_job_scheduler = Schema({
+schema_job_scheduler = _DataSchema({
     Optional("scheduler", default="slurm"):
     any_lambda(("slurm", "pbs")),
     Optional("nodes", default=1): int,
     Optional("tasks", default=1): int,
     Optional("wall_time", default="01:00:00"): str,
     Optional("job_name", default="namd"): str,
     Optional("queue_name", default="short"): str,
     Optional("load_modules", default=""): str,
     Optional("free_format", default=""): str
-})
+}, data_cls=_data.JobScheduler)
 
 #: Input options to distribute a job
 dict_distribute = {
 
     Optional("workdir", default=os.getcwd()): str,
 
     # Number of chunks to split the trajectory
@@ -258,20 +287,21 @@
 
     # Name of the workflow to run
     "workflow": equal_lambda("distribute_derivative_couplings")
 }
 
 
 #: Schema to validate the input to distribute a derivate coupling calculation
-schema_distribute_derivative_couplings = Schema(
+schema_distribute_derivative_couplings = _DataSchema(
     merge(
         dict_distribute,
-        merge(
-            dict_merged_derivative_couplings,
-            dict_distribute_derivative_couplings)))
+        merge(dict_merged_derivative_couplings, dict_distribute_derivative_couplings)
+    ),
+    data_cls=_data.DistributeDerivativeCoupling,
+)
 
 #: Input for an absorption spectrum calculation
 dict_absorption_spectrum = {
 
     # Name of the workflow to run
     "workflow": equal_lambda("absorption_spectrum"),
 
@@ -288,26 +318,33 @@
 }
 
 
 dict_merged_absorption_spectrum = merge(
     dict_general_options, dict_absorption_spectrum)
 
 #: Schema to validate the input for an absorption spectrum calculation
-schema_absorption_spectrum = Schema(dict_merged_absorption_spectrum)
+schema_absorption_spectrum = _DataSchema(
+    dict_merged_absorption_spectrum,
+    data_cls=_data.AbsorptionSpectrum,
+)
 
 
 dict_distribute_absorption_spectrum = {
 
     # Name of the workflow to run
     "workflow": equal_lambda("distribute_absorption_spectrum")
 }
 
-schema_distribute_absorption_spectrum = Schema(
-    merge(dict_distribute, merge(
-        dict_merged_absorption_spectrum, dict_distribute_absorption_spectrum)))
+schema_distribute_absorption_spectrum = _DataSchema(
+    merge(
+        dict_distribute,
+        merge(dict_merged_absorption_spectrum, dict_distribute_absorption_spectrum)
+    ),
+    data_cls=_data.DistributeAbsorptionSpectrum,
+)
 
 dict_single_points = {
     # Name of the workflow to run
     "workflow": any_lambda(("single_points", "ipr_calculation", "coop_calculation")),
 
     # General settings
     "cp2k_general_settings": schema_cp2k_general_settings
@@ -318,29 +355,34 @@
 
     # Name of the workflow to run
     "workflow": equal_lambda("distribute_single_points")
 }
 
 #: Input for a Crystal Orbital Overlap Population calculation
 dict_coop = {
-    # List of the two elements to calculate the COOP for
-    "coop_elements": list}
+    # List/tuple of the two elements to calculate the COOP for
+    "coop_elements": And(Use(tuple), lambda xs: len(xs) == 2),
+}
 
 
 dict_merged_single_points = merge(dict_general_options, dict_single_points)
 
 #: Schema to validate the input of a single pointe calculation
-schema_single_points = Schema(dict_merged_single_points)
+schema_single_points = _DataSchema(dict_merged_single_points, data_cls=_data.SinglePoints)
 
 #: Schema to validate the input for a Inverse Participation Ratio calculation
-schema_ipr = schema_single_points
+schema_ipr = _DataSchema(dict_merged_single_points, data_cls=_data.IPR)
 
 #: Input for a Crystal Orbital Overlap Population calculation
 dict_merged_coop = merge(dict_merged_single_points, dict_coop)
 
 #: Schema to validate the input for a Crystal Orbital Overlap Population calculation
-schema_coop = Schema(dict_merged_coop)
+schema_coop = _DataSchema(dict_merged_coop, data_cls=_data.COOP)
 
 #: Schema to validate the input to distribute a single point calculation
-schema_distribute_single_points = Schema(
-    merge(dict_distribute, merge(
-        dict_merged_single_points, dict_distribute_single_points)))
+schema_distribute_single_points = _DataSchema(
+    merge(
+        dict_distribute,
+        merge(dict_merged_single_points, dict_distribute_single_points),
+    ),
+    data_cls=_data.DistributeSinglePoints,
+)
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/templates.py` & `nano-qmflows-0.14.0/nanoqm/workflows/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 .. autosummary::
   create_settings_from_template
 
 """
 
 from __future__ import annotations
 
-__all__ = ["create_settings_from_template"]
-
 import os
+from collections.abc import Iterable
+from typing import TYPE_CHECKING
+
 import yaml
 from scm.plams import Molecule
-
 from qmflows import Settings
-from qmflows.type_hints import PathLike
 from nanoqm.common import UniqueSafeLoader, valence_electrons, aux_fit
-from typing import Any, Dict, Iterable, FrozenSet
+
+if TYPE_CHECKING:
+    from .. import _data
+
+__all__ = ["create_settings_from_template"]
 
 
 def generate_auxiliar_basis(
         sett: Settings, auxiliar_basis: str, quality: str) -> Settings:
     """Generate the `auxiliar_basis` for all the atoms in the `sett`.
 
     Use the`quality` of the auxiliar basis provided by the user.
@@ -427,31 +430,31 @@
     "scan_guess": cp2k_scan_guess, "scan_main": cp2k_scan_main,
     "pbe0_guess": cp2k_pbe0_guess, "pbe0_main": cp2k_pbe0_main,
     "hse06_guess": cp2k_hse06_guess, "hse06_main": cp2k_hse06_main,
     "b3lyp_guess": cp2k_b3lyp_guess, "b3lyp_main": cp2k_b3lyp_main}
 
 
 def create_settings_from_template(
-    general: Dict[str, Any],
+    general: _data.CP2KGeneralSetting,
     template_name: str,
     path_traj_xyz: str | os.PathLike[str],
 ) -> Settings:
     """Create a job Settings using the name provided by the user."""
     setts = templates_dict[template_name]
     elements = read_unique_atomic_labels(path_traj_xyz)
 
-    kinds = generate_kinds(elements, general['basis'], general['potential'])
+    kinds = generate_kinds(elements, general.basis, general.potential)
 
     if 'pbe0' in template_name:
         s = Settings()
-        return generate_auxiliar_basis(setts + s + kinds, general['basis'], general['aux_fit'])
+        return generate_auxiliar_basis(setts + s + kinds, general.basis, general.aux_fit)
     elif 'hse06' in template_name:
-        return generate_auxiliar_basis(setts + kinds, general['basis'], general['aux_fit'])
+        return generate_auxiliar_basis(setts + kinds, general.basis, general.aux_fit)
     else:
         return setts + kinds
 
 
-def read_unique_atomic_labels(path_traj_xyz: str | os.PathLike[str]) -> FrozenSet[str]:
+def read_unique_atomic_labels(path_traj_xyz: str | os.PathLike[str]) -> frozenset[str]:
     """Return the unique atomic labels."""
     mol = Molecule(path_traj_xyz, 'xyz')
 
     return frozenset(at.symbol for at in mol.atoms)
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/workflow_coop.py` & `nano-qmflows-0.14.0/nanoqm/workflows/workflow_coop.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,38 +6,37 @@
 .. autosummary::
     workflow_crystal_orbital_overlap_population
 
 """
 
 from __future__ import annotations
 
-__all__ = ['workflow_crystal_orbital_overlap_population']
-
-from typing import Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
 import numpy as np
-
 from qmflows.parsers import readXYZ
 
 from .. import logger
-from ..common import (DictConfig, MolXYZ, h2ev,
-                      number_spherical_functions_per_atom, retrieve_hdf5_data)
+from ..common import MolXYZ, h2ev, number_spherical_functions_per_atom, retrieve_hdf5_data
 from ..integrals.multipole_matrices import compute_matrix_multipole
 from .initialization import initialize
 from .tools import compute_single_point_eigenvalues_coefficients
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from numpy import float64 as f8, int64 as i8
+    from .. import _data
+
+__all__ = ['workflow_crystal_orbital_overlap_population']
 
 
-def workflow_crystal_orbital_overlap_population(config: DictConfig) -> NDArray[f8]:
+def workflow_crystal_orbital_overlap_population(config: _data.COOP) -> NDArray[f8]:
     """Compute the Crystal Orbital Overlap Population."""
     # Dictionary containing the general information
-    config.update(initialize(config))
+    initialize(config)
 
     # Checking hdf5 for eigenvalues and coefficients. If not present, they are
     # computed.
     compute_single_point_eigenvalues_coefficients(config)
 
     # Logger info
     logger.info("Starting COOP calculation.")
@@ -66,15 +65,15 @@
     # Lastly, we save the COOP as a txt-file
     result_coop = print_coop(energies, coop)
     logger.info("COOP calculation completed.")
 
     return result_coop
 
 
-def get_eigenvalues_coefficients(config: DictConfig) -> Tuple[NDArray[f8], NDArray[f8]]:
+def get_eigenvalues_coefficients(config: _data.COOP) -> tuple[NDArray[f8], NDArray[f8]]:
     """Retrieve eigenvalues and coefficients from hdf5 file."""
     # Define paths to eigenvalues and coefficients hdf5
     node_path_coefficients = 'coefficients/point_0/'
     node_path_eigenvalues = 'eigenvalues/point_0'
 
     # Retrieves eigenvalues and coefficients
     atomic_orbitals = retrieve_hdf5_data(config.path_hdf5, node_path_coefficients)
@@ -85,33 +84,34 @@
 
     # Return atomic orbitals and energies
     return atomic_orbitals, energies
 
 
 def compute_overlap_and_atomic_orbitals(
     mol: MolXYZ,
-    config: DictConfig,
-) -> Tuple[NDArray[i8], NDArray[i8], NDArray[f8]]:
+    config: _data.COOP,
+) -> tuple[NDArray[i8], NDArray[i8], NDArray[f8]]:
     """Compute the indices of the atomic orbitals of the two selected elements.
 
     Computes the overlap matrix, containing only the elements related to those two elements.
     """
     # Computing the overlap-matrix S
     overlap = compute_matrix_multipole(mol, config, 'overlap')
 
     # Computing number of spherical orbitals per atom
     sphericals = number_spherical_functions_per_atom(
         mol,
         'cp2k',
-        config["cp2k_general_settings"]["basis"],
-        config["path_hdf5"])
+        config.cp2k_general_settings.basis,
+        config.path_hdf5,
+    )
 
     # Getting the indices for the two selected elements
-    element_1 = config["coop_elements"][0]
-    element_2 = config["coop_elements"][1]
+    element_1 = config.coop_elements[0]
+    element_2 = config.coop_elements[1]
 
     element_1_index = [i for i, s in enumerate(mol) if element_1.lower() in s]
     element_2_index = [i for i, s in enumerate(mol) if element_2.lower() in s]
 
     # Making a list of the indices of the atomic orbitals for each of the two
     # elements
     atom_indices = np.zeros(len(mol) + 1, dtype=np.int64)
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/workflow_coupling.py` & `nano-qmflows-0.14.0/nanoqm/workflows/workflow_coupling.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 .. currentmodule:: nanoqm.workflows.workflow_coupling
 .. autosummary::
 
 """
 
 from __future__ import annotations
 
-__all__ = ['workflow_derivative_couplings']
-
 import os
 from os.path import join
-from typing import List, Tuple, Union
+from typing import List, Tuple, TYPE_CHECKING
 
 from noodles import gather, schedule, unpack
 from noodles.interface import PromisedObject
-from qmflows.type_hints import PathLike
 
 from .. import logger
-from ..common import DictConfig
 from ..schedule.components import calculate_mos
 from ..schedule.scheduleCoupling import (calculate_overlap, lazy_couplings,
                                          write_hamiltonians)
 from .orbitals_type import select_orbitals_type
 
+if TYPE_CHECKING:
+    from .. import _data
+
+__all__ = ['workflow_derivative_couplings']
+
 #: Type defining the derivative couplings calculation
 ResultPaths = Tuple[List[str], List[str]]
 
 
 def workflow_derivative_couplings(
-        config: DictConfig) -> Union[ResultPaths, Tuple[ResultPaths, ResultPaths]]:
+    config: _data.DerivativeCoupling
+) -> ResultPaths | tuple[ResultPaths, ResultPaths]:
     """Compute the derivative couplings for a molecular dynamic trajectory.
 
     Parameters
     ----------
     config
         Dictionary with the configuration to run the workflows
 
@@ -46,15 +48,15 @@
     ------
     Folders where the Hamiltonians are stored.
 
     """
     return select_orbitals_type(config, run_workflow_couplings)
 
 
-def run_workflow_couplings(config: DictConfig) -> PromisedObject:
+def run_workflow_couplings(config: _data.DerivativeCoupling) -> PromisedObject:
     """Run the derivative coupling workflow using `config`."""
     # compute the molecular orbitals
     logger.info("starting couplings calculation!")
     mo_paths_hdf5, energy_paths_hdf5 = unpack(calculate_mos(config), 2)
 
     # Overlap matrix at two different times
     promised_overlaps = calculate_overlap(config, mo_paths_hdf5)
@@ -66,15 +68,15 @@
     config.path_hamiltonians = create_path_hamiltonians(config.workdir, config.orbitals_type)
 
     # Inplace scheduling of write_hamiltonians function.
     # Equivalent to add @schedule on top of the function
     schedule_write_ham = schedule(write_hamiltonians)
 
     # Number of matrix computed
-    config["npoints"] = len(config.geometries) - 2
+    config.npoints = len(config.geometries) - 2
 
     # Write Hamilotians in PYXAID format
     promise_files = schedule_write_ham(
         config, promised_crossing_and_couplings, mo_paths_hdf5)
 
     return gather(promise_files, energy_paths_hdf5)
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/workflow_ipr.py` & `nano-qmflows-0.14.0/nanoqm/workflows/workflow_ipr.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,39 @@
 Index
 -----
 .. currentmodule:: nanoqm.workflows.workflow_ipr
 .. autosummary::
     workflow_ipr
 
 """
-__all__ = ['workflow_ipr']
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import numpy as np
 from scipy.linalg import sqrtm
-
 from qmflows.parsers import readXYZ
 
 from .. import logger
-from ..common import (DictConfig, h2ev, number_spherical_functions_per_atom,
-                      retrieve_hdf5_data)
+from ..common import h2ev, number_spherical_functions_per_atom, retrieve_hdf5_data
 from ..integrals.multipole_matrices import compute_matrix_multipole
 from .initialization import initialize
 from .tools import compute_single_point_eigenvalues_coefficients
 
+if TYPE_CHECKING:
+    from .. import _data
+
+__all__ = ['workflow_ipr']
+
 
-def workflow_ipr(config: DictConfig) -> np.ndarray:
+def workflow_ipr(config: _data.IPR) -> np.ndarray:
     """Compute the Inverse Participation Ratio main function."""
     # Dictionary containing the general information
-    config.update(initialize(config))
+    initialize(config)
 
     # Checking if hdf5 contains the required eigenvalues and coefficientsa
     compute_single_point_eigenvalues_coefficients(config)
 
     # Logger info
     logger.info("Starting IPR calculation.")
 
@@ -50,16 +56,17 @@
     # Converting the coeficients from AO-basis to MO-basis
     transformed_orbitals = np.dot(squared_overlap, atomic_orbitals)
 
     # Now we add up the rows of the c_MO that belong to the same atom
     sphericals = number_spherical_functions_per_atom(
         mol,
         'cp2k',
-        config.cp2k_general_settings["basis"],
-        config.path_hdf5)  # Array with number of spherical orbitals per atom
+        config.cp2k_general_settings.basis,
+        config.path_hdf5,
+    )  # Array with number of spherical orbitals per atom
 
     # New matrix with the atoms on the rows and the MOs on the columns
     indices = np.zeros(len(mol), dtype='int')
     indices[1:] = np.cumsum(sphericals[:-1])
     accumulated_transf_orbitals = np.add.reduceat(transformed_orbitals, indices, 0)
 
     # Finally, we can calculate the IPR
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/workflow_single_points.py` & `nano-qmflows-0.14.0/nanoqm/workflows/workflow_single_points.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,46 +4,49 @@
 -----
 .. currentmodule:: nanoqm.workflows.workflow_single_points
 .. autosummary::
     workflow_single_points
 
 """
 
-__all__ = ['workflow_single_points']
-
+from __future__ import annotations
 
-from typing import List
+from typing import TYPE_CHECKING
 
 from qmflows import run
-from qmflows.packages import Result
 
 from .. import logger
-from ..common import DictConfig
 from ..schedule.components import calculate_mos
 from .initialization import initialize
 
+if TYPE_CHECKING:
+    from .. import _data
+
+__all__ = ['workflow_single_points']
 
-def workflow_single_points(config: DictConfig) -> Result:
+
+def workflow_single_points(
+    config: _data.SinglePoints,
+) -> tuple[list[tuple[str, str, str]], list[str]]:
     """Perform single point calculations for a given trajectory.
 
     Parameters
     ----------
     config
         Input to run the workflow.
 
     Returns
     -------
     List with the node path to the molecular orbitals in the HDF5.
 
     """
     # Dictionary containing the general configuration
-    config.update(initialize(config))
+    initialize(config)
 
     logger.info("starting!")
 
     # compute the molecular orbitals
     # Unpack
     mo_paths_hdf5 = calculate_mos(config)
-    # Pack
-    results = run(mo_paths_hdf5, folder=config.workdir)
 
-    return results
+    # Pack
+    return tuple(run(mo_paths_hdf5, folder=config.workdir))
```

### Comparing `nano-qmflows-0.13.4/nanoqm/workflows/workflow_stddft_spectrum.py` & `nano-qmflows-0.14.0/nanoqm/workflows/workflow_stddft_spectrum.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,90 +6,95 @@
 .. autosummary::
     workflow_stddft
 
 """
 
 from __future__ import annotations
 
-__all__ = ['workflow_stddft']
-
+import copy
 import warnings
 from os.path import join
-from typing import Tuple, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
 import numpy as np
 from scipy.linalg import sqrtm
 from scipy.spatial.distance import cdist
 from noodles import gather, schedule, unpack
 from noodles.interface import PromisedObject
 from qmflows.parsers import parse_string_xyz
 from qmflows.warnings_qmflows import Orbital_Warning
-from qmflows.type_hints import PathLike
+from qmflows.common import AtomXYZ
 
+from .. import _data
 from .. import logger
-from ..common import (DictConfig, angs2au, change_mol_units, h2ev, hardness,
+from ..common import (angs2au, change_mol_units, h2ev, hardness,
                       is_data_in_hdf5, number_spherical_functions_per_atom,
                       retrieve_hdf5_data, store_arrays_in_hdf5, xc)
 from ..integrals.multipole_matrices import get_multipole_matrix
 from ..schedule.components import calculate_mos
 from .orbitals_type import select_orbitals_type
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from numpy import float64 as f8
 
+__all__ = ['workflow_stddft']
+
 
-def workflow_stddft(config: DictConfig) -> None:
+def workflow_stddft(config: _data.AbsorptionSpectrum) -> None:
     """Compute the excited states using simplified TDDFT.
 
     Both restricted and unrestricted orbitals calculations are available.
 
     Parameters
     ----------
     config
         Dictionary with the configuration to run the workflows
 
     """
     return select_orbitals_type(config, run_workflow_stddft)
 
 
-def run_workflow_stddft(config: DictConfig) -> PromisedObject:
+def run_workflow_stddft(config: _data.AbsorptionSpectrum) -> PromisedObject:
     """Compute the excited states using simplified TDDFT using `config`."""
     # Single Point calculations settings using CP2K
     mo_paths_hdf5, energy_paths_hdf5 = unpack(calculate_mos(config), 2)
 
     # Read structures
     molecules_au = [change_mol_units(parse_string_xyz(gs))
                     for i, gs in enumerate(config.geometries)
                     if (i % config.stride) == 0]
 
     # Noodles promised call
     scheduleTDDFT = schedule(compute_excited_states_tddft)
 
-    results = gather(
-        *[scheduleTDDFT(config, mo_paths_hdf5[i], DictConfig(
-            {'i': i * config.stride, 'mol': mol}))
-          for i, mol in enumerate(molecules_au)])
+    results = gather(*[
+        scheduleTDDFT(
+            config,
+            mo_paths_hdf5[i],
+            _data.AbsorptionData(i=i * config.stride, mol=mol),
+        ) for i, mol in enumerate(molecules_au)
+    ])
 
     return gather(results, energy_paths_hdf5)
 
 
 def validate_active_space(
-    config: DictConfig,
+    config: _data.AbsorptionSpectrum,
     nocc_molog: int,
     nvirt_molog: int,
 ) -> tuple[int, int]:
     """Validate and return the number of occupied and virtual MOs.
 
     The ``active_space`` keyword is treated as an upper bound by CP2K, so its values
     might be larger than the actual available number of occupied and/or virtual MOs.
 
     Parameters
     ----------
-    config : DictConfig
+    config
         The Nano-QMFlows configuration.
     nocc_molog/nvirt_molog : int
         The number of occupied and virtual orbitals as extracted from the MOLog orbital file.
 
     Returns
     -------
     tuple[int, int]
@@ -99,21 +104,21 @@
     nocc_inp = config.active_space[0]
     nvirt_inp = config.active_space[1]
 
     # Correct for the presence of SOMOs, which translates to either additional
     # occupied or unoccupied orbitals depending on the spin
     if config.orbitals_type == "alphas":
         nocc_inp += (config.multiplicity - 1)
-    elif config.orbitals_type == "beta":
+    elif config.orbitals_type == "betas":
         nvirt_inp += (config.multiplicity - 1)
 
     if (nocc_inp == nocc_molog) and (nvirt_inp == nvirt_molog):
         return nocc_inp, nvirt_inp
     else:
-        config.active_space = [nocc_molog, nvirt_molog]
+        config.active_space = (nocc_molog, nvirt_molog)
 
     # The input and MOlog file have different numbers of active and/or virtual orbitals;
     # issue a warning and return the correct number
     mo_type_list = []
     if nocc_inp > nocc_molog:
         mo_type_list.append("occupied")
     if nvirt_inp > nvirt_molog:
@@ -125,51 +130,57 @@
         f"The requested activate space is larger than the available number of {mo_type}MOs; "
         "adjusting active space", Orbital_Warning,
     )
     return nocc_molog, nvirt_molog
 
 
 def compute_excited_states_tddft(
-        config: DictConfig, path_MOs: list[str], dict_input: DictConfig) -> None:
+    config: _data.AbsorptionSpectrum,
+    path_MOs: list[str],
+    dict_input: _data.AbsorptionData,
+) -> None:
     """Compute the excited states properties (energy and coefficients).
 
     Take a given `mo_index_range`, the `tddft` method and `xc_dft` exchange functional.
     """
     logger.info("Reading energies and mo coefficients")
 
     # type of calculation
     energy, c_ao, nocc_nvirt = retrieve_hdf5_data(config.path_hdf5, path_MOs)
+    dict_input.energy = energy
+    dict_input.c_ao = c_ao
 
     # Number of virtual orbitals
     nocc, nvirt = validate_active_space(config, *nocc_nvirt)
-    dict_input.update({"energy": energy, "c_ao": c_ao,
-                       "nocc": nocc, "nvirt": nvirt})
+    dict_input.nocc = nocc
+    dict_input.nvirt = nvirt
 
     # Pass the molecule in Angstrom to the libint calculator
-    copy_dict = DictConfig(dict_input.copy())
-    copy_dict["mol"] = change_mol_units(dict_input["mol"], factor=1 / angs2au)
+    copy_dict = copy.copy(dict_input)
+    copy_dict.mol = change_mol_units(dict_input.mol, factor=1 / angs2au)
 
     # compute the multipoles if they are not stored
     multipoles = get_multipole_matrix(config, copy_dict, 'dipole')
 
     # read data from the HDF5 or calculate it on the fly
-    dict_input["overlap"] = multipoles[0]
+    dict_input.overlap = multipoles[0]
 
     # retrieve or compute the omega xia values
     omega, xia = get_omega_xia(config, dict_input)
-
-    # add arrays to the dictionary
-    dict_input.update(
-        {"multipoles": multipoles[1:], "omega": omega, "xia": xia})
+    dict_input.multipoles = multipoles[1:]
+    dict_input.omega = omega
+    dict_input.xia = xia
 
     compute_oscillator_strengths(config, dict_input)
 
 
 def get_omega_xia(
-        config: DictConfig, dict_input: DictConfig) -> Tuple[NDArray[f8], NDArray[f8]]:
+    config: _data.AbsorptionSpectrum,
+    dict_input: _data.AbsorptionData,
+) -> tuple[NDArray[f8], NDArray[f8]]:
     """Search for the multipole_matrices, Omega and xia values in the HDF5.
 
     if they are not available compute and store them.
 
     Returns
     -------
     tuple
@@ -199,39 +210,40 @@
             config.path_hdf5, paths_omega_xia[0], omega, dtype=omega.dtype)
         store_arrays_in_hdf5(
             config.path_hdf5, paths_omega_xia[1], xia, dtype=xia.dtype)
 
         return omega, xia
 
 
-def compute_sing_orb(inp: DictConfig) -> Tuple[NDArray[f8], NDArray[f8]]:
+def compute_sing_orb(inp: _data.AbsorptionData) -> tuple[NDArray[f8], NDArray[f8]]:
     """Compute the Single Orbital approximation."""
-    energy, nocc, nvirt = tuple(inp[x]for x in ("energy", "nocc", "nvirt"))
-
-    omega = energy[:nocc][..., None] - energy[nocc:][..., None].T
+    omega = inp.energy[:inp.nocc][..., None] - inp.energy[inp.nocc:][..., None].T
     xia = np.eye(omega.size)
     return -omega.ravel(), xia
 
 
 def compute_std_aproximation(
-        config: DictConfig, dict_input: DictConfig) -> Tuple[NDArray[f8], NDArray[f8]]:
+    config: _data.AbsorptionSpectrum,
+    dict_input: _data.AbsorptionData,
+) -> tuple[NDArray[f8], NDArray[f8]]:
     """Compute the oscillator strenght using either the stda or stddft approximations."""
     logger.info("Reading or computing the dipole matrices")
 
     # Make a function tha returns in transition density charges
     logger.info("Computing the transition density charges")
     # multipoles[0] is the overlap matrix
     q = transition_density_charges(
-        dict_input.mol, config, dict_input.overlap, dict_input.c_ao)
+        dict_input.mol, config, dict_input.overlap, dict_input.c_ao
+    )
 
     # Make a function that compute the Mataga-Nishimoto-Ohno_Klopman
     # damped Columb and Excgange law functions
     logger.info(
         "Computing the gamma functions for Exchange and Coulomb integrals")
-    gamma_J, gamma_K = compute_MNOK_integrals(dict_input["mol"], config.xc_dft)
+    gamma_J, gamma_K = compute_MNOK_integrals(dict_input.mol, config.xc_dft)
 
     # Compute the Couloumb and Exchange integrals
     # If xc_dft is a pure functional, ax=0, thus the pqrs_J ints are not needed
     # and can be set to 0
     logger.info("Computing the Exchange and Coulomb integrals")
     if (xc(config.xc_dft)['type'] == 'pure'):
         size = dict_input.energy.size
@@ -241,41 +253,41 @@
             q, gamma_J, axes=(0, 1)), axes=(0, 2))
     pqrs_K = np.tensordot(q, np.tensordot(
         q, gamma_K, axes=(0, 1)), axes=(0, 2))
 
     # Construct the Tamm-Dancoff matrix A for each pair of i->a transition
     logger.info("Constructing the A matrix for TDDFT calculation")
     a_mat = construct_A_matrix_tddft(
-        pqrs_J, pqrs_K, dict_input.nocc, dict_input.nvirt, config.xc_dft, dict_input.energy)
+        pqrs_J, pqrs_K, dict_input.nocc, dict_input.nvirt, config.xc_dft, dict_input.energy
+    )
 
-    if config.tddft == 'stddft':
-        logger.info('sTDDFT has not been implemented yet !')
-        # Solve the eigenvalue problem = A * cis = omega * cis
-    elif config.tddft == 'stda':
-        logger.info(
-            "This is a TDA calculation ! \n Solving the eigenvalue problem")
+    if config.tddft == 'stda':
+        logger.info("This is a TDA calculation ! \n Solving the eigenvalue problem")
         omega, xia = np.linalg.eig(a_mat)
     else:
         msg = f"The {config.tddft} method has not been implemented"
         raise NotImplementedError(msg)
+    return np.real_if_close(omega), np.real_if_close(xia)
 
-    return omega, xia
 
-
-def compute_oscillator_strengths(config: DictConfig, inp: DictConfig) -> None:
+def compute_oscillator_strengths(
+    config: _data.AbsorptionSpectrum,
+    inp: _data.AbsorptionData,
+) -> None:
     """Compute oscillator strengths.
 
     The formula can be rearranged like this:
     f_I = 2/3 * np.sqrt(2 * omega_I) * sum_ia ( np.sqrt(e_diff_ia) * xia * tdm_x) ** 2 + y^2 + z^2
     """
     tddft = config.tddft.lower()
     # 1) Get the inp.energy matrix i->a. Size: Inp.Nocc * Inp.Nvirt
     delta_ia = -np.subtract(
         inp.energy[:inp.nocc].reshape(inp.nocc, 1),
-        inp.energy[inp.nocc:].reshape(inp.nvirt, 1).T).reshape(inp.nocc * inp.nvirt)
+        inp.energy[inp.nocc:].reshape(inp.nvirt, 1).T
+    ).reshape(inp.nocc * inp.nvirt)
 
     def compute_transition_matrix(matrix):
         if tddft == 'sing_orb':
             tm = np.stack(
                 [np.sum(
                  delta_ia / inp.omega[i] * inp.xia[:, i] * matrix)
                  for i in range(inp.nocc * inp.nvirt)])
@@ -301,19 +313,20 @@
     d_x, d_y, d_z = tuple(
         compute_transition_matrix(m) for m in td_matrices)
 
     # 4) Compute the oscillator strength
     f = 2 / 3 * inp.omega * (d_x ** 2 + d_y ** 2 + d_z ** 2)
 
     # Write to output
-    inp.update({"dipole": (d_x, d_y, d_z), "oscillator": f})
+    inp.dipole = (d_x, d_y, d_z)
+    inp.oscillator = f
     write_output(config, inp)
 
 
-def write_output(config: DictConfig, inp: DictConfig) -> None:
+def write_output(config: _data.AbsorptionSpectrum, inp: _data.AbsorptionData) -> None:
     """Write the results using numpy functionality."""
     output = write_output_tddft(inp)
 
     path_output = join(config.workdir,
                        f'output_{inp.i + config.enumerate_from}_{config.tddft}.txt')
     fmt = '{:^5s}{:^14s}{:^8s}{:^11s}{:^11s}{:^11s}{:^11s}{:<5s}{:^10s}{:<5s}{:^11s}{:^11s}'
     header = fmt.format(
@@ -367,21 +380,23 @@
     cov = (xhxe - xh * xe) + (yhye - yh * ye) + (zhze - zh * ze)
     r_eh = cov / (sigma_h * sigma_e)
 
     # Compute approximate d_exc and binding energy
     omega_ab = get_omega_ab(d0I_ao, s, n_lowest, mol, config)
     r_ab = get_r_ab(mol)
 
-    d_exc_apprx = np.stack(
-        np.sqrt(np.sum(omega_ab[i, :, :] * (r_ab ** 2)) / om[i]) for i in range(n_lowest))
+    d_exc_apprx = np.stack([
+        np.sqrt(np.sum(omega_ab[i, :, :] * (r_ab ** 2)) / om[i]) for i in range(n_lowest)
+    ])
     # binding energy approximated
-    xs = np.stack((omega_ab[i, :, :] / r_ab) for i in range(n_lowest))
+    xs = np.stack([(omega_ab[i, :, :] / r_ab) for i in range(n_lowest)])
     xs[np.isinf(xs)] = 0
-    binding_en_apprx = np.stack(
-        (np.sum(xs[i, :, :]) / om[i]) for i in range(n_lowest))
+    binding_en_apprx = np.stack([
+        (np.sum(xs[i, :, :]) / om[i]) for i in range(n_lowest)
+    ])
 
     descriptors = write_output_descriptors(
         d_exc, d_exc_apprx, d_he, sigma_h, sigma_e, r_eh, binding_en_apprx, n_lowest, omega, f)
 
     return descriptors
 
 
@@ -421,20 +436,21 @@
 
 
 def get_omega_ab(d0I_ao, s, n_lowest, mol, config):
     """TODO: add Documentation."""
     # Lowdin transformation of the transition density matrix
     n_atoms = len(mol)
     s_sqrt = sqrtm(s)
-    d0I_mo = np.stack(
-        np.linalg.multi_dot([s_sqrt, d0I_ao[i, :, :], s_sqrt]) for i in range(n_lowest))
+    d0I_mo = np.stack([
+        np.linalg.multi_dot([s_sqrt, d0I_ao[i, :, :], s_sqrt]) for i in range(n_lowest)
+    ])
 
     # Compute the number of spherical functions for each atom
     n_sph_atoms = number_spherical_functions_per_atom(
-        mol, config['package_name'], config['basis_name'], config['path_hdf5'])
+        mol, config.package_name, config.basis_name, config.path_hdf5)
 
     # Compute omega_ab
     omega_ab = np.zeros((n_lowest, n_atoms, n_atoms))
     for i in range(n_lowest):
         index_a = 0
         for a in range(n_atoms):
             index_b = 0
@@ -447,43 +463,43 @@
 
     return omega_ab
 
 
 def get_exciton_positions(d0I_ao, s, moment, n_lowest, carrier):
     """TODO: add Documentation."""
     def compute_component_hole(k):
-        return np.stack(
+        return np.stack([
             np.trace(
                 np.linalg.multi_dot([d0I_ao[i, :, :].T, moment[k, :, :], d0I_ao[i, :, :], s]))
-            for i in range(n_lowest))
+            for i in range(n_lowest)])
 
     def compute_component_electron(k):
-        return np.stack(
+        return np.stack([
             np.trace(
                 np.linalg.multi_dot([d0I_ao[i, :, :].T, s, d0I_ao[i, :, :], moment[k, :, :]]))
-            for i in range(n_lowest))
+            for i in range(n_lowest)])
 
     def compute_component_he(k):
-        return np.stack(
+        return np.stack([
             np.trace(
                 np.linalg.multi_dot(
                     [d0I_ao[i, :, :].T, moment[0, :, :], d0I_ao[i, :, :], moment[0, :, :]]))
-            for i in range(n_lowest))
+            for i in range(n_lowest)])
 
     if carrier == 'hole':
         return tuple(compute_component_hole(k) for k in range(3))
     elif carrier == 'electron':
         return tuple(compute_component_electron(k) for k in range(3))
     elif carrier == 'both':
         return tuple(compute_component_he(k) for k in range(3))
     else:
         raise RuntimeError(f"unkown option: {carrier}")
 
 
-def write_output_tddft(inp: DictConfig) -> np.ndarray:
+def write_output_tddft(inp: _data.AbsorptionData) -> np.ndarray:
     """Write out as a table in plane text."""
     energy = inp.energy
 
     excs = [(i, a) for i in range(inp.nocc)
             for a in range(inp.nocc, inp.nvirt + inp.nocc)]
 
     output = np.empty((inp.nocc * inp.nvirt, 12))
@@ -524,40 +540,46 @@
     output = output[output[:, 1].argsort()]
     # Give a state number in the correct order
     output[:, 0] = np.arange(inp.nocc * inp.nvirt) + 1
 
     return output
 
 
-def transition_density_charges(mol, config, s, c_ao):
+def transition_density_charges(
+    mol: list[AtomXYZ],
+    config: _data.AbsorptionSpectrum,
+    s: NDArray[np.floating[Any]],
+    c_ao: NDArray[np.floating[Any]],
+) -> NDArray[f8]:
     """TODO: add Documentation."""
     n_atoms = len(mol)
 
     # Due to numerical noise `srtm(s)` can produce a complex array with
     # (approximately) 0-valued imaginary components; get rid of these
     sqrt_s = np.real_if_close(sqrtm(s))
     c_mo = np.dot(sqrt_s, c_ao)
 
     # Size of the transition density tensor : n_atoms x n_mos x n_mos
     q = np.zeros((n_atoms, c_mo.shape[1], c_mo.shape[1]))
     n_sph_atoms = number_spherical_functions_per_atom(
-        mol, config['package_name'], config.cp2k_general_settings['basis'], config['path_hdf5'])
+        mol, config.package_name, config.cp2k_general_settings.basis, config.path_hdf5
+    )
 
     index = 0
     for i in range(n_atoms):
         q[i, :, :] = np.dot(
             c_mo[index:(index + n_sph_atoms[i]), :].T,
             c_mo[index:(index + n_sph_atoms[i]), :],
         )
         index += n_sph_atoms[i]
 
     return q
 
 
-def compute_MNOK_integrals(mol, xc_dft):
+def compute_MNOK_integrals(mol: list[AtomXYZ], xc_dft: str) -> tuple[NDArray[f8], NDArray[f8]]:
     """TODO: add Documentation."""
     n_atoms = len(mol)
     r_ab = get_r_ab(mol)
     hardness_vec = np.stack([hardness(m[0]) for m in mol]).reshape(n_atoms, 1)
     hard = np.add(hardness_vec, hardness_vec.T)
     beta = xc(xc_dft)['beta1'] + xc(xc_dft)['ax'] * xc(xc_dft)['beta2']
     alpha = xc(xc_dft)['alpha1'] + xc(xc_dft)['ax'] * xc(xc_dft)['alpha2']
```

### Comparing `nano-qmflows-0.13.4/scripts/convert_legacy_hdf5.py` & `nano-qmflows-0.14.0/scripts/convert_legacy_hdf5.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/hamiltonians/plot_mos_energies.py` & `nano-qmflows-0.14.0/scripts/hamiltonians/plot_mos_energies.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/hamiltonians/plot_spectra.py` & `nano-qmflows-0.14.0/scripts/hamiltonians/plot_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,19 +108,17 @@
     energies = read_energies(path_hams, ts)
     couplings = read_couplings(path_hams, ts)
     # Compute the energy difference between pair of states
     d_E = energies[:, s1] - energies[:, s2]
     # Generate a matrix with s1, s2 and diff between them
     en_states = np.column_stack((energies[:, s1], energies[:, s2], d_E))
     # Compute autocorrelation function for each column (i.e. state)
-    acf = np.stack(
-        autocorrelate(en_states[:, i]) for i in range(en_states.shape[1])).transpose()
+    acf = np.stack([autocorrelate(en_states[:, i]) for i in range(en_states.shape[1])]).T
     # Compute the spectral density for each column using the normalized acf
-    sd = np.stack(
-        spectral_density(acf[:, 1, i], dt) for i in range(en_states.shape[1])).transpose()
+    sd = np.stack([spectral_density(acf[:, 1, i], dt) for i in range(en_states.shape[1])]).T
     # Compute the dephasing time for the uncorrelated acf between two states
     deph, rate = dephasing(acf[:, 0, 2], dt)
     # Plot stuff
     plot_stuff(
         en_states, couplings, acf, sd, deph, rate, s1, s2, ts, wsd, wdeph, dt)
```

### Comparing `nano-qmflows-0.13.4/scripts/pyxaid/plot_average_energy.py` & `nano-qmflows-0.14.0/scripts/pyxaid/plot_average_energy.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,26 +34,24 @@
     plt.show()
     plt.savefig(fileName, format='png', dpi=300)
 
 
 def read_energies(path, fn, nstates, nconds):
     inpfile = os.path.join(path, fn)
     cols = tuple(range(5, nstates * 2 + 5, 2))
-    xs = np.stack(np.loadtxt(f'{inpfile}{j}', usecols=cols)
-                  for j in range(nconds)).transpose()
+    xs = np.stack([np.loadtxt(f'{inpfile}{j}', usecols=cols) for j in range(nconds)]).T
     # Rows = timeframes ; Columns = states ; tensor = initial conditions
     xs = xs.swapaxes(0, 1)
     return xs
 
 
 def read_pops(path, fn, nstates, nconds):
     inpfile = os.path.join(path, fn)
     cols = tuple(range(3, nstates * 2 + 3, 2))
-    xs = np.stack(np.loadtxt(f'{inpfile}{j}', usecols=cols)
-                  for j in range(nconds)).transpose()
+    xs = np.stack([np.loadtxt(f'{inpfile}{j}', usecols=cols) for j in range(nconds)]).T
     # Rows = timeframes ; Columns = states ; tensor = initial conditions
     xs = xs.swapaxes(0, 1)
     return xs
 
 
 def main(path_output, nstates, nconds):
     outs = read_pops(path_output, 'out', nstates, nconds)
```

### Comparing `nano-qmflows-0.13.4/scripts/pyxaid/plot_cooling.py` & `nano-qmflows-0.14.0/scripts/pyxaid/plot_cooling.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,26 +35,26 @@
     interactive(True)
     plt.show()
 
     plt.figure(2)
     plt.xlabel('Time (fs)')
     plt.ylabel('Excess Energy (eV)')
     for iconds in range(nconds):
-        plt.imshow(y_grid_scaled[iconds, :, :].T, aspect='auto', extent=(0, len(ts)*dt, np.min(x_grid_scaled), np.max(x_grid_scaled)), origin='lower', interpolation='bicubic', cmap='hot')  
+        plt.imshow(y_grid_scaled[iconds, :, :].T, aspect='auto', extent=(0, len(ts)*dt, np.min(x_grid_scaled), np.max(x_grid_scaled)), origin='lower', interpolation='bicubic', cmap='hot')
     plt.plot(ts * dt, w_en_scaled, 'w')
     interactive(True)
     plt.show()
 
-    plt.figure(3) 
+    plt.figure(3)
     plt.xlabel('Time (fs)')
     plt.ylabel('State Number')
     for iconds in range(nconds):
-        plt.imshow(outs[:, :, iconds].T, aspect='auto', origin='lower', extent = ( 0, len(ts) * dt, 0, outs.shape[1]), interpolation='bicubic', cmap='hot')    
+        plt.imshow(outs[:, :, iconds].T, aspect='auto', origin='lower', extent = ( 0, len(ts) * dt, 0, outs.shape[1]), interpolation='bicubic', cmap='hot')
     interactive(True)
-    plt.show() 
+    plt.show()
 
     plt.figure(4)
     plt.xlabel('Energy (eV)')
     plt.ylabel('Counts')
     plt.hist(w_en, bins='auto')
     interactive(True)
     plt.show()
@@ -72,17 +72,17 @@
     plt.plot(ts*dt, energies[:, :, 0])
     interactive(True)
     plt.show()
 
     plt.figure(7)
     plt.ylabel('State Number')
     plt.xlabel('Freqencies cm-1')
-    sd_int = sd[:, 0, :int(sd.shape[2]/2)] 
+    sd_int = sd[:, 0, :int(sd.shape[2]/2)]
     sd_freq = sd[0, 1, :int(sd.shape[2]/2)]
-    plt.imshow(sd_int, aspect='auto', origin='lower', extent = (np.min(sd_freq), np.max(sd_freq), 0, sd_int.shape[0] ), interpolation='bicubic', cmap='hot')    
+    plt.imshow(sd_int, aspect='auto', origin='lower', extent = (np.min(sd_freq), np.max(sd_freq), 0, sd_int.shape[0] ), interpolation='bicubic', cmap='hot')
     interactive(False)
     plt.show()
 
 
 def main(path_output, nstates, nconds, dt, sigma):
     outs = read_pops_pyxaid(path_output, 'out', nstates, nconds)
     energies = read_energies_pyxaid(path_output, 'me_energies', nstates, nconds)
@@ -90,40 +90,48 @@
     # Remove the ground state and scale the energies to the lowest excitation energy
     outs = outs[:, 1:, :]
     energies = energies[:, 1:, :]
     lowest_hl_gap = np.amin(energies, axis=1)
     highest_hl_gap = np.amax(energies, axis=1)
     # Convolute a gaussian for each timestep and for each initial condition
     x_grid = np.linspace(np.min(lowest_hl_gap), np.max(highest_hl_gap), 100)
-    y_grid = np.stack(np.stack(
-        convolute(energies[time, :, iconds], outs[time, :, iconds], x_grid, sigma)
-        for time in range(energies.shape[0]) )
-        for iconds in range(nconds) )   
+    y_grid = np.stack([
+        np.stack([
+            convolute(energies[time, :, iconds], outs[time, :, iconds], x_grid, sigma)
+            for time in range(energies.shape[0])
+        ]) for iconds in range(nconds)
+    ])
     # Scale the energy for computing the excess energy plots
-    energies_scaled = np.stack(energies[:, istate, :] - lowest_hl_gap for istate in range(nstates-1)) 
-    energies_scaled = energies_scaled.swapaxes(0,1) # Just reshape to have the energies shape (time, nstates, nconds) 
+    energies_scaled = np.stack([
+        energies[:, istate, :] - lowest_hl_gap for istate in range(nstates-1)
+    ])
+    energies_scaled = energies_scaled.swapaxes(0,1) # Just reshape to have the energies shape (time, nstates, nconds)
     x_grid_scaled = np.linspace(0, np.max(energies_scaled), 100)
-    y_grid_scaled = np.stack(np.stack(
-        convolute(energies_scaled[time, :, iconds], outs[time, :, iconds], x_grid_scaled, sigma)
-        for time in range(energies_scaled.shape[0]) )
-        for iconds in range(nconds) ) 
+    y_grid_scaled = np.stack([
+        np.stack([
+            convolute(energies_scaled[time, :, iconds], outs[time, :, iconds], x_grid_scaled, sigma)
+            for time in range(energies_scaled.shape[0])
+        ]) for iconds in range(nconds)
+    ])
     # This part is done
     ##################################
     # Compute weighted energies vs population at a given time t
     eav_outs = energies * outs
     el_ene_outs = np.sum(eav_outs, axis=1)
     # Scale them to the lowest excitation energy
     ene_outs_ref0 = el_ene_outs - lowest_hl_gap
-    #Average over initial conditions 
-    ene_outs_ref0 = np.average(ene_outs_ref0, axis=1) 
-    el_ene_av = np.average(el_ene_outs, axis = 1) 
+    #Average over initial conditions
+    ene_outs_ref0 = np.average(ene_outs_ref0, axis=1)
+    el_ene_av = np.average(el_ene_outs, axis = 1)
     ##################################
-    # Compute autocorrelation function for consecutive pair of states 
-    d_en = np.stack(energies[:, istate, 0] - energies[:, istate-1, 0] for istate in range(1, nstates-1))
-    acf = np.stack(autocorrelate(d_en[istate, :]) for istate in range(d_en.shape[0]))
+    # Compute autocorrelation function for consecutive pair of states
+    d_en = np.stack(
+        [energies[:, istate, 0] - energies[:, istate-1, 0] for istate in range(1, nstates-1)]
+    )
+    acf = np.stack([autocorrelate(d_en[istate, :]) for istate in range(d_en.shape[0])])
     # Compute spectral density
     nacf = acf[:, 1, :]
     sd = np.stack(spectral_density(nacf[istate, :], dt) for istate in range(d_en.shape[0]))
     #################################
     # Call plotting function
     ts = np.arange(energies.shape[0])
     plot_stuff(x_grid, y_grid, x_grid_scaled, y_grid_scaled, sd, el_ene_av, ene_outs_ref0, nconds, outs, energies, ts, dt)
@@ -142,15 +150,15 @@
 # ============<>===============
 if __name__ == "__main__":
     msg = "plot_states_pops -p <path/to/output>\
      -nstates <number of states computed>\
       -nconds <number of initial conditions>\
       -dt <nuclear time step>\
       -sigma <line broadening for convoluton>"
-      
+
     parser = argparse.ArgumentParser(description=msg)
     parser.add_argument('-p', required=True,
                         help='path to the Hamiltonian files in Pyxaid format')
     parser.add_argument('-nstates', type=int, required=True,
                         help='Number of states')
     parser.add_argument('-nconds', type=int, required=True,
                         help='Number of initial conditions')
```

### Comparing `nano-qmflows-0.13.4/scripts/pyxaid/plot_spectra_pyxaid.py` & `nano-qmflows-0.14.0/scripts/pyxaid/plot_spectra_pyxaid.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,17 @@
     energies = np.loadtxt(inpfile, usecols=cols)
     # Compute the energy difference between pair of states
     d_E = energies[:, 0] - energies[:, 1]
     # Generate a matrix with s1, s2 and diff between them
     en_states = np.stack((energies[:, 0], energies[:, 1], d_E))
     # Compute autocorrelation function for each column (i.e. state)
     # Take the transpose to have the correct shape for spectral_density
-    acf = np.stack(autocorrelate(en_states[i, :])
-                   for i in range(en_states.shape[0])).T
+    acf = np.stack([autocorrelate(en_states[i, :]) for i in range(en_states.shape[0])]).T
     # Compute the spectral density for each column using the normalized acf
-    sd = np.stack(spectral_density(acf[:, 1, i], dt)
-                  for i in range(en_states.shape[0]))
+    sd = np.stack([spectral_density(acf[:, 1, i], dt)  for i in range(en_states.shape[0])])
     # Compute the dephasing time for the uncorrelated acf between two states
     deph, rate = dephasing(acf[:, 0, 2], dt)
     # Plot stuff
     plot_stuff(en_states, acf, sd, deph, rate, s1, s2, dt, wsd, wdeph)
 
 
 def read_cmd_line(parser):
```

### Comparing `nano-qmflows-0.13.4/scripts/pyxaid/plot_states_pops.py` & `nano-qmflows-0.14.0/scripts/pyxaid/plot_states_pops.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,22 @@
     outs_fin, pops_fin = [], []
 
     for x in outs_avg:
         if x.ndim == 1:
             outs_fin.append(x)
         else:
             outs_fin.append(np.sum(x, axis=1))
-    outs_fin = np.array(outs_fin).transpose()
+    outs_fin = np.array(outs_fin).T
 
     for x in pops_avg:
         if x.ndim == 1:
             pops_fin.append(x)
         else:
             pops_fin.append(np.sum(x, axis=1))
-    pops_fin = np.array(pops_fin).transpose()
+    pops_fin = np.array(pops_fin).T
 
     plot_stuff(outs_fin, pops_fin)
 
 
 def read_cmd_line(parser):
     """
     Parse Command line options.
```

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/convolution.py` & `nano-qmflows-0.14.0/scripts/qmflows/convolution.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/mergeHDF5.py` & `nano-qmflows-0.14.0/scripts/qmflows/mergeHDF5.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/plot_dos.py` & `nano-qmflows-0.14.0/scripts/qmflows/plot_dos.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 
 def convolute(x, y, x_points, sigma):
     # Compute gaussian prefactor
     prefactor = np.sqrt(2.0) / (sigma * np.sqrt(np.pi))
     # Convolute spectrum over grid
     y_points = prefactor * np.stack(
-        np.sum(y * g(x, x_point, sigma)) for x_point in x_points)
+        [np.sum(y * g(x, x_point, sigma)) for x_point in x_points]
+    )
     return y_points
 
 
 def plot_stuff(ys, energies, legends, emin, emax):
     # In case you need more colors, this list should be expanded
     colors = ['black', 'orange', 'blue', 'red',
               'green', 'magenta', 'cyan', 'black', 'yellow']
@@ -62,19 +63,17 @@
     interactive(True)
     plt.show()
 
 #   Prepare the cumulative density of states
     sigma = 0.2
     x_points = np.linspace(energies[0], energies[-1], 1000)
     # Take transpose to have it in (x_points, # dos) format
-    dos = np.stack(convolute(
-        energies, ys[:, i], x_points, sigma) for i in range(ys.shape[1])).T
+    dos = np.stack([convolute(energies, ys[:, i], x_points, sigma) for i in range(ys.shape[1])]).T
     # Cumulate dos for all atoms/ligands
-    cum_dos = np.stack(np.sum(dos[:, 0:i+1], axis=1)
-                       for i in range(dos.shape[1])).T
+    cum_dos = np.stack([np.sum(dos[:, 0:i+1], axis=1) for i in range(dos.shape[1])]).T
     #   Plotting now
     plt.figure(2)
     ref = np.zeros(x_points.size)
     # Add a zero line for filling colors
     cum_dos = np.column_stack((ref, cum_dos))
     plt.xlim(emin, emax)
     max_y_plot = np.amax(
@@ -106,16 +105,15 @@
     homo_indx = lumo_indx - 1
     hl_gap = (energies[lumo_indx] - energies[homo_indx])
     logger.info(f'The homo-lumo gap is: {hl_gap} eV')
 
     # Read Files with PDOS info
     xs = [np.loadtxt(files[i]) for i in range(len(files))]
     # Add up all orbitals contribution for each atom type
-    ys = np.stack(np.sum(xs[i][:, 3:], axis=1)
-                  for i in range(len(files))).transpose()
+    ys = np.stack([np.sum(xs[i][:, 3:], axis=1) for i in range(len(files))]).T
 
     if group:
         lig_atoms = 0
         lig_name = ''
         for i in range(len(group)):
             lig_atoms += ys[:, group[i]-1]
             lig_name += legends[group[i]-1]
```

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/rdf.py` & `nano-qmflows-0.14.0/scripts/qmflows/rdf.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/removeHDF5folders.py` & `nano-qmflows-0.14.0/scripts/qmflows/removeHDF5folders.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/scripts/qmflows/remove_mos_hdf5.py` & `nano-qmflows-0.14.0/scripts/qmflows/remove_mos_hdf5.py`

 * *Files identical despite different names*

### Comparing `nano-qmflows-0.13.4/setup.cfg` & `nano-qmflows-0.14.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [coverage:run]
 branch = True
 source = nanoqm
 
-[pycodestyle]
-ignore = E302,E301,E501,W504  # E302 & E301 due pycodestyle's awful support for @overload
+[flake8]
 max-line-length = 100
+per-file-ignores = 
+	nanoqm/workflows/input_validation.py: E704,E501
+	nanoqm/analysis/tools.py: F821
 
 [tool:pytest]
 testpaths = test
 addopts = --tb=short --cov --cov-report xml --cov-report term --cov-report html --cache-clear --pdbcls=IPython.terminal.debugger:TerminalPdb --durations=6
 markers = slow: A marker for slow tests requiring external quantum-chemical packages.
 filterwarnings = 
 	error::qmflows.warnings_qmflows.QMFlows_Warning
```

### Comparing `nano-qmflows-0.13.4/setup.py` & `nano-qmflows-0.14.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Installation recipe."""
 
 import os
 import sys
+import platform
 from os.path import join
 
-import setuptools
+import setuptools  # noqa: F401
+import pkg_resources
 import numpy as np
 from setuptools import Extension, find_packages, setup
 from setuptools.command.build_ext import build_ext
 from wheel.bdist_wheel import bdist_wheel
 
 here = os.path.abspath(os.path.dirname(__file__))
 
@@ -19,28 +21,40 @@
 
 def readme() -> str:
     """Load readme."""
     with open('README.rst', 'r', encoding='utf8') as f:
         return f.read()
 
 
+def is_macos_arm64() -> bool:
+    """Return whether nano-qmflows is being (cross) compiled for macosx_arm64."""
+    if sys.platform != "darwin":
+        return False
+    return "arm64" in os.environ.get("CIBW_ARCHS_MACOS", "") or platform.machine() == "arm64"
+
+
 class BuildExt(build_ext):
     """A custom build extension for adding compiler-specific options."""
 
     c_opts: "dict[str, list[str]]" = {
         'msvc': ['/EHsc'],
         'unix': ['-Wall'],
     }
     l_opts: "dict[str, list[str]]" = {
         'msvc': [],
         'unix': ['-Wall'],
     }
 
     if sys.platform == 'darwin':
-        darwin_opts = ['-stdlib=libc++', '-mmacosx-version-min=10.14', '-fno-sized-deallocation']
+        min_version = "11" if is_macos_arm64() else "10.14"
+        darwin_opts = [
+            '-stdlib=libc++',
+            '-mmacosx-version-min={}'.format(min_version),
+            '-fno-sized-deallocation',
+        ]
         c_opts['unix'] += darwin_opts
         l_opts['unix'] += darwin_opts
 
     def build_extensions(self) -> None:
         """Actual compilation."""
         ct = self.compiler.compiler_type
         opts = self.c_opts.get(ct, [])
@@ -56,29 +70,24 @@
 class BDistWheelABI3(bdist_wheel):
     """Ensure that wheels are built with the ``abi3`` tag."""
 
     def get_tag(self) -> "tuple[str, str, str]":
         python, abi, plat = super().get_tag()
 
         if python.startswith("cp"):
-            # on CPython, our wheels are abi3 and compatible back to 3.7
-            return "cp37", "abi3", plat
+            # on CPython, our wheels are abi3 and compatible back to 3.8
+            return "cp38", "abi3", plat
         else:
             return python, abi, plat
 
 
 def parse_requirements(path: "str | os.PathLike[str]") -> "list[str]":
-    """Parse a ``requirements.txt`` file and strip all empty and commented lines."""
-    ret = []
+    """Parse a ``requirements.txt`` file."""
     with open(path, "r", encoding="utf8") as f:
-        for i in f:
-            j = i.split("#", 1)[0].strip().rstrip()
-            if j:
-                ret.append(j)
-    return ret
+        return [str(i) for i in pkg_resources.parse_requirements(f)]
 
 
 def get_paths() -> "tuple[list[str], list[str]]":
     """Get the paths specified in the ``QMFLOWS_INCLUDEDIR`` and ``QMFLOWS_LIBDIR`` \
     environment variables.
 
     If not specified if specified use ``CONDA_PREFIX`` instead.
@@ -125,15 +134,15 @@
         )
     return include_list, lib_list
 
 
 include_list, lib_list = get_paths()
 libint_ext = Extension(
     'nanoqm.compute_integrals',
-    sources=['libint/compute_integrals.cc'],
+    sources=['libint/compute_integrals.cc', 'libint/py_compute_integrals.cc'],
     include_dirs=[
         "libint/include",
         *include_list,
         np.get_include(),
     ],
     libraries=['hdf5', 'int2'],
     library_dirs=lib_list,
@@ -159,27 +168,27 @@
         'Natural Language :: English',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: C++',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Typing :: Typed',
     ],
     install_requires=parse_requirements("install_requirements.txt"),
     cmdclass={'build_ext': BuildExt, "bdist_wheel": BDistWheelABI3},
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     ext_modules=[libint_ext],
     extras_require={
         'test': parse_requirements("test_requirements.txt"),
         'doc': parse_requirements("doc_requirements.txt"),
         'lint': parse_requirements("linting_requirements.txt"),
     },
     package_data={
```

