# Comparing `tmp/pyphysio-3.1.3.tar.gz` & `tmp/pyphysio-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphysio-3.1.3.tar", last modified: Wed Apr 19 12:20:22 2023, max compression
+gzip compressed data, was "pyphysio-3.1.4.tar", last modified: Thu Apr 20 13:17:17 2023, max compression
```

## Comparing `pyphysio-3.1.3.tar` & `pyphysio-3.1.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/
--rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.3/LICENSE
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-04-19 12:20:22.884463 pyphysio-3.1.3/PKG-INFO
--rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.3/README.md
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.876463 pyphysio-3.1.3/pyphysio/
--rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    12620 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/_base_algorithm.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/artefacts.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.3/pyphysio/filters.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/generators/
--rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/generators/__init__.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/indicators/
--rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.3/pyphysio/indicators/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/indicators/frequencydomain.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/indicators/nonlinear.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    17342 2023-04-14 08:49:08.000000 pyphysio-3.1.3/pyphysio/indicators/peaks.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/indicators/timedomain.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     7580 2023-04-19 07:35:54.000000 pyphysio-3.1.3/pyphysio/interactive.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/loaders/
--rwx------   0 bizzego   (1002) bizzego   (1002)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/loaders/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/loaders/_load_nirx.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    13169 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/segmenters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    17232 2023-04-06 12:32:55.000000 pyphysio-3.1.3/pyphysio/signal.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.876463 pyphysio-3.1.3/pyphysio/specialized/
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/activity/
--rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/activity/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/eda/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     6887 2023-04-13 12:45:40.000000 pyphysio-3.1.3/pyphysio/specialized/eda/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/specialized/eda/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/eeg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/eeg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/emg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/emg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/fnirs/
--rwx------   0 bizzego   (1002) bizzego   (1002)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_convert.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_data.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.3/pyphysio/specialized/fnirs/_dl_sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/heart/
--rwx------   0 bizzego   (1002) bizzego   (1002)    27262 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/specialized/heart/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.3/pyphysio/specialized/heart/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio/specialized/resp/
--rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.3/pyphysio/specialized/resp/_presets.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.3/pyphysio/sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/pyphysio/test_data/
--rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/test_data/info_medical
--rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.3/pyphysio/test_data/medical.txt.bz2
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34172 2023-04-13 12:44:09.000000 pyphysio-3.1.3/pyphysio/utils.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.880463 pyphysio-3.1.3/pyphysio.egg-info/
--rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/PKG-INFO
--rwx------   0 bizzego   (1002) bizzego   (1002)     1355 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/SOURCES.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/dependency_links.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)       54 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/requires.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-04-19 12:20:22.000000 pyphysio-3.1.3/pyphysio.egg-info/top_level.txt
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-04-19 12:20:22.884463 pyphysio-3.1.3/setup.cfg
--rwx------   0 bizzego   (1002) bizzego   (1002)     2290 2023-04-19 12:18:04.000000 pyphysio-3.1.3/setup.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-19 12:20:22.884463 pyphysio-3.1.3/tests/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8337 2023-04-13 12:55:10.000000 pyphysio-3.1.3/tests/test_eda_methods.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_filters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_fnirs.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_get_sampling_freq.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.3/tests/test_ibi_estimators.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.3/tests/test_segmenters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_signal.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.3/tests/test_tools.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.674972 pyphysio-3.1.4/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.4/LICENSE
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-04-20 13:17:17.674972 pyphysio-3.1.4/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.4/README.md
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.590971 pyphysio-3.1.4/pyphysio/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    12620 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/_base_algorithm.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/artefacts.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.4/pyphysio/filters.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/generators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/generators/__init__.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/indicators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.4/pyphysio/indicators/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/indicators/frequencydomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/indicators/nonlinear.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    17343 2023-04-17 09:46:09.000000 pyphysio-3.1.4/pyphysio/indicators/peaks.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/indicators/timedomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     9305 2023-04-20 13:09:16.000000 pyphysio-3.1.4/pyphysio/interactive.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/loaders/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/loaders/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/loaders/_load_nirx.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    13169 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    17232 2023-04-06 12:32:55.000000 pyphysio-3.1.4/pyphysio/signal.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.558970 pyphysio-3.1.4/pyphysio/specialized/
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/specialized/activity/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/activity/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/eda/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     6887 2023-04-13 12:45:40.000000 pyphysio-3.1.4/pyphysio/specialized/eda/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/specialized/eda/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/eeg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/eeg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/emg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/emg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/fnirs/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_convert.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_data.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_dl_sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/heart/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    27262 2023-04-19 14:25:16.000000 pyphysio-3.1.4/pyphysio/specialized/heart/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/specialized/heart/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/resp/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.4/pyphysio/specialized/resp/_presets.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.4/pyphysio/sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.618971 pyphysio-3.1.4/pyphysio/test_data/
+-rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/test_data/info_medical
+-rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/test_data/medical.txt.bz2
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34172 2023-04-13 12:44:09.000000 pyphysio-3.1.4/pyphysio/utils.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio.egg-info/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1355 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/SOURCES.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/dependency_links.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)       54 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/requires.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/top_level.txt
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-04-20 13:17:17.674972 pyphysio-3.1.4/setup.cfg
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2290 2023-04-20 13:16:46.000000 pyphysio-3.1.4/setup.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.674972 pyphysio-3.1.4/tests/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8337 2023-04-13 12:55:10.000000 pyphysio-3.1.4/tests/test_eda_methods.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_filters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_fnirs.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_get_sampling_freq.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.4/tests/test_ibi_estimators.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.4/tests/test_segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_signal.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_tools.py
```

### Comparing `pyphysio-3.1.3/LICENSE` & `pyphysio-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/PKG-INFO` & `pyphysio-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.3/README.md` & `pyphysio-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/__init__.py` & `pyphysio-3.1.4/pyphysio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/_base_algorithm.py` & `pyphysio-3.1.4/pyphysio/_base_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/artefacts.py` & `pyphysio-3.1.4/pyphysio/artefacts.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/filters.py` & `pyphysio-3.1.4/pyphysio/filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/generators/__init__.py` & `pyphysio-3.1.4/pyphysio/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/indicators/frequencydomain.py` & `pyphysio-3.1.4/pyphysio/indicators/frequencydomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/indicators/nonlinear.py` & `pyphysio-3.1.4/pyphysio/indicators/nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/indicators/peaks.py` & `pyphysio-3.1.4/pyphysio/indicators/peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding=utf-8
 # from __future__ import division
 # 
 # from abc import abstractmethod as _abstract, ABCMeta as _ABCMeta
 
 import numpy as _np
