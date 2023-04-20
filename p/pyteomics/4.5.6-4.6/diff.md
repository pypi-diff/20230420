# Comparing `tmp/pyteomics-4.5.6.tar.gz` & `tmp/pyteomics-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteomics-4.5.6.tar", last modified: Mon Oct 31 21:38:50 2022, max compression
+gzip compressed data, was "pyteomics-4.6.tar", last modified: Thu Apr 20 15:47:38 2023, max compression
```

## Comparing `pyteomics-4.5.6.tar` & `pyteomics-4.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-31 21:38:43.000000 pyteomics-4.5.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-10-31 21:38:43.000000 pyteomics-4.5.6/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    10173 2022-10-31 21:38:43.000000 pyteomics-4.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-31 21:38:43.000000 pyteomics-4.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-31 21:38:43.000000 pyteomics-4.5.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     4666 2022-10-31 21:38:50.807354 pyteomics-4.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-10-31 21:38:43.000000 pyteomics-4.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/pyteomics/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24735 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/_schema_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)    47949 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/achrom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/pyteomics/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    83715 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    40675 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/math.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)    15295 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    41484 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/target_decoy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7113 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/auxiliary/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/electrochem.py
--rw-r--r--   0 runner    (1001) docker     (121)    36267 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/fasta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/pyteomics/mass/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49353 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mass/mass.py
--rw-r--r--   0 runner    (1001) docker     (121)    25502 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mass/unimod.py
--rw-r--r--   0 runner    (1001) docker     (121)    29338 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mgf.py
--rw-r--r--   0 runner    (1001) docker     (121)    16255 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/ms1.py
--rw-r--r--   0 runner    (1001) docker     (121)     7121 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/ms2.py
--rw-r--r--   0 runner    (1001) docker     (121)    17527 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mzid.py
--rw-r--r--   0 runner    (1001) docker     (121)    20319 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mzml.py
--rw-r--r--   0 runner    (1001) docker     (121)    19931 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mzmlb.py
--rw-r--r--   0 runner    (1001) docker     (121)    28522 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mztab.py
--rw-r--r--   0 runner    (1001) docker     (121)    11821 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/mzxml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/pyteomics/openms/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/openms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/openms/featurexml.py
--rw-r--r--   0 runner    (1001) docker     (121)    15906 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/openms/idxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/openms/trafoxml.py
--rw-r--r--   0 runner    (1001) docker     (121)    41487 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9204 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/peff.py
--rw-r--r--   0 runner    (1001) docker     (121)    24099 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/pepxml.py
--rw-r--r--   0 runner    (1001) docker     (121)    75016 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/proforma.py
--rw-r--r--   0 runner    (1001) docker     (121)    11255 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/protxml.py
--rw-r--r--   0 runner    (1001) docker     (121)    33492 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/pylab_aux.py
--rw-r--r--   0 runner    (1001) docker     (121)    13835 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/tandem.py
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/traml.py
--rw-r--r--   0 runner    (1001) docker     (121)    17738 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/usi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    48714 2022-10-31 21:38:43.000000 pyteomics-4.5.6/pyteomics/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:38:50.807354 pyteomics-4.5.6/pyteomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4666 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-31 21:38:50.000000 pyteomics-4.5.6/pyteomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 21:38:50.807354 pyteomics-4.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-10-31 21:38:43.000000 pyteomics-4.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 15:47:27.000000 pyteomics-4.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-20 15:47:27.000000 pyteomics-4.6/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-20 15:47:27.000000 pyteomics-4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 15:47:27.000000 pyteomics-4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-20 15:47:27.000000 pyteomics-4.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-20 15:47:38.830234 pyteomics-4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 15:47:27.000000 pyteomics-4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/pyteomics/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24735 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/_schema_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47949 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/achrom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/pyteomics/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83715 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40314 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41484 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/target_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/auxiliary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/electrochem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/fasta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/pyteomics/mass/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49128 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mass/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25502 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mass/unimod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33178 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/ms1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/ms2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mzid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mzml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mzmlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mztab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/mzxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/pyteomics/openms/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/openms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/openms/featurexml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/openms/idxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/openms/trafoxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41487 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/peff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24099 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/pepxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77062 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/proforma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/protxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33492 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/pylab_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/tandem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/traml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/usi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48203 2023-04-20 15:47:27.000000 pyteomics-4.6/pyteomics/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:47:38.830234 pyteomics-4.6/pyteomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 15:47:38.000000 pyteomics-4.6/pyteomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:47:38.830234 pyteomics-4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-20 15:47:27.000000 pyteomics-4.6/setup.py
```

### Comparing `pyteomics-4.5.6/AUTHORS` & `pyteomics-4.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/LICENSE` & `pyteomics-4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/NOTICE` & `pyteomics-4.6/NOTICE`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/README.rst` & `pyteomics-4.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,18 @@
    :target: https://github.com/levitsky/pyteomics/actions?query=workflow%3Atests
    :alt: Test status
 
 .. image:: https://img.shields.io/pypi/v/pyteomics.svg
     :target: https://pypi.org/project/pyteomics/
     :alt: PyPI
 
+.. image:: https://img.shields.io/conda/vn/bioconda/pyteomics
+    :target: http://bioconda.github.io/recipes/pyteomics/README.html
+    :alt: conda
+
 .. image:: https://img.shields.io/readthedocs/pyteomics.svg
     :target: https://pyteomics.readthedocs.io/
     :alt: Read the Docs (latest)
 
 .. image:: https://img.shields.io/github/license/levitsky/pyteomics
     :target: https://www.apache.org/licenses/LICENSE-2.0
     :alt: Apache License
```

### Comparing `pyteomics-4.5.6/pyteomics/__init__.py` & `pyteomics-4.6/pyteomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/_schema_defaults.py` & `pyteomics-4.6/pyteomics/_schema_defaults.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/achrom.py` & `pyteomics-4.6/pyteomics/achrom.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/__init__.py` & `pyteomics-4.6/pyteomics/auxiliary/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     _calculate_qvalues, _qvalues_df, _decoy_or_pep_label,
     _construct_dtype, _make_qvalues, _make_filter,
     _itercontext, _iter, qvalues, filter, log_factorial,
     _expectation, _confidence_value, _log_pi_r,
     _log_pi, _make_fdr, fdr, sigma_T, sigma_fdr)
 
 from .utils import (
-    print_tree, memoize, BinaryDataArrayTransformer,
-    _decode_base64_data_array)
+    print_tree, memoize, BinaryDataArrayTransformer, ArrayConversionMixin, BinaryArrayConversionMixin,
+    MaskedArrayConversionMixin, _decode_base64_data_array)
```

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/constants.py` & `pyteomics-4.6/pyteomics/auxiliary/constants.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/file_helpers.py` & `pyteomics-4.6/pyteomics/auxiliary/file_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,36 +389,42 @@
     """Abstract class for text file readers that keep an index of records for random access.
     This requires reading the file in binary mode."""
 
     delimiter = None
     label = None
     block_size = 1000000
     label_group = 1
+    _kw_keys = ['delimiter', 'label', 'block_size', 'label_group']
 
     def __init__(self, source, **kwargs):
         # the underlying _file_obj gets None as encoding
         # to avoid transparent decoding of StreamReader on read() calls
         encoding = kwargs.pop('encoding', 'utf-8')
         super(IndexedTextReader, self).__init__(source, mode='rb', encoding=None, **kwargs)
         self.encoding = encoding
-        for attr in ['delimiter', 'label', 'block_size', 'label_group']:
+        for attr in self._kw_keys:
             if attr in kwargs:
                 setattr(self, attr, kwargs.pop(attr))
         self._offset_index = None
         if not kwargs.pop('_skip_index', False):
             self._offset_index = self.build_byte_index()
 
     def __getstate__(self):
         state = super(IndexedTextReader, self).__getstate__()
         state['offset_index'] = self._offset_index
+        for key in self._kw_keys:
+            state[key] = getattr(self, key)
         return state
 
     def __setstate__(self, state):
         super(IndexedTextReader, self).__setstate__(state)
         self._offset_index = state['offset_index']
+        for key in self._kw_keys:
+            if key in state:
+                setattr(self, key, state[key])
 
     def _chunk_iterator(self):
         fh = self._source.file
         delim = remove_bom(self.delimiter.encode(self.encoding))
         buff = fh.read(self.block_size)
         parts = buff.split(delim)
         started_with_delim = buff.startswith(delim)
@@ -566,38 +572,27 @@
                     encoding=kwargs.pop('encoding', None))
             source = kwargs.pop('source', None)
             return FileReader(source, mode=_mode, parser_func=_func, pass_file=True, args=(), kwargs=kwargs, encoding=kwargs.pop('encoding', None))
         return helper
     return decorator
 
 
-def _file_writer(_mode='a'):
+def _file_writer(_mode='w'):
     def decorator(_func):
         """A decorator that opens output files for writer functions.
         """
         @wraps(_func)
         def helper(*args, **kwargs):
-            if 'file_mode' in kwargs:
-                m = kwargs.pop('file_mode')
-                warn = False
-            else:
-                m = _mode
-                warn = True
+            m = kwargs.pop('file_mode', _mode)
             enc = kwargs.pop('encoding', None)
             if len(args) > 1:
                 out_arg = args[1]
             else:
                 out_arg = kwargs.pop('output', None)
 
-            # warn about the change in default mode if an existing file name is given
-            if isinstance(out_arg, basestring) and warn and os.path.exists(out_arg):
-                warnings.warn("Opening an existing file in append mode. "
-                    "The default mode will change from 'a' to 'w' in a future version. "
-                    "Pass `file_mode='a'` to keep old behavior and suppress this warning.", FutureWarning)
-
             with _file_obj(out_arg, m, encoding=enc) as out:
                 if len(args) > 1:
                     call_args = (args[0], out) + args[2:]
                     call_kwargs = kwargs
                 else:
                     call_args = args
                     call_kwargs = dict(output=out, **kwargs)
```

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/math.py` & `pyteomics-4.6/pyteomics/auxiliary/math.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/structures.py` & `pyteomics-4.6/pyteomics/auxiliary/structures.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/auxiliary/target_decoy.py` & `pyteomics-4.6/pyteomics/auxiliary/target_decoy.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/electrochem.py` & `pyteomics-4.6/pyteomics/electrochem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/fasta.py` & `pyteomics-4.6/pyteomics/fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,19 @@
         except KeyError:
             if self._id2header:
                 header = self._id2header.get(key)
                 if header is not None:
                     return super(TwoLayerIndexedFASTA, self).get_entry(header)
         raise KeyError(key)
 
+    def get_header(self, key):
+        if key in self._id2header:
+            return self._id2header[key]
+        raise KeyError(key)
+
     def __contains__(self, key):
         return super(TwoLayerIndexedFASTA, self).__contains__(key) or key in self._id2header
 
 
 class FlavoredMixin():
     """Parser aimed at a specific FASTA flavor.
     Subclasses should define `parser` and `header_pattern`.
@@ -398,24 +403,24 @@
     """
     def __init__(self, parse=True):
         if not parse:
             self.parser = None
 
 
 class UniProtMixin(FlavoredMixin):
-    header_pattern = r'^(\w+)\|([-\w]+)\|(\w+)\s+([^=]*\S)((\s+\w+=[^=]+(?!\w*=))+)\s*$'
-    header_group = 2
+    header_pattern = r'^(?P<db>\w+)\|(?P<id>[-\w]+)\|(?P<entry>\w+)\s+(?P<name>.*?)(?:(\s+OS=(?P<OS>[^=]+))|(\s+OX=(?P<OX>\d+))|(\s+GN=(?P<GN>\S+))|(\s+PE=(?P<PE>\d))|(\s+SV=(?P<SV>\d+)))*\s*$'
+    header_group = 'id'
 
     def parser(self, header):
-        db, ID, entry, name, pairs, _ = re.match(self.header_pattern, header).groups()
-        gid, taxon = entry.split('_')
-        info = {'db': db, 'id': ID, 'entry': entry,
-                'name': name, 'gene_id': gid, 'taxon': taxon}
-        info.update(_split_pairs(pairs))
-        _intify(info, ('PE', 'SV'))
+        info = re.match(self.header_pattern, header).groupdict()
+        for key in ['OS', 'OX', 'GN', 'PE', 'SV']:
+            if info[key] is None:
+                del info[key]
+        info['gene_id'], info['taxon'] = info['entry'].split('_')
+        _intify(info, ('PE', 'SV', 'OX'))
         return info
 
 
 def _add_init(cls):
     """Add an __init__ method to a flavored parser class,
     which simply calls __init__ of its two bases."""
     flavor, typ = cls.__bases__
@@ -452,24 +457,23 @@
 
 @_add_init
 class IndexedUniProt(UniProtMixin, TwoLayerIndexedFASTA):
     pass
 
 
 class UniRefMixin(FlavoredMixin):
-    header_pattern = r'^(\S+)\s+([^=]*\S)((\s+\w+=[^=]+(?!\w*=))+)\s*$'
+    header_pattern = r'^(?P<id>\S+)\s+(?P<cluster>.*?)(?:(\s+n=(?P<n>\d+))|(\s+Tax=(?P<Tax>.+?))|(\s+TaxID=(?P<TaxID>\S+))|(\s+RepID=(?P<RepID>\S+)))*\s*$'
+    header_group = 'id'
 
     def parser(self, header):
         assert 'Tax' in header
-        ID, cluster, pairs, _ = re.match(self.header_pattern, header).groups()
-        info = {'id': ID, 'cluster': cluster}
-        info.update(_split_pairs(pairs))
-        gid, taxon = info['RepID'].split('_')
-        type_, acc = ID.split('_')
-        info.update({'taxon': taxon, 'gene_id': gid, 'type': type_, 'accession': acc})
+        info = re.match(self.header_pattern, header).groupdict()
+        for key in ['TaxID', 'Tax', 'RepID', 'n']:
+            if info[key] is None:
+                del info[key]
         _intify(info, ('n',))
         return info
 
 
 @_add_init
 class UniRef(UniRefMixin, FASTA):
     pass
@@ -617,19 +621,27 @@
 
     Parameters
     ----------
     entries : iterable of (str, str) tuples
         An iterable of 2-tuples in the form (description, sequence).
     output : file-like or str, optional
         A file open for writing or a path to write to. If the file exists,
-        it will be opened for appending. Default is :py:const:`None`, which
+        it will be opened for writing. Default is :py:const:`None`, which
         means write to standard output.
+
+        .. note::
+            The default mode for output files specified by name has been changed
+            from `a` to `w` in *pyteomics 4.6*. See `file_mode` to override the mode.
+
     file_mode : str, keyword only, optional
         If `output` is a file name, defines the mode the file will be opened in.
-        Otherwise will be ignored. Default is 'a'.
+        Otherwise will be ignored. Default is `'w'`.
+
+        .. note ::
+            The default changed from `'a'` in *pyteomics 4.6*.
 
     Returns
     -------
     output_file : file object
         The file where the FASTA is written.
     """
     for descr, seq in entries:
@@ -694,46 +706,46 @@
     decoy_sequence : str
         The decoy sequence.
     """
 
     # empty sequence
     if len(sequence) == 0:
         return ''
-    
+
     # presereve the first position
     if (keep_nterm_M and sequence[0] == 'M') or keep_nterm:
