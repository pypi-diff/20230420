# Comparing `tmp/ephysiopy-1.9.0.tar.gz` & `tmp/ephysiopy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.0.tar", last modified: Thu Apr 20 09:52:35 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.1.tar", last modified: Thu Apr 20 12:23:37 2023, max compression
```

## Comparing `ephysiopy-1.9.0.tar` & `ephysiopy-1.9.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.229127 ephysiopy-1.9.0/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.229127 ephysiopy-1.9.0/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22339 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:52:35.229127 ephysiopy-1.9.0/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 09:52:35.000000 ephysiopy-1.9.0/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 09:52:35.000000 ephysiopy-1.9.0/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:52:35.000000 ephysiopy-1.9.0/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 09:52:35.000000 ephysiopy-1.9.0/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 09:52:35.000000 ephysiopy-1.9.0/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 09:52:35.233127 ephysiopy-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 09:52:24.000000 ephysiopy-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.966935 ephysiopy-1.9.1/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32228 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:23:37.970935 ephysiopy-1.9.1/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 12:23:37.000000 ephysiopy-1.9.1/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 12:23:37.000000 ephysiopy-1.9.1/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:23:37.000000 ephysiopy-1.9.1/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 12:23:37.000000 ephysiopy-1.9.1/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 12:23:37.000000 ephysiopy-1.9.1/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 12:23:37.974935 ephysiopy-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 12:23:29.000000 ephysiopy-1.9.1/setup.py
```

### Comparing `ephysiopy-1.9.0/LICENSE` & `ephysiopy-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/PKG-INFO` & `ephysiopy-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.0/README.md` & `ephysiopy-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.1/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.1/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.1/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.1/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/binning.py` & `ephysiopy-1.9.1/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.1/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.1/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.1/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.1/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.1/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.1/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.1/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.1/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/common/utils.py` & `ephysiopy-1.9.1/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.1/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.1/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/io/recording.py` & `ephysiopy-1.9.1/ephysiopy/io/recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,29 +371,34 @@
 
     def get_spike_times(self, cluster: int, tetrode: int = None):
         ts = self.kilodata.spk_times
         times = ts[self.kilodata.spk_clusters == cluster]
         return times.astype(np.int64) / self.sample_rate
 
     def load_lfp(self, pname: Path, *args, **kwargs):
+        '''
+        Valid kwargs are:
+        'target_sample_rate' - int
+            the sample rate to downsample to from the original
+        '''
         from scipy import signal
         if self.path2LFPdata is not None:
             lfp = memmapBinaryFile(
                 os.path.join(self.path2LFPdata, "continuous.dat"),
                 n_channels=self.channel_count)
             channel = 0
             if "channel" in kwargs.keys():
                 channel = kwargs["channel"]
-            sample_rate = 500
-            if "sample_rate" in kwargs.keys():
-                sample_rate = kwargs["sample_rate"]
+            target_sample_rate = 500
+            if "target_sample_rate" in kwargs.keys():
+                target_sample_rate = kwargs["target_sample_rate"]
             n_samples = np.shape(lfp[channel, :])[0]
             sig = signal.resample(lfp[channel, :], int(
-                n_samples / 3e4) * sample_rate)
-            self.EEGCalcs = EEGCalcsGeneric(sig, sample_rate)
+                n_samples / self.sample_rate) * target_sample_rate)
+            self.EEGCalcs = EEGCalcsGeneric(sig, target_sample_rate)
 
     def load_neural_data(self, pname: Path) -> None:
         pass
 
     def load_settings(self):
         if self._settings is None:
             # pname_root gets walked through and over-written with
```

### Comparing `ephysiopy-1.9.0/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.1/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.1/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.1/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.1/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.1/ephysiopy/visualise/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,14 @@
     def makeRateMap(self, spk_times: np.ndarray,
                     ax: matplotlib.axes = None) -> matplotlib.axes:
         self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         spk_weights = np.bincount(
             spk_times_in_pos_samples, minlength=self.npos)
         rmap = self.RateMapMaker.getMap(spk_weights)
-        print(f"len rmap = {len(rmap)}")
-        for i, r in enumerate(rmap):
-            print(f"rmap[{i}] shape = {np.shape(r)}")
-            print(f"rmap[{i}] = {r}")
         ratemap = np.ma.MaskedArray(rmap[0], np.isnan(rmap[0]), copy=True)
         x, y = np.meshgrid(rmap[1][1][0:-1].data, rmap[1][0][0:-1].data)
         vmax = np.nanmax(np.ravel(ratemap))
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.pcolormesh(
```

### Comparing `ephysiopy-1.9.0/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.1/ephysiopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.0/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.1/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.0/setup.py` & `ephysiopy-1.9.1/setup.py`

 * *Files identical despite different names*