-import xarray as _xr
+#import xarray as _xr
 from .._base_algorithm import _Algorithm
 from ..utils import PeakDetection as _PeakDetection,\
     PeakSelection as _PeakSelection
 
 # __author__ = 'AleB'
 
 #TODO: create just one function for duration and slopes
```

### Comparing `pyphysio-3.1.3/pyphysio/indicators/timedomain.py` & `pyphysio-3.1.4/pyphysio/indicators/timedomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/loaders/_load_nirx.py` & `pyphysio-3.1.4/pyphysio/loaders/_load_nirx.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/segmenters.py` & `pyphysio-3.1.4/pyphysio/segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/signal.py` & `pyphysio-3.1.4/pyphysio/signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/activity/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/activity/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/eda/__init__.py` & `pyphysio-3.1.4/pyphysio/specialized/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/eda/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/eda/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/eeg/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/eeg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/emg/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/emg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/fnirs/__init__.py` & `pyphysio-3.1.4/pyphysio/specialized/fnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/fnirs/_convert.py` & `pyphysio-3.1.4/pyphysio/specialized/fnirs/_convert.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/fnirs/_data.py` & `pyphysio-3.1.4/pyphysio/specialized/fnirs/_data.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/fnirs/_dl_sqi.py` & `pyphysio-3.1.4/pyphysio/specialized/fnirs/_dl_sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/heart/__init__.py` & `pyphysio-3.1.4/pyphysio/specialized/heart/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/heart/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/heart/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/specialized/resp/_presets.py` & `pyphysio-3.1.4/pyphysio/specialized/resp/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/sqi.py` & `pyphysio-3.1.4/pyphysio/sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/test_data/medical.txt.bz2` & `pyphysio-3.1.4/pyphysio/test_data/medical.txt.bz2`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio/utils.py` & `pyphysio-3.1.4/pyphysio/utils.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/pyphysio.egg-info/PKG-INFO` & `pyphysio-3.1.4/pyphysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.3
+Version: 3.1.4
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.3/pyphysio.egg-info/SOURCES.txt` & `pyphysio-3.1.4/pyphysio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/setup.py` & `pyphysio-3.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
               'pyphysio.specialized.fnirs',
               'pyphysio.specialized.heart',
               'pyphysio.specialized.resp',
               'pyphysio.indicators',
               'pyphysio.generators'],
     package_data={'pyphysio': ['test_data/*']},
     # data_files={'test_data_out': ['info_medical', 'medical.txt.bz2']},
-    version='3.1.3',
+    version='3.1.4',
     description='Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)',
     author='a.bizzego',
     author_email='andrea.bizzego@unitn.it',
     url='https://gitlab.com/a.bizzego/pyphysio',
     keywords=['eda', 'gsr', 'ecg', 'bvp', 'fnirs', 'signal', 
               'analysis', 'physiological', 'psychopysiology', 'neuroscience'],
     classifiers=[
```

### Comparing `pyphysio-3.1.3/tests/test_eda_methods.py` & `pyphysio-3.1.4/tests/test_eda_methods.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_filters.py` & `pyphysio-3.1.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_fnirs.py` & `pyphysio-3.1.4/tests/test_fnirs.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_get_sampling_freq.py` & `pyphysio-3.1.4/tests/test_get_sampling_freq.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_ibi_estimators.py` & `pyphysio-3.1.4/tests/test_ibi_estimators.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_segmenters.py` & `pyphysio-3.1.4/tests/test_segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_signal.py` & `pyphysio-3.1.4/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.3/tests/test_tools.py` & `pyphysio-3.1.4/tests/test_tools.py`

 * *Files identical despite different names*