-        return sequence[0] + shuffle(sequence[1:], keep_cterm=keep_cterm, 
+        return sequence[0] + shuffle(sequence[1:], keep_cterm=keep_cterm,
                        fix_aa=fix_aa)
-    
+
     # presereve the last position
     if keep_cterm:
         return shuffle(sequence[:-1], fix_aa=fix_aa) + sequence[-1]
-    
-    
+
+
     if not isinstance(fix_aa, str):
         fix_aa = ''.join(fix_aa)
-    
+
     fixed = []
     position = 0
     if len(fix_aa) > 0:  # non-empty fixed list
         shuffled = []
         for match in re.finditer(r'[{}]'.format(fix_aa), sequence):
             fixed.append((match.start(), sequence[match.start()]))
             shuffled.extend(sequence[position:match.start()])
             position = match.end()
         shuffled.extend(sequence[position:])
-        
+
     else:  # shuffle everything
         shuffled = list(sequence)
-    
+
     random.shuffle(shuffled)
-    
+
     for fix in fixed:
         shuffled.insert(fix[0], fix[1])
-    
+
     return ''.join(shuffled)
 
 
 def fused_decoy(sequence, decoy_mode='reverse', sep='R', **kwargs):
     """
     Create a "fused" decoy sequence by concatenating a decoy sequence with the original one.
     The method and its use cases are described in:
```

### Comparing `pyteomics-4.5.6/pyteomics/mass/mass.py` & `pyteomics-4.6/pyteomics/mass/mass.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,31 +404,32 @@
         ion_comp : dict, optional
             A dict with the relative elemental compositions of peptide ion
             fragments (default is :py:data:`std_ion_comp`).
         ion_type : str, optional
             If specified, then the polypeptide is considered to be in the form
             of the corresponding ion. Do not forget to specify the charge state!
         absolute : bool, optional
-            If :py:const:`True`, the m/z value returned will always be positive,
+            If :py:const:`True` (default), the m/z value returned will always be positive,
             even for negatively charged ions.
 
-            .. warning::
-                Default is :py:const:`False` now, but will be changed in a future version.
+            .. note ::
+                `absolute` only applies when `charge` is negative.
+                The mass can still be negative for negative compositions.
 
         Returns
         -------
         mass : float
         """
         composition = self
         mass_data = kwargs.get('mass_data', nist_mass)
 
         # Calculate mass
         mass = 0.0
         average = kwargs.get('average', False)
-        absolute = kwargs.get('absolute')
+        absolute = kwargs.get('absolute', True)
 
         for isotope_string, amount in composition.items():
             element_name, isotope_num = _parse_isotope_string(isotope_string)
             # Calculate average mass if required and the isotope number is
             # not specified.
             if (not isotope_num) and average:
                 for isotope, data in mass_data[element_name].items():
@@ -467,18 +468,15 @@
         if charge and composition['H+']:
             raise PyteomicsError('Composition contains protons and charge is explicitly specified.')
         if charge is None and composition['H+']:
             warnings.warn('Charge is not specified, but the Composition contains protons. Assuming m/z calculation.')
             charge = composition['H+']
         if charge:
             mass /= charge
-        if mass < 0 and absolute is None:
-            warnings.warn('Returning a signed value. The default will change in the future.'
-                ' Specify `absolute` kwarg to suppress this warning', FutureWarning)
-        if absolute:
+        if charge and charge < 0 and absolute:
             mass = abs(mass)
         return mass
 
 
 std_aa_comp.update({
     'A':   Composition({'H': 5, 'C': 3, 'O': 1, 'N': 1}),
     'C':   Composition({'H': 5, 'C': 3, 'S': 1, 'O': 1, 'N': 1}),
@@ -611,34 +609,34 @@
     ion_comp : dict, optional
         A dict with the relative elemental compositions of peptide ion
         fragments (default is :py:data:`std_ion_comp`).
     ion_type : str, optional
         If specified, then the polypeptide is considered to be in the form
         of the corresponding ion. Do not forget to specify the charge state!
     absolute : bool, optional
-            If :py:const:`True`, the m/z value returned will always be positive,
-            even for negatively charged ions.
+        If :py:const:`True` (default), the m/z value returned will always be positive,
+        even for negatively charged ions.
 
-            .. warning::
-                Default is :py:const:`False` now, but will be changed in a future version.
+        .. note ::
+            `absolute` only applies when `charge` is negative.
+            The mass can still be negative for negative compositions.
 
     Returns
     -------
     mass : float
     """
-    # These parameters must not be passed to mass(), not __init__
-    charge = kwargs.pop('charge', None)
-    charge_carrier = kwargs.pop('charge_carrier', None)
-    carrier_charge = kwargs.pop('carrier_charge', None)
-    absolute = kwargs.pop('absolute', None)
+    # These parameters must be passed to mass(), not __init__
+    mass_kw = {}
+    for k in ['charge', 'charge_carrier', 'carrier_charge', 'absolute']:
+        if k in kwargs:
+            mass_kw[k] = kwargs.pop(k)
     # Make a copy of `composition` keyword argument.
     composition = (Composition(kwargs['composition']) if 'composition' in kwargs else Composition(*args, **kwargs))
-    return composition.mass(
-        charge=charge, charge_carrier=charge_carrier, carrier_charge=carrier_charge,
-        absolute=absolute, **kwargs)
+    kwargs.update(mass_kw)
+    return composition.mass(**kwargs)
 
 
 def most_probable_isotopic_composition(*args, **kwargs):
     """Calculate the most probable isotopic composition of a peptide
     molecule/ion defined by a sequence string, parsed sequence,
     chemical formula or :py:class:`Composition` object.
```

### Comparing `pyteomics-4.5.6/pyteomics/mass/unimod.py` & `pyteomics-4.6/pyteomics/mass/unimod.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/mgf.py` & `pyteomics-4.6/pyteomics/mgf.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
   :py:class:`MGFBase` - abstract class, the common ancestor of the two classes above.
   Can be used for type checking.
 
 Functions
 ---------
 
-  :py:func:`read` - iterate through spectra in MGF file. Data from a
-  single spectrum are converted to a human-readable dict.
+  :py:func:`read` - an alias for :py:class:`MGF` or :py:class:`IndexedMGF`.
 
   :py:func:`get_spectrum` - read a single spectrum with given title from a file.
 
   :py:func:`chain` - read multiple files at once.
 
   :py:func:`chain.from_iterable` - read multiple files at once, using an
   iterable of files.
@@ -69,29 +68,21 @@
 
 try:
     import numpy as np
 except ImportError:
     np = None
 import itertools as it
 import sys
+import warnings
 from . import auxiliary as aux
 
 
-class MGFBase(object):
+class MGFBase(aux.MaskedArrayConversionMixin):
     """Abstract mixin class representing an MGF file. Subclasses implement different approaches to parsing."""
     _comments = set('#;!/')
-    _array = (lambda x, dtype: np.array(x, dtype=dtype)) if np is not None else None
-    _ma = (lambda x, dtype: np.ma.masked_equal(np.array(x, dtype=dtype), 0)) if np is not None else None
-    _identity = lambda x, **kw: x
-    _array_converters = {
-        'm/z array': [_identity, _array, _array],
-        'intensity array': [_identity, _array, _array],
-        'charge array': [_identity, _array, _ma],
-        'ion array': [_identity, _array,  _array]
-    }
     _array_keys = ['m/z array', 'intensity array', 'charge array', 'ion array']
     _array_keys_unicode = [u'm/z array', u'intensity array', u'charge array', u'ion array']
     encoding = None
 
     def __init__(self, source=None, **kwargs):
         """Create an MGF file object, set MGF-specific parameters.
 
@@ -104,15 +95,15 @@
 
         use_header : bool, optional, keyword only
             Add the info from file header to each dict. Spectrum-specific parameters
             override those from the header in case of conflict.
             Default is :py:const:`True`.
 
         convert_arrays : one of {0, 1, 2}, optional, keyword only
-            If `0`, m/z, intensities and (possibly) charges or (possibly) ions will be returned as regular lists
+            If `0`, m/z, intensities and (possibly) charges or (possibly) ions will be returned as regular lists.
             If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
             If `2`, charges will be reported as a masked array (default).
             The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
 
         read_charges : bool, optional, keyword only
             If `True` (default), fragment charges are reported. Disabling it improves performance.
 
@@ -126,29 +117,38 @@
 
         encoding : str, optional, keyword only
             File encoding.
         """
 
         super(MGFBase, self).__init__(source, **kwargs)
         self._use_header = kwargs.pop('use_header', True)
-        self._convert_arrays = kwargs.pop('convert_arrays', 2)
-        if self._convert_arrays and np is None:
-            raise aux.PyteomicsError('numpy is required for array conversion')
         self._read_charges = kwargs.pop('read_charges', True)
         self._read_ions = kwargs.pop('read_ions', False)
         # Make sure no charges are read if ions are read
         if self._read_ions:
             self._read_charges = False
-        dtype = kwargs.pop('dtype', None)
-        self._dtype_dict = dtype if isinstance(dtype, dict) else {k: dtype for k in self._array_keys}
         if self._use_header:
             self._read_header()
         else:
             self._header = None
 
+    def __reduce_ex__(self, protocol):
+        return (self.__class__, (self._source_init,), self.__getstate__())
+
+    def __getstate__(self):
+        state = super(MGFBase, self).__getstate__()
+        state['use_header'] = self._use_header
+        state['header'] = self._header
+        return state
+
+    def __setstate__(self, state):
+        super(MGFBase, self).__setstate__(state)
+        self._header = state['header']
+        self._use_header = state['use_header']
+
     @staticmethod
     def parse_precursor_charge(charge_text, list_only=False):
         return aux._parse_charge(charge_text, list_only=list_only)
 
     @staticmethod
     def parse_peak_charge(charge_text, list_only=False):
         return aux._parse_charge(charge_text, list_only=False)
@@ -210,22 +210,20 @@
                                 'PEPMASS = {}'.format(params['pepmass']))
                     else:
                         params['pepmass'] = pepmass + (None,) * (2-len(pepmass))
                 if isinstance(params.get('charge'), aux.basestring):
                     params['charge'] = self.parse_precursor_charge(params['charge'], True)
                 if 'rtinseconds' in params:
                     params['rtinseconds'] = aux.unitfloat(params['rtinseconds'], 'second')
-                out = {'params': params}
-                data = {'m/z array': masses, 'intensity array': intensities}
+                out = {'params': params, 'm/z array': masses, 'intensity array': intensities}
                 if self._read_charges:
-                    data['charge array'] = charges
+                    out['charge array'] = charges
                 if self._read_ions:
-                    data['ion array'] = ions
-                for key, values in data.items():
-                    out[key] = self._array_converters[key][self._convert_arrays](values, dtype=self._dtype_dict.get(key))
+                    out['ion array'] = ions
+                self._build_all_arrays(out)
                 if self.encoding and sys.version_info.major == 2:
                     for key, ukey in zip(self._array_keys + ['params'], self._array_keys_unicode + [u'params']):
                         if key in out:
                             out[ukey] = out.pop(key)
                 return out
 
             else:
@@ -269,53 +267,87 @@
     'intensity array', 'charge array', 'ion array' and 'params'. 'm/z array' and
     'intensity array' store :py:class:`numpy.ndarray`'s of floats,
     'charge array' is a masked array (:py:class:`numpy.ma.MaskedArray`) of ints,
     'ion_array' is an array of Ions (str)
     and 'params' stores a :py:class:`dict` of parameters (keys and values are
     :py:class:`str`, keys corresponding to MGF, lowercased).
 
-
     Attributes
     ----------
 
     header : dict
         The file header.
     time : RTLocator
         A property used for accessing spectra by retention time.
     """
     delimiter = 'BEGIN IONS'
 
     def __init__(self, source=None, use_header=True, convert_arrays=2, read_charges=True,
                  dtype=None, encoding='utf-8', index_by_scans=False, read_ions=False, _skip_index=False, **kwargs):
+        """
+        Create an :py:class:`IndexedMGF` (binary-mode) reader for a given MGF file.
+
+        Parameters
+        ----------
+
+        source : str or file or None, optional
+            A file object (or file name) with data in MGF format. Default is
+            :py:const:`None`, which means read standard input.
+
+            .. note :: If a file object is given, it must be opened in binary mode.
+
+        use_header : bool, optional
+            Add the info from file header to each dict. Spectrum-specific parameters
+            override those from the header in case of conflict.
+            Default is :py:const:`True`.
+
+        convert_arrays : one of {0, 1, 2}, optional
+            If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+            If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+            If `2`, charges will be reported as a masked array (default).
+            The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
+
+        read_charges : bool, optional
+            If `True` (default), fragment charges are reported. Disabling it improves performance.
+
+        read_ions : bool, optional
+            If `True` (default: False), fragment ion types are reported. Disabling it improves performance.
+            Note that right now, only one of (read_charges, read_ions) may be True.
+
+        dtype : type or str or dict, optional
+            dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
+            Keys should be 'm/z array', 'intensity array', 'charge array' and/or 'ion array'.
+
+        encoding : str, optional
+            File encoding.
+
+        block_size : int, optinal
+            Size of the chunk (in bytes) used to parse the file when creating the byte offset index.
+
+        Returns
+        -------
+
+        out : IndexedMGF
+            The reader object.
+        """
+        self._index_by_scans = index_by_scans
+        self._read_ions = read_ions
         self.label = r'SCANS=(\d+)\s*' if index_by_scans else r'TITLE=([^\n]*\S)\s*'
         super(IndexedMGF, self).__init__(source, parser_func=self._read, pass_file=False, args=(), kwargs={},
                                          use_header=use_header, convert_arrays=convert_arrays,
                                          read_charges=read_charges,
                                          dtype=dtype, encoding=encoding, read_ions=read_ions, _skip_index=_skip_index,
                                          **kwargs)
 
     def __reduce_ex__(self, protocol):
         return (self.__class__,
                 (self._source_init, False, self._convert_arrays, self._read_charges,
-                 self._dtype_dict, self.encoding, True),
+                 None, self.encoding, self._index_by_scans, self._read_ions, True),
                 self.__getstate__())
 
-    def __getstate__(self):
-        state = super(IndexedMGF, self).__getstate__()
-        state['use_header'] = self._use_header
-        state['header'] = self._header
-        state['read_ions'] = self._read_ions
-        return state
-
-    def __setstate__(self, state):
-        super(IndexedMGF, self).__setstate__(state)
-        self._header = state['header']
-        self._use_header = state['use_header']
-        self._read_ions = state['read_ions']
-
     @aux._keepstate_method
     def _read_header(self):
         try:
             first = next(v for v in self._offset_index.values())[0]
         except StopIteration:  # the index is empty, no spectra in file
             first = -1
         header_lines = self.read(first).decode(self.encoding).split('\n')
@@ -357,18 +389,60 @@
     header : dict
         The file header.
 
     """
 
     def __init__(self, source=None, use_header=True, convert_arrays=2, read_charges=True,
             read_ions=False, dtype=None, encoding=None):
+        """
+        Create an :py:class:`MGF` (text-mode) reader for a given MGF file.
+
+        Parameters
+        ----------
+
+        source : str or file or None, optional
+            A file object (or file name) with data in MGF format. Default is
+            :py:const:`None`, which means read standard input.
+
+            ..note :: If a file object is given, it must be opened in text mode.
+
+        use_header : bool, optional
+            Add the info from file header to each dict. Spectrum-specific parameters
+            override those from the header in case of conflict.
+            Default is :py:const:`True`.
+
+        convert_arrays : one of {0, 1, 2}, optional
+            If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+            If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+            If `2`, charges will be reported as a masked array (default).
+            The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
+
+        read_charges : bool, optional
+            If `True` (default), fragment charges are reported. Disabling it improves performance.
+
+        read_ions : bool, optional
+            If `True` (default: False), fragment ion types are reported. Disabling it improves performance.
+            Note that right now, only one of (read_charges, read_ions) may be True.
+
+        dtype : type or str or dict, optional
+            dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
+            Keys should be 'm/z array', 'intensity array', 'charge array' and/or 'ion array'.
+
+        encoding : str, optional
+            File encoding.
+
+        Returns
+        -------
+
+        out : MGF
+            The reader object.
+        """
         super(MGF, self).__init__(source, mode='r', parser_func=self._read, pass_file=False, args=(), kwargs={},
             encoding=encoding, use_header=use_header, convert_arrays=convert_arrays, read_charges=read_charges,
             read_ions=read_ions, dtype=dtype)
-        # self.encoding = encoding
 
     @aux._keepstate_method
     def _read_header(self):
         return self._read_header_lines(self._source)
 
     def _read_spectrum(self):
         return self._read_spectrum_lines(self._source)
@@ -415,15 +489,15 @@
         If `2`, charges will be reported as a masked array (default).
         The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
 
     read_charges : bool, optional
         If `True` (default), fragment charges are reported. Disabling it improves performance.
 
     read_ions : bool, optional
-        If `True` (default: False), fragment charges are reported. Disabling it improves performance.
+        If `True` (default: False), fragment ion types are reported. Disabling it improves performance.
         Note that right now, only one of (read_charges, read_ions) may be True.
 
     dtype : type or str or dict, optional
         dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
         Keys should be 'm/z array', 'intensity array', 'charge array' and/or 'ion array'.
 
     encoding : str, optional
@@ -551,33 +625,44 @@
     """
     Create a file in MGF format.
 
     Parameters
     ----------
 
     spectra : iterable
-        A sequence of dictionaries with keys 'm/z array', 'intensity array',
+        A **sequence** of dictionaries with keys 'm/z array', 'intensity array',
         and 'params'. 'm/z array' and 'intensity array' should be sequences of
         :py:class:`int`, :py:class:`float`, or :py:class:`str`. Strings will
         be written 'as is'. The sequences should be of equal length, otherwise
         excessive values will be ignored.
 
         'params' should be a :py:class:`dict` with keys corresponding to MGF
         format. Keys must be strings, they will be uppercased and used as is,
         without any format consistency tests. Values can be of any type allowing
         string representation.
 
-        'charge array' can also be specified.
+        'charge array' or 'ion array' can also be specified.
+
+        .. note ::
+            Passing a single spectrum will work, but will trigger a warning. This usage pattern is discouraged.
+            To ensure correct output when writing multiple spectra,
+            it is recommended to construct a sequence of spectra first and then call :py:func:`write` once.
+
+        .. seealso ::
+            This discussion of usage patterns of :py:func:`write`: https://github.com/levitsky/pyteomics/discussions/109
 
     output : str or file or None, optional
         Path or a file-like object open for writing. If an existing file is
-        specified by file name, it will be opened for appending. In this case
-        writing with a header can result in violation of format conventions.
+        specified by file name, it will be opened for writing.
         Default value is :py:const:`None`, which means using standard output.
 
+        .. note::
+            The default mode for output files specified by name has been changed
+            from `a` to `w` in *pyteomics 4.6*. See `file_mode` to override the mode.
+
     header : dict or (multiline) str or list of str, optional
         In case of a single string or a list of strings, the header will be
         written 'as is'. In case of dict, the keys (must be strings) will be
         uppercased.
 
     write_charges : bool, optional
         If :py:const:`False`, fragment charges from 'charge array' will not be written.
@@ -625,15 +710,18 @@
         You may want to disable this if you need to save spectra with 'charge arrays' with missing values.
 
         If not specified, will be set to the opposite of `write_chrages`.
         If :py:mod:`numpy` is not available, this parameter has no effect.
 
     file_mode : str, keyword only, optional
         If `output` is a file name, defines the mode the file will be opened in.
-        Otherwise will be ignored. Default is 'a'.
+        Otherwise will be ignored. Default is `'w'`.
+
+        .. note ::
+            The default changed from `'a'` in *pyteomics 4.6*.
 
     encoding : str, keyword only, optional
         Output file encoding (if `output` is specified by name).
 
     Returns
     -------
 
@@ -675,14 +763,20 @@
                 continue
             l = line.split('=')
             if len(l) == 2:
                 head_dict[l[0].lower()] = l[1].strip()
     if head_str:
         output.write(head_str + '\n\n')
 
+    if isinstance(spectra, dict) and 'm/z array' in spectra:
+        spectra = (spectra, )
+        warnings.warn("Passing a single spectrum to `write()` is discouraged. "
+            "To write a set of spectra, pass them to `write()` all at once. "
+            "For more info, see: https://github.com/levitsky/pyteomics/discussions/109.")
+
     for spectrum in spectra:
         output.write('BEGIN IONS\n')
         found = set()
         for key in it.chain(key_order, spectrum['params']):
             if key not in found and key in spectrum['params']:
                 found.add(key)
                 val = spectrum['params'][key]
```

### Comparing `pyteomics-4.5.6/pyteomics/ms1.py` & `pyteomics-4.6/pyteomics/ms1.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 ms1 - read and write MS/MS data in MS1 format
 =============================================
 
 Summary
 -------
 
 `MS1 <http://dx.doi.org/10.1002/rcm.1603>`_ is a simple
-human-readable format for MS1 data. It allows storing MS1 peak lists and
-exprimental parameters.
+human-readable format for MS1 data. It allows storing MS1 peak lists and exprimental parameters.
 
-This module provides minimalistic infrastructure for access to data stored in
-MS1 files.
+This module provides minimalistic infrastructure for access to data stored in MS1 files.
 Two main classes are :py:class:`MS1`, which provides an iterative, text-mode parser,
 and :py:class:`IndexedMS1`, which is a binary-mode parser that supports random access using scan IDs
 and retention times.
 The function :py:func:`read` helps dispatch between the two classes.
-Also, common parameters can be read from MS1 file header with
-:py:func:`read_header` function.
+Also, common parameters can be read from MS1 file header with :py:func:`read_header` function.
+
+Classes
+-------
+
+  :py:class:`MS1` - a text-mode MS1 parser. Suitable to read spectra from a file consecutively.
+  Needs a file opened in text mode (or will open it if given a file name).
+
+  :py:class:`IndexedMS1` - a binary-mode MS1 parser. When created, builds a byte offset index
+  for fast random access by spectrum ID. Sequential iteration is also supported.
+  Needs a seekable file opened in binary mode (if created from existing file object).
+
+  :py:class:`MS1Base` - abstract class, the common ancestor of the two classes above.
+  Can be used for type checking.
 
 Functions
 ---------
 
-  :py:func:`read` - iterate through spectra in MS1 file. Data from a
-  single spectrum are converted to a human-readable dict.
+  :py:func:`read` - an alias for :py:class:`MS1` or :py:class:`IndexedMS1`.
 
   :py:func:`chain` - read multiple files at once.
 
   :py:func:`chain.from_iterable` - read multiple files at once, using an
   iterable of files.
 
   :py:func:`read_header` - get a dict with common parameters for all spectra
@@ -52,31 +61,61 @@
 from . import auxiliary as aux
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
-class MS1Base(object):
+class MS1Base(aux.ArrayConversionMixin):
     """Abstract class representing an MS1 file. Subclasses implement different approaches to parsing."""
     _array_keys = ['m/z array', 'intensity array']
+    _float_keys = ['RTime', 'RetTime']
 
-    def __init__(self, source=None, use_header=False, convert_arrays=True, dtype=None, **kwargs):
-        super(MS1Base, self).__init__(source, **kwargs)
+    def __init__(self, source=None, use_header=False, convert_arrays=True, dtype=None, encoding=None, **kwargs):
+        """
+        Create an instance of a :py:class:`MS1Base` parser.
+
+        Parameters
+        ----------
+
+        source : str or file or None, optional
+            A file object (or file name) with data in MS1 format. Default is
+            :py:const:`None`, which means read standard input.
+
+        use_header : bool, optional
+            Add the info from file header to each dict. Spectrum-specific parameters
+            override those from the header in case of conflict.
+            Default is :py:const:`False`.
+
+        convert_arrays : one of {0, 1, 2}, optional
+            If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+            If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+            If `2`, charges will be reported as a masked array (default).
+            The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
+
+        dtype : type or str or dict, optional
+            dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
+            Keys should be 'm/z array', 'intensity array', 'charge array'.
+
+        encoding : str, optional
+            File encoding.
+        """
+        super(MS1Base, self).__init__(source, use_header=use_header, convert_arrays=convert_arrays, dtype=dtype, encoding=encoding, **kwargs)
         if convert_arrays and np is None:
             raise aux.PyteomicsError('numpy is required for array conversion')
-        self._convert_arrays = convert_arrays
-        self._dtype_dict = dtype if isinstance(dtype, dict) else {k: dtype for k in self._array_keys}
         self._use_header = use_header
         if use_header:
             self._header = self._read_header()
         else:
             self._header = None
         self._source_name = getattr(source, 'name', str(source))
 
+    def reset(self):
+        super(MS1Base, self).reset()
+        self._pending_line = None
 
     @property
     def header(self):
         return self._header
 
     def _read_header_lines(self, lines):
         header = {}
@@ -87,26 +126,20 @@
             if len(tokens) < 3:
                 tokens = line.split(None, 2)
             key = tokens[1]
             val = tokens[2].strip()
             header[key] = val
         return header
 
-    def _make_scan(self, params, masses, intensities):
-        if 'RTime' in params:
-            params['RTime'] = float(params['RTime'])
-        out = {'params': params}
-        if self._convert_arrays:
-            data = {'m/z array': masses, 'intensity array': intensities}
-            for key, values in data.items():
-                out[key] = np.array(values, dtype=self._dtype_dict.get(key))
-        else:
-            out['m/z array'] = masses
-            out['intensity array'] = intensities
-        return out
+    def _make_scan(self, info):
+        for key in self._float_keys:
+            if key in info['params']:
+                info['params'][key] = float(info['params'][key])
+        self._build_all_arrays(info)
+        return info
 
     def _handle_S(self, line, sline, params):
         sline = line.strip().split(None, 3)
         params['scan'] = tuple(sline[1:3])
         if len(sline) == 4:  # in MS2 the S line contains the precursor m/z as a 4th column
             params['precursor m/z'] = float(sline[3])
 
@@ -116,55 +149,83 @@
     def _handle_Z(self, line, sline, params):
         params.setdefault('charge', []).append(float(sline[1]))
         params.setdefault('neutral mass', []).append(float(sline[2]))
 
     def _handle_D(self, line, sline, params):
         params.setdefault('analyzer', []).append(sline[1:])
 
+    def _handle_peak(self, line, sline, info):
+        try:
+            info['m/z array'].append(float(sline[0]))            # this may cause
+            info['intensity array'].append(float(sline[1]))      # exceptions...
+        except ValueError:
+            raise aux.PyteomicsError(
+                'Error when parsing %s. Line: %s' % (self._source_name, line))
+        except IndexError:
+            pass
+
     def _read_spectrum_lines(self, lines):
-        reading_spectrum = False
         params = {}
-        masses = []
-        intensities = []
+        info = {'params': params}
+        for k in self._array_keys:
+            info[k] = []
         if self._use_header:
             params.update(self.header)
-
-        for line in lines:
+        if self._pending_line:
+            reading_spectrum = True
+            self._handle_S(self._pending_line, None, params)
+        else:
+            reading_spectrum = False
+        line_count = 0
+        for i, line in enumerate(lines):
+            line_count = i
             sline = line.strip().split(None, 2)
             if not sline:
                 continue
             if not reading_spectrum:
                 if sline[0] == 'S':
                     reading_spectrum = True
                     self._handle_S(line, sline, params)
                 # otherwise we are not interested; do nothing, just move along
             else:
                 if not sline:
                     pass
                 elif sline[0] == 'S':
-                    return self._make_scan(params, masses, intensities)
+                    self._pending_line = line
+                    return self._make_scan(info)
 
                 else:
                     if sline[0] == 'I':  # spectrum-specific parameters!
                         self._handle_I(line, sline, params)
                     elif sline[0] == 'Z':  # MS2-specific charge state guess
                         self._handle_Z(line, sline, params)
                     elif sline[0] == 'D':  # MS2-specific analyzer annotation
                         self._handle_D(line, sline, params)
                     else:  # this must be a peak list
-                        try:
-                            masses.append(float(sline[0]))            # this may cause
-                            intensities.append(float(sline[1]))       # exceptions...\
-                        except ValueError:
-                            raise aux.PyteomicsError(
-                                'Error when parsing %s. Line: %s' % (
-                                    self._source_name, line))
-                        except IndexError:
-                            pass
-        return self._make_scan(params, masses, intensities)
+                        self._handle_peak(line, sline, info)
+        self._pending_line = None
+        if line_count == 0:
+            return
+        return self._make_scan(info)
+
+    def __getstate__(self):
+        state = super(MS1Base, self).__getstate__()
+        state['use_header'] = self._use_header
+        state['header'] = self._header
+        return state
+
+    def __setstate__(self, state):
+        super(MS1Base, self).__setstate__(state)
+        self._use_header = state['use_header']
+        self._header = state['header']
+
+    def __reduce_ex__(self, protocol):
+        return (self.__class__,
+            (self._source_init, False, self._convert_arrays, None, self.encoding),
+            self.__getstate__())
 
 
 class MS1(MS1Base, aux.FileReader):
     """
     A class representing an MS1 file. Supports the `with` syntax and direct iteration for sequential
     parsing.
 
@@ -178,84 +239,74 @@
     ----------
 
     header : dict
         The file header.
 
     """
     def __init__(self, source=None, use_header=False, convert_arrays=True, dtype=None, encoding=None, **kwargs):
+        """
+        Create an :py:class:`MS1` (text-mode) reader for a given MS1 file.
+
+        Parameters
+        ----------
+
+        source : str or file or None, optional
+            A file object (or file name) with data in MS1 format. Default is
+            :py:const:`None`, which means read standard input.
+
+            .. note :: If a file object is given, it must be opened in text mode.
+
+        use_header : bool, optional
+            Add the info from file header to each dict. Spectrum-specific parameters
+            override those from the header in case of conflict.
+            Default is :py:const:`False`.
+
+        convert_arrays : one of {0, 1, 2}, optional
+            If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+            If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+            If `2`, charges will be reported as a masked array (default).
+            The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
+
+        dtype : type or str or dict, optional
+            dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
+            Keys should be 'm/z array', 'intensity array', 'charge array'.
+
+        encoding : str, optional
+            File encoding.
+
+        Returns
+        -------
+
+        out : MS1
+            The reader object.
+        """
         super(MS1, self).__init__(source, use_header=use_header, convert_arrays=convert_arrays, dtype=dtype, encoding=encoding,
             mode='r', parser_func=self._read, pass_file=False, args=(), kwargs={})
-        # aux.FileReader.__init__(self, source, 'r', self._read, False, (), {}, encoding)
-        # MS1Base.__init__(self, source, use_header, convert_arrays, dtype)
-        # self.encoding = encoding
 
     @aux._keepstate_method
     def _read_header(self):
         return self._read_header_lines(self._source)
 
-    def _read_spectrum(self, firstline):
-        return self._read_spectrum_lines(self._source, firstline)
-
     def _read(self):
-        reading_spectrum = False
-        params = {}
-        masses = []
-        intensities = []
-        if self._use_header:
-            params.update(self.header)
-
-        for line in self._source:
-            sline = line.strip().split(None, 2)
-            if not sline:
-                continue
-            if not reading_spectrum:
-                if sline[0] == 'S':
-                    reading_spectrum = True
-                    self._handle_S(line, sline, params)
-                # otherwise we are not interested; do nothing, just move along
-            else:
-                if not sline:
-                    pass
-                elif sline[0] == 'S':
-                    yield self._make_scan(params, masses, intensities)
-                    params = dict(self.header) if self._use_header else {}
-                    masses = []
-                    intensities = []
-                    self._handle_S(line, sline, params)
-                else:
-                    if sline[0] == 'I':  # spectrum-specific parameters!
-                        self._handle_I(line, sline, params)
-                    elif sline[0] == 'Z':  # MS2-specific charge state guess
-                        self._handle_Z(line, sline, params)
-                    elif sline[0] == 'D':  # MS2-specific analyzer annotation
-                        self._handle_D(line, sline, params)
-                    else:  # this must be a peak list
-                        try:
-                            masses.append(float(sline[0]))            # this may cause
-                            intensities.append(float(sline[1]))       # exceptions...
-                        except ValueError:
-                            raise aux.PyteomicsError(
-                                'Error when parsing %s. Line: %s' % (self._source_name, line))
-                        except IndexError:
-                            pass
+        def get_next_spectrum():
+            return self._read_spectrum_lines(self._source)
 
-        yield self._make_scan(params, masses, intensities)
+        for spectrum in iter(get_next_spectrum, None):
+            yield spectrum
 
 
 class IndexedMS1(MS1Base, aux.TaskMappingMixin, aux.TimeOrderedIndexedReaderMixin, aux.IndexedTextReader):
     """
     A class representing an MS1 file. Supports the `with` syntax and direct iteration for sequential
     parsing. Specific spectra can be accessed by title using the indexing syntax in constant time.
     If created using a file object, it needs to be opened in binary mode.
 
     When iterated, :py:class:`IndexedMS1` object yields spectra one by one.
-    Each 'spectrum' is a :py:class:`dict` with four keys: 'm/z array',
-    'intensity array', 'charge array' and 'params'. 'm/z array' and
-    'intensity array' store :py:class:`numpy.ndarray`'s of floats,
-    'charge array' is a masked array (:py:class:`numpy.ma.MaskedArray`) of ints,
+    Each 'spectrum' is a :py:class:`dict` with three keys: 'm/z array', 'intensity array' and 'params'.
+    'm/z array' and 'intensity array' store :py:class:`numpy.ndarray`'s of floats,
     and 'params' stores a :py:class:`dict` of parameters (keys and values are
     :py:class:`str`, keys corresponding to MS1).
 
     .. warning ::
         Labels for scan objects are constructed as the first number in the S line, as follows:
         for a line ``S  0   1`` the label is `'0'`. If these labels are not unique
         for the scans in the file, the indexed parser will not work correctly. Consider using
@@ -270,37 +321,61 @@
         A property used for accessing spectra by retention time.
     """
 
     delimiter = '\nS'
     label = r'^[\n]?S\s+(\S+)'
 
     def __init__(self, source=None, use_header=False, convert_arrays=True, dtype=None, encoding='utf-8', _skip_index=False, **kwargs):
+        """
+        Create an :py:class:`IndexedMS1` (binary-mode) reader for a given MS1 file.
+
+        Parameters
+        ----------
+
+        source : str or file or None, optional
+            A file object (or file name) with data in MS1 format. Default is
+            :py:const:`None`, which means read standard input.
+
+            .. note :: If a file object is given, it must be opened in binary mode.
+
+        use_header : bool, optional
+            Add the info from file header to each dict. Spectrum-specific parameters
+            override those from the header in case of conflict.
+            Default is :py:const:`True`.
+
+        convert_arrays : one of {0, 1, 2}, optional
+            If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+            If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+            If `2`, charges will be reported as a masked array (default).
+            The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
+
+        dtype : type or str or dict, optional
+            dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
+            Keys should be 'm/z array', 'intensity array', 'charge array'.
+
+        encoding : str, optional
+            File encoding.
+
+        block_size : int, optinal
+            Size of the chunk (in bytes) used to parse the file when creating the byte offset index.
+
+        Returns
+        -------
+
+        out : IndexedMS1
+            The reader object.
+        """
         super(IndexedMS1, self).__init__(source, use_header=use_header, convert_arrays=convert_arrays, dtype=dtype, encoding=encoding,
-            parser_func=self._read, pass_file=False, args=(), kwargs={}, _skip_index=_skip_index)
-        # aux.TimeOrderedIndexedReaderMixin.__init__(self, source, self._read, False, (), {}, encoding,
-        #     block_size, _skip_index=_skip_index)
-        # MS1Base.__init__(self, source, use_header, convert_arrays, dtype)
+            parser_func=self._read, pass_file=False, args=(), kwargs={}, _skip_index=_skip_index, **kwargs)
 
     def __reduce_ex__(self, protocol):
         return (self.__class__,
-            (self._source_init, False, self._convert_arrays,
-                self._read_charges, self._dtype_dict, self.encoding, self.block_size, True),
+            (self._source_init, False, self._convert_arrays, None, self.encoding, True),
             self.__getstate__())
 
-    def __getstate__(self):
-        state = super(IndexedMS1, self).__getstate__()
-        state['use_header'] = self._use_header
-        state['header'] = self._header
-        return state
-
-    def __setstate__(self, state):
-        super(IndexedMS1, self).__setstate__(state)
-        self._use_header = state['use_header']
-        self._header = state['header']
-
     @aux._keepstate_method
     def _read_header(self):
         try:
             first = next(v for v in self._offset_index.values())[0]
         except StopIteration: # the index is empty, no spectra in file
             first = -1
         header_lines = self.read(first).decode(self.encoding).split('\n')
@@ -363,18 +438,19 @@
         :py:const:`None`, which means read standard input.
 
     use_header : bool, optional
         Add the info from file header to each dict. Spectrum-specific parameters
         override those from the header in case of conflict.
         Default is :py:const:`False`.
 
-    convert_arrays : bool, optional
-        If :py:const:`False`, m/z and intensities will be returned as regular lists.
-        If :py:const:`True` (default), they will be converted to regular :py:class:`numpy.ndarray`'s.
-        Conversion requires :py:mod:`numpy`.
+    convert_arrays : one of {0, 1, 2}, optional
+        If `0`, m/z, intensities and (possibly) charges will be returned as regular lists.
+        If `1`, they will be converted to regular :py:class:`numpy.ndarray`'s.
+        If `2`, charges will be reported as a masked array (default).
+        The default option is the slowest. `1` and `2` require :py:mod:`numpy`.
 
     dtype : type or str or dict, optional
         dtype argument to :py:mod:`numpy` array constructor, one for all arrays or one for each key.
         Keys should be 'm/z array' and/or 'intensity array'.
 
     encoding : str, optional
         File encoding.
```

### Comparing `pyteomics-4.5.6/pyteomics/mzid.py` & `pyteomics-4.6/pyteomics/mzid.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/mzml.py` & `pyteomics-4.6/pyteomics/mzml.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,37 +113,51 @@
     'mean ion mobility drift time array',
     'mass array',
     'scanning quadrupole position lower bound m/z array',
     'scanning quadrupole position upper bound m/z array',
 ])
 
 
-class MzML(xml.ArrayConversionMixin, aux.TimeOrderedIndexedReaderMixin, xml.MultiProcessingXML, xml.IndexSavingXML):
+class MzML(aux.BinaryArrayConversionMixin, aux.TimeOrderedIndexedReaderMixin, xml.MultiProcessingXML, xml.IndexSavingXML):
     """Parser class for mzML files."""
     file_format = 'mzML'
     _root_element = 'mzML'
     _default_schema = _schema_defaults._mzml_schema_defaults
     _default_version = '1.1.0'
     _default_iter_tag = 'spectrum'
     _structures_to_flatten = {'binaryDataArrayList', 'referenceableParamGroupRef'}
     _indexed_tags = {'spectrum', 'chromatogram'}
 
     def __init__(self, *args, **kwargs):
         self.decode_binary = kwargs.pop('decode_binary', True)
+        self._referenceable_param_groups = {}
         super(MzML, self).__init__(*args, **kwargs)
 
     def __getstate__(self):
         state = super(MzML, self).__getstate__()
         state['decode_binary'] = self.decode_binary
         return state
 
     def __setstate__(self, state):
         super(MzML, self).__setstate__(state)
         self.decode_binary = state['decode_binary']
 
+    def _handle_referenceable_param_group(self, param_group_ref, **kwargs):
+        ref_name = param_group_ref.attrib['ref']
+        if ref_name not in self._referenceable_param_groups:
+            params = self._referenceable_param_groups[ref_name] = self._retrieve_param_group(ref_name)
+            return params
+        return self._referenceable_param_groups[ref_name]
+
+    @xml._keepstate
+    def _retrieve_param_group(self, ref_name):
+        group = self.get_by_id(ref_name)
+        group.pop("id", None)
+        return [xml._XMLParam(k, v, None) for k, v in group.items()]
+
     def _detect_array_name(self, info):
         """Determine what the appropriate name for this
         array is by inspecting the available param-based
         keys.
 
         Parameters
         ----------
@@ -339,15 +353,15 @@
                     info.pop('id', None)
 
     @staticmethod
     def _get_time(scan):
         return scan['scanList']['scan'][0]['scan start time']
 
 
-def read(source, read_schema=False, iterative=True, use_index=False, dtype=None, huge_tree=False):
+def read(source, read_schema=False, iterative=True, use_index=False, dtype=None, huge_tree=False, decode_binary=True):
     """Parse `source` and iterate through spectra.
 
     Parameters
     ----------
     source : str or file
         A path to a target mzML file or the file object itself.
 
@@ -385,15 +399,16 @@
     Returns
     -------
     out : iterator
        An iterator over the dicts with spectrum properties.
     """
 
     return MzML(source, read_schema=read_schema, iterative=iterative,
-        use_index=use_index, dtype=dtype, huge_tree=huge_tree)
+                use_index=use_index, dtype=dtype, huge_tree=huge_tree,
+                decode_binary=decode_binary)
 
 def iterfind(source, path, **kwargs):
     """Parse `source` and yield info on elements with specified local
     name or by specified "XPath".
 
     .. note:: This function is provided for backward compatibility only.
         If you do multiple :py:func:`iterfind` calls on one file, you should
```

### Comparing `pyteomics-4.5.6/pyteomics/mzmlb.py` & `pyteomics-4.6/pyteomics/mzmlb.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/mztab.py` & `pyteomics-4.6/pyteomics/mztab.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,783 +1,783 @@
-"""
-mztab - mzTab file reader
-=========================
-
-Summary
--------
-
-`mzTab <https://github.com/HUPO-PSI/mzTab>`_  is one of the standards
-developed by the Proteomics Informatics working group of the HUPO Proteomics
-Standard Initiative.
-
-This module provides a way to read mzTab files into a collection of
-:py:class:`pandas.DataFrame` instances in memory, along with a mapping
-of the file-level metadata. MzTab specifications 1.0 and 2.0 are supported.
-
-Data access
------------
-
-  :py:class:`MzTab` - a class representing a single mzTab file.
-
-Helpers
--------
-
-    :py:class:`Group` - a collection of metadata relating to one entity.
-
-
-Internals
----------
-
-    :py:class:`_MzTabTable` - a single table in an mzTab file.
-
-
-Property Management
-~~~~~~~~~~~~~~~~~~~
-
-:mod:`mztab` uses metaprogramming to generate its metadata accessors, generated by
-these classes working in concert.
-
-    :py:class:`MetadataBackedProperty`
-
-    :py:class:`MetadataBackedCollection`
-
-    :py:class:`MetadataPropertyAnnotator`
-
--------------------------------------------------------------------------------
-"""
-
-import re
-import warnings
-
-try:
-    import pandas as pd
-except ImportError:
-    pd = None
-
-
-from collections import OrderedDict
-
-from pyteomics.auxiliary import _file_obj
-from pyteomics.auxiliary import cvstr
-from pyteomics.auxiliary.utils import add_metaclass
-
-
-def _require_pandas():
-    if pd is None:
-        raise ImportError(
-            "To load an mzTab file into pandas.DataFrame objects, you must install pandas!")
-
-
-class MetadataBackedProperty(object):
-    '''Our descriptor type which uses the instance's metadata attribute to carry its values'''
-
-    def __init__(self, name, variant_required=None):
-        if variant_required is None:
-            variant_required = ()
-        self.name = name
-        self.variant_required = variant_required
-        self.__doc__ = self.build_docstring()
-
-    def __repr__(self):
-        return "{self.__class__.__name__}(name={self.name!r}, variant_required={self.variant_required})".format(self=self)
-
-    def __get__(self, obj, objtype=None):
-        if obj is None and objtype is not None:
-            # So the property can be seen for what it is
-            return self
-        value = obj.metadata.get(self.name)
-        if value is None and self.variant_required and obj.variant in self.variant_required:
-            raise AttributeError("{0} is missing from a mzTab-\"{1}\" document where it is required!".format(
-                self.name, obj.variant))
-        return value
-
-    def __set__(self, obj, value):
-        obj.metadata[self.name] = value
-
-    def __delete__(self, obj):
-        del obj.metadata[self.name]
-
-    def build_docstring(self):
-        doc = '''Accesses the {self.name!r} key in the :attr:`metadata` mapping attached
-to this object.
-'''
-        if self.variant_required:
-            if len(self.variant_required) > 1:
-                plural = 's'
-            else:
-                plural = ''
-            requires = ' or '.join(['-%s' % v for v in self.variant_required])
-            doc += '''
-This key must be present when the file is of {requires} variant{plural}.
-        '''.format(requires=requires, plural=plural)
-        doc += '''
-Returns
--------
-object
-        '''
-        doc = doc.format(self=self)
-        return doc
-
-
-class MetadataBackedCollection(object):
-    def __init__(self, name, variant_required=None):
-        if variant_required is None:
-            variant_required = ()
-        self.name = name
-        self.variant_required = variant_required
-        self.__doc__ = self.build_docstring()
-
-    def __get__(self, obj, objtype=None):
-        if obj is None and objtype is not None:
-            # So the property can be seen for what it is
-            return self
-        groups = obj.gather(obj.metadata)
-        value = groups.get(self.name)
-        if value is None and self.variant_required and obj.variant in self.variant_required:
-            raise AttributeError("{0} is missing from a mzTab-\"{1}\" document where it is required!".format(
-                self.name, obj.variant))
-        return value
-
-    def build_docstring(self):
-        doc = '''Accesses the {self.name!r} key group gathered in the :attr:`metadata` mapping attached
-to this object.
-
-This group is dynamically generated on each access and may be expensive for repeated use.
-'''
-        if self.variant_required:
-            if len(self.variant_required) > 1:
-                plural = 's'
-            else:
-                plural = ''
-            requires = ' or '.join(['-%s' % v for v in self.variant_required])
-            doc += '''
-This key must be present when the file is of {requires} variant{plural}.
-        '''.format(requires=requires, plural=plural)
-        doc += '''
-Returns
--------
-:class:`~.Group`
-        '''
-        doc = doc.format(self=self)
-        return doc
-
-
-class MetadataPropertyAnnotator(type):
-    '''A simple metaclass to do some class-creation time introspection
-    and descriptor binding.
-
-    Uses a list of strings or 3-tuples from :attr:`__metadata_properties__` to
-    bind :class:`MetadataBackedProperty` or :class:`MetadataBackedCollection`
-    onto the class during its creation.
-
-    The specification for a property is a tuple of three values:
-        1. The metadata key to fetch
-        2. The property name to expose on the object
-        3. The variant(s) which require this metadata key be present
-
-    :obj:`("mzTab-version", "version", ("M", "P"))` would be interpreted as
-    Expose a property "version" on instances which serves the key "mzTab-version"
-    from the instance's :attr:`metadata`, and raise an error if it is absent in
-    the "M" or "P" variants.
-
-    Alternatively a specification may be a single string which will be interpreted
-    as the metadata key, and used to generate the property name replacing all '-'
-    with '_' and assumed to be optional in all variants.
-
-    If a metadata key ends with "[]" the property is assumed to be a collection. mzTab
-    makes heavy use of "<collection_name>[<index>]..." keys to define groups of homogenous
-    object types, often with per-element attributes.
-
-    .. code-block::
-
-        variable_mod[1]    CHEMMOD:15.9949146221
-        variable_mod[1]-site  M
-        variable_mod[1]-position    Anywhere
-        variable_mod[2]    CHEMMOD:42.0105646863
-        variable_mod[2]-site  N-term
-        variable_mod[2]-position Protein N-term
-
-    A specification :obj:`("variable_mod[]", "variable_mods", ())` would create a property
-    that returns:
-
-    .. code-block:: python
-
-        >>>instance.variable_mods
-        Group([(1,
-                    {'name': 'CHEMMOD:15.9949146221',
-                     'position': 'Anywhere',
-                     'site': 'M'}),
-                (2,
-                    {'name': 'CHEMMOD:42.0105646863',
-                     'position': 'Protein N-term',
-                     'site': 'N-term'})])
-
-    For precise description of the property collection algorithm, see
-    :meth:`~_MzTabParserBase.collapse_properties` and
-    :meth:`~_MzTabParserBase.gather`.
-
-    If any base classes have a :attr:`__metadata_properties__` attribute, it will
-    also be included unless :attr:`__inherit_metadata_properties__` is set to
-    :const:`False`. Any names explicitly set by the current class override this
-    automatic property generation.
-    '''
-    def __new__(mcls, name, bases, attrs):
-        props = attrs.get('__metadata_properties__', [])
-        inherit_props = attrs.get("__inherit_metadata_properties__", True)
-        # Gather from parent classes so we can use inheritance for overriding this
-        # behavior too.
-        if inherit_props:
-            for base in bases:
-                props.extend(getattr(base, '__metadata_properties__', []))
-
-        keys = set(attrs)
-
-        # Iterate in reverse to ensure that classes nearer to the new classes override
-        # more basal classes, ending with the new class to make sure overrides are
-        # applied.
-        for prop in reversed(props):
-            # If the property definition is a single string, interpret the specification
-            # as the property name, and apply some simple normalization to make it a valid
-            # Python attribute name and assume the property is always optional.
-            if isinstance(prop, str):
-                prop_name = prop
-                attr_name = prop_name.replace("mzTab-", '').replace('-', '_')
-                variant_required = None
-            else:
-                # Otherwise unpack the triple
-                prop_name, attr_name, variant_required = prop
-            # Attach the new descriptor to the class definition to be created. These descriptors
-            # will then be used when instances of that class try to get/set those attribute names.
-            if attr_name in keys:
-                continue
-            if prop_name.endswith('[]'):
-                # If the property name ends with "[]", then we're dealing with a collection so
-                # use the :class:`MetadataBackedCollection` descriptor
-                attrs[attr_name] = MetadataBackedCollection(
-                    prop_name[:-2], variant_required=variant_required)
-            else:
-                # Otherwise it is a scalar-valued property, using the :class:`MetadataBackedProperty`
-                # descriptor
-                prop = attrs[attr_name] = MetadataBackedProperty(
-                    prop_name, variant_required=variant_required)
-
-        return super(MetadataPropertyAnnotator, mcls).__new__(mcls, name, bases, attrs)
-
-
-class _MzTabParserBase(object):
-    def _parse_param(self, tuplet):
-        """Parse a controlled vocabulary or user specified parameter tuplet
-        into a Python object
-
-        Parameters
-        ----------
-        tuplet : str
-            A square brace enclosed tuplet of values describing the parameter
-
-        Returns
-        -------
-        tuple
-            The reduced representation of the parameter
-        """
-        cv, acc, name, value = re.split(r"\s*,\s*", tuplet[1:-1])
-        param_name = cvstr(name, acc)
-        if value:
-            return (param_name, value)
-        else:
-            return (param_name)
-
-    def collapse_properties(self, proplist):
-        '''Collapse a flat property list into a hierchical structure.
-
-        This is intended to operate on :py:class:`Mapping` objects, including
-        :class:`dict`, :class:`pandas.Series` and :class:`pandas.DataFrame`.
-
-        .. code-block:: python
-
-            {
-              "ms_run[1]-format": "Andromeda:apl file format",
-              "ms_run[1]-location": "file://...",
-              "ms_run[1]-id_format": "scan number only nativeID format"
-            }
-
-        to
-
-        .. code-block:: python
-
-            {
-              "ms_run": [
-                {
-                  "format": "Andromeda:apl file format",
-                  "location": "file://...",
-                  "id_format": "scan number only nativeID format"
-                }
-              ]
-            }
-
-        Parameters
-        ----------
-        proplist: :class:`Mapping`
-            Key-Value pairs to collapse
-
-        Returns
-        -------
-        :class:`OrderedDict`:
-            The collapsed property list
-        '''
-        entities = OrderedDict()
-        rest = {}
-        for key, value in proplist.items():
-            try:
-                entity, prop_name = key.rsplit("-", 1)
-            except ValueError:
-                rest[key] = value
-                continue
-            try:
-                entity_dict = entities[entity]
-            except KeyError:
-                entity_dict = entities[entity] = {}
-            entity_dict[prop_name] = value
-        for key, value in proplist.items():
-            if key in entities:
-                entity = entities[key]
-                if 'name' not in entity:
-                    entity['name'] = value
-        for key, value in rest.items():
-            if key in entities:
-                entities[key]['name'] = value
-            else:
-                entities[key] = value
-        return entities
-
-    def _collapse_collections(self, entities):
-        gathered = Group()
-        for key, props in entities.items():
-            if '[' in key:
-                k, ix = key.split('[', 1)
-                if '[' in ix:
-                    # If we have multiple [ in a key, we are dealing with a path
-                    path = extract_path(key)
-                    for k, ix in path[:-1]:
-                        store = gathered[k]
-                        store = store[int(ix)]
-                    k, ix = path[-1]
-                    store[k][int(ix)] = props
-
-                else:
-                    ix = int(ix[:-1])
-                    gathered[k][ix] = props
-            else:
-                gathered[key] = props
-        return gathered
-
-    def _cast_value(self, value):
-        """Convert a cell value to the appropriate Python type
-
-        Parameters
-        ----------
-        value : str
-            The cell value as text
-
-        Returns
-        -------
-        object
-            The most specialized type recognized
-        """
-        if value == 'null':
-            return None
-        # is it a parameter?
-        if value.startswith("["):
-            try:
-                if "|" in value:
-                    return [self._cast_value(v) for v in value.split("|")]
-                else:
-                    return self._parse_param(value)
-            except ValueError:
-                return value
-        else:
-            # begin guessing dtype
-            try:
-                value = int(value)
-            except ValueError:
-                try:
-                    value = float(value)
-                except ValueError:
-                    pass
-            return value
-
-    def gather(self, mapping):
-        '''Collapse property lists using :meth:`collapse_properties`
-        and then gather collections of entites into lists.
-
-        Parameters
-        ----------
-        mapping : dict
-            The flattened hierarchy of properties to re-construct
-
-        Returns
-        -------
-        Group :
-            A :class:`Group` of all entities and collections of entities
-        '''
-        return self._collapse_collections(self.collapse_properties(mapping))
-
-
-class _MzTabTable(_MzTabParserBase):
-
-    """An internal class for accumulating information about an single table
-    represented in an mzTab file
-
-    Attributes
-    ----------
-    header : list
-        The column names for the table
-    name : str
-        The table's name, human readable
-    rows : list
-        An accumulator of table rows
-    """
-
-    def __init__(self, name, header=None, rows=None):
-        if rows is None:
-            rows = []
-        self.name = name
-        self.header = header
-        self.rows = rows
-
-    def __repr__(self):
-        n_cols = len(self.header) if self.header is not None else 0
-        n_rows = len(self.rows)
-        template = "<_MzTabTable {name} with {n_cols} columns and {n_rows} rows>"
-        return template.format(n_cols=n_cols, n_rows=n_rows, name=self.name)
-
-    def add(self, row):
-        self.rows.append([self._cast_value(v) for v in row])
-
-    def __len__(self):
-        return len(self.rows)
-
-    def __getitem__(self, i):
-        if isinstance(i, int):
-            return self.gather({h: r for h, r in zip(self.header, self.rows[i])})
-        elif isinstance(i, slice):
-            out = []
-            for i in range(i.start or 0, i.stop or len(self), i.step or 1):
-                out.append(self[i])
-            return out
-        raise TypeError("Cannot access table with object of type %r" % type(i))
-
-    def as_dict(self):
-        return {"rows": [dict(zip(self.header, row)) for row in self.rows],
-                "name": self.name}
-
-    def as_df(self, index=None):
-        """Convert the table to a DataFrame in memory.
-
-        Returns
-        -------
-        pd.DataFrame
-        """
-        _require_pandas()
-        table = pd.DataFrame(data=self.rows, columns=self.header)
-        if index is not None and len(table.index) > 0:
-            table = table.set_index(index, drop=False)
-        table.name = self.name
-        return table
-
-    def clear(self):
-        self.header = None
-        self.rows = []
-
-
-DATA_FRAME_FORMAT = 'df'
-DICT_FORMAT = 'dict'
-RAW_FORMAT = 'raw'
-
-PATH_PARSER = re.compile(r"([^\[]+)\[(\d+)\]_?")
-
-
-def extract_path(path):
-    '''Parse `key[index]_next_key[next_index]...` sequences into
-    lists of (key, index) pairs.
-
-    Parameters
-    ----------
-    path : str
-        The path key to parse
-
-    Returns
-    -------
-    list
-    '''
-    return [(t, int(i)) for t, i in PATH_PARSER.findall(path)]
-
-
-class Group(OrderedDict):
-    '''A type for holding collections of arbitrarily nested keys from rows
-    and metadata mappings.
-
-    Implemented as an autovivifying :class:`OrderedDict` variant. As such implements
-    the :class:`~collections.abc.Mapping` interface.
-    '''
-
-    def get_path(self, path, default=None):
-        '''As :meth:`get` but over a path key parsed with :func:`extract_path`.
-
-        Parameters
-        ----------
-        path : str
-            The path to search down
-        default : object, optional
-            The return value when the path is missing
-
-        Returns
-        -------
-        object
-        '''
-        tokens = extract_path(path)
-        if not tokens:
-            return self.get(path, default)
-        layer = self
-        for k, i in tokens[:-1]:
-            i = int(i)
-            layer = layer.get(k)
-            if layer is None:
-                return None
-            layer = layer.get(i)
-            if layer is None:
-                return None
-        k, i = tokens[-1]
-        i = int(i)
-        layer = layer.get(k)
-        if layer is None:
-            return default
-        value = layer.get(i, default)
-        return value
-
-    def __missing__(self, key):
-        value = self.__class__()
-        self[key] = value
-        return value
-
-
-@add_metaclass(MetadataPropertyAnnotator)
-class MzTab(_MzTabParserBase):
-    """Parser for mzTab format files.
-
-    Attributes
-    ----------
-    comments : list
-        A list of comments across the file
-    file : _file_obj
-        A file stream wrapper for the file to be read
-    metadata : OrderedDict
-        A mapping of metadata that was entities.
-    peptide_table : _MzTabTable or pd.DataFrame
-        The table of peptides. Not commonly used.
-    protein_table : _MzTabTable or pd.DataFrame
-        The table of protein identifications.
-    small_molecule_table : _MzTabTable or pd.DataFrame
-        The table of small molecule identifications.
-    spectrum_match_table : _MzTabTable or pd.DataFrame
-        The table of spectrum-to-peptide match identifications.
-    table_format: 'df', 'dict', or callable
-        The structure type to replace each table with. The string
-        'df' will use pd.DataFrame instances. 'dict' will create
-        a dictionary of dictionaries for each table. A callable
-        will be called on each raw _MzTabTable object
-
-    Additional components of :attr:`metadata` are exposed as properties, returning
-    single values or aggregated collections of objects.
-    """
-
-    __metadata_properties__ = [
-        ('mzTab-version', 'version', ()),
-        ('mzTab-mode', 'mode', 'P'),
-        ('mzTab-type', 'type', 'P'),
-        ('mzTab-ID', 'id', 'M'),
-        'title',
-        'description',
-        ('ms_run[]', 'ms_runs', 'MP'),
-        ('instrument[]', 'instruments', ()),
-        ('software[]', 'software', ()),
-        ('publication[]', 'publications', ()),
-        ('contact[]', 'contacts', ()),
-        ('uri[]', 'uris', ()),
-        ('external_study_uri[]', 'external_study_uris', ()),
-        ('quantification_method', 'quantification_method', 'M'),
-        ('sample[]', 'samples', ()),
-        ('assay[]', 'assays', ()),
-        ('study_variable[]', 'study_variables', 'M'),
-        ('custom[]', 'custom', ()),
-        ('cv[]', 'cvs', 'M'),
-        ('database[]', 'databases', 'M'),
-
-        ('psm_search_engine_score[]', 'psm_search_engine_scores', ()),
-        ('protein_search_engine_score[]', 'protein_search_engine_scores', ()),
-        ('fixed_mod[]', 'fixed_mods', 'P'),
-        ('variable_mod[]', 'variable_mods', 'P'),
-        'colunit_protein',
-        'colunit_peptide',
-        'colunit_psm',
-        'colunit_small_molecule',
-        'false_discovery_rate',
-
-        ('derivatization_agent[]', 'derivatization_agents', ()),
-        ('small_molecule-quantification_unit',
-         'small_molecule_quantification_unit', 'M'),
-        ('small_molecule_feature-quantification_unit', 'small_molecule_feature_quantification_unit', 'M'),
-        ('small_molecule-identification_reliability',
-         'small_molecule_identification_reliability', ()),
-        ('id_confidence_measure[]', 'id_confidence_measures', 'M'),
-        ('colunit-small_molecule', 'colunit_small_molecule', ()),
-        ('colunit-small_molecule_feature', 'colunit_small_molecule_feature', ()),
-        ('colunit-small_molecule_evidence', 'colunit_small_molecule_evidence', ()),
-
-        ('sample_processing[]', 'sample_processing', ())
-    ]
-
-    def __init__(self, path, encoding='utf8', table_format=DATA_FRAME_FORMAT):
-        if table_format == DATA_FRAME_FORMAT:
-            _require_pandas()
-        # Must be defined in order for metadata properties to work
-        self.variant = None
-        self.file = _file_obj(path, mode='r', encoding=encoding)
-        self.metadata = OrderedDict()
-        self.comments = []
-        self._table_format = table_format
-        self._init_tables()
-        self._parse()
-        self._determine_schema_version()
-        self._transform_tables()
-
-    @property
-    def table_format(self):
-        return self._table_format
-
-    def __getitem__(self, key):
-        key = key.lower().strip()
-        if key in ('psm', ):
-            return self.spectrum_match_table
-        if key in ('pep', ):
-            return self.peptide_table
-        if key in ('prt', ):
-            return self.protein_table
-        if key in ('sml', ):
-            return self.small_molecule_table
-        if key in ('smf', ):
-            return self.small_molecule_feature_table
-        if key in ('sme', ):
-            return self.small_molecule_evidence_table
-        else:
-            raise KeyError(key)
-
-    def __iter__(self):
-        if self.variant == "P":
-            yield 'PRT', self.protein_table
-            yield 'PEP', self.peptide_table
-            yield 'PSM', self.spectrum_match_table
-            yield 'SML', self.small_molecule_table
-        elif self.variant == "M":
-            yield 'SML', self.small_molecule_table
-            yield 'SMF', self.small_molecule_feature_table
-            yield 'SME', self.small_molecule_evidence_table
-
-    def _init_tables(self):
-        self.protein_table = _MzTabTable("protein")
-        self.peptide_table = _MzTabTable("peptide")
-        self.spectrum_match_table = _MzTabTable('psm')
-        self.small_molecule_table = _MzTabTable('small molecule')
-        self.small_molecule_feature_table = _MzTabTable('small molecule feature')
-        self.small_molecule_evidence_table = _MzTabTable('small molecule evidence')
-
-    def _transform_tables(self):
-        if self._table_format == DATA_FRAME_FORMAT:
-            self.protein_table = self.protein_table.as_df('accession')
-            self.peptide_table = self.peptide_table.as_df()
-            self.spectrum_match_table = self.spectrum_match_table.as_df('PSM_ID')
-            self.small_molecule_table = self.small_molecule_table.as_df()
-            self.small_molecule_feature_table = self.small_molecule_feature_table.as_df()
-            self.small_molecule_evidence_table = self.small_molecule_evidence_table.as_df()
-        elif self._table_format in (DICT_FORMAT, dict):
-            self.protein_table = self.protein_table.as_dict()
-            self.peptide_table = self.peptide_table.as_dict()
-            self.spectrum_match_table = self.spectrum_match_table.as_dict()
-            self.small_molecule_table = self.small_molecule_table.as_dict()
-            self.small_molecule_feature_table = self.small_molecule_feature_table.as_dict()
-            self.small_molecule_evidence_table = self.small_molecule_evidence_table.as_dict()
-        elif callable(self._table_format):
-            self.protein_table = self._table_format(self.protein_table)
-            self.peptide_table = self._table_format(self.peptide_table)
-            self.spectrum_match_table = self._table_format(self.spectrum_match_table)
-            self.small_molecule_table = self._table_format(self.small_molecule_table)
-            self.small_molecule_feature_table = self._table_format(self.small_molecule_feature_table)
-            self.small_molecule_evidence_table = self._table_format(self.small_molecule_evidence_table)
-
-    def _parse(self):
-        for i, line in enumerate(self.file):
-            line = line.strip()
-            tokens = line.split("\t")
-            if not tokens:
-                continue
-            if tokens[0] == ("MTD"):
-                name = tokens[1]
-                value = self._cast_value(tokens[2])
-                self.metadata[name] = value
-            elif tokens[0] == 'COM':
-                self.comments.append(self._cast_value(tokens[1]))
-            # headers
-            elif tokens[0] == "PRH":
-                self.protein_table.header = tokens[1:]
-            elif tokens[0] == "PEH":
-                self.peptide_table.header = tokens[1:]
-            elif tokens[0] == "PSH":
-                self.spectrum_match_table.header = tokens[1:]
-            elif tokens[0] == "SMH":
-                self.small_molecule_table.header = tokens[1:]
-            elif tokens[0] == "SFH":
-                self.small_molecule_feature_table.header = tokens[1:]
-            elif tokens[0] == "SEH":
-                self.small_molecule_evidence_table.header = tokens[1:]
-            # rows
-            elif tokens[0] == "PRT":
-                self.protein_table.add(tokens[1:])
-            elif tokens[0] == "PEP":
-                self.peptide_table.add(tokens[1:])
-            elif tokens[0] == "PSM":
-                self.spectrum_match_table.add(tokens[1:])
-            elif tokens[0] == "SML":
-                self.small_molecule_table.add(tokens[1:])
-            elif tokens[0] == "SMF":
-                self.small_molecule_feature_table.add(tokens[1:])
-            elif tokens[0] == "SME":
-                self.small_molecule_evidence_table.add(tokens[1:])
-
-    def _determine_schema_version(self):
-        if self.version is not None:
-            version = str(self.version)
-        else:
-            warnings.warn("The mzTab-version metadata header was missing. Assuming the schema version is 1.0.0")
-            version = "1.0.0"
-            self.version = version
-        match = re.search(r"(?P<schema_version>\d+(?:\.\d+(?:\.\d+)?)?)(?:-(?P<schema_variant>[MP]))?", version)
-        if match is None:
-            warnings.warn("mzTab-version does not match the expected pattern: %r" % version)
-            version_parsed = '1.0.0'
-            variant = 'P'
-        else:
-            version_parsed, variant = match.groups()
-        if variant is None:
-            variant = "P"
-        self.num_version = [int(v) for v in version_parsed.split(".")]
-        # Ensure self.num_version is 3-tuple
-        while len(self.num_version) < 3:
-            self.num_version.append(0)
-        self.variant = variant
-
-    def keys(self):
-        return OrderedDict(list(self)).keys()
-
-    def values(self):
-        return OrderedDict(list(self)).values()
-
-    def items(self):
-        return OrderedDict(list(self)).items()
+"""
+mztab - mzTab file reader
+=========================
+
+Summary
+-------
+
+`mzTab <https://github.com/HUPO-PSI/mzTab>`_  is one of the standards
+developed by the Proteomics Informatics working group of the HUPO Proteomics
+Standard Initiative.
+
+This module provides a way to read mzTab files into a collection of
+:py:class:`pandas.DataFrame` instances in memory, along with a mapping
+of the file-level metadata. MzTab specifications 1.0 and 2.0 are supported.
+
+Data access
+-----------
+
+  :py:class:`MzTab` - a class representing a single mzTab file.
+
+Helpers
+-------
+
+    :py:class:`Group` - a collection of metadata relating to one entity.
+
+
+Internals
+---------
+
+    :py:class:`_MzTabTable` - a single table in an mzTab file.
+
+
+Property Management
+~~~~~~~~~~~~~~~~~~~
+
+:mod:`mztab` uses metaprogramming to generate its metadata accessors, generated by
+these classes working in concert.
+
+    :py:class:`MetadataBackedProperty`
+
+    :py:class:`MetadataBackedCollection`
+
+    :py:class:`MetadataPropertyAnnotator`
+
+-------------------------------------------------------------------------------
+"""
+
+import re
+import warnings
+
+try:
+    import pandas as pd
+except ImportError:
+    pd = None
+
+
+from collections import OrderedDict
+
+from pyteomics.auxiliary import _file_obj
+from pyteomics.auxiliary import cvstr
+from pyteomics.auxiliary.utils import add_metaclass
+
+
+def _require_pandas():
+    if pd is None:
+        raise ImportError(
+            "To load an mzTab file into pandas.DataFrame objects, you must install pandas!")
+
+
+class MetadataBackedProperty(object):
+    '''Our descriptor type which uses the instance's metadata attribute to carry its values'''
+
+    def __init__(self, name, variant_required=None):
+        if variant_required is None:
+            variant_required = ()
+        self.name = name
+        self.variant_required = variant_required
+        self.__doc__ = self.build_docstring()
+
+    def __repr__(self):
+        return "{self.__class__.__name__}(name={self.name!r}, variant_required={self.variant_required})".format(self=self)
+
+    def __get__(self, obj, objtype=None):
+        if obj is None and objtype is not None:
+            # So the property can be seen for what it is
+            return self
+        value = obj.metadata.get(self.name)
+        if value is None and self.variant_required and obj.variant in self.variant_required:
+            raise AttributeError("{0} is missing from a mzTab-\"{1}\" document where it is required!".format(
+                self.name, obj.variant))
+        return value
+
+    def __set__(self, obj, value):
+        obj.metadata[self.name] = value
+
+    def __delete__(self, obj):
+        del obj.metadata[self.name]
+
+    def build_docstring(self):
+        doc = '''Accesses the {self.name!r} key in the :attr:`metadata` mapping attached
+to this object.
+'''
+        if self.variant_required:
+            if len(self.variant_required) > 1:
+                plural = 's'
+            else:
+                plural = ''
+            requires = ' or '.join(['-%s' % v for v in self.variant_required])
+            doc += '''
+This key must be present when the file is of {requires} variant{plural}.
+        '''.format(requires=requires, plural=plural)
+        doc += '''
+Returns
+-------
+object
+        '''
+        doc = doc.format(self=self)
+        return doc
+
+
+class MetadataBackedCollection(object):
+    def __init__(self, name, variant_required=None):
+        if variant_required is None:
+            variant_required = ()
+        self.name = name
+        self.variant_required = variant_required
+        self.__doc__ = self.build_docstring()
+
+    def __get__(self, obj, objtype=None):
+        if obj is None and objtype is not None:
+            # So the property can be seen for what it is
+            return self
+        groups = obj.gather(obj.metadata)
+        value = groups.get(self.name)
+        if value is None and self.variant_required and obj.variant in self.variant_required:
+            raise AttributeError("{0} is missing from a mzTab-\"{1}\" document where it is required!".format(
+                self.name, obj.variant))
+        return value
+
+    def build_docstring(self):
+        doc = '''Accesses the {self.name!r} key group gathered in the :attr:`metadata` mapping attached
+to this object.
+
+This group is dynamically generated on each access and may be expensive for repeated use.
+'''
+        if self.variant_required:
+            if len(self.variant_required) > 1:
+                plural = 's'
+            else:
+                plural = ''
+            requires = ' or '.join(['-%s' % v for v in self.variant_required])
+            doc += '''
+This key must be present when the file is of {requires} variant{plural}.
+        '''.format(requires=requires, plural=plural)
+        doc += '''
+Returns
+-------
+:class:`~.Group`
+        '''
+        doc = doc.format(self=self)
+        return doc
+
+
+class MetadataPropertyAnnotator(type):
+    '''A simple metaclass to do some class-creation time introspection
+    and descriptor binding.
+
+    Uses a list of strings or 3-tuples from :attr:`__metadata_properties__` to
+    bind :class:`MetadataBackedProperty` or :class:`MetadataBackedCollection`
+    onto the class during its creation.
+
+    The specification for a property is a tuple of three values:
+        1. The metadata key to fetch
+        2. The property name to expose on the object
+        3. The variant(s) which require this metadata key be present
+
+    :obj:`("mzTab-version", "version", ("M", "P"))` would be interpreted as
+    Expose a property "version" on instances which serves the key "mzTab-version"
+    from the instance's :attr:`metadata`, and raise an error if it is absent in
+    the "M" or "P" variants.
+
+    Alternatively a specification may be a single string which will be interpreted
+    as the metadata key, and used to generate the property name replacing all '-'
+    with '_' and assumed to be optional in all variants.
+
+    If a metadata key ends with "[]" the property is assumed to be a collection. mzTab
+    makes heavy use of "<collection_name>[<index>]..." keys to define groups of homogenous
+    object types, often with per-element attributes.
+
+    .. code-block::
+
+        variable_mod[1]    CHEMMOD:15.9949146221
+        variable_mod[1]-site  M
+        variable_mod[1]-position    Anywhere
+        variable_mod[2]    CHEMMOD:42.0105646863
+        variable_mod[2]-site  N-term
+        variable_mod[2]-position Protein N-term
+
+    A specification :obj:`("variable_mod[]", "variable_mods", ())` would create a property
+    that returns:
+
+    .. code-block:: python
+
+        >>>instance.variable_mods
+        Group([(1,
+                    {'name': 'CHEMMOD:15.9949146221',
+                     'position': 'Anywhere',
+                     'site': 'M'}),
+                (2,
+                    {'name': 'CHEMMOD:42.0105646863',
+                     'position': 'Protein N-term',
+                     'site': 'N-term'})])
+
+    For precise description of the property collection algorithm, see
+    :meth:`~_MzTabParserBase.collapse_properties` and
+    :meth:`~_MzTabParserBase.gather`.
+
+    If any base classes have a :attr:`__metadata_properties__` attribute, it will
+    also be included unless :attr:`__inherit_metadata_properties__` is set to
+    :const:`False`. Any names explicitly set by the current class override this
+    automatic property generation.
+    '''
+    def __new__(mcls, name, bases, attrs):
+        props = attrs.get('__metadata_properties__', [])
+        inherit_props = attrs.get("__inherit_metadata_properties__", True)
+        # Gather from parent classes so we can use inheritance for overriding this
+        # behavior too.
+        if inherit_props:
+            for base in bases:
+                props.extend(getattr(base, '__metadata_properties__', []))
+
+        keys = set(attrs)
+
+        # Iterate in reverse to ensure that classes nearer to the new classes override
+        # more basal classes, ending with the new class to make sure overrides are
+        # applied.
+        for prop in reversed(props):
+            # If the property definition is a single string, interpret the specification
+            # as the property name, and apply some simple normalization to make it a valid
+            # Python attribute name and assume the property is always optional.
+            if isinstance(prop, str):
+                prop_name = prop
+                attr_name = prop_name.replace("mzTab-", '').replace('-', '_')
+                variant_required = None
+            else:
+                # Otherwise unpack the triple
+                prop_name, attr_name, variant_required = prop
+            # Attach the new descriptor to the class definition to be created. These descriptors
+            # will then be used when instances of that class try to get/set those attribute names.
+            if attr_name in keys:
+                continue
+            if prop_name.endswith('[]'):
+                # If the property name ends with "[]", then we're dealing with a collection so
+                # use the :class:`MetadataBackedCollection` descriptor
+                attrs[attr_name] = MetadataBackedCollection(
+                    prop_name[:-2], variant_required=variant_required)
+            else:
+                # Otherwise it is a scalar-valued property, using the :class:`MetadataBackedProperty`
+                # descriptor
+                prop = attrs[attr_name] = MetadataBackedProperty(
+                    prop_name, variant_required=variant_required)
+
+        return super(MetadataPropertyAnnotator, mcls).__new__(mcls, name, bases, attrs)
+
+
+class _MzTabParserBase(object):
+    def _parse_param(self, tuplet):
+        """Parse a controlled vocabulary or user specified parameter tuplet
+        into a Python object
+
+        Parameters
+        ----------
+        tuplet : str
+            A square brace enclosed tuplet of values describing the parameter
+
+        Returns
+        -------
+        tuple
+            The reduced representation of the parameter
+        """
+        cv, acc, name, value = re.split(r"\s*,\s*", tuplet[1:-1])
+        param_name = cvstr(name, acc)
+        if value:
+            return (param_name, value)
+        else:
+            return (param_name)
+
+    def collapse_properties(self, proplist):
+        '''Collapse a flat property list into a hierchical structure.
+
+        This is intended to operate on :py:class:`Mapping` objects, including
+        :class:`dict`, :class:`pandas.Series` and :class:`pandas.DataFrame`.
+
+        .. code-block:: python
+
+            {
+              "ms_run[1]-format": "Andromeda:apl file format",
+              "ms_run[1]-location": "file://...",
+              "ms_run[1]-id_format": "scan number only nativeID format"
+            }
+
+        to
+
+        .. code-block:: python
+
+            {
+              "ms_run": [
+                {
+                  "format": "Andromeda:apl file format",
+                  "location": "file://...",
+                  "id_format": "scan number only nativeID format"
+                }
+              ]
+            }
+
+        Parameters
+        ----------
+        proplist: :class:`Mapping`
+            Key-Value pairs to collapse
+
+        Returns
+        -------
+        :class:`OrderedDict`:
+            The collapsed property list
+        '''
+        entities = OrderedDict()
+        rest = {}
+        for key, value in proplist.items():
+            try:
+                entity, prop_name = key.rsplit("-", 1)
+            except ValueError:
+                rest[key] = value
+                continue
+            try:
+                entity_dict = entities[entity]
+            except KeyError:
+                entity_dict = entities[entity] = {}
+            entity_dict[prop_name] = value
+        for key, value in proplist.items():
+            if key in entities:
+                entity = entities[key]
+                if 'name' not in entity:
+                    entity['name'] = value
+        for key, value in rest.items():
+            if key in entities:
+                entities[key]['name'] = value
+            else:
+                entities[key] = value
+        return entities
+
+    def _collapse_collections(self, entities):
+        gathered = Group()
+        for key, props in entities.items():
+            if '[' in key:
+                k, ix = key.split('[', 1)
+                if '[' in ix:
+                    # If we have multiple [ in a key, we are dealing with a path
+                    path = extract_path(key)
+                    for k, ix in path[:-1]:
+                        store = gathered[k]
+                        store = store[int(ix)]
+                    k, ix = path[-1]
+                    store[k][int(ix)] = props
+
+                else:
+                    ix = int(ix[:-1])
+                    gathered[k][ix] = props
+            else:
+                gathered[key] = props
+        return gathered
+
+    def _cast_value(self, value):
+        """Convert a cell value to the appropriate Python type
+
+        Parameters
+        ----------
+        value : str
+            The cell value as text
+
+        Returns
+        -------
+        object
+            The most specialized type recognized
+        """
+        if value == 'null':
+            return None
+        # is it a parameter?
+        if value.startswith("["):
+            try:
+                if "|" in value:
+                    return [self._cast_value(v) for v in value.split("|")]
+                else:
+                    return self._parse_param(value)
+            except ValueError:
+                return value
+        else:
+            # begin guessing dtype
+            try:
+                value = int(value)
+            except ValueError:
+                try:
+                    value = float(value)
+                except ValueError:
+                    pass
+            return value
+
+    def gather(self, mapping):
+        '''Collapse property lists using :meth:`collapse_properties`
+        and then gather collections of entites into lists.
+
+        Parameters
+        ----------
+        mapping : dict
+            The flattened hierarchy of properties to re-construct
+
+        Returns
+        -------
+        Group :
+            A :class:`Group` of all entities and collections of entities
+        '''
+        return self._collapse_collections(self.collapse_properties(mapping))
+
+
+class _MzTabTable(_MzTabParserBase):
+
+    """An internal class for accumulating information about an single table
+    represented in an mzTab file
+
+    Attributes
+    ----------
+    header : list
+        The column names for the table
+    name : str
+        The table's name, human readable
+    rows : list
+        An accumulator of table rows
+    """
+
+    def __init__(self, name, header=None, rows=None):
+        if rows is None:
+            rows = []
+        self.name = name
+        self.header = header
+        self.rows = rows
+
+    def __repr__(self):
+        n_cols = len(self.header) if self.header is not None else 0
+        n_rows = len(self.rows)
+        template = "<_MzTabTable {name} with {n_cols} columns and {n_rows} rows>"
+        return template.format(n_cols=n_cols, n_rows=n_rows, name=self.name)
+
+    def add(self, row):
+        self.rows.append([self._cast_value(v) for v in row])
+
+    def __len__(self):
+        return len(self.rows)
+
+    def __getitem__(self, i):
+        if isinstance(i, int):
+            return self.gather({h: r for h, r in zip(self.header, self.rows[i])})
+        elif isinstance(i, slice):
+            out = []
+            for i in range(i.start or 0, i.stop or len(self), i.step or 1):
+                out.append(self[i])
+            return out
+        raise TypeError("Cannot access table with object of type %r" % type(i))
+
+    def as_dict(self):
+        return {"rows": [dict(zip(self.header, row)) for row in self.rows],
+                "name": self.name}
+
+    def as_df(self, index=None):
+        """Convert the table to a DataFrame in memory.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        _require_pandas()
+        table = pd.DataFrame(data=self.rows, columns=self.header)
+        if index is not None and len(table.index) > 0:
+            table = table.set_index(index, drop=False)
+        table.name = self.name
+        return table
+
+    def clear(self):
+        self.header = None
+        self.rows = []
+
+
+DATA_FRAME_FORMAT = 'df'
+DICT_FORMAT = 'dict'
+RAW_FORMAT = 'raw'
+
+PATH_PARSER = re.compile(r"([^\[]+)\[(\d+)\]_?")
+
+
+def extract_path(path):
+    '''Parse `key[index]_next_key[next_index]...` sequences into
+    lists of (key, index) pairs.
+
+    Parameters
+    ----------
+    path : str
+        The path key to parse
+
+    Returns
+    -------
+    list
+    '''
+    return [(t, int(i)) for t, i in PATH_PARSER.findall(path)]
+
+
+class Group(OrderedDict):
+    '''A type for holding collections of arbitrarily nested keys from rows
+    and metadata mappings.
+
+    Implemented as an autovivifying :class:`OrderedDict` variant. As such implements
+    the :class:`~collections.abc.Mapping` interface.
+    '''
+
+    def get_path(self, path, default=None):
+        '''As :meth:`get` but over a path key parsed with :func:`extract_path`.
+
+        Parameters
+        ----------
+        path : str
+            The path to search down
+        default : object, optional
+            The return value when the path is missing
+
+        Returns
+        -------
+        object
+        '''
+        tokens = extract_path(path)
+        if not tokens:
+            return self.get(path, default)
+        layer = self
+        for k, i in tokens[:-1]:
+            i = int(i)
+            layer = layer.get(k)
+            if layer is None:
+                return None
+            layer = layer.get(i)
+            if layer is None:
+                return None
+        k, i = tokens[-1]
+        i = int(i)
+        layer = layer.get(k)
+        if layer is None:
+            return default
+        value = layer.get(i, default)
+        return value
+
+    def __missing__(self, key):
+        value = self.__class__()
+        self[key] = value
+        return value
+
+
+@add_metaclass(MetadataPropertyAnnotator)
+class MzTab(_MzTabParserBase):
+    """Parser for mzTab format files.
+
+    Attributes
+    ----------
+    comments : list
+        A list of comments across the file
+    file : _file_obj
+        A file stream wrapper for the file to be read
+    metadata : OrderedDict
+        A mapping of metadata that was entities.
+    peptide_table : _MzTabTable or pd.DataFrame
+        The table of peptides. Not commonly used.
+    protein_table : _MzTabTable or pd.DataFrame
+        The table of protein identifications.
+    small_molecule_table : _MzTabTable or pd.DataFrame
+        The table of small molecule identifications.
+    spectrum_match_table : _MzTabTable or pd.DataFrame
+        The table of spectrum-to-peptide match identifications.
+    table_format: 'df', 'dict', or callable
+        The structure type to replace each table with. The string
+        'df' will use pd.DataFrame instances. 'dict' will create
+        a dictionary of dictionaries for each table. A callable
+        will be called on each raw _MzTabTable object
+
+    Additional components of :attr:`metadata` are exposed as properties, returning
+    single values or aggregated collections of objects.
+    """
+
+    __metadata_properties__ = [
+        ('mzTab-version', 'version', ()),
+        ('mzTab-mode', 'mode', 'P'),
+        ('mzTab-type', 'type', 'P'),
+        ('mzTab-ID', 'id', 'M'),
+        'title',
+        'description',
+        ('ms_run[]', 'ms_runs', 'MP'),
+        ('instrument[]', 'instruments', ()),
+        ('software[]', 'software', ()),
+        ('publication[]', 'publications', ()),
+        ('contact[]', 'contacts', ()),
+        ('uri[]', 'uris', ()),
+        ('external_study_uri[]', 'external_study_uris', ()),
+        ('quantification_method', 'quantification_method', 'M'),
+        ('sample[]', 'samples', ()),
+        ('assay[]', 'assays', ()),
+        ('study_variable[]', 'study_variables', 'M'),
+        ('custom[]', 'custom', ()),
+        ('cv[]', 'cvs', 'M'),
+        ('database[]', 'databases', 'M'),
+
+        ('psm_search_engine_score[]', 'psm_search_engine_scores', ()),
+        ('protein_search_engine_score[]', 'protein_search_engine_scores', ()),
+        ('fixed_mod[]', 'fixed_mods', 'P'),
+        ('variable_mod[]', 'variable_mods', 'P'),
+        'colunit_protein',
+        'colunit_peptide',
+        'colunit_psm',
+        'colunit_small_molecule',
+        'false_discovery_rate',
+
+        ('derivatization_agent[]', 'derivatization_agents', ()),
+        ('small_molecule-quantification_unit',
+         'small_molecule_quantification_unit', 'M'),
+        ('small_molecule_feature-quantification_unit', 'small_molecule_feature_quantification_unit', 'M'),
+        ('small_molecule-identification_reliability',
+         'small_molecule_identification_reliability', ()),
+        ('id_confidence_measure[]', 'id_confidence_measures', 'M'),
+        ('colunit-small_molecule', 'colunit_small_molecule', ()),
+        ('colunit-small_molecule_feature', 'colunit_small_molecule_feature', ()),
+        ('colunit-small_molecule_evidence', 'colunit_small_molecule_evidence', ()),
+
+        ('sample_processing[]', 'sample_processing', ())
+    ]
+
+    def __init__(self, path, encoding='utf8', table_format=DATA_FRAME_FORMAT):
+        if table_format == DATA_FRAME_FORMAT:
+            _require_pandas()
+        # Must be defined in order for metadata properties to work
+        self.variant = None
+        self.file = _file_obj(path, mode='r', encoding=encoding)
+        self.metadata = OrderedDict()
+        self.comments = []
+        self._table_format = table_format
+        self._init_tables()
+        self._parse()
+        self._determine_schema_version()
+        self._transform_tables()
+
+    @property
+    def table_format(self):
+        return self._table_format
+
+    def __getitem__(self, key):
+        key = key.lower().strip()
+        if key in ('psm', ):
+            return self.spectrum_match_table
+        if key in ('pep', ):
+            return self.peptide_table
+        if key in ('prt', ):
+            return self.protein_table
+        if key in ('sml', ):
+            return self.small_molecule_table
+        if key in ('smf', ):
+            return self.small_molecule_feature_table
+        if key in ('sme', ):
+            return self.small_molecule_evidence_table
+        else:
+            raise KeyError(key)
+
+    def __iter__(self):
+        if self.variant == "P":
+            yield 'PRT', self.protein_table
+            yield 'PEP', self.peptide_table
+            yield 'PSM', self.spectrum_match_table
+            yield 'SML', self.small_molecule_table
+        elif self.variant == "M":
+            yield 'SML', self.small_molecule_table
+            yield 'SMF', self.small_molecule_feature_table
+            yield 'SME', self.small_molecule_evidence_table
+
+    def _init_tables(self):
+        self.protein_table = _MzTabTable("protein")
+        self.peptide_table = _MzTabTable("peptide")
+        self.spectrum_match_table = _MzTabTable('psm')
+        self.small_molecule_table = _MzTabTable('small molecule')
+        self.small_molecule_feature_table = _MzTabTable('small molecule feature')
+        self.small_molecule_evidence_table = _MzTabTable('small molecule evidence')
+
+    def _transform_tables(self):
+        if self._table_format == DATA_FRAME_FORMAT:
+            self.protein_table = self.protein_table.as_df('accession')
+            self.peptide_table = self.peptide_table.as_df()
+            self.spectrum_match_table = self.spectrum_match_table.as_df('PSM_ID')
+            self.small_molecule_table = self.small_molecule_table.as_df()
+            self.small_molecule_feature_table = self.small_molecule_feature_table.as_df()
+            self.small_molecule_evidence_table = self.small_molecule_evidence_table.as_df()
+        elif self._table_format in (DICT_FORMAT, dict):
+            self.protein_table = self.protein_table.as_dict()
+            self.peptide_table = self.peptide_table.as_dict()
+            self.spectrum_match_table = self.spectrum_match_table.as_dict()
+            self.small_molecule_table = self.small_molecule_table.as_dict()
+            self.small_molecule_feature_table = self.small_molecule_feature_table.as_dict()
+            self.small_molecule_evidence_table = self.small_molecule_evidence_table.as_dict()
+        elif callable(self._table_format):
+            self.protein_table = self._table_format(self.protein_table)
+            self.peptide_table = self._table_format(self.peptide_table)
+            self.spectrum_match_table = self._table_format(self.spectrum_match_table)
+            self.small_molecule_table = self._table_format(self.small_molecule_table)
+            self.small_molecule_feature_table = self._table_format(self.small_molecule_feature_table)
+            self.small_molecule_evidence_table = self._table_format(self.small_molecule_evidence_table)
+
+    def _parse(self):
+        for i, line in enumerate(self.file):
+            line = line.strip()
+            tokens = line.split("\t")
+            if not tokens:
+                continue
+            if tokens[0] == ("MTD"):
+                name = tokens[1]
+                value = self._cast_value(tokens[2])
+                self.metadata[name] = value
+            elif tokens[0] == 'COM':
+                self.comments.append(self._cast_value(tokens[1]))
+            # headers
+            elif tokens[0] == "PRH":
+                self.protein_table.header = tokens[1:]
+            elif tokens[0] == "PEH":
+                self.peptide_table.header = tokens[1:]
+            elif tokens[0] == "PSH":
+                self.spectrum_match_table.header = tokens[1:]
+            elif tokens[0] == "SMH":
+                self.small_molecule_table.header = tokens[1:]
+            elif tokens[0] == "SFH":
+                self.small_molecule_feature_table.header = tokens[1:]
+            elif tokens[0] == "SEH":
+                self.small_molecule_evidence_table.header = tokens[1:]
+            # rows
+            elif tokens[0] == "PRT":
+                self.protein_table.add(tokens[1:])
+            elif tokens[0] == "PEP":
+                self.peptide_table.add(tokens[1:])
+            elif tokens[0] == "PSM":
+                self.spectrum_match_table.add(tokens[1:])
+            elif tokens[0] == "SML":
+                self.small_molecule_table.add(tokens[1:])
+            elif tokens[0] == "SMF":
+                self.small_molecule_feature_table.add(tokens[1:])
+            elif tokens[0] == "SME":
+                self.small_molecule_evidence_table.add(tokens[1:])
+
+    def _determine_schema_version(self):
+        if self.version is not None:
+            version = str(self.version)
+        else:
+            warnings.warn("The mzTab-version metadata header was missing. Assuming the schema version is 1.0.0")
+            version = "1.0.0"
+            self.version = version
+        match = re.search(r"(?P<schema_version>\d+(?:\.\d+(?:\.\d+)?)?)(?:-(?P<schema_variant>[MP]))?", version)
+        if match is None:
+            warnings.warn("mzTab-version does not match the expected pattern: %r" % version)
+            version_parsed = '1.0.0'
+            variant = 'P'
+        else:
+            version_parsed, variant = match.groups()
+        if variant is None:
+            variant = "P"
+        self.num_version = [int(v) for v in version_parsed.split(".")]
+        # Ensure self.num_version is 3-tuple
+        while len(self.num_version) < 3:
+            self.num_version.append(0)
+        self.variant = variant
+
+    def keys(self):
+        return OrderedDict(list(self)).keys()
+
+    def values(self):
+        return OrderedDict(list(self)).values()
+
+    def items(self):
+        return OrderedDict(list(self)).items()
```

### Comparing `pyteomics-4.5.6/pyteomics/mzxml.py` & `pyteomics-4.6/pyteomics/mzxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                         break
                     yield item
         while self.queue:
             idx, item = heapq.heappop(self.queue)
             yield item
 
 
-class MzXML(xml.ArrayConversionMixin, aux.TimeOrderedIndexedReaderMixin, xml.MultiProcessingXML, xml.IndexSavingXML):
+class MzXML(aux.BinaryArrayConversionMixin, aux.TimeOrderedIndexedReaderMixin, xml.MultiProcessingXML, xml.IndexSavingXML):
     """Parser class for mzXML files."""
     _root_element = 'mzXML'
     _default_iter_tag = 'scan'
     _indexed_tags = {'scan'}
     _indexed_tag_keys = {'scan': 'num'}
     _default_version = None
     _default_schema = _schema_defaults._mzxml_schema_defaults
@@ -219,15 +219,16 @@
             for item in super(MzXML, self).iterfind(path, **kwargs):
                 yield item
 
     def _get_time(self, scan):
         return scan['retentionTime']
 
 
-def read(source, read_schema=False, iterative=True, use_index=False, dtype=None, huge_tree=False):
+def read(source, read_schema=False, iterative=True, use_index=False, dtype=None,
+         huge_tree=False, decode_binary=True):
     """Parse `source` and iterate through spectra.
 
     Parameters
     ----------
     source : str or file
         A path to a target mzML file or the file object itself.
 
@@ -261,15 +262,16 @@
     Returns
     -------
     out : iterator
        An iterator over the dicts with spectrum properties.
     """
 
     return MzXML(source, read_schema=read_schema, iterative=iterative,
-        use_index=use_index, dtype=dtype, huge_tree=huge_tree)
+                 use_index=use_index, dtype=dtype, huge_tree=huge_tree,
+                 decode_binary=decode_binary)
 
 
 def iterfind(source, path, **kwargs):
     """Parse `source` and yield info on elements with specified local
     name or by specified XPath.
 
     .. note:: This function is provided for backward compatibility only.
```

### Comparing `pyteomics-4.5.6/pyteomics/openms/featurexml.py` & `pyteomics-4.6/pyteomics/openms/featurexml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/openms/idxml.py` & `pyteomics-4.6/pyteomics/openms/idxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/openms/trafoxml.py` & `pyteomics-4.6/pyteomics/openms/trafoxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/parser.py` & `pyteomics-4.6/pyteomics/parser.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/peff.py` & `pyteomics-4.6/pyteomics/peff.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,277 +1,277 @@
-"""
-peff - PSI Extended FASTA Format
-================================
-
-PEFF is a forth-coming standard from PSI-HUPO formalizing and extending the
-encoding of protein features and annotations for building search spaces for
-proteomics. See `The PEFF specification <http://www.psidev.info/peff>`_ for
-more up-to-date information on the standard.
-
-Data manipulation
------------------
-
-Classes
-.......
-
-The PEFF parser inherits several properties from implementation in the :mod:`~.fasta` module,
-building on top of the :class:`~.TwoLayerIndexedFASTA` reader.
-
-Available classes:
-
-  :py:class:`IndexedPEFF` - Parse a PEFF format file in binary-mode, supporting
-  direct indexing by header string or by tag.
-
-"""
-
-#   Copyright 2018 Joshua Klein, Lev Levitsky
-#
-#   Licensed under the Apache License, Version 2.0 (the "License");
-#   you may not use this file except in compliance with the License.
-#   You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#   Unless required by applicable law or agreed to in writing, software
-#   distributed under the License is distributed on an "AS IS" BASIS,
-#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#   See the License for the specific language governing permissions and
-#   limitations under the License.
-
-import re
-try:
-    from collections.abc import Sequence as SequenceABC, Mapping
-except ImportError:
-    from collections import Sequence as SequenceABC, Mapping
-from collections import OrderedDict, defaultdict
-
-from .fasta import TwoLayerIndexedFASTA
-
-
-class Header(Mapping):
-    """Hold parsed properties of a key-value pair like a sequence's
-    definition line.
-
-    This object supports the :class:`Mapping` interface, and
-    keys may be accessed by attribute access notation.
-    """
-    def __init__(self, mapping, original=None):
-        self._mapping = mapping
-
-    def __getitem__(self, key):
-        return self._mapping[key]
-
-    def __iter__(self):
-        return iter(self._mapping)
-
-    def items(self):
-        return self._mapping.items()
-
-    def keys(self):
-        return self._mapping.keys()
-
-    def values(self):
-        return self._mapping.values()
-
-    def __len__(self):
-        return len(self._mapping)
-
-    def __contains__(self, key):
-        return key in self._mapping
-
-    def __getattr__(self, key):
-        if key == "_mapping":
-            raise AttributeError(key)
-        try:
-            return self._mapping[key]
-        except KeyError:
-            raise AttributeError(key)
-
-    def __repr__(self):
-        return "{self.__class__.__name__}({mapping})".format(self=self, mapping=dict(self._mapping))
-
-    def __hash__(self):
-        return hash(self.defline)
-
-    def __eq__(self, other):
-        try:
-            return self._mapping == other._mapping
-        except AttributeError:
-            return str(self) == str(other)
-
-    def __ne__(self, other):
-        return not (self == other)
-
-    def __dir__(self):
-        base = set(dir(super(Header, self)))
-        keys = set(self._mapping.keys())
-        return list(base | keys)
-
-
-class IndexedPEFF(TwoLayerIndexedFASTA):
-    """Creates an :py:class:`IndexedPEFF` object.
-
-    Parameters
-    ----------
-    source : str or file
-        The file to read. If a file object, it needs to be in *rb* mode.
-    parse : bool, optional
-        Defines whether the descriptions should be parsed in the produced tuples.
-        Default is :py:const:`True`.
-    kwargs : passed to the :py:class:`TwoLayerIndexedFASTA` constructor.
-    """
-
-    kv_pattern = re.compile(r"\\(?P<key>\S+)=(?P<value>.+?)(?:\s(?=\\)|$)")
-    header_pattern = re.compile(r"^>?(\S+):(\S+)")
-    has_feature_index = re.compile(r"^\(?(\d+):")
-    header_group = 2
-
-    class _PEFFFeature(SequenceABC):
-        def __init__(self, *fields, **kwargs):
-            self.fields = tuple(fields)
-            self.id = kwargs.get('id')
-            self.feature_type = kwargs.get("feature_type")
-
-        def __eq__(self, other):
-            return tuple(self) == tuple(other)
-
-        def __ne__(self, other):
-            return not (self == other)
-
-        def __getitem__(self, i):
-            return self.fields[i]
-
-        def __len__(self):
-            return len(self.fields)
-
-        def __repr__(self):
-            return repr(tuple(self))
-
-        def __str__(self):
-            return "(%s%s)" % (
-                '%r:' % self.id if self.id is not None else '',
-                '|'.join(map(str, self)), )
-
-    def __init__(self, source, ignore_comments=False, **kwargs):
-        super(IndexedPEFF, self).__init__(
-            source, ignore_comments=ignore_comments, parser=self.parser,
-            header_pattern=self.header_pattern, **kwargs)
-        self.header_blocks = []
-        self.comments = []
-        self.version = None
-        self.number_of_entries = 0
-        self._parse_header()
-
-    def _parse_header(self):
-        self.seek(0)
-        line = self.readline().decode("ascii")
-        if not line.startswith("# PEFF"):
-            raise ValueError("Not a PEFF File")
-        self.version = tuple(map(int, line.strip()[7:].split(".")))
-        current_block = defaultdict(list)
-        in_header = True
-        while in_header:
-            line = self.readline().decode("ascii")
-            if not line.startswith("#"):
-                in_header = False
-            line = line.strip()[2:]
-            if '=' in line:
-                key, value = line.split("=", 1)
-                if key == "GeneralComment":
-                    self.comments.append(value)
-                else:
-                    current_block[key].append(value)
-            if line.startswith("//"):
-                if current_block:
-                    self.header_blocks.append(
-                        Header(OrderedDict((k, v if len(v) > 1 else v[0])
-                                           for k, v in current_block.items())))
-                current_block = defaultdict(list)
-        number_of_entries = 0
-        for block in self.header_blocks:
-            try:
-                number_of_entries += int(block['NumberOfEntries'])
-            except KeyError:
-                pass
-        self.number_of_entries = number_of_entries
-
-    def _extract_parenthesis_list(self, text):
-        chunks = []
-        chunk = []
-        paren_level = 0
-        i = 0
-        n = len(text)
-        while i < n:
-            c = text[i]
-            i += 1
-            if c == "(":
-                if paren_level > 0:
-                    chunk.append(c)
-                paren_level += 1
-            elif c == ")":
-                if paren_level > 1:
-                    chunk.append(c)
-                paren_level -= 1
-                if paren_level == 0:
-                    if chunk:
-                        chunks.append(chunk)
-                    chunk = []
-            else:
-                chunk.append(c)
-        chunks = list(map(''.join, chunks))
-        return chunks
-
-    def _split_pipe_separated_tuple(self, text):
-        parts = text.split("|")
-        return parts
-
-    def _coerce_types(self, key, value):
-        value = value.strip()
-        feature_id_match = self.has_feature_index.search(value)
-        if feature_id_match:
-            feature_id = int(feature_id_match.group(1))
-            value = self.has_feature_index.sub('', value)
-        else:
-            feature_id = None
-        if "|" in value:
-            value = self._split_pipe_separated_tuple(value)
-            result = []
-            for i, v in enumerate(value):
-                result.append(self._coerce_value(key, v, i))
-            return self._PEFFFeature(*result, feature_type=key, id=feature_id)
-        else:
-            return self._coerce_value(key, value, 0)
-
-    def _coerce_value(self, key, value, index):
-        try:
-            return int(value)
-        except ValueError:
-            pass
-        try:
-            return float(value)
-        except ValueError:
-            pass
-        return str(value)
-
-    def parser(self, line):
-        match = self.header_pattern.match(line)
-        if not match:
-            raise ValueError(
-                "Failed to parse {!r} using {!r}".format(
-                    line, self))
-        storage = OrderedDict()
-        prefix = None
-        db_uid = None
-        if line.startswith(">"):
-            line = line[1:]
-        prefix, line = line.split(":", 1)
-        db_uid, line = line.split(" ", 1)
-        storage['Prefix'] = prefix
-        storage['Tag'] = db_uid
-        kv_pattern = re.compile(r"\\(?P<key>\S+)=(?P<value>.+?)(?:\s(?=\\)|$)")
-        for key, value in kv_pattern.findall(line):
-            if not (value.startswith("(") or " (" in value):
-                storage[key] = self._coerce_types(key, value)
-            else:
-                # multi-value
-                storage[key] = [self._coerce_types(key, v) for v in self._extract_parenthesis_list(value)]
-        return Header(storage)
+"""
+peff - PSI Extended FASTA Format
+================================
+
+PEFF is a forth-coming standard from PSI-HUPO formalizing and extending the
+encoding of protein features and annotations for building search spaces for
+proteomics. See `The PEFF specification <http://www.psidev.info/peff>`_ for
+more up-to-date information on the standard.
+
+Data manipulation
+-----------------
+
+Classes
+.......
+
+The PEFF parser inherits several properties from implementation in the :mod:`~.fasta` module,
+building on top of the :class:`~.TwoLayerIndexedFASTA` reader.
+
+Available classes:
+
+  :py:class:`IndexedPEFF` - Parse a PEFF format file in binary-mode, supporting
+  direct indexing by header string or by tag.
+
+"""
+
+#   Copyright 2018 Joshua Klein, Lev Levitsky
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
+import re
+try:
+    from collections.abc import Sequence as SequenceABC, Mapping
+except ImportError:
+    from collections import Sequence as SequenceABC, Mapping
+from collections import OrderedDict, defaultdict
+
+from .fasta import TwoLayerIndexedFASTA
+
+
+class Header(Mapping):
+    """Hold parsed properties of a key-value pair like a sequence's
+    definition line.
+
+    This object supports the :class:`Mapping` interface, and
+    keys may be accessed by attribute access notation.
+    """
+    def __init__(self, mapping, original=None):
+        self._mapping = mapping
+
+    def __getitem__(self, key):
+        return self._mapping[key]
+
+    def __iter__(self):
+        return iter(self._mapping)
+
+    def items(self):
+        return self._mapping.items()
+
+    def keys(self):
+        return self._mapping.keys()
+
+    def values(self):
+        return self._mapping.values()
+
+    def __len__(self):
+        return len(self._mapping)
+
+    def __contains__(self, key):
+        return key in self._mapping
+
+    def __getattr__(self, key):
+        if key == "_mapping":
+            raise AttributeError(key)
+        try:
+            return self._mapping[key]
+        except KeyError:
+            raise AttributeError(key)
+
+    def __repr__(self):
+        return "{self.__class__.__name__}({mapping})".format(self=self, mapping=dict(self._mapping))
+
+    def __hash__(self):
+        return hash(self.defline)
+
+    def __eq__(self, other):
+        try:
+            return self._mapping == other._mapping
+        except AttributeError:
+            return str(self) == str(other)
+
+    def __ne__(self, other):
+        return not (self == other)
+
+    def __dir__(self):
+        base = set(dir(super(Header, self)))
+        keys = set(self._mapping.keys())
+        return list(base | keys)
+
+
+class IndexedPEFF(TwoLayerIndexedFASTA):
+    """Creates an :py:class:`IndexedPEFF` object.
+
+    Parameters
+    ----------
+    source : str or file
+        The file to read. If a file object, it needs to be in *rb* mode.
+    parse : bool, optional
+        Defines whether the descriptions should be parsed in the produced tuples.
+        Default is :py:const:`True`.
+    kwargs : passed to the :py:class:`TwoLayerIndexedFASTA` constructor.
+    """
+
+    kv_pattern = re.compile(r"\\(?P<key>\S+)=(?P<value>.+?)(?:\s(?=\\)|$)")
+    header_pattern = re.compile(r"^>?(\S+):(\S+)")
+    has_feature_index = re.compile(r"^\(?(\d+):")
+    header_group = 2
+
+    class _PEFFFeature(SequenceABC):
+        def __init__(self, *fields, **kwargs):
+            self.fields = tuple(fields)
+            self.id = kwargs.get('id')
+            self.feature_type = kwargs.get("feature_type")
+
+        def __eq__(self, other):
+            return tuple(self) == tuple(other)
+
+        def __ne__(self, other):
+            return not (self == other)
+
+        def __getitem__(self, i):
+            return self.fields[i]
+
+        def __len__(self):
+            return len(self.fields)
+
+        def __repr__(self):
+            return repr(tuple(self))
+
+        def __str__(self):
+            return "(%s%s)" % (
+                '%r:' % self.id if self.id is not None else '',
+                '|'.join(map(str, self)), )
+
+    def __init__(self, source, ignore_comments=False, **kwargs):
+        super(IndexedPEFF, self).__init__(
+            source, ignore_comments=ignore_comments, parser=self.parser,
+            header_pattern=self.header_pattern, **kwargs)
+        self.header_blocks = []
+        self.comments = []
+        self.version = None
+        self.number_of_entries = 0
+        self._parse_header()
+
+    def _parse_header(self):
+        self.seek(0)
+        line = self.readline().decode("ascii")
+        if not line.startswith("# PEFF"):
+            raise ValueError("Not a PEFF File")
+        self.version = tuple(map(int, line.strip()[7:].split(".")))
+        current_block = defaultdict(list)
+        in_header = True
+        while in_header:
+            line = self.readline().decode("ascii")
+            if not line.startswith("#"):
+                in_header = False
+            line = line.strip()[2:]
+            if '=' in line:
+                key, value = line.split("=", 1)
+                if key == "GeneralComment":
+                    self.comments.append(value)
+                else:
+                    current_block[key].append(value)
+            if line.startswith("//"):
+                if current_block:
+                    self.header_blocks.append(
+                        Header(OrderedDict((k, v if len(v) > 1 else v[0])
+                                           for k, v in current_block.items())))
+                current_block = defaultdict(list)
+        number_of_entries = 0
+        for block in self.header_blocks:
+            try:
+                number_of_entries += int(block['NumberOfEntries'])
+            except KeyError:
+                pass
+        self.number_of_entries = number_of_entries
+
+    def _extract_parenthesis_list(self, text):
+        chunks = []
+        chunk = []
+        paren_level = 0
+        i = 0
+        n = len(text)
+        while i < n:
+            c = text[i]
+            i += 1
+            if c == "(":
+                if paren_level > 0:
+                    chunk.append(c)
+                paren_level += 1
+            elif c == ")":
+                if paren_level > 1:
+                    chunk.append(c)
+                paren_level -= 1
+                if paren_level == 0:
+                    if chunk:
+                        chunks.append(chunk)
+                    chunk = []
+            else:
+                chunk.append(c)
+        chunks = list(map(''.join, chunks))
+        return chunks
+
+    def _split_pipe_separated_tuple(self, text):
+        parts = text.split("|")
+        return parts
+
+    def _coerce_types(self, key, value):
+        value = value.strip()
+        feature_id_match = self.has_feature_index.search(value)
+        if feature_id_match:
+            feature_id = int(feature_id_match.group(1))
+            value = self.has_feature_index.sub('', value)
+        else:
+            feature_id = None
+        if "|" in value:
+            value = self._split_pipe_separated_tuple(value)
+            result = []
+            for i, v in enumerate(value):
+                result.append(self._coerce_value(key, v, i))
+            return self._PEFFFeature(*result, feature_type=key, id=feature_id)
+        else:
+            return self._coerce_value(key, value, 0)
+
+    def _coerce_value(self, key, value, index):
+        try:
+            return int(value)
+        except ValueError:
+            pass
+        try:
+            return float(value)
+        except ValueError:
+            pass
+        return str(value)
+
+    def parser(self, line):
+        match = self.header_pattern.match(line)
+        if not match:
+            raise ValueError(
+                "Failed to parse {!r} using {!r}".format(
+                    line, self))
+        storage = OrderedDict()
+        prefix = None
+        db_uid = None
+        if line.startswith(">"):
+            line = line[1:]
+        prefix, line = line.split(":", 1)
+        db_uid, line = line.split(" ", 1)
+        storage['Prefix'] = prefix
+        storage['Tag'] = db_uid
+        kv_pattern = re.compile(r"\\(?P<key>\S+)=(?P<value>.+?)(?:\s(?=\\)|$)")
+        for key, value in kv_pattern.findall(line):
+            if not (value.startswith("(") or " (" in value):
+                storage[key] = self._coerce_types(key, value)
+            else:
+                # multi-value
+                storage[key] = [self._coerce_types(key, v) for v in self._extract_parenthesis_list(value)]
+        return Header(storage)
```

### Comparing `pyteomics-4.5.6/pyteomics/pepxml.py` & `pyteomics-4.6/pyteomics/pepxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/proforma.py` & `pyteomics-4.6/pyteomics/proforma.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,16 @@
     @property
     def mass(self):
         return self.value
 
 
 class ModificationResolver(object):
     def __init__(self, name, **kwargs):
-        self.name = name
+        self.name = name.lower()
+        self.symbol = self.name[0]
         self._database = None
 
     def load_database(self):
         raise NotImplementedError()
 
     @property
     def database(self):
@@ -298,14 +299,45 @@
             self._database = self.load_database()
         return self._database
 
     @database.setter
     def database(self, database):
         self._database = database
 
+    def parse_identifier(self, identifier):
+        """Parse a string that is either a CV prefixed identifier or name.
+
+        Parameters
+        ----------
+        identifier : str
+            The identifier string to parse, removing CV prefix as needed.
+
+        Returns
+        -------
+        name : str, optional
+            A textual identifier embedded in the qualified identifier, if any, otherwise
+            :const:`None`.
+        id : int, optional
+            An integer ID embedded in the qualified identifier, if any, otherwise
+            :const:`None`.
+        """
+        tokens = identifier.split(":", 1)
+        if len(tokens) > 1:
+            prefix = tokens[0].lower()
+            if prefix == self.name or prefix == self.symbol:
+                identifier = tokens[1]
+
+        if identifier.isdigit():
+            id = int(identifier)
+            name = None
+        else:
+            name = identifier
+            id = None
+        return name, id
+
     def resolve(self, name=None, id=None, **kwargs):
         raise NotImplementedError()
 
     def __call__(self, name=None, id=None, **kwargs):
         return self.resolve(name, id, **kwargs)
 
     def __eq__(self, other):
@@ -564,14 +596,35 @@
     def __init__(self, resolvers, **kwargs):
         super(GenericResolver, self).__init__('generic', **kwargs)
         self.resolvers = list(resolvers)
 
     def load_database(self):
         return None
 
+    def parse_identifier(self, identifier):
+        """Parse a string that is either a CV prefixed identifier or name.
+
+        Does no parsing as a :class:`GenericModification` is never qualified.
+
+        Parameters
+        ----------
+        identifier : str
+            The identifier string to parse, removing CV prefix as needed.
+
+        Returns
+        -------
+        name : str, optional
+            A textual identifier embedded in the qualified identifier, if any, otherwise
+            :const:`None`.
+        id : int, optional
+            An integer ID embedded in the qualified identifier, if any, otherwise
+            :const:`None`.
+        """
+        return identifier, None
+
     def resolve(self, name=None, id=None, **kwargs):
         defn = None
         for resolver in self.resolvers:
             try:
                 defn = resolver(name=name, id=id, **kwargs)
                 break
             except KeyError:
@@ -686,32 +739,18 @@
 
     def _populate_from_definition(self, definition):
         self._definition = definition
 
     def _format_main(self):
         return "{self.prefix_name}:{self.value}".format(self=self)
 
-    def _parse_identifier(self):
-        tokens = self.value.split(":", 1)
-        if len(tokens) > 1:
-            value = tokens[1]
-        else:
-            value = self.value
-        if value.isdigit():
-            id = int(value)
-            name = None
-        else:
-            name = value
-            id = None
-        return name, id
-
     def resolve(self):
         '''Find the term and return it's properties
         '''
-        keys = self._parse_identifier()
+        keys = self.resolver.parse_identifier(self.value)
         return self.resolver(*keys)
 
 
 class FormulaModification(ModificationBase):
     prefix_name = "Formula"
 
     isotope_pattern = re.compile(r'\[(?P<isotope>\d+)(?P<element>[A-Z][a-z]*)(?P<quantity>[\-+]?\d+)\]')
@@ -889,15 +928,15 @@
     def _format_main(self):
         return self.value
 
     def resolve(self):
         '''Find the term, searching through all available vocabularies and
         return the first match's properties
         '''
-        keys = self._parse_identifier()
+        keys = self.resolver.parse_identifier(self.value)
         defn = self.resolver(*keys)
         if defn is not None:
             return defn
         raise KeyError(keys)
 
 
 def set_unimod_path(path):
@@ -1099,16 +1138,21 @@
     elif main_tag[0] == '#':
         main_tag = process_marker(main_tag)
     else:
         prefix, value = find_prefix(main_tag)
         if prefix is None:
             main_tag = GenericModification(''.join(value))
         else:
-            tag_type = TagBase.find_by_tag(prefix)
-            main_tag = tag_type(value)
+            try:
+                tag_type = TagBase.find_by_tag(prefix)
+                main_tag = tag_type(value)
+            except KeyError:
+                main_tag_str = ''.join(main_tag)
+                main_tag = GenericModification(main_tag_str)
+
     if len(parts) > 1:
         extras = []
         for part in parts[1:]:
             prefix, value = find_prefix(part)
             if prefix is None:
                 if value[0] == "#":
                     marker = process_marker(value)
@@ -1116,16 +1160,21 @@
                         main_tag.group_id = ''.join(value)
                     else:
                         main_tag.group_id = marker.group_id
                         extras.append(marker)
                 else:
                     extras.append(GenericModification(''.join(value)))
             else:
-                tag_type = TagBase.find_by_tag(prefix)
-                extras.append(tag_type(value))
+                try:
+                    tag_type = TagBase.find_by_tag(prefix)
+                    extra_tag = tag_type(value)
+                except KeyError:
+                    part_str = ''.join(part)
+                    extra_tag = GenericModification(part_str)
+                extras.append(extra_tag)
         main_tag.extra = extras
     return main_tag
 
 
 class ModificationRule(object):
     '''Define a fixed modification rule which dictates a modification tag is
     always applied at one or more amino acid residues.
@@ -1981,25 +2030,35 @@
 
     def __str__(self):
         return to_proforma(self.sequence, **self.properties)
 
     def __repr__(self):
         return "{self.__class__.__name__}({self.sequence}, {self.properties})".format(self=self)
 
+    def __len__(self):
+        return len(self.sequence)
+
     def __getitem__(self, i):
         if isinstance(i, slice):
             props = self.properties.copy()
             ivs = []
             for iv in props['intervals']:
                 iv = iv._update_coordinates_sliced(
                     i.start, i.stop)
                 if iv is None:
                     continue
                 ivs.append(iv)
             props['intervals'] = ivs
+
+            if not (i.start is None or i.start == 0):
+                props['n_term'] = None
+            n = len(self)
+            if not (i.stop is None or i.stop >= n):
+                props['c_term'] = None
+
             return self.__class__(self.sequence[i], props)
         else:
             return self.sequence[i]
 
     def __eq__(self, other):
         if isinstance(other, str):
             return str(self) == other
```

### Comparing `pyteomics-4.5.6/pyteomics/protxml.py` & `pyteomics-4.6/pyteomics/protxml.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/pylab_aux.py` & `pyteomics-4.6/pyteomics/pylab_aux.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
 
     # peptide can be modX or proforma. spectrum_utils supports proforma only
     aa_comp = kwargs.get('aa_comp')
     mod_names = kwargs.get('mod_names')
     prefix = kwargs.get('prefix')
 
     try:
-        parsed_proforma = proforma.Proforma.parse(peptide)
+        parsed_proforma = proforma.ProForma.parse(peptide)
         peptide_pro = peptide
     except Exception:
         parsed_proforma = None
         try:
             peptide_pro = parser.to_proforma(peptide, aa_mass=aa_mass, aa_comp=aa_comp, mod_names=mod_names, prefix=prefix)
         except Exception:
             raise PyteomicsError("Cannot parse {} as ProForma or convert from modX".format(peptide))
```

### Comparing `pyteomics-4.5.6/pyteomics/tandem.py` & `pyteomics-4.6/pyteomics/tandem.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/traml.py` & `pyteomics-4.6/pyteomics/traml.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-"""
-traml - targeted MS transition data in TraML format
-===================================================
-
-Summary
--------
-
-TraML is a standard rich XML-format for targeted mass spectrometry method definitions.
-Please refer to `psidev.info <http://www.psidev.info/traml>`_
-for the detailed specification of the format and structure of TraML files.
-
-This module provides a minimalistic way to extract information from TraML
-files. You can use the object-oriented interface (:class:`TraML` instances) to
-access target definitions and transitions. :class:`TraML` objects also support
-indexing with entity IDs directly.
-
-Data access
------------
-
-  :py:class:`TraML` - a class representing a single TraML file.
-  Other data access functions use this class internally.
-
-  :py:func:`read` - iterate through transitions in TraML format.
-
-  :py:func:`chain` - read multiple TraML files at once.
-
-  :py:func:`chain.from_iterable` - read multiple files at once, using an
-  iterable of files.
-
-Controlled Vocabularies
-~~~~~~~~~~~~~~~~~~~~~~~
-TraML relies on controlled vocabularies to describe its contents extensibly. See
-`Controlled Vocabulary Terms <../data.html#controlled-vocabulary-terms-in-structured-data>`_
-for more details on how they are used.
-
-Handling Time Units and Other Qualified Quantities
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-TraML contains information which may be described as using a variety of different time units.
-See `Unit Handling <../data.html#unit-handling>`_ for more information.
-
-Deprecated functions
---------------------
-
-  :py:func:`version_info` - get version information about the TraML file.
-  You can just read the corresponding attribute of the :py:class:`TraML` object.
-
-  :py:func:`iterfind` - iterate over elements in an TraML file.
-  You can just call the corresponding method of the :py:class:`TraML` object.
-
-Dependencies
-------------
-
-This module requires :py:mod:`lxml`
-
--------------------------------------------------------------------------------
-"""
-
-#   Copyright 2018 Joshua Klein, Lev Levitsky
-#
-#   Licensed under the Apache License, Version 2.0 (the "License");
-#   you may not use this file except in compliance with the License.
-#   You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#   Unless required by applicable law or agreed to in writing, software
-#   distributed under the License is distributed on an "AS IS" BASIS,
-#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#   See the License for the specific language governing permissions and
-#   limitations under the License.
-
-
-import warnings
-from . import xml, _schema_defaults, auxiliary as aux
-
-
-class TraML(xml.MultiProcessingXML, xml.IndexSavingXML):
-    """Parser class for TraML files."""
-    file_format = 'TraML'
-    _root_element = 'TraML'
-    _default_schema = _schema_defaults._traml_schema_defaults
-    _default_version = '1.0.0'
-
-    _default_iter_tag = 'Transition'
-    _indexed_tags = {
-        'Transition',
-        'Peptide',
-        'Compound',
-        'Target',
-        'Protein',
-        'Compound',
-    }
-
-    _element_handlers = xml.XML._element_handlers.copy()
-    _element_handlers.update({
-        'Modification': xml.XML._promote_empty_parameter_to_name,
-        'Interpretation': xml.XML._promote_empty_parameter_to_name,
-        'Software': xml.XML._promote_empty_parameter_to_name,
-    })
-
-    def __init__(self, *args, **kwargs):
-        kwargs.setdefault('retrieve_refs', True)
-        super(TraML, self).__init__(*args, **kwargs)
-
-    def _get_info_smart(self, element, **kw):
-        kwargs = dict(kw)
-        rec = kwargs.pop('recursive', None)
-        info = self._get_info(
-            element,
-            recursive=(rec if rec is not None else True),
-            **kwargs)
-        return info
-
-    def _retrieve_refs(self, info, **kwargs):
-        """Retrieves and embeds the data for each attribute in `info` that
-        ends in `Ref`. Removes the id attribute from `info`"""
-        for k, v in dict(info).items():
-            if k[-3:] in {'Ref', 'ref'}:
-                if isinstance(v, str):
-                    key = v
-                elif isinstance(v, dict):
-                    key = v['ref']
-                else:
-                    if k != 'ref':
-                        info[k[:-3]] = info.pop(k)
-                    continue
-                try:
-                    by_id = self.get_by_id(key, retrieve_refs=True)
-                except KeyError:
-                    warnings.warn('Ignoring unresolved reference: ' + key)
-                else:
-                    if k == 'ref':
-                        info.update(by_id)
-                    else:
-                        # by_id.pop('id', None)
-                        info[k[:-3]] = by_id
-                        del info[k]
-
-
-
-def read(source, retrieve_refs=True, read_schema=False, iterative=True, use_index=False, huge_tree=False):
-    """Parse `source` and iterate through transitions.
-
-    Parameters
-    ----------
-    source : str or file
-        A path to a target TraML file or the file object itself.
-
-    retrieve_refs : bool, optional
-        If :py:const:`True`, additional information from references will be
-        automatically added to the results. The file processing time will
-        increase. Default is :py:const:`True`.
-
-    read_schema : bool, optional
-        If :py:const:`True`, attempt to extract information from the XML schema
-        mentioned in the TraML header. Otherwise, use default parameters.
-        Not recommended without Internet connection or
-        if you don't like to get the related warnings.
-
-    iterative : bool, optional
-        Defines whether iterative parsing should be used. It helps reduce
-        memory usage at almost the same parsing speed. Default is
-        :py:const:`True`.
-
-    use_index : bool, optional
-        Defines whether an index of byte offsets needs to be created for
-        spectrum elements. Default is :py:const:`False`.
-
-    huge_tree : bool, optional
-        This option is passed to the `lxml` parser and defines whether
-        security checks for XML tree depth and node size should be disabled.
-        Default is :py:const:`False`.
-        Enable this option for trusted files to avoid XMLSyntaxError exceptions
-        (e.g. `XMLSyntaxError: xmlSAX2Characters: huge text node`).
-
-    Returns
-    -------
-    out : TraML
-       A :py:class:`TraML` object, suitable for iteration and possibly random access.
-    """
-
-    return TraML(source, retrieve_refs=retrieve_refs, read_schema=read_schema, iterative=iterative,
-                 use_index=use_index, huge_tree=huge_tree)
-
-
-def iterfind(source, path, **kwargs):
-    """Parse `source` and yield info on elements with specified local
-    name or by specified "XPath".
-
-    .. note:: This function is provided for backward compatibility only.
-        If you do multiple :py:func:`iterfind` calls on one file, you should
-        create an :py:class:`TraML` object and use its
-        :py:meth:`!iterfind` method.
-
-    Parameters
-    ----------
-    source : str or file
-        File name or file-like object.
-
-    path : str
-        Element name or XPath-like expression. Only local names separated
-        with slashes are accepted. An asterisk (`*`) means any element.
-        You can specify a single condition in the end, such as:
-        ``"/path/to/element[some_value>1.5]"``
-        Note: you can do much more powerful filtering using plain Python.
-        The path can be absolute or "free". Please don't specify
-        namespaces.
-
-    recursive : bool, optional
-        If :py:const:`False`, subelements will not be processed when
-        extracting info from elements. Default is :py:const:`True`.
-
-    iterative : bool, optional
-        Specifies whether iterative XML parsing should be used. Iterative
-        parsing significantly reduces memory usage and may be just a little
-        slower. When `retrieve_refs` is :py:const:`True`, however, it is
-        highly recommended to disable iterative parsing if possible.
-        Default value is :py:const:`True`.
-
-    read_schema : bool, optional
-        If :py:const:`True`, attempt to extract information from the XML schema
-        mentioned in the mzIdentML header. Otherwise, use default
-        parameters. Not recommended without Internet connection or
-        if you don't like to get the related warnings.
-
-    Returns
-    -------
-    out : iterator
-    """
-    return TraML(source, **kwargs).iterfind(path, **kwargs)
-
-
-version_info = xml._make_version_info(TraML)
-
-chain = aux.ChainBase._make_chain(TraML)
+"""
+traml - targeted MS transition data in TraML format
+===================================================
+
+Summary
+-------
+
+TraML is a standard rich XML-format for targeted mass spectrometry method definitions.
+Please refer to `psidev.info <http://www.psidev.info/traml>`_
+for the detailed specification of the format and structure of TraML files.
+
+This module provides a minimalistic way to extract information from TraML
+files. You can use the object-oriented interface (:class:`TraML` instances) to
+access target definitions and transitions. :class:`TraML` objects also support
+indexing with entity IDs directly.
+
+Data access
+-----------
+
+  :py:class:`TraML` - a class representing a single TraML file.
+  Other data access functions use this class internally.
+
+  :py:func:`read` - iterate through transitions in TraML format.
+
+  :py:func:`chain` - read multiple TraML files at once.
+
+  :py:func:`chain.from_iterable` - read multiple files at once, using an
+  iterable of files.
+
+Controlled Vocabularies
+~~~~~~~~~~~~~~~~~~~~~~~
+TraML relies on controlled vocabularies to describe its contents extensibly. See
+`Controlled Vocabulary Terms <../data.html#controlled-vocabulary-terms-in-structured-data>`_
+for more details on how they are used.
+
+Handling Time Units and Other Qualified Quantities
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+TraML contains information which may be described as using a variety of different time units.
+See `Unit Handling <../data.html#unit-handling>`_ for more information.
+
+Deprecated functions
+--------------------
+
+  :py:func:`version_info` - get version information about the TraML file.
+  You can just read the corresponding attribute of the :py:class:`TraML` object.
+
+  :py:func:`iterfind` - iterate over elements in an TraML file.
+  You can just call the corresponding method of the :py:class:`TraML` object.
+
+Dependencies
+------------
+
+This module requires :py:mod:`lxml`
+
+-------------------------------------------------------------------------------
+"""
+
+#   Copyright 2018 Joshua Klein, Lev Levitsky
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
+
+
+import warnings
+from . import xml, _schema_defaults, auxiliary as aux
+
+
+class TraML(xml.MultiProcessingXML, xml.IndexSavingXML):
+    """Parser class for TraML files."""
+    file_format = 'TraML'
+    _root_element = 'TraML'
+    _default_schema = _schema_defaults._traml_schema_defaults
+    _default_version = '1.0.0'
+
+    _default_iter_tag = 'Transition'
+    _indexed_tags = {
+        'Transition',
+        'Peptide',
+        'Compound',
+        'Target',
+        'Protein',
+        'Compound',
+    }
+
+    _element_handlers = xml.XML._element_handlers.copy()
+    _element_handlers.update({
+        'Modification': xml.XML._promote_empty_parameter_to_name,
+        'Interpretation': xml.XML._promote_empty_parameter_to_name,
+        'Software': xml.XML._promote_empty_parameter_to_name,
+    })
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault('retrieve_refs', True)
+        super(TraML, self).__init__(*args, **kwargs)
+
+    def _get_info_smart(self, element, **kw):
+        kwargs = dict(kw)
+        rec = kwargs.pop('recursive', None)
+        info = self._get_info(
+            element,
+            recursive=(rec if rec is not None else True),
+            **kwargs)
+        return info
+
+    def _retrieve_refs(self, info, **kwargs):
+        """Retrieves and embeds the data for each attribute in `info` that
+        ends in `Ref`. Removes the id attribute from `info`"""
+        for k, v in dict(info).items():
+            if k[-3:] in {'Ref', 'ref'}:
+                if isinstance(v, str):
+                    key = v
+                elif isinstance(v, dict):
+                    key = v['ref']
+                else:
+                    if k != 'ref':
+                        info[k[:-3]] = info.pop(k)
+                    continue
+                try:
+                    by_id = self.get_by_id(key, retrieve_refs=True)
+                except KeyError:
+                    warnings.warn('Ignoring unresolved reference: ' + key)
+                else:
+                    if k == 'ref':
+                        info.update(by_id)
+                    else:
+                        # by_id.pop('id', None)
+                        info[k[:-3]] = by_id
+                        del info[k]
+
+
+
+def read(source, retrieve_refs=True, read_schema=False, iterative=True, use_index=False, huge_tree=False):
+    """Parse `source` and iterate through transitions.
+
+    Parameters
+    ----------
+    source : str or file
+        A path to a target TraML file or the file object itself.
+
+    retrieve_refs : bool, optional
+        If :py:const:`True`, additional information from references will be
+        automatically added to the results. The file processing time will
+        increase. Default is :py:const:`True`.
+
+    read_schema : bool, optional
+        If :py:const:`True`, attempt to extract information from the XML schema
+        mentioned in the TraML header. Otherwise, use default parameters.
+        Not recommended without Internet connection or
+        if you don't like to get the related warnings.
+
+    iterative : bool, optional
+        Defines whether iterative parsing should be used. It helps reduce
+        memory usage at almost the same parsing speed. Default is
+        :py:const:`True`.
+
+    use_index : bool, optional
+        Defines whether an index of byte offsets needs to be created for
+        spectrum elements. Default is :py:const:`False`.
+
+    huge_tree : bool, optional
+        This option is passed to the `lxml` parser and defines whether
+        security checks for XML tree depth and node size should be disabled.
+        Default is :py:const:`False`.
+        Enable this option for trusted files to avoid XMLSyntaxError exceptions
+        (e.g. `XMLSyntaxError: xmlSAX2Characters: huge text node`).
+
+    Returns
+    -------
+    out : TraML
+       A :py:class:`TraML` object, suitable for iteration and possibly random access.
+    """
+
+    return TraML(source, retrieve_refs=retrieve_refs, read_schema=read_schema, iterative=iterative,
+                 use_index=use_index, huge_tree=huge_tree)
+
+
+def iterfind(source, path, **kwargs):
+    """Parse `source` and yield info on elements with specified local
+    name or by specified "XPath".
+
+    .. note:: This function is provided for backward compatibility only.
+        If you do multiple :py:func:`iterfind` calls on one file, you should
+        create an :py:class:`TraML` object and use its
+        :py:meth:`!iterfind` method.
+
+    Parameters
+    ----------
+    source : str or file
+        File name or file-like object.
+
+    path : str
+        Element name or XPath-like expression. Only local names separated
+        with slashes are accepted. An asterisk (`*`) means any element.
+        You can specify a single condition in the end, such as:
+        ``"/path/to/element[some_value>1.5]"``
+        Note: you can do much more powerful filtering using plain Python.
+        The path can be absolute or "free". Please don't specify
+        namespaces.
+
+    recursive : bool, optional
+        If :py:const:`False`, subelements will not be processed when
+        extracting info from elements. Default is :py:const:`True`.
+
+    iterative : bool, optional
+        Specifies whether iterative XML parsing should be used. Iterative
+        parsing significantly reduces memory usage and may be just a little
+        slower. When `retrieve_refs` is :py:const:`True`, however, it is
+        highly recommended to disable iterative parsing if possible.
+        Default value is :py:const:`True`.
+
+    read_schema : bool, optional
+        If :py:const:`True`, attempt to extract information from the XML schema
+        mentioned in the mzIdentML header. Otherwise, use default
+        parameters. Not recommended without Internet connection or
+        if you don't like to get the related warnings.
+
+    Returns
+    -------
+    out : iterator
+    """
+    return TraML(source, **kwargs).iterfind(path, **kwargs)
+
+
+version_info = xml._make_version_info(TraML)
+
+chain = aux.ChainBase._make_chain(TraML)
```

### Comparing `pyteomics-4.5.6/pyteomics/usi.py` & `pyteomics-4.6/pyteomics/usi.py`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/pyteomics/version.py` & `pyteomics-4.6/pyteomics/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
   :py:const:`version` - a string with the current version.
 
   :py:const:`version_info` - a tuple with structured information about the current version.
 
 """
 
