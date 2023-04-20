# Comparing `tmp/ephysiopy-1.8.98.tar.gz` & `tmp/ephysiopy-1.8.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.8.98.tar", last modified: Tue Apr 18 15:56:53 2023, max compression
+gzip compressed data, was "ephysiopy-1.8.99.tar", last modified: Thu Apr 20 09:45:42 2023, max compression
```

## Comparing `ephysiopy-1.8.98.tar` & `ephysiopy-1.8.99.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:53.200770 ephysiopy-1.8.98/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:56:53.000000 ephysiopy-1.8.98/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 15:56:53.204770 ephysiopy-1.8.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 15:56:45.000000 ephysiopy-1.8.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.233246 ephysiopy-1.8.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-20 09:45:42.233246 ephysiopy-1.8.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.233246 ephysiopy-1.8.99/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.233246 ephysiopy-1.8.99/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:45:42.229246 ephysiopy-1.8.99/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-20 09:45:42.000000 ephysiopy-1.8.99/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 09:45:42.000000 ephysiopy-1.8.99/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:45:42.000000 ephysiopy-1.8.99/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 09:45:42.000000 ephysiopy-1.8.99/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 09:45:42.000000 ephysiopy-1.8.99/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 09:45:42.233246 ephysiopy-1.8.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 09:45:32.000000 ephysiopy-1.8.99/setup.py
```

### Comparing `ephysiopy-1.8.98/LICENSE` & `ephysiopy-1.8.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/PKG-INFO` & `ephysiopy-1.8.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.8.98
+Version: 1.8.99
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.8.98/README.md` & `ephysiopy-1.8.99/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.8.99/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/axona/file_headers.py` & `ephysiopy-1.8.99/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.8.99/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.8.99/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/binning.py` & `ephysiopy-1.8.99/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.8.99/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.8.99/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/gridcell.py` & `ephysiopy-1.8.99/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.8.99/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/phasecoding.py` & `ephysiopy-1.8.99/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.8.99/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.8.99/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/statscalcs.py` & `ephysiopy-1.8.99/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/common/utils.py` & `ephysiopy-1.8.99/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.8.99/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.8.99/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/io/recording.py` & `ephysiopy-1.8.99/ephysiopy/io/recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,28 +332,38 @@
             return self.TETRODE.get_spike_samples(tetrode, cluster)
 
 
 class OpenEphysBase(TrialInterface):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
         setattr(self, "sync_message_file", None)
+        # Attempt to find the files contained in the parent directory
+        # related to the recording with the default experiment and
+        # recording name
+        self.find_files(pname)
         self.load_settings()
         record_methods = ["Acquisition Board",
                           "Neuropix-PXI", "Sources/Neuropix-PXI",
                           "Rhythm FPGA", "Sources/Rhythm FPGA"]
         rec_method = [i for i in self.settings.processors.keys()
                       if i in record_methods][0]
         if 'Sources/' in rec_method:
             tmp_rec_method = rec_method.lstrip('Sources/')
             self.rec_kind = Xml2RecordingKind[tmp_rec_method]
         else:
             self.rec_kind = Xml2RecordingKind[rec_method]
         self.sample_rate = None
         self.sample_rate = self.settings.processors[rec_method].sample_rate
+        if self.sample_rate is None:
+            if self.rec_kind == RecordingKind.NEUROPIXELS:
+                self.sample_rate = 30000
         self.channel_count = self.settings.processors[rec_method].channel_count
+        if self.channel_count is None:
+            if self.rec_kind == RecordingKind.NEUROPIXELS:
+                self.channel_count = 384
         self.kilodata = None
 
     def __load_kilo__(self):
         """Loads KiloSort data"""
         self.kilodata = KiloSortSession(self.pname)
         self.kilodata.load()
         self.kilodata.removeNoiseClusters()
```

### Comparing `ephysiopy-1.8.98/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.8.99/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.8.99/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/conftest.py` & `ephysiopy-1.8.99/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_binning.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/tests/test_utils.py` & `ephysiopy-1.8.99/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy/visualise/plotting.py` & `ephysiopy-1.8.99/ephysiopy/visualise/plotting.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.8.99/ephysiopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.8.98
+Version: 1.8.99
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.8.98/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.8.99/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.8.98/setup.py` & `ephysiopy-1.8.99/setup.py`

 * *Files identical despite different names*