-__version__ = '4.5.6'
+__version__ = '4.6'
 
 from collections import namedtuple
 import re
 
 
 class _VersionInfo(namedtuple('_VersionInfo', ('major', 'minor', 'micro', 'releaselevel', 'serial'))):
     """Tuple mimicking :py:const:`sys.version_info`"""
```

### Comparing `pyteomics-4.5.6/pyteomics/xml.py` & `pyteomics-4.6/pyteomics/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -368,17 +368,21 @@
                 value = unitfloat(value, unit_info)
         except ValueError:
             value = unitstr(value, unit_info)
 
         # return {cvstr(attribs['name'], accession, unit_accesssion): value}
         return _XMLParam(cvstr(attribs['name'], accession, unit_accesssion), value, _local_name(element))
 
+    def _handle_referenceable_param_group(self, param_group_ref, **kwargs):
+        raise NotImplementedError()
+        return []
+
     def _find_immediate_params(self, element, **kwargs):
         return element.xpath(
-            './*[local-name()="cvParam" or local-name()="userParam" or local-name()="UserParam"]')
+            './*[local-name()="cvParam" or local-name()="userParam" or local-name()="UserParam" or local-name()="referenceableParamGroupRef"]')
 
     def _insert_param(self, info_dict, param):
         key = param.name
         if key in info_dict:
             if isinstance(info_dict[key], list):
                 info_dict[key].append(param.value)
             else:
@@ -406,35 +410,43 @@
         try:
             name = kwargs.pop('ename')
         except KeyError:
             name = _local_name(element)
         schema_info = self.schema_info
         if name in {'cvParam', 'userParam', 'UserParam'}:
             return self._handle_param(element, **kwargs)
+        elif name == "referenceableParamGroupRef":
+            return self._handle_referenceable_param_group(element, **kwargs)
 
         info = dict(element.attrib)
         # process subelements
         params = []
         if kwargs.get('recursive'):
             for child in element.iterchildren():
                 cname = _local_name(child)
                 if cname in {'cvParam', 'userParam', 'UserParam'}:
                     newinfo = self._handle_param(child, **kwargs)
                     params.append(newinfo)
+                elif cname == "referenceableParamGroupRef":
+                    params.extend(self._handle_referenceable_param_group(child, **kwargs))
                 else:
                     if cname not in schema_info['lists']:
                         info[cname] = self._get_info_smart(child, ename=cname, **kwargs)
                     else:
                         info.setdefault(cname, []).append(
                             self._get_info_smart(child, ename=cname, **kwargs))
         else:
             # handle the case where we do not want to unpack all children, but
             # *Param tags are considered part of the current entity, semantically
             for child in self._find_immediate_params(element, **kwargs):
-                params.append(self._handle_param(child, **kwargs))
+                param_or_group = self._handle_param(child, **kwargs)
+                if isinstance(param_or_group, list):
+                    params.extend(param_or_group)
+                else:
+                    params.append(param_or_group)
 
         handler = self._element_handlers.get(name)
         if handler is not None:
             info, params = handler(self, info, params)
 
         for param in params:
             self._insert_param(info, param)
@@ -1196,48 +1208,14 @@
         with open(self._byte_offset_filename, 'r') as f:
             index = self._index_class.load(f)
             if index.schema_version is None:
                 raise TypeError("Legacy Offset Index!")
             self._offset_index = index
 
 
-class ArrayConversionMixin(BinaryDataArrayTransformer):
-    _dtype_dict = {}
-    _array_keys = ['m/z array', 'intensity array']
-
-    def __init__(self, *args, **kwargs):
-        self._dtype_dict = {None: None}
-        dtype = kwargs.pop('dtype', None)
-        if isinstance(dtype, dict):
-            self._dtype_dict.update(dtype)
-        elif dtype:
-            self._dtype_dict = {k: dtype for k in self._array_keys}
-            self._dtype_dict[None] = dtype
-        super(ArrayConversionMixin, self).__init__(*args, **kwargs)
-
-    def __getstate__(self):
-        state = super(ArrayConversionMixin, self).__getstate__()
-        state['_dtype_dict'] = self._dtype_dict
-        return state
-
-    def __setstate__(self, state):
-        super(ArrayConversionMixin, self).__setstate__(state)
-        self._dtype_dict = state['_dtype_dict']
-
-    def _convert_array(self, k, array):
-        dtype = self._dtype_dict.get(k)
-        if dtype is not None:
-            return array.astype(dtype)
-        return array
-
-    def _finalize_record_conversion(self, array, record):
-        key = record.key
-        return self._convert_array(key, array)
-
-
 class Iterfind(object):
     def __init__(self, parser, tag_name, **kwargs):
         self.parser = parser
         self.tag_name = tag_name
         self.config = kwargs
         self._iterator = None
```

### Comparing `pyteomics-4.5.6/pyteomics.egg-info/SOURCES.txt` & `pyteomics-4.6/pyteomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyteomics-4.5.6/setup.py` & `pyteomics-4.6/setup.py`

 * *Files identical despite different names*

