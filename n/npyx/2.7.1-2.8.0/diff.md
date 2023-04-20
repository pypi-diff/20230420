# Comparing `tmp/npyx-2.7.1.tar.gz` & `tmp/npyx-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npyx-2.7.1.tar", last modified: Mon Mar 20 15:37:20 2023, max compression
+gzip compressed data, was "npyx-2.8.0.tar", last modified: Thu Apr 20 18:46:21 2023, max compression
```

## Comparing `npyx-2.7.1.tar` & `npyx-2.8.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-20 15:37:20.354274 npyx-2.7.1/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.7.1/LICENSE.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32016 2023-03-20 15:37:20.354274 npyx-2.7.1/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    31524 2023-03-09 12:41:06.000000 npyx-2.7.1/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-20 15:37:20.350274 npyx-2.7.1/npyx/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      818 2023-03-20 15:32:56.000000 npyx-2.7.1/npyx/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.7.1/npyx/behav.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/circuitProphyler.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   106772 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/corr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    21524 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/datasets.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    56343 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/feat.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17032 2023-03-01 11:21:05.000000 npyx-2.7.1/npyx/gl.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    33625 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/h5.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.7.1/npyx/histo.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.7.1/npyx/info.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    49225 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/inout.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/merger.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/metrics.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   148556 2023-03-13 14:58:27.000000 npyx-2.7.1/npyx/plot.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/preprocess.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37478 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/spk_t.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    44507 2023-03-20 15:37:11.000000 npyx-2.7.1/npyx/spk_wvf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/stats.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/testing.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-01 11:06:59.000000 npyx-2.7.1/npyx/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-20 15:37:20.354274 npyx-2.7.1/npyx.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32016 2023-03-20 15:37:20.000000 npyx-2.7.1/npyx.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      481 2023-03-20 15:37:20.000000 npyx-2.7.1/npyx.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-03-20 15:37:20.000000 npyx-2.7.1/npyx.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      126 2023-03-20 15:37:20.000000 npyx-2.7.1/npyx.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-03-20 15:37:20.000000 npyx-2.7.1/npyx.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-03-20 15:37:20.354274 npyx-2.7.1/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1471 2022-11-30 14:15:19.000000 npyx-2.7.1/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 18:46:21.425756 npyx-2.8.0/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2022-11-30 14:14:46.000000 npyx-2.8.0/LICENSE.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-20 18:46:21.425756 npyx-2.8.0/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    31591 2023-03-28 09:45:46.000000 npyx-2.8.0/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 18:46:21.425756 npyx-2.8.0/npyx/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      789 2023-04-20 18:43:34.000000 npyx-2.8.0/npyx/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   142298 2023-03-06 16:29:02.000000 npyx-2.8.0/npyx/behav.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/circuitProphyler.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   106772 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/corr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    28838 2023-04-20 18:33:44.000000 npyx-2.8.0/npyx/datasets.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    56695 2023-04-14 12:13:22.000000 npyx-2.8.0/npyx/feat.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)    17109 2023-04-20 18:33:44.000000 npyx-2.8.0/npyx/gl.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37417 2023-04-20 18:41:50.000000 npyx-2.8.0/npyx/h5.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-11-30 14:14:47.000000 npyx-2.8.0/npyx/histo.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16050 2022-11-30 14:14:47.000000 npyx-2.8.0/npyx/info.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    49232 2023-04-14 12:13:22.000000 npyx-2.8.0/npyx/inout.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/merger.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2023-03-20 15:37:11.000000 npyx-2.8.0/npyx/metrics.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4936 2023-04-20 18:33:44.000000 npyx-2.8.0/npyx/ml.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   149739 2023-04-12 12:27:42.000000 npyx-2.8.0/npyx/plot.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/preprocess.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    40521 2023-04-20 18:33:44.000000 npyx-2.8.0/npyx/spk_t.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    47559 2023-04-20 18:33:44.000000 npyx-2.8.0/npyx/spk_wvf.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    14661 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/stats.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2023-03-01 11:06:59.000000 npyx-2.8.0/npyx/testing.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    65528 2023-03-24 11:24:27.000000 npyx-2.8.0/npyx/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-20 18:46:21.425756 npyx-2.8.0/npyx.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32083 2023-04-20 18:46:21.000000 npyx-2.8.0/npyx.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      492 2023-04-20 18:46:21.000000 npyx-2.8.0/npyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-20 18:46:21.000000 npyx-2.8.0/npyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      143 2023-04-20 18:46:21.000000 npyx-2.8.0/npyx.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2023-04-20 18:46:21.000000 npyx-2.8.0/npyx.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2023-04-20 18:46:21.425756 npyx-2.8.0/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1491 2023-04-14 12:19:49.000000 npyx-2.8.0/setup.py
```

### Comparing `npyx-2.7.1/LICENSE.md` & `npyx-2.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/PKG-INFO` & `npyx-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.7.1
+Version: 2.8.0
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 [![PyPI Version](https://img.shields.io/pypi/v/npyx.svg)](https://pypi.org/project/npyx/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5509776.svg)](https://doi.org/10.5281/zenodo.5509776)
 [![License](https://img.shields.io/pypi/l/npyx.svg)](https://github.com/m-beau/NeuroPyxels/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/npyx/month)](https://pepy.tech/project/npyx)
 
 [NeuroPyxels](https://github.com/m-beau/NeuroPyxels) (npyx) is a python library built for electrophysiologists using Neuropixels electrodes. This package stems from the need of a pythonist who really did not want to transition to MATLAB to work with Neuropixels: it features a suite of core utility functions for loading, processing and plotting Neuropixels data.
 
-There isn't any better doc atm - post an issue if you have any question, or email [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
+**Questions**: There isn't any better doc atm, but feel free to post an issue here (preferred option, so that everyone can benefit from it 🙂) or drop me an email at [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
 
 
 - **[Documentation](https://github.com/m-beau/NeuroPyxels#documentation)**
   - [Load synchronization channel](https://github.com/m-beau/NeuroPyxels#load-synchronization-channel)
   - [Get good units from dataset](https://github.com/m-beau/NeuroPyxels#get-good-units-from-dataset)
   - [Load spike times from unit u](https://github.com/m-beau/NeuroPyxels#load-spike-times-from-unit-u)
   - [Load waveforms from unit u](https://github.com/m-beau/NeuroPyxels#load-waveforms-from-unit-u)
@@ -37,27 +37,27 @@
   - [Bonus: cool npyx plotting utilities which could turn out useful](https://github.com/m-beau/NeuroPyxels#bonus-cool-matplotlib-plotting-utilities-which-could-turn-out-useful)
 - **[Installation](https://github.com/m-beau/NeuroPyxels#installation)**
 - **[Acknowledgement](https://github.com/m-beau/NeuroPyxels#acknowledgement)**
 - **[Developer cheatsheet](https://github.com/m-beau/NeuroPyxels#developer-cheatsheet)**
 
 
 ## Documentation:
-Npyx works in harmony with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html, results stored in `path/mydata/mydata.GUI`)). Any dataset you can run phy on can also be analyzed with npyx, in essence.
+Npyx works with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) (binary data and meta data) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html), results stored in `path/mydata/mydata.GUI`). **Any dataset compatible with phy can also be analyzed with npyx, in essence.**
 
-<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **kilosort_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
+<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **npix_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
 
-Most npyx functions take at least one input: **`dp`**, which is the path to your Kilosort-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on phy documentation.
+Most npyx functions take at least one input: **`dp`**, which is the path to your Neuropixels-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on the phy documentation.
 
 Other typical parameters are: **`verbose`** (whether to print a bunch of informative messages, useful when debugging), **`saveFig`** (boolean) and **`saveDir`** (whether to save the figure in saveDir for plotting functions).
 
 Importantly, **`dp`** can also be the path to a **merged dataset**, generated with `npyx.merge_datasets()` - <ins>every function will run as smoothly on merged datasets as on any regular dataset</ins>. See below for more details.
 
-More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin``myrecording.dat`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `sync_chan` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
+More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `dataset/sync_chan/` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
 
-DISCLAIMER: some parts of the code (in particular contents of feat.py) are experimental - use at your own risk!
+DISCLAIMER: some parts of the code are experimental - use at your own risk!
 
 ### Directory structure
 
 The **`dp`** parameter of all npyx functions must be the **absolute path to `myrecording`** below.
 
 For SpikeGLX recordings:
 ```
```

### Comparing `npyx-2.7.1/README.md` & `npyx-2.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI Version](https://img.shields.io/pypi/v/npyx.svg)](https://pypi.org/project/npyx/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5509776.svg)](https://doi.org/10.5281/zenodo.5509776)
 [![License](https://img.shields.io/pypi/l/npyx.svg)](https://github.com/m-beau/NeuroPyxels/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/npyx/month)](https://pepy.tech/project/npyx)
 
 [NeuroPyxels](https://github.com/m-beau/NeuroPyxels) (npyx) is a python library built for electrophysiologists using Neuropixels electrodes. This package stems from the need of a pythonist who really did not want to transition to MATLAB to work with Neuropixels: it features a suite of core utility functions for loading, processing and plotting Neuropixels data.
 
-There isn't any better doc atm - post an issue if you have any question, or email [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
+**Questions**: There isn't any better doc atm, but feel free to post an issue here (preferred option, so that everyone can benefit from it 🙂) or drop me an email at [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
 
 
 - **[Documentation](https://github.com/m-beau/NeuroPyxels#documentation)**
   - [Load synchronization channel](https://github.com/m-beau/NeuroPyxels#load-synchronization-channel)
   - [Get good units from dataset](https://github.com/m-beau/NeuroPyxels#get-good-units-from-dataset)
   - [Load spike times from unit u](https://github.com/m-beau/NeuroPyxels#load-spike-times-from-unit-u)
   - [Load waveforms from unit u](https://github.com/m-beau/NeuroPyxels#load-waveforms-from-unit-u)
@@ -24,27 +24,27 @@
   - [Bonus: cool npyx plotting utilities which could turn out useful](https://github.com/m-beau/NeuroPyxels#bonus-cool-matplotlib-plotting-utilities-which-could-turn-out-useful)
 - **[Installation](https://github.com/m-beau/NeuroPyxels#installation)**
 - **[Acknowledgement](https://github.com/m-beau/NeuroPyxels#acknowledgement)**
 - **[Developer cheatsheet](https://github.com/m-beau/NeuroPyxels#developer-cheatsheet)**
 
 
 ## Documentation:
-Npyx works in harmony with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html, results stored in `path/mydata/mydata.GUI`)). Any dataset you can run phy on can also be analyzed with npyx, in essence.
+Npyx works with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) (binary data and meta data) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html), results stored in `path/mydata/mydata.GUI`). **Any dataset compatible with phy can also be analyzed with npyx, in essence.**
 
-<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **kilosort_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
+<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **npix_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
 
-Most npyx functions take at least one input: **`dp`**, which is the path to your Kilosort-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on phy documentation.
+Most npyx functions take at least one input: **`dp`**, which is the path to your Neuropixels-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on the phy documentation.
 
 Other typical parameters are: **`verbose`** (whether to print a bunch of informative messages, useful when debugging), **`saveFig`** (boolean) and **`saveDir`** (whether to save the figure in saveDir for plotting functions).
 
 Importantly, **`dp`** can also be the path to a **merged dataset**, generated with `npyx.merge_datasets()` - <ins>every function will run as smoothly on merged datasets as on any regular dataset</ins>. See below for more details.
 
-More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin``myrecording.dat`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `sync_chan` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
+More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `dataset/sync_chan/` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
 
-DISCLAIMER: some parts of the code (in particular contents of feat.py) are experimental - use at your own risk!
+DISCLAIMER: some parts of the code are experimental - use at your own risk!
 
 ### Directory structure
 
 The **`dp`** parameter of all npyx functions must be the **absolute path to `myrecording`** below.
 
 For SpikeGLX recordings:
 ```
```

### Comparing `npyx-2.7.1/npyx/__init__.py` & `npyx-2.8.0/npyx/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from . import (
-    utils,
-    inout,
-    gl,
-    spk_t,
-    spk_wvf,
-    corr,
-    stats,
-    plot,
-    behav,
-    merger,
-    circuitProphyler,
-    feat,
-    metrics,
-    info,
-    model,
-    h5,
-    testing,
-)
+from . import utils, inout, gl, spk_t, spk_wvf, corr, stats, plot,\
+              behav, merger, circuitProphyler, feat, metrics,\
+              info, model, h5, testing, ml, datasets
 
 from .utils import *
 from .inout import *
 from .gl import *
 from .spk_t import *
 from .spk_wvf import *
 from .corr import *
@@ -52,10 +36,10 @@
  .behav
  .merger
  .circuitProphyler
  .feat
  .h5
 """
 
-__version__ = "2.7.1"
+__version__ = "2.8.0"
 
 print(f"npyx version {__version__} imported.")
```

### Comparing `npyx-2.7.1/npyx/behav.py` & `npyx-2.8.0/npyx/behav.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/circuitProphyler.py` & `npyx-2.8.0/npyx/circuitProphyler.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/corr.py` & `npyx-2.8.0/npyx/corr.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/datasets.py` & `npyx-2.8.0/npyx/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# -*- coding: utf-8 -*-
+"""
+2022-12
+Authors: @fededagos
+
+This module contains the functions to load the data from the hdf5 files used
+in the C4 collaboration. It also contains the functions to preprocess the data.
+"""
 import copy
 import pickle
 
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -165,14 +173,24 @@
     # Select final points to remove
     idxes = np.ones_like(new_y).astype(bool)
     idxes[-2 * window_size :: 2] = False
 
     return new_y[idxes]
 
 
+def get_h5_absolute_ids(h5_path):
+    neuron_ids = []
+    with h5py.File(h5_path, "r") as hdf5_file:
+        for name in hdf5_file:
+            if "neuron" in name:
+                neuron_id = name.split("_")[-1]
+                neuron_ids.append(int(neuron_id))
+    return neuron_ids
+
+
 class NeuronsDataset:
     """
     Custom class for the cerebellum dataset, containing all information about the labelled and unlabelled neurons.
     """
 
     def __init__(
         self,
@@ -184,69 +202,85 @@
         cut_acg=True,
         central_range=CENTRAL_RANGE,
         n_channels=N_CHANNELS,
         reshape_fortran_to_c=False,
         _label="optotagged_label",
         _labelling=LABELLING,
         _use_amplitudes=False,
+        _bin_size=1,
+        _win_size=200,
+        _debug=False,
+        _lisberger=False,
+        _labels_only=False,
     ):
 
         # Store useful metadata about how the dataset was extracted
+        self.dataset = dataset
         self._n_channels = n_channels
         self._central_range = central_range
+        self._sampling_rate = get_neuron_attr(dataset, 0, "sampling_rate").item()
 
         # Initialise empty lists to extract data
         self.wf_list = []
         self.acg_list = []
         self.spikes_list = []
         self.labels_list = []
         self.info = []
+        self.chanmap_list = []
+        self.genetic_line_list = []
 
         if _use_amplitudes:
             self.amplitudes_list = []
 
-        neuron_ids = []
-        with h5py.File(dataset, "r") as hdf5_file:
-            for name in hdf5_file:
-                if "neuron" in name:
-                    neuron_id = name.split("_")[-1]
-                    neuron_ids.append(int(neuron_id))
+        neuron_ids = get_h5_absolute_ids(dataset)
 
         if not quality_check:
-            self.quality_checks_mask = np.ones(len(neuron_ids), dtype=bool)
+            self.quality_checks_mask = []
+            self.fn_fp_list = []
+            self.sane_spikes_list = []
 
         discarded_df = pd.DataFrame(columns=["neuron_id", "label", "dataset", "reason"])
-        for wf_n in tqdm(np.sort(neuron_ids), desc="Reading dataset", leave=False):
+        for i, wf_n in tqdm(
+            enumerate(np.sort(neuron_ids)),
+            total=len(neuron_ids),
+            desc="Reading dataset",
+            leave=False,
+        ):
             try:
                 # Get the label for this wvf
                 label = get_neuron_attr(dataset, wf_n, _label).ravel()[0]
 
                 # If the neuron is labelled we extract it anyways
                 if label != 0 and not isinstance(label, (np.ndarray, np.int64)):
                     label = str(label.decode("utf-8"))
                     self.labels_list.append(label)
 
                 elif label != 0:
                     label = label.item()
                     self.labels_list.append(label)
                 else:
+                    if _labels_only:
+                        continue
                     self.labels_list.append("unlabelled")
 
-                spike_idxes = get_neuron_attr(dataset, wf_n, "spike_indices")
+                spikes = get_neuron_attr(dataset, wf_n, "spike_indices")
 
-                sane_spikes = get_neuron_attr(dataset, wf_n, "sane_spikes")
-                fn_fp_spikes = get_neuron_attr(dataset, wf_n, "fn_fp_filtered_spikes")
-                quality_mask = fn_fp_spikes & sane_spikes
+                if not _lisberger:
+                    sane_spikes = get_neuron_attr(dataset, wf_n, "sane_spikes")
+                    fn_fp_spikes = get_neuron_attr(
+                        dataset, wf_n, "fn_fp_filtered_spikes"
+                    )
+                else:
+                    sane_spikes = np.ones_like(spikes, dtype=bool)
+                    fn_fp_spikes = np.ones_like(spikes, dtype=bool)
 
-                spikes = (
-                    spike_idxes[quality_mask].copy() if quality_check else spike_idxes
-                )
+                quality_mask = fn_fp_spikes & sane_spikes
 
                 # if spikes is void after quality checks, skip this neuron (if quality checks are enabled)
-                if len(spikes) == 0 and quality_check:
+                if len(spikes[quality_mask].copy()) == 0 and quality_check:
                     dataset_name = (
                         get_neuron_attr(dataset, wf_n, "dataset_id")
                         .ravel()[0]
                         .decode("utf-8")
                     )
                     discarded_df = pd.concat(
                         (
@@ -265,21 +299,51 @@
                             ),
                         ),
                         ignore_index=True,
                     )
                     del self.labels_list[-1]
                     continue
 
-                if len(spike_idxes[quality_mask].copy()) == 0:
-                    self.quality_checks_mask[wf_n] = False
+                # Even without quality checks, we want to save only the spikes in the spontaneous period
+                if quality_check:
+                    self.spikes_list.append(spikes[quality_mask].astype(int))
+                else:
+                    self.spikes_list.append(spikes[sane_spikes].astype(int))
+                    self.fn_fp_list.append(fn_fp_spikes)
+                    self.sane_spikes_list.append(sane_spikes)
+
+                    if len(spikes[quality_mask].copy()) == 0:
+                        self.quality_checks_mask.append(False)
+                    else:
+                        self.quality_checks_mask.append(True)
 
                 # Extract amplitudes if requested
                 if _use_amplitudes:
                     amplitudes = get_neuron_attr(dataset, wf_n, "amplitudes")
-                    self.amplitudes_list.append(amplitudes)
+                    try:
+                        self.amplitudes_list.append(
+                            amplitudes[sane_spikes]
+                            if not quality_check
+                            else amplitudes[quality_mask]
+                        )
+                    except IndexError:
+                        # print(
+                        #     f"Shape mismatch between amplitudes and spikes for neuron {wf_n}. {len(amplitudes)} vs {len(spikes)}."
+                        # )
+                        # print("Enforcing them to be of equal size.")
+                        if quality_check:
+                            amplitudes, quality_mask = force_amplitudes_length(
+                                amplitudes, quality_mask
+                            )
+                            self.amplitudes_list.append(amplitudes[quality_mask])
+                        else:
+                            amplitudes, sane_spikes = force_amplitudes_length(
+                                amplitudes, sane_spikes
+                            )
+                            self.amplitudes_list.append(amplitudes[sane_spikes])
 
                 # Extract waveform using provided parameters
                 wf = get_neuron_attr(dataset, wf_n, "mean_waveform_preprocessed")
 
                 if reshape_fortran_to_c:
                     wf = wf.reshape(list(wf.shape)[::-1])
 
@@ -334,35 +398,72 @@
                     )
                     del self.labels_list[-1]
                     del self.wf_list[-1]
                     if hasattr(self, "amplitudes_list"):
                         del self.amplitudes_list[-1]
                     continue
 
-                if normalise_acg:
-                    acg = npyx.corr.acg("hello", 4, 1, 200, train=spikes)
-                    normal_acg = np.clip(acg / np.max(acg), 0, 10)
-                    self.acg_list.append(normal_acg.astype(float))
+                # Extract ACG. Even if we don't apply quality checks, we still want to use spikes from the spontaneous period
+
+                acg_spikes = (
+                    spikes[quality_mask] if quality_check else spikes[sane_spikes]
+                )
+
+                if len(acg_spikes) == 0:
+                    self.acg_list.append(
+                        np.zeros(int(_win_size / _bin_size + 1)).astype(float)
+                    )
+
                 else:
-                    acg = npyx.corr.acg("hello", 4, 1, 200, train=spikes)
-                    self.acg_list.append(acg.astype(float))
-                self.spikes_list.append(spikes.astype(int))
+                    if normalise_acg:
+                        acg = npyx.corr.acg(
+                            ".npyx_placeholder",
+                            4,
+                            _bin_size,
+                            _win_size,
+                            train=acg_spikes,
+                        )
+                        normal_acg = np.clip(acg / np.max(acg), 0, 10)
+                        # For some bin and window sizes, the ACG is all zeros. In this case, we want to set it to a constant value
+                        normal_acg = np.nan_to_num(normal_acg, nan=0)
+                        self.acg_list.append(normal_acg.astype(float))
+                    else:
+                        acg = npyx.corr.acg(
+                            ".npyx_placeholder",
+                            4,
+                            _bin_size,
+                            _win_size,
+                            train=acg_spikes,
+                        )
+                        self.acg_list.append(acg.astype(float))
+
                 # Extract useful metadata
                 dataset_name = (
                     get_neuron_attr(dataset, wf_n, "dataset_id")
                     .ravel()[0]
                     .decode("utf-8")
                 )
                 neuron_id = get_neuron_attr(dataset, wf_n, "neuron_id").ravel()[0]
                 if not isinstance(neuron_id, (np.ndarray, np.int64, int)):
                     neuron_id = neuron_id.decode("utf-8")
                 neuron_metadata = dataset_name + "/" + str(neuron_id)
                 self.info.append(str(neuron_metadata))
 
+                chanmap = get_neuron_attr(dataset, wf_n, "channelmap")
+                self.chanmap_list.append(np.array(chanmap))
+
+                try:
+                    genetic_line = get_neuron_attr(dataset, wf_n, "line")
+                    self.genetic_line_list.append(genetic_line.item().decode("utf-8"))
+                except KeyError:
+                    self.genetic_line_list.append("unknown")
+
             except KeyError:
+                if _debug:
+                    raise
                 dataset_name = (
                     get_neuron_attr(dataset, wf_n, "dataset_id")
                     .ravel()[0]
                     .decode("utf-8")
                 )
                 discarded_df = pd.concat(
                     (
@@ -396,14 +497,17 @@
 
         self.targets = np.array(
             (pd.Series(self.labels_list).replace(_labelling).values)
         )
         self.wf = np.stack(self.wf_list, axis=0)
         self.acg = np.stack(acg_list_resampled, axis=0)
 
+        if hasattr(self, "quality_checks_mask"):
+            self.quality_checks_mask = np.array(self.quality_checks_mask)
+
         print(
             f"{len(self.wf_list)} neurons loaded, of which labelled: {sum(self.targets != -1)} \n"
             f"{len(discarded_df)} neurons discarded, of which labelled: {len(discarded_df[discarded_df.label != 0])}. More details at the 'discarded_df' attribute."
         )
 
     def make_labels_only(self):
         """
@@ -422,20 +526,37 @@
     def _apply_mask(self, mask):
         self.wf = self.wf[mask]
         self.acg = self.acg[mask]
         self.targets = self.targets[mask]
         self.info = np.array(self.info)[mask].tolist()
         self.spikes_list = np.array(self.spikes_list, dtype=object)[mask].tolist()
         self.labels_list = np.array(self.labels_list)[mask].tolist()
+        self.acg_list = np.array(self.acg_list)[mask].tolist()
+        try:
+            self.chanmap_list = np.array(self.chanmap_list, dtype=object)[mask].tolist()
+        # Numpy has still a bug in treating arrays as objects
+        except ValueError:
+            self.chanmap_list = [self.chanmap_list[i] for i in np.where(mask)[0]]
+
+        self.genetic_line_list = np.array(self.genetic_line_list, dtype=object)[
+            mask
+        ].tolist()
+
         if hasattr(self, "amplitudes_list"):
             self.amplitudes_list = np.array(self.amplitudes_list, dtype=object)[
                 mask
             ].tolist()
         if hasattr(self, "quality_checks_mask"):
             self.quality_checks_mask = self.quality_checks_mask[mask]
+            self.fn_fp_list = np.array(self.fn_fp_list, dtype=object)[mask].tolist()
+            self.sane_spikes_list = np.array(self.sane_spikes_list, dtype=object)[
+                mask
+            ].tolist()
+        if hasattr(self, "full_dataset"):
+            self.full_dataset = self.full_dataset[mask]
 
     def make_full_dataset(self, wf_only=False, acg_only=False):
         """
         This function takes the waveform and ACG data and concatenates them into a single array
 
         Args:
             wf_only: If True, only the waveform data will be used. Defaults to False
@@ -471,16 +592,15 @@
     def filter_out_granule_cells(self):
         """
         Filters out granule cells from the dataset and returns new LABELLING and CORRESPONDENCE dictionaries for plotting.
         """
 
         granule_cell_mask = self.targets == LABELLING["GrC"]
 
-        self._apply_mask(granule_cell_mask)
-
+        self._apply_mask(~granule_cell_mask)
         self.targets = (self.targets - 1).astype(int)
         self.targets[self.targets < 0] = -1  # Reset the label of unlabeled cells
 
         # To convert text labels to numbers
         new_labelling = {
             "PkC_cs": 4,
             "PkC_ss": 3,
@@ -520,74 +640,138 @@
         assert info_path in self.info, "No neuron for the dp and unit provided"
 
         wvf = self.wvf_from_info(dp, unit)
         train = self.train_from_info(dp, unit)
 
         npyx.plot.plt_wvf(wvf.T)
         plt.show()
-        npyx.plot.plot_acg("hello", 0, train=train)
+        npyx.plot.plot_acg(".npyx_placeholder", 0, train=train)
         plt.show()
 
     def apply_quality_checks(self):
         """
         It takes a dataset, checks that it has a quality_checks_mask attribute, and then applies that
         mask to the dataset
 
         Returns:
           A new dataset with the quality checks applied.
         """
         assert hasattr(
             self, "quality_checks_mask"
         ), "No quality checks mask found, perhaps you have applied them already?"
         checked_dataset = copy.deepcopy(self)
+        checked_dataset.spikes_list = [
+            train[fn_fp_mask[sane_mask]]
+            for train, fn_fp_mask, sane_mask in zip(
+                self.spikes_list, self.fn_fp_list, self.sane_spikes_list
+            )
+        ]
         checked_dataset._apply_mask(checked_dataset.quality_checks_mask)
         del checked_dataset.quality_checks_mask
+        del checked_dataset.fn_fp_list
+        del checked_dataset.sane_spikes_list
+
         return checked_dataset
 
     def __len__(self):
         return len(self.wf)
 
 
 def merge_h5_datasets(*args: NeuronsDataset) -> NeuronsDataset:
     """Merges multiple NeuronsDatasets instances into one"""
     new_dataset = copy.deepcopy(args[0])
     for dataset in args[1:]:
         assert isinstance(dataset, NeuronsDataset)
         new_dataset.wf = np.vstack((new_dataset.wf, dataset.wf))
         new_dataset.acg = np.vstack((new_dataset.acg, dataset.acg))
         new_dataset.targets = np.hstack((new_dataset.targets, dataset.targets))
+        new_dataset.chanmap_list = new_dataset.chanmap_list + dataset.chanmap_list
+        new_dataset.genetic_line_list = (
+            new_dataset.genetic_line_list + dataset.genetic_line_list
+        )
         new_dataset.info = np.hstack(
             (np.array(new_dataset.info), np.array(dataset.info))
         ).tolist()
+        new_dataset.acg_list = np.vstack(
+            (np.array(new_dataset.acg_list), np.array(dataset.acg_list))
+        ).tolist()
         new_dataset.spikes_list = np.hstack(
             (
                 np.array(new_dataset.spikes_list, dtype=object),
                 np.array(dataset.spikes_list, dtype=object),
             )
         ).tolist()
         new_dataset.discarded_df = pd.concat(
             (new_dataset.discarded_df, dataset.discarded_df), axis=0
         )
         new_dataset.labels_list = new_dataset.labels_list + dataset.labels_list
 
-        if hasattr(new_dataset, "amplitudes_list") and hasattr(
-            dataset, "amplitudes_list"
-        ):
-            new_dataset.amplitudes_list = (
-                new_dataset.amplitudes_list + dataset.amplitudes_list
-            )
-        else:
-            raise NotImplementedError(
-                "Attempted to merge datasets with different attributes"
-            )
+        if hasattr(new_dataset, "amplitudes_list"):
+            if hasattr(dataset, "amplitudes_list"):
+                new_dataset.amplitudes_list = (
+                    new_dataset.amplitudes_list + dataset.amplitudes_list
+                )
+            else:
+                raise NotImplementedError(
+                    "Attempted to merge datasets with different attributes"
+                )
+
+        if hasattr(new_dataset, "quality_checks_mask"):
+            if hasattr(dataset, "quality_checks_mask"):
+                new_dataset.quality_checks_mask = np.hstack(
+                    (new_dataset.quality_checks_mask, dataset.quality_checks_mask)
+                )
+                new_dataset.fn_fp_list = new_dataset.fn_fp_list + dataset.fn_fp_list
+                new_dataset.sane_spikes_list = (
+                    new_dataset.sane_spikes_list + dataset.sane_spikes_list
+                )
+            else:
+                raise NotImplementedError(
+                    "Attempted to merge datasets with different attributes"
+                )
+    new_dataset.dataset = "merged"
 
-        if hasattr(new_dataset, "quality_checks_mask") and hasattr(
-            dataset, "quality_checks_mask"
-        ):
-            new_dataset.quality_checks_mask = np.hstack(
-                (new_dataset.quality_checks_mask, dataset.quality_checks_mask)
-            )
-        else:
-            raise NotImplementedError(
-                "Attempted to merge datasets with different attributes"
-            )
     return new_dataset
+
+
+def resample_waveforms(
+    dataset: NeuronsDataset, sampling_rate: int = 30_000
+) -> NeuronsDataset:
+    """
+    It takes a dataset, resizes the waveforms to a new sampling rate, and returns a new dataset with the
+    resized waveforms
+
+    Args:
+      dataset (NeuronsDataset): the dataset to be resampled
+      sampling_rate (int): the sampling rate of the new waveforms. Defaults to 30_000
+
+    Returns:
+      A new dataset with the same properties as the original dataset, but with the waveforms resampled.
+    """
+
+    import torch
+    from torchvision import transforms
+
+    original_wf = dataset.wf.reshape(-1, 1, dataset._n_channels, dataset._central_range)
+
+    new_range = int(dataset._central_range * sampling_rate / dataset._sampling_rate)
+
+    resize = transforms.Resize((dataset._n_channels, new_range))
+
+    resized_wf = resize(torch.tensor(original_wf)).squeeze().numpy()
+
+    resized_wf = resized_wf.reshape(-1, dataset._n_channels * new_range)
+
+    resampled_dataset = copy.deepcopy(dataset)
+    resampled_dataset.wf = resized_wf
+    resampled_dataset._central_range = new_range
+    resampled_dataset.wf_list = [wf for wf in resized_wf]
+
+    return resampled_dataset
+
+
+def force_amplitudes_length(amplitudes, times):
+    if len(times) > len(amplitudes):
+        times = times[: len(amplitudes)]
+    if len(amplitudes) > len(times):
+        amplitudes = amplitudes[: len(times)]
+    return amplitudes, times
```

### Comparing `npyx-2.7.1/npyx/feat.py` & `npyx-2.8.0/npyx/feat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 2021-4-22
 Authors: @fededagos, @agolajko
 
 Functions needed to extract temporal and waveform features from Neuropixels recordings.
 """
+from __future__ import annotations
+
 import json
 import os
 import sys
 from datetime import date
 from pathlib import Path
 
 import h5py
@@ -30,15 +32,15 @@
 from .spk_t import acg, trn_filtered
 from .spk_wvf import wvf_dsmatch
 
 # pylint: disable=unsupported-binary-operation
 
 FEATURES = [
     "label",
-    "dp",
+    "dataset",
     "unit",
     "mfr",
     "mifr",
     "med_isi",
     "mode_isi",
     "prct5ISI",
     "entropy",
@@ -72,15 +74,20 @@
     "multiplicative_a_recovery",
     "repolarisation_slope",
     "depolarisation_slope",
     "spatial_decay_24um",
     "dendritic_comp_amp",
 ]
 
-AMPLITUDE_FEATURES = ["peak_voltage", "trough_voltage", "onset_amp"]
+AMPLITUDE_FEATURES = [
+    "peak_voltage",
+    "trough_voltage",
+    "onset_amp",
+    "multiplicative_a_recovery",
+]
 
 CORRELATED_FEATURES = [
     "mifr",
     "CV2_mean",
     "med_isi",
     "prct5ISI",
     "Lv",
@@ -1171,15 +1178,15 @@
     waveform_2d, peak_chan, relevant_channel, somatic_mask, chanmap
 ):
     """
     - peak_chan: channel from which the 1D waveworm features will be extracted
     """
 
     # ratio between max amplitude among 4/5 closest channels at 23.61 um and max amplitude on peak channel
-
+    chanmap = np.array(chanmap)
     spatial_spread_ratio = chan_spread(waveform_2d, peak_chan, chanmap)
     # set to 1 if relevant waveform is dendritic already (because normalized)
     max_dendritic_voltage = (
         dendritic_component(waveform_2d, relevant_channel, somatic_mask)
         if somatic_mask.any()
         else 1
     )
@@ -1582,14 +1589,15 @@
     quality_check=True,
     labels_only=True,
     _debug=False,
     _n_channels=21,
     _central_range=82,
     _label=None,
     _sampling_rate=30_000,
+    _use_chanmap=True,
 ):
     """
     It takes a NeuronsDataset instance coming from an h5 dataset and extracts the features.
 
     Params:
 
         dataset_path (str):  path to the h5 dataset
@@ -1605,43 +1613,54 @@
     """
     if _label is None:
         _label = "optotagged_label"
     columns = FEATURES
 
     feat_df = pd.DataFrame(columns=columns)
 
-    dataset = NeuronsDataset(
-        dataset_path,
-        quality_check=quality_check,
-        normalise_wvf=False,
-        n_channels=_n_channels,
-        central_range=_central_range,
-        _use_amplitudes=True,
-        _label=_label,
-    )
+    if isinstance(dataset_path, NeuronsDataset):
+        dataset = dataset_path
+    else:
+        dataset = NeuronsDataset(
+            dataset_path,
+            quality_check=quality_check,
+            normalise_wvf=False,
+            n_channels=_n_channels,
+            central_range=_central_range,
+            _use_amplitudes=True,
+            _label=_label,
+        )
+
+    if labels_only:
+        dataset.make_labels_only()
 
     if labels_only:
         dataset.make_labels_only()
 
     for i in tqdm(range(len(dataset)), desc="Extracting features"):
         dp = "/".join(dataset.info[i].split("/")[:-1])
         unit = int(dataset.info[i].split("/")[-1])
         label = CORRESPONDENCE[dataset.targets[i]]
         waveform = dataset.wf[i].reshape(dataset._n_channels, dataset._central_range)
         spike_train = dataset.spikes_list[i]
         # Recover the channelmap
-        try:
-            chanmap_path = f"datasets/{dataset.info[i]}/channelmap"
-            with h5py.File(dataset_path, "r") as hdf5_file:
-                chanmap = hdf5_file[chanmap_path][(...)]
-                if fix_chanmap:
-                    chanmap = recover_chanmap(chanmap)
-        except KeyError:
+        if _use_chanmap:
+            try:
+                if isinstance(dataset_path, NeuronsDataset):
+                    chanmap = dataset.chanmap_list[i]
+                else:
+                    chanmap_path = f"datasets/{dataset.info[i]}/channelmap"
+                    with h5py.File(dataset_path, "r") as hdf5_file:
+                        chanmap = hdf5_file[chanmap_path][(...)]
+                        if fix_chanmap:
+                            chanmap = recover_chanmap(chanmap)
+            except KeyError:
+                chanmap = None
+        else:
             chanmap = None
-
         try:
             wvf_features = waveform_features(
                 waveform,
                 dataset._n_channels // 2,
                 chanmap,
                 plot_debug=_debug,
             )
@@ -1652,69 +1671,67 @@
 
         except Exception as e:
             exc_type, _, exc_tb = sys.exc_info()
             print(
                 f"Something went wrong for the feature computation of neuron {i} (unit {unit} in {dp})"
             )
             print(f"{exc_type} at line {exc_tb.tb_lineno}: {e}")
-            if ignore_exceptions:
-                curr_feat = np.zeros(len(columns))[3:].tolist()
-                discarded_info = [label, dp, unit]
-                curr_feat = discarded_info + curr_feat
-                feat_df = feat_df.append(
-                    dict(zip(columns, curr_feat)), ignore_index=True
-                )
-            else:
+            if not ignore_exceptions:
                 raise
 
+            curr_feat = np.zeros(len(columns))[3:].tolist()
+            discarded_info = [label, dp, unit]
+            curr_feat = discarded_info + curr_feat
+            feat_df = feat_df.append(dict(zip(columns, curr_feat)), ignore_index=True)
     feat_df = feat_df.infer_objects()
     if save_path is None:
         save_path = os.getcwd()
         today = date.today().strftime("%b-%d-%Y")
         feat_df.to_csv(os.path.join(save_path, f"{today}_all_features.csv"))
     else:
         feat_df.to_csv(save_path)
 
     return feat_df
 
 
-def filter_df(df: pd.DataFrame) -> pd.DataFrame:
+def get_unusable_features(df: pd.DataFrame) -> pd.DataFrame:
     """
-    Filters out datapoints with unusable features.
+    Returns the index of unusable features
     """
+    df = df.replace([np.inf, -np.inf], np.nan)
     features_only = df.iloc[:, 2:]
     bad_idx = []
     for i, row in features_only.iterrows():
         value, count = np.unique(row.to_numpy(), return_counts=True)
         zeros = count[value == 0]
         if zeros.size > 0 and zeros > 5:
             bad_idx.append(i)
-    keep = [i for i in range(len(df)) if i not in bad_idx]
-    df.dropna(inplace=True)
-    return df.iloc[keep]
+    bad_idx += df.index[df.isna().any(axis=1)].tolist()
 
+    return np.unique(bad_idx)
 
-def generate_train_and_labels(df: pd.DataFrame, drop_cols=None):
-    """
-    It takes a dataframe and returns a tuple of two dataframes, one with the features and one with the
-    labels
-
-    Args:
-      df (pd.DataFrame): the dataframe to generate the train and labels from
-      drop_cols: a list of columns to drop from the dataframe.
 
-    Returns:
-      The dataframe with the columns dropped and the labels
+def prepare_classification(
+    df: pd.DataFrame, bad_idx=None, drop_cols=None
+) -> tuple[pd.DataFrame, pd.Series]:
+    """
+    Prepares the dataframe for classification.
     """
+
     if drop_cols is None:
         drop_cols = [
             "label",
-            "dp",
+            "dataset",
             "unit",
             "relevant_channel",
             "any_somatic",
             "max_peaks",
-            "trough_t",
-            "peak_t",
-        ] + AMPLITUDE_FEATURES
-    new_df = df.drop(columns=drop_cols)
-    return new_df.copy(), df.loc[:, "label"].copy()
+        ]
+    if bad_idx is not None:
+        df = df.drop(index=bad_idx)
+        df = df.reset_index(drop=True)
+
+    df = df.infer_objects()
+
+    X, y = df.drop(columns=drop_cols, axis=1), df["label"]
+
+    return X, y
```

### Comparing `npyx-2.7.1/npyx/gl.py` & `npyx-2.8.0/npyx/gl.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,22 +260,22 @@
         # if first time this is ran on a merged dataset
         return True
 
     if qualities is None:
         assert "merged" not in str(
             dp
         ), "this function should be ran on an original sorted dataset, not on a merged dataset."
-        last_spikesort  = os.path.getmtime(dp / "spike_clusters.npy")
+        last_spikesort = os.path.getmtime(dp / "spike_clusters.npy")
         last_tsv_update = os.path.getmtime(dp / "cluster_group.tsv")
-        spikesorted     = last_tsv_update == last_spikesort
+        spikesorted = last_tsv_update == last_spikesort
 
     else:
         qualities_old = pd.read_csv(dp / "cluster_group.tsv", delim_whitespace=True)
-        old_clusters  = qualities_old.loc[:, "cluster_id"]
-        new_clusters  = qualities.loc[:, "cluster_id"]
+        old_clusters = qualities_old.loc[:, "cluster_id"]
+        new_clusters = qualities.loc[:, "cluster_id"]
         if not np.all(np.isin(old_clusters, new_clusters)):
             spikesorted = True
 
     if spikesorted and print_message:
         print("\n\033[34;1m--- New spike-sorting detected.\033[0m")
 
     return spikesorted
@@ -283,14 +283,17 @@
 
 def save_qualities(dp, qualities):
     dp = Path(dp)
     qualities.to_csv(dp / "cluster_group.tsv", sep="\t", index=False)
 
 
 def generate_units_qualities(dp):
+    """
+    Creates an empty table of units qualities ("groups" as in good, mua,...).
+    """
     units = np.unique(np.load(Path(dp, "spike_clusters.npy")))
     qualities = pd.DataFrame({"cluster_id": units, "group": ["unsorted"] * len(units)})
     return qualities
 
 
 def load_units_qualities(dp, again=False):
     """
@@ -319,15 +322,15 @@
             qualities = generate_units_qualities(dp)
         else:
             if "unsorted" not in qualities["group"].values:
                 regenerate = True
         if regenerate:
             qualities_new = generate_units_qualities(dp)
 
-            sorted_clusters     = qualities.loc[qualities["group"] != "unsorted", :]
+            sorted_clusters = qualities.loc[qualities["group"] != "unsorted", :]
             unsorted_clusters_m = ~np.isin(
                 qualities_new["cluster_id"], sorted_clusters["cluster_id"]
             )
             unsorted_clusters = qualities_new.loc[unsorted_clusters_m, :]
 
             qualities = unsorted_clusters.append(sorted_clusters).sort_values(
                 "cluster_id"
@@ -360,15 +363,15 @@
     """
 
     dp_merged = Path(dp_merged)
 
     if ds_table is None:
         ds_table = get_ds_table(dp_merged)
 
-    qualities = pd.DataFrame(columns = ["cluster_id", "group"])
+    qualities = pd.DataFrame(columns=["cluster_id", "group"])
     for ds_i in ds_table.index:
         cl_grp = load_units_qualities(ds_table.loc[ds_i, "dp"])
         cl_grp["cluster_id"] = cl_grp["cluster_id"] + 1e-1 * ds_i
         qualities = qualities.append(cl_grp, ignore_index=True)
 
     return qualities
 
@@ -391,15 +394,15 @@
     else:
         qualities = load_units_qualities(dp, again=again)
 
     if quality == "all":
         units = qualities["cluster_id"].values
     else:
         quality_m = qualities["group"] == quality
-        units     = qualities.loc[quality_m, "cluster_id"].values
+        units = qualities.loc[quality_m, "cluster_id"].values
 
     if chan_range is None:
         return units
 
     assert len(chan_range) == 2, "chan_range should be a list or array with 2 elements!"
 
     # For regular datasets
@@ -432,9 +435,9 @@
         np.diff(periods, axis=1) > 0
     ), "all pairs of periods must be in ascendent order (t1.1<t1.2 etc in [[t1.1,t1.2],...])!"
     return periods
 
 
 # circular imports
 from npyx.inout import read_metadata
-from npyx.spk_wvf import get_depthSort_peakChans
 from npyx.merger import assert_multi, get_ds_table, merge_datasets
+from npyx.spk_wvf import get_depthSort_peakChans
```

### Comparing `npyx-2.7.1/npyx/h5.py` & `npyx-2.8.0/npyx/h5.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,550 +1,701 @@
+import gc
 import json
 import re
-import gc
 import sys
 import time
 import warnings
 from pathlib import Path
 
 import h5py
 import numpy as np
 from tqdm import tqdm
 
 from npyx.gl import check_periods, get_units
-from npyx.inout import (chan_map, detect_hardware_filter, extract_rawChunk,
-                        get_binary_file_path, get_npix_sync,
-                        preprocess_binary_file, read_metadata)
-from npyx.spk_t import ids, trn, trn_filtered
-from npyx.spk_wvf import wvf_dsmatch
-from npyx.utils import assert_float, assert_int
+from npyx.inout import (
+    chan_map,
+    detect_hardware_filter,
+    extract_rawChunk,
+    get_binary_file_path,
+    get_npix_sync,
+    preprocess_binary_file,
+    read_metadata,
+)
+from npyx.spk_t import (
+    duplicates_mask,
+    find_stable_recording_period,
+    ids,
+    trn,
+    trn_filtered,
+)
+from npyx.spk_wvf import across_channels_SNR, get_waveforms, wvf_dsmatch
+from npyx.utils import assert_float, assert_int, docstring_decorator
 
+## Ground truth labelling functions
 
-# High level C4 functions
-def label_optotagged_unit_h5(h5_path, dataset, unit, label, prnt=False):
+
+def label_optotagged_unit_h5(h5_path, dataset, unit, label, source=None, prnt=False):
     """
     Add optotagged label to neuron.
 
     - h5_path: full path to h5 file
     - dataset: str, neuron dataset (yy-mm-dd_mouse_probex)
     - unit: neuron unit index
     - label: label to add
     """
     authorized_labels = ["PkC_ss", "PkC_cs", "MLI", "MFB", "GoC", "GrC"]
-    assert label in authorized_labels, f"{label} must match either of the following: {authorized_labels}"
-    add_data_to_unit_h5(h5_path, dataset, unit, label, 'optotagged_label') 
-    if prnt: print(f"Labelled unit {unit} as {label}.")
+    assert (
+        label in authorized_labels
+    ), f"{label} must match either of the following: {authorized_labels}"
+    add_data_to_unit_h5(h5_path, dataset, unit, label, "ground_truth_label")
+    if source is not None:
+        add_data_to_unit_h5(h5_path, dataset, unit, source, "ground_truth_source")
+    if prnt:
+        print(f"Labelled unit {unit} as {label}.")
+
 
 def reset_optotagged_labels(h5_path):
     """Resets all optotagged labels to 0"""
     with h5py.File(h5_path, "a") as h5_f:
         for neuron in h5_f.keys():
-            if 'hausser_neuron' not in neuron: continue
-            data_path = f"{neuron}/optotagged_label"
+            if "hausser_neuron" not in neuron:
+                continue
+            data_path = f"{neuron}/ground_truth_label"
             write_to_dataset(h5_f, data_path, 0, overwrite=True)
 
-def add_units_to_h5(h5_path, dp, units=None, **kwargs):
-    f"""
-    Add all or specified units at the respective data path to an HDF5 file.
-
-    This is a high-level function designed to add many units at the
-    specified datapath to an HDF5 file. All additional key-value 
-    arguments are passed to `add_unit_h5`
 
-    Example:
-      add_units_to_h5('my_lab_data.h5', '/path/to/dataset_id', lab_id='pi_last_name')
-    Will add all sorted units in the 'kilosort_results' directory 
-    to the HDF5 file called 'my_lab_data.h5' (in the current directory).
+### Major C4 database generation function
 
-    Other arguments from add_unit_h5:
-    {add_unit_h5.__doc__}
-    """
 
-    if units is None:
-        units = get_units(dp)
+def add_unit_h5(
+    h5_path,
+    dp,
+    unit_id,
+    lab_id,
     
-    for u in units:
-        add_unit_h5(h5_path, dp, u, **kwargs)
-
-
-def relative_unit_path_h5(dataset, unit):
-    return f"datasets/{dataset}/{unit}"
-
-
-def get_unit_paths_h5(h5_file, dataset, unit,
-                      lab_id = 'hausser', unit_absolute_id = None):
-    relative_unit_path = relative_unit_path_h5(dataset, unit)
-    if relative_unit_path in h5_file:
-            absolute_unit_path = h5_file[f'{relative_unit_path}/neuron_absolute_id'][()].decode()
-    else:
-        if unit_absolute_id is None:
-            if f"{lab_id}_neuron_0" not in h5_file:
-                unit_absolute_id = 0
-            else:
-                root_groups = list(h5_file.keys())
-                neuron_ids = [int(x.split('_')[-1]) for x in root_groups if f"{lab_id}_neuron" in x]
-                unit_absolute_id = np.sort(neuron_ids)[-1] + 1
-        absolute_unit_path = f'{lab_id}_neuron_{unit_absolute_id}'
-            
-    return relative_unit_path, absolute_unit_path
-
-
-def remove_unit_h5(h5_path, dp, unit, lab_id='hausser'):
-    dataset = Path(dp).name
-    with h5py.File(h5_path, "a") as h5_file:
-        relative_unit_path, absolute_unit_path = get_unit_paths_h5(h5_file, dataset, unit, lab_id)
-        del h5_file[relative_unit_path]
-        del h5_file[absolute_unit_path]
-        dataset_path = str(Path(relative_unit_path).parent)
-        if len(h5_file[dataset_path].keys()) == 0:
-            del h5_file[dataset_path]
-
-
-def add_unit_h5(h5_path, dp, unit, lab_id, periods='all',
-                sync_chan_id=None, overwrite_h5=False,
-                again=False, again_wvf=False, plot_debug=False, verbose=False,
-                dataset=None,
-                raw_window=[0.1, 30.1], center_raw_window_on_spikes=True,
-                include_raw_snippets=True, include_whitened_snippets=True,
-                raw_snippet_halfrange=2, mean_wvf_half_range=11,
-                sane_spikes=None, sane_periods=None, sane_before_opto=False, include_fp_fn_mask=True,
-                optostims=None, optostims_from_sync=False, optostims_threshold=None,
-                n_waveforms_for_matching=5000, selective_overwrite=None,
-                **kwargs):
+    genetic_line             = "",
+    dataset                  = None,
+    sane_periods             = None,
+    sane_spikes              = None,
+    sane_before_opto         = False,
+    
+    again_npyx               = False,
+    again_npyx_wvf           = False,
+    
+    overwrite_h5             = False,
+    selective_overwrite      = None,
+    
+    include_fp_fn_mask       = True,
+    include_raw_snippets     = True,
+    
+    raw_window               = None,
+    raw_snippet_halfrange    = 3,
+    mean_wvf_half_range      = 11,
+    
+    opto_sync_chan_id        = None,
+    optostims                = None,
+    optostims_from_sync      = False,
+    optostims_threshold      = None,
+    
+    n_waveforms_for_matching = 5000,
+    n_raw_waveforms          = 1000,
+    plot_debug               = False,
+    **kwargs,
+):
     """
-    Add a spike-sorted unit to an HDF5 file (on a phy compatible dataformat).
-
     Adds a spike-sorted unit to a new or existing HDF5 five file using the
     file format specified by the C4 collaboration.
-    
-     ---->>> data format details here www.tinyurl.com/c4database <<<---
+
+    Data format details here ---->>> www.tinyurl.com/c4database <<<---
 
     Each unit can be accessed from 2 paths which point to the same data:
     - an absolute path, {unit_absolute_id}/
                         which allows for a flat hierarchy and makes it easier to compute features,
                         easier to work on data from other labs
     - a relative path, datasets/{dataset}/{unit}/
                        which allows to index units per dataset,
                        easier to work on your own data
 
     Example:
         add_unit_h5('my_lab_data.h5', '/path/to/kilosort_results', 1, lab_id='pi_last_name')
     Adds the unit with id 1 to the HDF5 file in the current directory called 'my_lab_data.h5'.
-    Additional units can be added by calling the same function with identical arguments,
-    but incrementing the unit id field.
+    Additional units can be added by calling the same function with identical
+    arguments, but incrementing the unit_id field.
 
     Required Arguments:
     - h5_path: Path to the h5 file to create/append
     - dp: Path the Kilosort data directory
-    - unit: The unit id/neuron unit index
+    - unit_id: The unit id/neuron unit index
     - lab_id: The lab/PI id to use to label the units
-    - periods: 'all' or [[t1,t2],[t3,t4],...] in seconds
 
-    Key-value Arguments:
-    - unit_absolute_id: unit absolute id. Will increment from the last unit added to h5 file.
-    - sync_chan_id: The channel id used to denote opto stimulation. Defaults to None.
-    - again: Whether to use cached results for storage in the HDF5 file (defaults to False)
-    - again_wvf: Whether to recompute drift-shift matched waveform in particular (very computationally intensive, defaults to False)
-    - verbose: Additional verbosity/progress
+
+    Optional Arguments:
+
+    - genetic_line: The genetic line of the animal used to record this data. None by default.
     - dataset: A unique ID for this dataset. By default this value is None, in which case
-      the dataset id is assumed to the dirname of the data directory passed as the dp argument
-      
-    - raw_window: A two item list containing the start and stop times (in SECONDS) of the snippet of raw data used for
-                  1) computing noise RMS (-> SNR)
-                  2) extracting representative examples of raw data (raw, and whitened).
-    - center_raw_window_on_spikes: bool, whether to roughly center the raw voltage snippets window (raw_window) on neuron's first spike
-    - raw_snippet_halfrange: int, range of channels around peak channel to consider for the snippet of raw data (max 10)
-    - include_raw_snippets: bool, whether to include (memory heavy) raw data snippets (normally median subtracted and forward high pass filtered).
-    - include_whitened_snippets: bool, whether to include (memory heavy) preprocessed (whitened, filtered backward) data snippets (raw).
-    
-    - sane_spikes: optional bool array, custom definition of 'sane spikes' for whatever reason.
-                   By default, will be all spikes within 'periods'.
-    - sane_periods: optional list of [start, stop] periods, in seconds, to define 'sane spikes'. Will prevail over "sane_before_opto" if both are defined.
+                the dataset id is assumed to the dirname of the data directory passed as the dp argument.
+
+    - sane_periods: optional list of [start, stop] periods, in seconds, to define the 'sane spikes' boolean mask.
+                    These will be the spikes used to compute the mean waveform and included in any futher analysis.
+                    Will prevail over "sane_before_opto" if both are defined.
+    - sane_spikes: optional bool array, custom definition of 'sane spikes'.
+                   By default, will be all spikes within 'sane_periods' and will prevail over them if both are defined.
     - sane_before_opto: bool, whether to consider all spikes before the 1st optostim
                         to constitute the sane_spikes boolean mask.
                         Will only work if optostims are provided (or alternatively optostims_from_sync is True.)
+
+    - again_npyx: Whether to recompute data from scratch rather than load NeuroPyxels cached results for storage in the HDF5 file (defaults to False)
+    - again_npyx_wvf: Whether to recompute drift-shift matched waveform in particular (very computationally intensive, defaults to False)
+    - overwrite_h5: Whether to fully delete any pre-existing unit data and overwrite it (defaults to False).
+    - selective_overwrite: list of strings, which fields to specifically recompute even if again is False (much faster if only one field to overwrite).
+
     - include_fp_fn_mask: bool, whether to compute the false positive and false negative rates for recording periods
                           and subsequently compute the 'fn_fp_filtered_spikes', which is True for spikes in periods
                           passing the 5% fp and 5% fn quality requirement and False for other spikes.
-                   
+    - include_raw_snippets: bool, whether to include 30sec raw data snippets
+                            alongside a 3d matrix of 1000 randomly sampled waveforms.
+
+    - raw_window: A two item list containing the start and stop times (in SECONDS) of the snippet of raw data used for
+                  1) computing single channel noise RMS (-> SNR)
+                  2) extracting representative examples of raw data (raw, and whitened).
+                  If None, will use a period of 30 seconds within sane_periods with the most spikes.
+    - raw_snippet_halfrange: int, range of channels around peak channel to consider for the snippet
+                             of raw data (max 10, default 3 resulting in 7 channels total)
+    - mean_wvf_half_range: int, range of channels around peak channel to consider for the mean waveform. Default 11 (23 channels total).
+
+    - opto_sync_chan_id: The index of the npix binary channel where the optostim triggers are written. Defaults to None.
     - optostims: an optional 2D array (n_stims, 2) containing the optostimuli times in seconds
                  (1st column: onsets, 2nd column: offsets).
-                 By default None, will be read from sync channel (at sync_chan_id) if optostims_from_sync is True.
+                 By default None, will be read from sync channel (at opto_sync_chan_id) if optostims_from_sync is True.
     - optostims_from_sync: bool, whether to pick up optostims from sync channel if None are provided.
     - optostims_threshold: float, time before which optostims will be ignored (same units as optostims, seconds if optostims_from_sync=True).
                            (handles sync signals without light at beginning of recording)
-                           
+
     - n_waveforms_for_matching: int, number of waveforms to subsample for drift-shift matching
-    - selective_overwrite: list of strings, which fields to specifically recompute even if again is False (much faster if only one field to overwrite).
+    - n_raw_waveforms: int, number of raw waveforms to store in the HDF5 file at "raw_waveforms"
+    - plot_debug: bool, whether to save the debugging plots showing the the false positive/negative rate estimations
 
-    Additional key-value parameteters:
+    Additional key-value parameters:
     - *any_key* = *any_value*
-    All additional key-value parameters passed to this function are stored in the HDF5 file.
-    Therefore, custom keys can be stored in the HDF5 file should additional
-    information be required for an individual neuron. E.g., calling
-        add_unit_h5('my_lab_data.h5', '/path_to_kilosort_results', 1, my_note="Cool info")
-    will result in a key of 'my_note' and a value of "Cool info" being stored in the HDF5 file
-    for this unit.
+        All additional key-value parameters passed to this function are stored in the HDF5 file.
+        Therefore, custom keys can be stored in the HDF5 file should additional
+        information be required for an individual neuron. E.g., calling
+            add_unit_h5('my_lab_data.h5', '/path_to_kilosort_results', 1, my_note="Cool info")
+        will result in a key of 'my_note' and a value of "Cool info" being stored in the HDF5 file
+        for this unit.
     """
-    
+
     if selective_overwrite is not None:
-        assert isinstance(selective_overwrite, list), "Selective_overwrite must be a list of strings."
+        assert isinstance(
+            selective_overwrite, list
+        ), "Selective_overwrite must be a list of strings."
     else:
         selective_overwrite = []
-    
-    dp=Path(dp)
-    meta = read_metadata(dp) 
-    samp_rate = meta['highpass']['sampling_rate']
-    pbar = tqdm(total=11, desc=f"Adding unit {unit} to {h5_path}", position=0, leave=False, disable=(not verbose))
+
+    dp        = Path(dp)
+    meta      = read_metadata(dp)
+    samp_rate = meta["highpass"]["sampling_rate"]
     # hard-coded parameters
     waveform_samples = 6  # ms
-    waveform_samples = int(waveform_samples*samp_rate/1000)
+    waveform_samples = int(waveform_samples * samp_rate / 1000)
 
     # open file in append mode
     h5_path = Path(h5_path)
     assert_h5_file(h5_path)
     with h5py.File(h5_path, "a") as h5_file:
         
+        # --------------- h5 preformatting ---------------#
+
         # format dataset name
         if dataset is None:
             dataset = dp.name
         check_dataset_format(dataset)
-        
+
         # Define or fetch unit h5 paths
-        relative_unit_path, absolute_unit_path = get_unit_paths_h5(h5_file, dataset, unit, lab_id)
+        relative_unit_path, absolute_unit_path = get_unit_paths_h5(
+            h5_file, dataset, unit_id, lab_id
+        )
         if relative_unit_path in h5_file:
             if overwrite_h5:
                 del h5_file[relative_unit_path]
                 del h5_file[absolute_unit_path]
             else:
-                print(f"Neuron found in h5 file: {relative_unit_path} ({absolute_unit_path})")
+                print(f"Neuron found in h5 file: '{relative_unit_path}' ({absolute_unit_path})")
                 neuron_group = h5_file[absolute_unit_path]
         # redefine unit paths in case the unit got deleted
-        #relative_unit_path, absolute_unit_path = get_unit_paths_h5(h5_file, dataset, unit, lab_id)
-        
+        # relative_unit_path, absolute_unit_path = get_unit_paths_h5(h5_file, dataset, unit, lab_id)
+
         # create group for new neuron if necessary
         if relative_unit_path not in h5_file:
             neuron_group = h5_file.create_group(absolute_unit_path)
             h5_file[relative_unit_path] = neuron_group
-            print(f"Adding data at {relative_unit_path} ({absolute_unit_path})...")
+            print(f"Adding neuron at '{relative_unit_path}' ({absolute_unit_path})...")
+        pbar = tqdm(
+            total    = 7,
+            desc     = f"Adding unit at '{relative_unit_path}' ({absolute_unit_path})...",
+            position = 0,
+            leave    = True,
+            disable  = False,
+        )
+
+
+        # --------------- metadata ---------------#
 
-        # metadata
-        pbar.set_description(f"Adding metadata for unit {unit} to {h5_path}")
+        pbar.set_description(f"Adding metadata for unit '{relative_unit_path}'...")
         pbar.update(1)
-        write_to_group(neuron_group, 'lab_id', lab_id, overwrite_h5)
-        write_to_group(neuron_group, 'dataset_id', dataset, overwrite_h5)
-        write_to_group(neuron_group, 'neuron_id', unit, overwrite_h5)
-        write_to_group(neuron_group, 'neuron_absolute_id', neuron_group.name, overwrite_h5)
-        write_to_group(neuron_group, 'sampling_rate', samp_rate, overwrite_h5)
-        write_to_group(neuron_group, 'periods', samp_rate, overwrite_h5)
-        
+        write_to_group(neuron_group, "lab_id",             lab_id,            overwrite_h5)
+        write_to_group(neuron_group, "line",               genetic_line,      overwrite_h5)
+        write_to_group(neuron_group, "dataset_id",         dataset,           overwrite_h5)
+        write_to_group(neuron_group, "neuron_relative_id", unit_id,           overwrite_h5)
+        write_to_group(neuron_group, "neuron_id",          neuron_group.name, overwrite_h5)
+        write_to_group(neuron_group, "sampling_rate",      samp_rate,         overwrite_h5)
+
         # add any additional keys passed to this function
         for key, value in kwargs.items():
             write_to_group(neuron_group, key, value, overwrite_h5)
 
-        # spike_times
-        change_spike_train = overwrite_h5 or ("spike_times" in selective_overwrite)
-        periods = check_periods(periods)
-        pbar.set_description(f"Adding spike times for unit {unit} to {h5_path}")
+
+        # --------------- spike time-related ---------------#
+
+        pbar.set_description(f"Adding spike times for unit '{relative_unit_path}'...")
         pbar.update(1)
-        if 'spike_indices' not in neuron_group or change_spike_train:
-            t = trn(dp, unit, periods=periods, again=again)
-            write_to_group(neuron_group, 'spike_indices', t, change_spike_train)
-        else:
-            t = neuron_group['spike_indices']
+
+        # sane periods
+        if sane_periods is None:
+            sane_periods = "all"
+        sane_periods = check_periods(sane_periods)
+        write_to_group(neuron_group, "sane_periods", sane_periods, overwrite_h5)
+
+        # spike_times
+        key = "spike_indices"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+            t = trn(dp, unit_id, again=again_npyx).astype(np.uint32)
+            write_to_group(neuron_group, key, t)
 
         # optostims
-        pbar.set_description(f"Adding optostims for unit {unit} to {h5_path}")
+        pbar.set_description(f"Adding optostims for unit '{relative_unit_path}'...")
         pbar.update(1)
-        change_optostims = overwrite_h5 or ("optostims" in selective_overwrite)
-        if 'optostims' not in neuron_group or change_optostims:
-            pbar.set_description("Reading optostims...")
+        keys = ["optostims", "sane_spikes"]
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
             if optostims is None and optostims_from_sync:
-                ons, offs = get_npix_sync(dp, verbose=False)
-                if sync_chan_id is None:
-                    sync_chan_id = get_stim_chan(ons)
-                ons, offs = ons[sync_chan_id], offs[sync_chan_id]
+                ons, offs = get_npix_sync(dp)
+                if opto_sync_chan_id is None:
+                    opto_sync_chan_id = get_stim_chan(ons)
+                ons, offs = ons[opto_sync_chan_id], offs[opto_sync_chan_id]
                 if ons[0] > offs[0]:
-                    ons, offs = offs, ons 
+                    ons, offs = offs, ons
                 if len(offs) == len(ons) - 1:
-                    offs = np.append(offs, meta['recording_length_seconds'])
+                    offs = np.append(offs, meta["recording_length_seconds"])
                 optostims = np.hstack([ons[:, None], offs[:, None]])
             if optostims is not None and optostims_threshold is not None:
-                opto_m = optostims[:,0] > optostims_threshold
-                optostims = optostims[opto_m,:]
+                opto_m = optostims[:, 0] > optostims_threshold
+                optostims = optostims[opto_m, :]
 
             if optostims is not None:
-                write_to_group(neuron_group, 'optostims', optostims, change_optostims)
-    
-        # usable spikes mask
-        pbar.set_description(f"Adding sane spikes for unit {unit} to {h5_path}")
+                write_to_group(neuron_group, "optostims", optostims)
+
+        # sane spikes
+        key = "sane_spikes"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+            t = neuron_group["spike_indices"][...]
+            if sane_spikes is None:
+                if sane_before_opto:
+                    if "optostims" in neuron_group:
+                        optostims = neuron_group["optostims"][...]
+                    # Only consider spikes 10s before first opto onset
+                    end_spont_period = (optostims[0, 0] - 10) * samp_rate
+                    sane_spikes = t < end_spont_period
+                elif sane_periods is not None and sane_periods != "all":
+                    sane_spikes = (t * 0).astype(bool)
+                    for sane_period in sane_periods:
+                        sane_spikes = sane_spikes | (t >= sane_period[0] * samp_rate) & (t <= sane_period[1] * samp_rate)
+                else:
+                    # if sane_periods is None or 'all', keep them all
+                    sane_spikes = (t * 0 + 1).astype(bool)
+            write_to_group(neuron_group, key, sane_spikes)
+
+
+        # --------------- quality metrics 1/2 ---------------#
+        # required to define the snippet raw_window and the single waveforms to pick
+
+        pbar.set_description(f"Computing false positive/negative rate estimates for unit '{relative_unit_path}'...")
         pbar.update(1)
-        change_mask = overwrite_h5 or ("sane_spikes" in selective_overwrite)
-        if 'sane_spikes' not in neuron_group or change_mask:
-            if sane_spikes is None and\
-                sane_periods is not None:
-                sane_periods = check_periods(sane_periods)
-                sane_periods*=samp_rate
-                sane_spikes = (t*0).astype(bool)
-                for sane_period in sane_periods:
-                    sane_spikes = sane_spikes|(t>=sane_period[0])&(t<=sane_period[1])
-            elif sane_spikes is None and\
-                optostims is not None and\
-                sane_before_opto:
-                # Only consider spikes 10s before first opto onset
-                sane_spikes = (t < (optostims[0,0]-10)*samp_rate)
-            else:
-                sane_spikes = (t*0+1).astype(bool)
-            write_to_group(neuron_group, 'sane_spikes', sane_spikes, change_mask)
+        # false positive and negative estimation
+        key = "fn_fp_filtered_spikes"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite) and include_fp_fn_mask:
+            # get good spikes mask for all spikes
+            # because trn_filtered can only work on a contiguous chunk
+            periods_m_range = [0, meta["recording_length_seconds"] / 60]
+            fp_fn_good_spikes = trn_filtered(dp, unit_id,
+                                             plot_debug=plot_debug, again=again_npyx, 
+                                             period_m=periods_m_range)[1]
+            write_to_group(neuron_group, key, fp_fn_good_spikes)
 
 
-        # waveforms
-        pbar.set_description(f"Adding waveforms for unit {unit} to {h5_path}")
+        # --------------- waveform-related ---------------#
+
+        pbar.set_description(f"Extracting waveform-related data for unit '{relative_unit_path}'...")
         pbar.update(1)
-        include_sample = ["voltage_sample"] if include_raw_snippets else []
-        k = ['mean_waveform_preprocessed', 'amplitudes', 'peakchan_SNR'] + include_sample
-        change_waveforms = overwrite_h5 or any([key in selective_overwrite for key in k])
-        if not all_keys_in_group(k, neuron_group) or change_waveforms:
-            pbar.set_description("Reading waveforms...")
+
+        # make sure that peak channel is reloaded if raw voltage data must be included
+        raw_voltage_keys = ["raw_voltage_snippet", "raw_waveforms"] if include_raw_snippets else []
+
+        # extract waveforms (and also load peak channel found by dsmatching)
+        keys = [
+            "mean_waveform_preprocessed",
+            "channel_ids",
+            "channelmap",
+            "amplitudes",
+            "peakchan_SNR",
+            "raw_voltage_snippet",
+            "raw_waveforms",
+        ] + raw_voltage_keys
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
             # must recompute chan_bottom and chan_top - suboptimal, can be rewritten
-            dsm_tuple = wvf_dsmatch(dp, unit, t_waveforms=waveform_samples, periods=periods,
-                                    again=again_wvf, plot_debug=plot_debug, verbose=verbose,
-                                    n_waves_used_for_matching=n_waveforms_for_matching, 
-                                    med_sub = True, nRangeMedSub=None)
+            dsm_tuple = wvf_dsmatch(dp, unit_id,
+                t_waveforms=waveform_samples, periods=sane_periods,
+                again=again_npyx_wvf, plot_debug=plot_debug,
+                n_waves_used_for_matching=n_waveforms_for_matching,
+                med_sub=True, nRangeMedSub=None)
             dsm_waveform, peak_chan = dsm_tuple[1], dsm_tuple[3]
-            write_to_group(neuron_group, 'primary_channel', peak_chan)
-            chan_range = np.arange(peak_chan-mean_wvf_half_range, peak_chan+mean_wvf_half_range)
-            chan_range_m = (chan_range>=0)&(chan_range<=383)
-            chan_bottom, chan_top = chan_range[chan_range_m][0], chan_range[chan_range_m][-1]
-            peak_chan_rel = np.nonzero(peak_chan == chan_range[chan_range_m])[0]
+            peak_chan          = int(peak_chan)
+            chan_bottom        = np.max([0, peak_chan - mean_wvf_half_range])
+            chan_top           = np.min([383, peak_chan + mean_wvf_half_range])
+            chan_range         = np.arange(chan_bottom, chan_top)
+            peak_chan_rel      = np.nonzero(peak_chan == chan_range)[0][0]
             dsm_waveform_chunk = dsm_waveform[:, chan_bottom:chan_top]
-            write_to_group(neuron_group, 'mean_waveform_preprocessed',
-                           dsm_waveform_chunk.T, change_waveforms)
-            write_to_group(neuron_group, 'consensus_waveform',
-                           dsm_waveform_chunk.T*np.nan, change_waveforms)
-            cm = chan_map(dp)
-            write_to_group(neuron_group, 'channel_ids',
-                           np.arange(chan_bottom, chan_top, dtype=np.dtype('uint16')),
-                           change_waveforms)
-            write_to_group(neuron_group, 'channelmap', cm[chan_bottom:chan_top, 1:2], change_waveforms)
+            cm                 = chan_map(dp)
 
-        # Extract voltage snippets
-        pbar.set_description(f"Extracting voltage snippets for unit {unit} to {h5_path}")
-        pbar.update(1)
-        k = ['amplitudes', 'channel_noise_std', 'peakchan_SNR'] + include_sample
-        change_snippet = overwrite_h5 or any([key in selective_overwrite for key in k])
-        if not all_keys_in_group(k, neuron_group)\
-            or change_snippet:
-            pbar.set_description("Reading voltage sample...")
-            if center_raw_window_on_spikes:
-                t = h5_file[relative_unit_path+'/spike_indices'][...]/samp_rate
-                if raw_window[1]>t[0]: # spike starting after end of original window
-                    raw_window = np.array(raw_window)+t[0]
-                    raw_window[1]=min(raw_window[1], t[-1])
-            chunk = extract_rawChunk(dp, raw_window, channels=np.arange(chan_bottom, chan_top), 
-                                        scale=False, med_sub=False, whiten=False, center_chans_on_0=False,
-                                        hpfilt=False, verbose=False)
+            write_to_group(neuron_group, "mean_waveform_preprocessed", dsm_waveform_chunk.T)
+            write_to_group(neuron_group, "channel_ids", np.arange(chan_bottom, chan_top, dtype=np.dtype("uint16")))
+            write_to_group(neuron_group, "channelmap", cm[chan_bottom:chan_top, 1:3])
+
+        # scaling factor
+        write_to_group(neuron_group, "scaling_factor", meta["bit_uV_conv_factor"], overwrite_h5)
+
+        # Extraction of voltage snippet
+        keys = ["channel_noise_std", "peakchan_SNR", "raw_voltage_snippet"]
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
+            # find optimal window for raw snippet
+            if raw_window is None:
+                good_t = neuron_group["spike_indices"][...][neuron_group["fn_fp_filtered_spikes"][...]]
+                # handle cases where there is no good fp/fn section
+                if not np.any(good_t):
+                    good_t = neuron_group["spike_indices"][...]
+                raw_window = find_stable_recording_period(
+                    good_t,
+                    samp_rate,
+                    meta["recording_length_seconds"] * samp_rate,
+                    target_period = 30,
+                    b             = 1000,
+                    sd            = 10000,
+                    minimum_fr    = 0.4)
+                raw_window = np.array(raw_window) / samp_rate  # converge to seconds
+                
+            chunk = extract_rawChunk(dp, raw_window,
+                channels          = np.arange(chan_bottom, chan_top),
+                scale             = False,
+                med_sub           = False,
+                whiten            = False,
+                center_chans_on_0 = False,
+                hpfilt            = False) # already int16
+
+        # inclusion of voltage snippet
+        keys = ["raw_voltage_snippet", "voltage_snippet_start_index"]
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite) and include_raw_snippets:
+            raw_snippet_halfrange = np.clip(raw_snippet_halfrange, 0, 10)
+            c1                    = max(0, peak_chan_rel - raw_snippet_halfrange)
+            c2                    = min(chunk.shape[0] - 1, peak_chan_rel + raw_snippet_halfrange + 1)
+            raw_snippet           = chunk[c1:c2, :]
+            write_to_group(neuron_group, "raw_voltage_snippet", raw_snippet)  # still centered on peak channel, but half the size
+            write_to_group(neuron_group, "voltage_snippet_start_index", int(raw_window[0] * samp_rate))
+
+        # extraction of raw waveforms 3d matrix
+        key = "raw_waveforms"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite) and include_raw_snippets:
+            # relect spike ids
+            spike_ids  = ids(dp, unit_id, enforced_rp=0)
+            spike_mask = neuron_group["fn_fp_filtered_spikes"][...] & neuron_group["sane_spikes"][...]
+            if np.any(spike_mask):
+                spike_ids = spike_ids[spike_mask]
+
+            assert n_raw_waveforms > 0, "n_raw_waveforms must be > 0"
+            if len(spike_ids) > n_raw_waveforms:
+                random_ids = np.random.randint(0, spike_ids.shape[0]-1, n_raw_waveforms)
+                spike_ids  = spike_ids[random_ids]
+                
+            # load waveforms
+            raw_waveforms = get_waveforms(dp, unit_id, t_waveforms=180,
+                                            spike_ids=spike_ids, med_sub_in_time=False)
+            raw_waveforms = raw_waveforms[:, :, chan_bottom:chan_top].transpose(0,2,1)
+
+            # recast to int16
+            raw_waveforms = raw_waveforms / meta["bit_uV_conv_factor"]
+            raw_waveforms = raw_waveforms.astype(np.int16)
 
-        # quality metrics
-        pbar.set_description(f"Adding quality metrics for unit {unit} to {h5_path}")
-        pbar.update(1)
-        k = ['amplitudes', 'channel_noise_std', 'peakchan_SNR']
-        change_metrics = overwrite_h5 or any([key in selective_overwrite for key in k])
-        if not all_keys_in_group(k, neuron_group) or change_metrics:
-            pbar.set_description("Reading quality metrics...")
-            amps = np.load(dp/'amplitudes.npy').squeeze()[ids(dp, unit, periods=periods)]
-            
-            mad = np.median(np.abs(chunk) - np.median(chunk, axis=1)[:, None], axis=1) 
-            std_estimate = (mad / 0.6745) # Convert to std
-            peakchan_S = np.ptp(dsm_waveform[:,peak_chan])
-            peakchan_N = std_estimate[peak_chan_rel]
-            peakchan_SNR = peakchan_S / peakchan_N
-            
-            write_to_group(neuron_group, 'amplitudes', amps, change_metrics)
-            write_to_group(neuron_group, 'channel_noise_std', std_estimate, change_metrics)
-            write_to_group(neuron_group, 'peakchan_SNR', peakchan_SNR, change_metrics)
+            write_to_group(neuron_group, key, raw_waveforms)
 
-        pbar.set_description(f"Adding false positive and negative spikes for unit {unit} to {h5_path}")
+
+        # --------------- quality metrics 2/2 ---------------#
+
+        pbar.set_description(f"Computing SNR for unit '{relative_unit_path}'...")
         pbar.update(1)
-        change_fn_fp = overwrite_h5 or ('fn_fp_filtered_spikes' in selective_overwrite)
-        if ('fn_fp_filtered_spikes' not in neuron_group or overwrite_h5) and include_fp_fn_mask or change_fn_fp:
-            pbar.set_description("Reading false positive and false negative spikes...")
-            # get good spikes mask for all spikes
-            # because trn_filtered can only work on a contiguous chunk
-            if isinstance(periods, str): # can only be 'all', given check_periods
-                periods_m_range = [0, meta['recording_length_seconds']/60]
-            else:
-                periods_m_range = [periods.min()/60, periods.max()/60]
-            fp_fn_good_spikes = trn_filtered(dp, unit, plot_debug=plot_debug,
-                                             again=again, period_m=periods_m_range)[1]
-
-
-            # if periods is not all, trim down the mask to spikes in periods
-            if not isinstance(periods, str): # if str, can only be 'all', given check_periods
-                t = trn(dp, unit, periods=periods) # if again, as recomputed just above anyway, so don't pass the argument
-                t_all = trn(dp, unit) # grab all spikes
-                periods_mask = np.isin(t_all, t)
-                fp_fn_good_spikes = fp_fn_good_spikes[periods_mask]
-
-            write_to_group(neuron_group, 'fn_fp_filtered_spikes', fp_fn_good_spikes, change_fn_fp)
-            
-        # voltage snippets
-        pbar.set_description(f"Adding voltage snippets for unit {unit} to {h5_path}")
+
+        # SNR
+        keys = ["channel_noise_std", "peakchan_SNR"]
+        if assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
+            # both chunk and raw waveforms are in bits (int16)
+            mad           = np.median(np.abs(chunk - np.median(chunk, axis=1)[:, None]), axis=1)
+            std_estimate  = mad / 0.6745  # Convert to std
+            # peakchan_S  = np.ptp(dsm_waveform[:, peak_chan]) #overestimate
+            w             = neuron_group["raw_waveforms"][()].mean(0)
+            emp_peak_chan = np.argmax(np.ptp(w, axis=1))
+            peakchan_S    = np.ptp(w, axis=1)[emp_peak_chan]
+            peakchan_N    = std_estimate[emp_peak_chan]
+            peakchan_SNR  = peakchan_S / peakchan_N
+
+            write_to_group(neuron_group, "channel_noise_std", std_estimate)
+            write_to_group(neuron_group, "peakchan_SNR", peakchan_SNR)
+
+        # across channels SNR
+        key = "acrosschan_SNR"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+            acrosschan_SNR = across_channels_SNR(dp, unit_id)
+            write_to_group(neuron_group, key, acrosschan_SNR)
+
+        # amplitudes
+        key = "amplitudes"
+        if assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+            amps = np.load(dp / "amplitudes.npy").squeeze()[
+                ids(dp, unit_id, enforced_rp=0)
+            ]
+            write_to_group(neuron_group, key, amps)
+
+
+        # --------------- unit labels ---------------#
+
+        pbar.set_description(f"Adding labels for unit '{relative_unit_path}'...")
         pbar.update(1)
-        change_voltage_snippets = overwrite_h5 or ('voltage_sample' in selective_overwrite)
-        if ('voltage_sample' not in neuron_group or change_voltage_snippets)\
-            and include_raw_snippets:
-            pbar.set_description("Processing voltage snippets...")
-            # Only store the voltage sample for the primary channel
-            peak_chan = neuron_group['primary_channel']
-            raw_snippet_halfrange = np.clip(raw_snippet_halfrange, 0, 10)
-            c1 = max(0,int(chunk.shape[0]/2-raw_snippet_halfrange))
-            c2 = min(chunk.shape[0]-1, int(chunk.shape[0]/2+raw_snippet_halfrange+1))
-            raw_snippet = chunk[c1:c2,:]
-            write_to_group(neuron_group, 'voltage_sample', raw_snippet, change_voltage_snippets) # still centered on peak channel, but half the size
-            write_to_group(neuron_group, 'voltage_sample_start_index', int(raw_window[0] * samp_rate), change_voltage_snippets)
-            write_to_group(neuron_group, 'scaling_factor', meta['bit_uV_conv_factor'], change_voltage_snippets)
         
-        pbar.set_description(f"Adding whitened voltage snippets for unit {unit} to {h5_path}")
-        pbar.update(1)    
-        if ('whitened_voltage_sample' not in neuron_group or change_voltage_snippets)\
-            and include_whitened_snippets:
-            pbar.set_description("Reading whitened voltage snippets...")
-            if center_raw_window_on_spikes:
-                t = h5_file[relative_unit_path+'/spike_indices'][...]/samp_rate
-                if raw_window[1]>t[0]: # spike starting after end of original window
-                    raw_window = np.array(raw_window)+t[0]
-                    raw_window[1]=min(raw_window[1], t[-1])
-            # check that file filtered properly
-            bin_f = get_binary_file_path(dp)
-            if 'medsub' not in bin_f.name:
-                warnings.warn((f"WARNING file {bin_f.name} is expected to have been median subtracted,"
-                                " but its file name does not contain medsub..."))
-            if 'tempfiltNone300TrueFalse' not in bin_f.name:
-                warnings.warn((f"WARNING file {bin_f.name} is expected to have been highpass filtered forward only at 300Hz,"
-                                " but its file name does not contain tempfiltNone300TrueFalse..."))
-            # reprocess it
-            white_chunk = extract_rawChunk(dp, raw_window, channels=np.arange(chan_bottom, chan_top), 
-                                    scale=True, med_sub=False, hpfilt=True, filter_forward=False, filter_backward=True,
-                                    whiten=True, use_ks_w_matrix=True,
-                                    verbose=False)
-            raw_snippet_halfrange = np.clip(raw_snippet_halfrange, 0, 10)
-            c1 = max(0,int(white_chunk.shape[0]/2-raw_snippet_halfrange))
-            c2 = min(white_chunk.shape[0]-1, int(white_chunk.shape[0]/2+raw_snippet_halfrange+1))
-            raw_snippet = white_chunk[c1:c2,:].astype(np.float32)
-            write_to_group(neuron_group, 'whitened_voltage_sample', raw_snippet, change_voltage_snippets)
-
-        pbar.set_description(f"Adding labels for {unit} to {h5_path}")
         # layer
-        write_to_group(neuron_group, 'phyllum_layer', 0, overwrite_h5)
-        write_to_group(neuron_group, 'human_layer', 0, overwrite_h5)
+        write_to_group(neuron_group, "phyllum_layer",       "", overwrite_h5)
+        write_to_group(neuron_group, "human_layer",         "", overwrite_h5)
 
         # ground truth labels
-        write_to_group(neuron_group, 'expert_label', 0, overwrite_h5)
-        write_to_group(neuron_group, 'optotagged_label', 0, overwrite_h5)
-
-        # predicted labels
-        write_to_group(neuron_group, 'lisberger_label', 0, overwrite_h5)
-        write_to_group(neuron_group, 'hausser_label', 0, overwrite_h5)
-        write_to_group(neuron_group, 'medina_label', 0, overwrite_h5)
+        write_to_group(neuron_group, "expert_label",        "", overwrite_h5)
+        write_to_group(neuron_group, "ground_truth_label",  "", overwrite_h5)
+        write_to_group(neuron_group, "ground_truth_source", "", overwrite_h5)
+        write_to_group(neuron_group, "mli_cluster",         "", overwrite_h5)
 
-        pbar.update(1)
-        pbar.set_description(f"Done adding {unit} to {h5_path}")
+        pbar.set_description(f"Done with '{relative_unit_path}'.")
         pbar.refresh()
         time.sleep(0.01)
         pbar.close()
 
     return relative_unit_path
 
-def load_json_datasets(json_path, include_missing_datasets=False):
-    with open(json_path) as f:
-        json_f = json.load(f)
-
-    print(f"\nLoading data from file {json_path}...\n")
 
-    DSs = {}
-    for ds in json_f.values():
+### json wrapper functions
 
-        for key in ['dp', 'ct', 'units', 'ss', 'cs']:
-            assert key in ds, f"{key} not in json file for dataset #{ds}!"
-        
-        dp=Path(ds['dp'])
-        
-        if not dp.exists():
-            print(f"Dataset {dp} not found on system!\n")
-            if include_missing_datasets: DSs[dp.name] = ds
-            continue
-        DSs[dp.name] = ds
-        units = list(ds['units'])
-        ss = list(ds['ss'])
-        cs = list(ds['cs'])
-        print(f"Dataset {dp} found with opto responsive units {units}, simple spikes {ss}, complex spikes {cs}.\n")
-        all_units = units+ss+cs
-        units_m=np.isin(all_units, get_units(dp))
-        assert all(units_m), f"Units {np.array(all_units)[~units_m]} not found in {dp}!"
 
-    return DSs
+def add_json_datasets_to_h5(json_path, h5_path, lab_id,
+                            preprocess_if_raw             = False,
+                            delete_original_data          = False,
+                            data_deletion_double_check    = False,
+                            include_all_good              = True,
+                            selective_overwrite           = None,
+                            overwrite_h5                  = False,
+                            **kwargs): 
+    """
+    Wrapper function to loop over all datasets in a json file
+    and add them to an HDF5 file according to the C4 data format specification.
 
+    Data format details here ---->>> www.tinyurl.com/c4database <<<---
 
-def add_json_datasets_to_h5(json_path, h5_path, lab_id, preprocess_if_raw=False,
-                            delete_original_data=False, data_deletion_double_check=False,
-                            again=False, include_raw_snippets=False, verbose=False,
-                            include_all_good = False, **kwargs):
+    Arguments:
+        - json_path: str, path to the json file containing the datasets info
+            according to the following structure ("sane_periods" is optional):
+            "0": {
+                "ct": "celltype", see format at www.tinyurl.com/c4database
+                "line": "mouseline", see format at www.tinyurl.com/c4database
+                "dp": "/path/to/dataset",
+                "units": [u1, u2, u3, u4],
+                "ss": [u5, u6],
+                "cs": [u7, u8],
+                "sane_periods":{u1:[[t1,t2], [t3,t4]], u2:[], u3:[], u4:[], u5:[], u6:[], u7:[], u8:[]}
+                }
+        - h5_path: path/to/database_file.h5
+        - lab_id: str, lab id. see format at www.tinyurl.com/c4database
+        - preprocess_if_raw: bool, whether to high-pass filter the raw data
+                             if it is found to be so (for Hull lab)
+        - delete_original_data: bool, whether to delete the original raw file if it is preprocessed
+                                according to preprocess_if_raw
+        - data_deletion_double_check: bool, double check which must also be set to True
+                                      to allow deletion of the original data.
+        - include_all_good: bool, whether to include all good units in the dataset.
+                            Useful for unlabelled data, to train variational autoencoders.
+        - selective_overwrite: list of fields (e.g. spike_indices...) to recompute
+                                and overwrite if they already exist in the h5 file.
+        - overwrite_h5: bool, whether to recompute everything from scratch and overwrite the data
+                         (only for the reworked units, the other units will be left untouched in the file)
+    """
 
     DSs = load_json_datasets(json_path, include_missing_datasets=False)
 
-    for ds_name, ds in DSs.items():
-        dp=Path(ds['dp'])
+    for ds_name_ct, ds in DSs.items():
+        dp = Path(ds["dp"])
 
         if preprocess_if_raw:
             if not detect_hardware_filter(dp):
-                print("\033[34;1mRaw file detected - filtering with 1st order butterworth highpass at 300Hz...\033[0m")
-                preprocess_binary_file(dp,
+                print(
+                    "\033[34;1mRaw file detected - filtering with 1st order butterworth highpass at 300Hz...\033[0m"
+                )
+                preprocess_binary_file(
+                    dp,
                     delete_original_data=delete_original_data,
                     data_deletion_double_check=data_deletion_double_check,
-                    median_subtract=False, filter_forward=True, filter_backward=False, order=1)
-
-        optolabel=ds['ct']
-        if optolabel=="PkC": optolabel="PkC_ss"
-        units=ds['units']
-        ss=ds['ss']
-        cs=ds['cs']
-        good_units = list(get_units(dp, 'good', again=again))
-        sane_times = ds["sane_times"] if "sane_times" in ds else None
+                    median_subtract=False,
+                    filter_forward=True,
+                    filter_backward=False,
+                    order=1,
+                )
+
+        ds_name, optolabel = ds_name_ct.split("&")
+        assert optolabel == ds["ct"]
+        if optolabel == "PkC":
+            optolabel = "PkC_ss"
+        genetic_line = ds["line"]
+        units = ds["units"]
+        ss = ds["ss"]
+        cs = ds["cs"]
+        good_units = list(get_units(dp, "good", again=True))
+        sane_periods_dic = ds["sane_periods"] if "sane_periods" in ds else {}
 
         if include_all_good:
-            units_for_h5 = np.unique(units+ss+cs+good_units)
+            units_for_h5 = np.unique(units + ss + cs + good_units)
         else:
-            units_for_h5 = units+ss+cs
+            units_for_h5 = units + ss + cs
 
         for u in units_for_h5:
-            add_unit_h5(h5_path, dp, u, lab_id, periods='all',
-                    again=again, again_wvf=again, verbose=verbose,
-                    include_raw_snippets=include_raw_snippets, include_whitened_snippets=include_raw_snippets,
-                    sane_periods=sane_times, **kwargs)
+            sane_periods = sane_periods_dic[u] if u in sane_periods_dic else None
+
+            add_unit_h5(
+                h5_path,
+                dp,
+                u,
+                lab_id,
+                genetic_line=genetic_line,
+                dataset=None,  # end of dp by default
+                sane_periods=sane_periods,
+                selective_overwrite=selective_overwrite,
+                overwrite_h5=overwrite_h5,
+                **kwargs,
+            )
             if u in units:
                 label = optolabel
+                source = "optogagged"
             elif u in ss:
-                label="PkC_ss"
+                label = "PkC_ss"
+                source = "CSxSS"
             elif u in cs:
-                label="PkC_cs"
+                label = "PkC_cs"
+                source = "CSxSS"
             else:
                 continue
-            label_optotagged_unit_h5(h5_path, ds_name, u, label)
+            label_optotagged_unit_h5(h5_path, ds_name, u, label, source)
             gc.collect()
 
-def add_json_datasets_to_h5_hausser(json_path, h5_path, again=False, include_raw_snippets=False,
-                                    delete_original_data=False, data_deletion_double_check=False,
-                                    include_all_good=False, overwrite_h5=False, **kwargs):
-
-    add_json_datasets_to_h5(json_path, h5_path, "hausser", preprocess_if_raw=False,
-                            delete_original_data=delete_original_data, data_deletion_double_check=data_deletion_double_check,
-                            again=again, include_raw_snippets=include_raw_snippets,
-                            optostims_from_sync=True, optostims_threshold=20*60, sane_before_opto=True,
-                            include_all_good=include_all_good, overwrite_h5=overwrite_h5, **kwargs)
+
+def add_json_datasets_to_h5_hausser(
+    json_path,
+    h5_path,
+    include_all_good=True,
+    selective_overwrite=None,
+    overwrite_h5=False,
+    **kwargs,
+):
+    # parameters ensuring that only the
+    # spontaneous period before opto is used
+    sane_before_opto = True
+    optostims_from_sync = True
+    optostims_threshold = 20 * 60
+
+    add_json_datasets_to_h5(
+        json_path,
+        h5_path,
+        "hausser",
+        include_all_good=include_all_good,
+        optostims_from_sync=optostims_from_sync,
+        optostims_threshold=optostims_threshold,
+        sane_before_opto=sane_before_opto,
+        selective_overwrite=selective_overwrite,
+        overwrite_h5=overwrite_h5,
+        **kwargs,
+    )
+
+
+def load_json_datasets(json_path, include_missing_datasets=False):
+    with open(json_path) as f:
+        json_f = json.load(f)
+
+    print(f"\nLoading data from file {json_path}...\n")
+
+    DSs = {}
+    for ds in json_f.values():
+        for key in ["dp", "ct", "line", "units", "ss", "cs"]:
+            assert key in ds, f"{key} not in json file for dataset #{ds}!"
+
+        dp = Path(ds["dp"])
+
+        if not dp.exists():
+            print(f"Dataset {dp} NOT found on system!\n")
+            if include_missing_datasets:
+                DSs[dp.name] = ds
+            continue
+        DSs[dp.name + "&" + ds["ct"]] = ds
+
+        units = list(ds["units"])
+        ss = list(ds["ss"])
+        cs = list(ds["cs"])
+        print(
+            f"Dataset {dp} found with opto responsive units {units}, simple spikes {ss}, complex spikes {cs}.\n"
+        )
+        all_units = units + ss + cs
+        units_m = np.isin(all_units, get_units(dp))
+        assert all(units_m), f"Units {np.array(all_units)[~units_m]} not found in {dp}!"
+
+    return DSs
+
+
+### h5 unit management wrapper functions
+
+
+@docstring_decorator(add_unit_h5.__doc__)
+def add_units_to_h5(h5_path, dp, units=None, **kwargs):
+    """
+    Add all or specified units at the respective data path to an HDF5 file.
+
+    This is a high-level function designed to add many units at the
+    specified datapath to an HDF5 file. All additional key-value
+    arguments are passed to `add_unit_h5`
+
+    Example:
+      add_units_to_h5('my_lab_data.h5', '/path/to/dataset_id', lab_id='pi_last_name')
+    Will add all sorted units in the 'kilosort_results' directory
+    to the HDF5 file called 'my_lab_data.h5' (in the current directory).
+
+    Other arguments from add_unit_h5:
+    {0}
+    """
+
+    if units is None:
+        units = get_units(dp)
+
+    for u in units:
+        add_unit_h5(h5_path, dp, u, **kwargs)
 
 
 def add_data_to_unit_h5(h5_path, dataset, unit, data, field):
     """
     Add data to neuron already in h5 file.
 
     - h5_path: full path to h5 file
@@ -552,18 +703,58 @@
     - unit: unit index
     - data: data to add to unit
     - field: name of dataset to add data (id exists already, will overwrite)
     """
     check_dataset_format(dataset)
     unit_path = relative_unit_path_h5(dataset, unit)
     with h5py.File(h5_path, "a") as h5_file:
-        assert unit_path in h5_file, f"WARNING unit {unit_path} does not seem to be present in the file. To add it, use add_unit_h5()."
+        assert (
+            unit_path in h5_file
+        ), f"WARNING unit {unit_path} does not seem to be present in the file. To add it, use add_unit_h5()."
         write_to_group(h5_file[unit_path], field, data, True)
 
-# h5 vizualisattion functions
+
+def get_unit_paths_h5(h5_file, dataset, unit, lab_id="hausser", unit_absolute_id=None):
+    relative_unit_path = relative_unit_path_h5(dataset, unit)
+    if relative_unit_path in h5_file:
+        absolute_unit_path = h5_file[f"{relative_unit_path}/neuron_id"][()].decode()
+    else:
+        if unit_absolute_id is None:
+            if f"{lab_id}_neuron_0" not in h5_file:
+                unit_absolute_id = 0
+            else:
+                root_groups = list(h5_file.keys())
+                neuron_ids = [
+                    int(x.split("_")[-1])
+                    for x in root_groups
+                    if f"{lab_id}_neuron" in x
+                ]
+                unit_absolute_id = np.sort(neuron_ids)[-1] + 1
+        absolute_unit_path = f"{lab_id}_neuron_{unit_absolute_id}"
+
+    return relative_unit_path, absolute_unit_path
+
+
+def remove_unit_h5(h5_path, dp, unit, lab_id="hausser", dataset=None):
+    if dataset is None:
+        dataset = Path(dp).name
+    with h5py.File(h5_path, "a") as h5_file:
+        relative_unit_path, absolute_unit_path = get_unit_paths_h5(
+            h5_file, dataset, unit, lab_id
+        )
+        del h5_file[relative_unit_path]
+        del h5_file[absolute_unit_path]
+        dataset_path = str(Path(relative_unit_path).parent)
+        if len(h5_file[dataset_path].keys()) == 0:
+            del h5_file[dataset_path]
+
+
+### h5 vizualisation functions
+
+
 def print_h5_contents(h5_path, txt_output=False):
     """
     h5_path: str, path to .h5 file
     txt_output: bool, if True prints contents to file
     (same name as h5 name_content.txt)
     """
     h5_path = Path(h5_path)
@@ -575,76 +766,82 @@
                 original_stdout = sys.stdout
                 sys.stdout = txt
                 visititems(hdf, visitor_func)
                 sys.stdout = original_stdout
         else:
             visititems(hdf, visitor_func)
 
+
 def visititems(group, func):
     with h5py._hl.base.phil:
+
         def proxy(name):
-            """ Call the function with the text name, not bytes """
+            """Call the function with the text name, not bytes"""
             name = group._d(name)
             return func(name, group[name])
+
         return group.id.links.visit(proxy)
-       
+
+
 def visitor_func(name, node):
     """
     prints name followed by a meangingful description of an hdf5 node.
     Node is either an h5 dataset (array, string...) or a group.
     """
     if isinstance(node, h5py.Dataset):
-        n=node[()]
+        n = node[()]
         if isinstance(n, bytes):
-            s=n.decode()
+            s = n.decode()
         elif isinstance(n, np.ndarray):
-            s=f"ndarray {n.shape}"
+            s = f"ndarray {n.shape}"
         elif assert_int(n) or assert_float(n):
-            s=n
+            s = n
         else:
-            s=type(n)
+            s = type(n)
         string = f"{name}: {s}"
     else:
         string = name
     print(string)
 
+
 def check_dataset_format(dataset):
     """
     Checks whether dataset name is formatted properly
     i.e. aa-mm-dd_iiXXX_probeX (mouse can only be names )
     """
     warning = "WARNING last folder of path should match format: aa-mm-dd_ii[0-1000]_probe[0-9] (ii = 2 [a-z] initials)"
     pattern = "[0-9]{2}-[0-9]{2}-[0-9]{2}_[a-z]{2}[0-9]{3}_probe[0-9]"
     if re.match(pattern, dataset, re.IGNORECASE) is None:
         warnings.warn(warning)
 
+
 def assert_h5_file(h5_path):
     assert check_h5_file(h5_path), f"WARNING file at {h5_path} is not a .h5 file."
 
+
 def check_h5_file(h5_path):
     """
     Check whether h5_path indeed points to h5
     returns True or False
     """
-    return h5_path.name[-3:] == '.h5'
+    return h5_path.name[-3:] == ".h5"
+
 
-# h5 writing functions
-def write_to_h5(h5_path, data_path, data,
-                overwrite=False, must_exist=False):
+### h5 writing functions
+def write_to_h5(h5_path, data_path, data, overwrite=False, must_exist=False):
     """
     Writes data at data_path to .h5 file at h5_path
     (creates non existing groups and datasets).
     """
     assert_h5_file(h5_path)
     with h5py.File(h5_path, "a") as h5_file:
-        write_to_group(h5_file, data_path, data,
-                       overwrite, must_exist)
+        write_to_group(h5_file, data_path, data, overwrite, must_exist)
 
-def write_to_group(group, dataset, data,
-                         overwrite=True, must_exist=False):
+
+def write_to_group(group, dataset, data, overwrite=True, must_exist=False):
     """Write data to hdf5 group
     i.e. create a dataset +/- groups on the path to dataset
     and write data to this dataset.
     Arguments:
     - group: h5py group
     - dataset: str, name of dataset
     - data: data to add to dataset
@@ -656,53 +853,74 @@
             del group[dataset]
         else:
             return
     elif must_exist:
         raise KeyError(f"Dataset {dataset} does not exist in group {group.name}!")
     group[dataset] = data
 
+
 def write_to_dataset(group, dataset, data, overwrite=True):
     """write_to_groupwrite_to_group
     Write data to pre-existing dataset in group.
     Will crash if dataset does not exist in group.
     """
-    write_to_group(group, dataset, data,
-                         overwrite, True)
+    write_to_group(group, dataset, data, overwrite, True)
 
-# h5 reading functions
+
+### h5 reading functions
 def read_h5(h5_path, datapath):
     """
     Returns data at datapath from h5 file at h5_path
     """
 
     h5_path = Path(h5_path)
-    
+
     assert_h5_file(h5_path)
     with h5py.File(h5_path) as h5_file:
         assert datapath in h5_file, f"WARNING {datapath} not found in {h5_path}"
         data = h5_file[datapath][()]
         if isinstance(data, bytes):
-            data = data.decode() # for strings
+            data = data.decode()  # for strings
     return data
-    
+
+
+### C4 utilities
+def get_stim_chan(ons, min_th=20):
+    chan = -1
+    for k, v in ons.items():
+        if len(v) > min_th:
+            chan = k
+    assert chan != -1
+    return chan
+
+
+def assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite):
+    return (key not in neuron_group) or overwrite_h5 or (key in selective_overwrite)
+
+
+def assert_recompute_any(keys, neuron_group, overwrite_h5, selective_overwrite):
+    return np.any(
+        [
+            assert_recompute(key, neuron_group, overwrite_h5, selective_overwrite)
+            for key in keys
+        ]
+    )
+
+
 def h5_group_keys(group):
     """
     Returns list of keys of h5 file group
     to allow easy overview of group content.
     """
     return list(group.keys())
 
+
 def all_keys_in_group(keys, group):
     assert isinstance(keys, list)
     b = True
     for k in keys:
         b = b & (k in group)
     return b
 
-# C4 utilities
-def get_stim_chan(ons, min_th=20):
-    chan = -1
-    for k, v in ons.items():
-        if len(v) > min_th:
-            chan = k
-    assert chan != -1
-    return chan
+
+def relative_unit_path_h5(dataset, unit):
+    return f"datasets/{dataset}/{unit}"
```

### Comparing `npyx-2.7.1/npyx/info.py` & `npyx-2.8.0/npyx/info.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/inout.py` & `npyx-2.8.0/npyx/inout.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 Created on Fri May  3 16:30:50 2019
 
 @author: Maxime Beau, Hausser lab, University College London
 
 Input/output utilitaries to deal with Neuropixels files.
 """
 
-import psutil
-import shutil
 import os
+import shutil
 from ast import literal_eval as ale
+from math import ceil
 from pathlib import Path
-from tqdm.auto import tqdm
 
-from math import ceil
 import numpy as np
+import psutil
+from tqdm.auto import tqdm
+
 try:
     import cupy as cp
 except ImportError:
     print(("cupy could not be imported - "
     "some functions dealing with the binary file (filtering, whitening...) will not work."))
 
-from npyx.utils import npa, read_pyfile, list_files
-
 import json
 
+from npyx.utils import list_files, npa, read_pyfile
+
 #%% Load metadata and channel map
 
 def read_metadata(dp):
     f'''
     {metadata.__doc__}
 
     If ran on a merged dataset, an additional layer of keys is added: the probes used as keys of
@@ -422,15 +423,15 @@
     '''
     xshape = list(x.shape)
     x = x.reshape([-1,1])
     to_and = 2**np.arange(num_bits).reshape([1,num_bits])
     return (x & to_and).astype(bool).astype(np.int64).reshape(xshape + [num_bits])
 
 def get_npix_sync(dp, output_binary = False, filt_key='highpass', unit='seconds',
-                  verbose=False, again=False, sample_span=1e6):
+                  verbose=False, again=False, sample_span=int(1e6)):
     '''Unpacks neuropixels external input data, to align spikes to events.
     Arguments:
         - dp: str, datapath
         - output_binary: bool, whether to output binary sync channel as 0/1s
         - filt_key: str, 'highpass' or 'lowpass' (SpikeGLX: ap/lf, OIpenEphys: Neuropix-PXI-100.0/.1)
         - unit: str, 'seconds' or 'samples', units of returned onsets/offset times
         - verbose: bool, whether to print rich information
@@ -1093,9 +1094,15 @@
             "units": units,
             "rate": rate}
 
 class ImplementationError(Exception):
     pass
 
 from npyx.gl import assert_multi, get_ds_table, get_npyx_memory
-from npyx.preprocess import whitening, approximated_whitening_matrix, med_substract,\
-                            gpufilter, adc_realign, kfilt
+from npyx.preprocess import (
+    adc_realign,
+    approximated_whitening_matrix,
+    gpufilter,
+    kfilt,
+    med_substract,
+    whitening,
+)
```

### Comparing `npyx-2.7.1/npyx/merger.py` & `npyx-2.8.0/npyx/merger.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/metrics.py` & `npyx-2.8.0/npyx/metrics.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/model.py` & `npyx-2.8.0/npyx/model.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/plot.py` & `npyx-2.8.0/npyx/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.ticker import AutoLocator
 from cmcrameri import cm as cmcr
 cmcr=cmcr.__dict__
 from IPython.core.display import HTML,display
 
-#mpl.rcParams['figure.dpi']=100
-mpl.rcParams['pdf.fonttype'] = 42 # necessary to make the text editable
+# Make matplotlib saved figures text text editable
+mpl.rcParams["svg.fonttype"] = 'none'
+mpl.rcParams['pdf.fonttype'] = 42 
 mpl.rcParams['ps.fonttype'] = 42
 
 from npyx.utils import phyColorsDic, npa, zscore, isnumeric, assert_iterable, save_np_array, pprint_dic, docstring_decorator
 from npyx.stats import fractile_normal, fractile_poisson
 
 from npyx.inout import read_metadata, extract_rawChunk, assert_chan_in_dataset, chan_map, predefined_chanmap
 from npyx.gl import get_units
@@ -349,14 +350,15 @@
     fonttype1 = mpl.rcParams['pdf.fonttype']
     fonttype2 = mpl.rcParams['ps.fonttype']
 
     mpl.rcParams['figure.dpi']=dpi
     mpl.rcParams['pdf.fonttype']=42
     mpl.rcParams['ps.fonttype']=42
 
+    if saveDir is None: saveDir = '~/Downloads'
     saveDir=Path(saveDir).expanduser()
     if not saveDir.exists():
         assert saveDir.parent.exists(), f'WARNING can only create a path of a single directory level, {saveDir.parent} must exist already!'
         saveDir.mkdir()
     p=saveDir/f"{figname}.{_format}"
     fig.savefig(p, dpi=dpi, bbox_inches='tight')
 
@@ -2685,15 +2687,16 @@
 
 def imshow_cbar(im, origin='top', xevents_toplot=[], yevents_toplot=[], events_color='k', events_lw=2,
                 xvalues=None, yvalues=None, xticks=None, yticks=None,
                 xticklabels=None, yticklabels=None, xlabel=None, ylabel=None, xtickrot=45, title='',
                 cmapstr="RdBu_r", vmin=None, vmax=None, center=None, colorseq='nonlinear',
                 clabel='', cticks=None,
                 figsize=(6,4), aspect='auto', function='imshow',
-                ax=None, tight_layout=True, cmap_h=0.3, prettify=True,
+                ax=None, tight_layout=True, cmap_w=0.02, cmap_h=0.5, cmap_pad=0.01,
+                prettify=True, show_values=False, saveDir=None, saveFig=False, _format='pdf',
                 **kwargs):
     '''
     Essentially plt.imshow(im, cmap=cmapstr), but with a nicer and actually customizable colorbar.
 
     Arguments:
         - im: 2D array def to matplotlib.pyplot.imshow
         - origin: y axis origin, either top or bottom | Default: top
@@ -2722,17 +2725,20 @@
         - cticks: list of ticks to show
 
         - figsize: (x,y) tuple, size of figure in inches
         - aspect: {'equal', 'auto'}, see matplotlib.pyplot.imshow documentation
         - function: {'imshow', 'pcolormesh'}, whether to use imshow or pcolormesh to plot the image
         - ax: matplotlib axis, if None, a new figure is created
         - tight_layout: bool, whether to use plt.tight_layout() or not
-        - cmap_h: float, height of the colorbar in inches
+        - cmap_w: float, width of the colorbar in axes fraction
+        - cmap_h: float, height of the colorbar in axes fraction
+        - cmap_pad: cmap padding in axes fraction
 
         - prettify: bool, whether to apply mplp() prettification or not
+        - show_values: bool, whether to overlay the values of the pixels or not
         - **kwargs: additional arguments to be passed to the plotting function imshow or pcolormesh (e.g. interpolation='nearest')
     '''
     assert colorseq in ['linear', 'nonlinear']
     if im.ndim==1:
         print('Single row of pixels detected - plotting it horizontally.')
         im=im[np.newaxis,:]
     assert im.ndim==2
@@ -2748,71 +2754,93 @@
     if cticks is not None: assert cticks[-1]<=vmax and cticks[0]>=vmin
 
     # Make custom colormap.
     # If center if provided, reindex colors accordingly
     if center is None:
         cmap = get_cmap(cmapstr)
     else:
-        cmap=get_bounded_cmap(cmapstr, vmin, center, vmax, colorseq)
+        cmap = get_bounded_cmap(cmapstr, vmin, center, vmax, colorseq)
 
     # Define pixel coordinates (default is 0 to n_rows-1 for y and n_columns=1 for x)
     if xvalues is None: xvalues=np.arange(im.shape[1])
-    assert len(xvalues)==im.shape[1], f'xvalues should contain {im.shape[1]} values but contains {len(xvalues)}!'
+    assert len(xvalues)==im.shape[1],\
+        f'xvalues should contain {im.shape[1]} values but contains {len(xvalues)}!'
     dx = (xvalues[1]-xvalues[0])/2 if len(xvalues)>1 else xvalues[0]
     if yvalues is None: yvalues=np.arange(im.shape[0])
-    assert len(yvalues)==im.shape[0], f'yvalues should contain {im.shape[0]} values but contains {len(yvalues)}!'
+    assert len(yvalues)==im.shape[0],\
+        f'yvalues should contain {im.shape[0]} values but contains {len(yvalues)}!'
     dy = (yvalues[1]-yvalues[0])/2 if len(yvalues)>1 else yvalues[0]
     extent = [xvalues[0]-dx, xvalues[-1]+dx, yvalues[-1]+dy, yvalues[0]-dy]
 
     # Plot image with custom colormap
-    fig,ax=plt.subplots(figsize=figsize) if ax is None else (ax.get_figure(), ax)
-    if function=='imshow': axim=ax.imshow(im, cmap=cmap, vmin=vmin, vmax=vmax, aspect=aspect,
-                                          origin={'top':'upper', 'bottom':'lower'}[origin],
-                                          extent=extent, interpolation='nearest',
-                                          **kwargs)
-    elif function=='pcolor': axim=ax.pcolormesh(im, X=xvalues, Y=yvalues,
-                                                cmap=cmap, vmin=vmin, vmax=vmax, **kwargs)
+    fig, ax = plt.subplots(figsize=figsize) if ax is None else (ax.get_figure(), ax)
+    if function=='imshow':
+        axim = ax.imshow(im, cmap=cmap, vmin=vmin, vmax=vmax, aspect=aspect,
+                         origin={'top':'upper', 'bottom':'lower'}[origin],
+                         extent=extent, interpolation='nearest',
+                         **kwargs)
+    elif function=='pcolor':
+        axim = ax.pcolormesh(im, X=xvalues, Y=yvalues,
+                             cmap=cmap, vmin=vmin, vmax=vmax, **kwargs)
+    if show_values:
+        min_edge = np.min([ax.get_position().width  / im.shape[0],
+                           ax.get_position().height / im.shape[1]])
+        fontsize = (0.8*min_edge)/0.01 # roughly inch to pt
+        colors = axim.cmap(axim.norm(im.ravel()))[:,:-1]
+        colors = mpl.colors.rgb_to_hsv(colors).reshape(im.shape + (3,))
+        for (j,i),label in np.ndenumerate(im):
+            if origin == 'bottom':
+                i = im.shape[0]-1-i
+            c = 'white' if colors[j, i,-1] < 0.5 else 'black'
+            ax.text(i, j, label, fontsize=fontsize,
+                    color=c, ha='center', va='center')
+            ax.text(i, j, label, fontsize=fontsize,
+                    color=c, ha='center', va='center')
+
     if any(xevents_toplot):
         for e in xevents_toplot:
             yl=ax.get_ylim()
             ax.plot([e,e],yl,lw=events_lw,ls='--',c=events_color)
             ax.set_ylim(yl)
     if any(yevents_toplot):
         for e in yevents_toplot:
             xl=ax.get_xlim()
             ax.plot(xl,[e,e],lw=events_lw,ls='--',c=events_color)
             ax.set_xlim(xl)
 
     if xticks is None:
-        xticks=np.arange(im.shape[1]) if im.shape[1]<=6 else get_bestticks_from_array(np.arange(im.shape[1]), step=None, light=0)
+        xticks = np.arange(im.shape[1]) if im.shape[1]<=6 else get_bestticks_from_array(np.arange(im.shape[1]), step=None, light=0)
     if yticks is None:
-        yticks=np.arange(im.shape[0]) if im.shape[0]<=6 else get_bestticks_from_array(np.arange(im.shape[0]), step=None, light=0)
+        yticks = np.arange(im.shape[0]) if im.shape[0]<=6 else get_bestticks_from_array(np.arange(im.shape[0]), step=None, light=0)
     mplp(fig, ax, figsize=figsize,
           xlim=None, ylim=None, xlabel=xlabel, ylabel=ylabel,
           xticks=xticks, yticks=yticks, xtickslabels=xticklabels, ytickslabels=yticklabels,
           reset_xticks=False, reset_yticks=False, xtickrot=xtickrot, ytickrot=0,
           xtickha={0:'center',45:'right'}[xtickrot], xtickva='top', ytickha='right', ytickva='center',
-          axlab_w='bold', axlab_s=16,
-          ticklab_w='regular', ticklab_s=12, ticks_direction='out', lw=1,
+          axlab_w='bold', axlab_s=20,
+          ticklab_w='regular', ticklab_s=16, ticks_direction='out', lw=1,
           title=title, title_w='regular', title_s=12,
           hide_top_right=False, hide_axis=False, tight_layout=False,
           prettify=prettify)
 
     if tight_layout: fig.tight_layout(rect=[0,0,0.8,1])
 
     # Add colorbar, nicely formatted
     fig = add_colorbar(fig, ax, axim, vmin, vmax,
-                        0.01, cmap_h, cticks, clabel, 'bold')
+                        cmap_w, cmap_h, cticks, clabel, 'bold', pad=cmap_pad)
+
+    if saveFig:
+        save_mpl_fig(fig, 'heatmap', saveDir, _format, dpi=500)
 
     return fig
 
 def add_colorbar(fig, ax, mappable=None, vmin=None, vmax=None,
                  width=0.01, height=0.5, cticks=None,
-                 clabel=None, clabel_w='regular', clabel_s=16, cticks_s=14,
-                 cmap=None):
+                 clabel=None, clabel_w='regular', clabel_s=20, cticks_s=16,
+                 cmap=None, pad = 0.01):
     """
     Add colorbar to figure with a predefined axis.
     
     Makes sure that the size of the predefined axis does not change, but that the figure extends.
     """
 
     # format vmin and vmax
@@ -2825,36 +2853,35 @@
 
     # define mappable
     if mappable is None:
         assert vmin is not None or vmax is not None,\
             "If you do not provide a mappable (e.g. ax.collections[0]), you must provide vmin and vmax!"
         assert cmap is not None,\
             "If you do not provide a mappable (e.g. ax.collections[0]), you must provide a colormap (e.g. 'viridis')!"
-        norm = plt.Normalize(vmin, vmax)
+        norm     = plt.Normalize(vmin, vmax)
         mappable = plt.cm.ScalarMappable(cmap=cmap, norm=norm)
         mappable.set_array([])
 
     # create colorbar axis
-    axpos=ax.get_position()
-    pad = 0.01
-    bottom_left_x, bottom_left_y = float(axpos.x1+pad), float(axpos.y0)
-    cbar_ax = fig.add_axes([bottom_left_x, bottom_left_y, width, height])
+    axpos   = ax.get_position()
+    cbar_ax = fig.add_axes([axpos.x1+pad*axpos.width, axpos.y0,
+                            width*axpos.width, height*axpos.height])
 
     # add colorbar
     fig.colorbar(mappable, cax=cbar_ax, ax=ax,
              orientation='vertical', label=clabel,
              ticks=cticks, use_gridspec=True)
 
     # format colorbar ticks, labels etc
     if clabel is not None:
         cbar_ax.yaxis.label.set_font_properties(mpl.font_manager.FontProperties(family='arial', weight=clabel_w, size=clabel_s))
         cbar_ax.yaxis.label.set_rotation(-90)
         cbar_ax.yaxis.label.set_va('bottom')
         cbar_ax.yaxis.label.set_ha('center')
-        cbar_ax.yaxis.labelpad=5
+        cbar_ax.yaxis.labelpad = 5
     cbar_ax.yaxis.set_ticklabels(cticks, ha='left')
     cbar_ax.yaxis.set_tick_params(pad=5, labelsize=cticks_s)
 
     fig.canvas.draw()
     set_ax_size(ax,*fig.get_size_inches())
 
     return fig
```

### Comparing `npyx-2.7.1/npyx/preprocess.py` & `npyx-2.8.0/npyx/preprocess.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/spk_t.py` & `npyx-2.8.0/npyx/spk_t.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # -*- coding: utf-8 -*-
 """
 2018-07-20
 @author: Maxime Beau, Neural Computations Lab, University College London
 """
-from IPython.core.debugger import set_trace as breakpoint 
 import os.path as op
+
+from IPython.core.debugger import set_trace as breakpoint
+
 opj=op.join
 from pathlib import Path, PosixPath, WindowsPath
 
 from joblib import Memory
+
 cachedir = Path(op.expanduser("~")) / ".NeuroPyxels"
 cache_memory = Memory(cachedir, verbose=0)
 
 import matplotlib.pyplot as plt
-
 import numpy as np
 import pandas as pd
-from scipy.stats import iqr
-from scipy.optimize import curve_fit
-from scipy.stats import norm
-from npyx.utils import smooth, thresh_consec, npa, assert_int, assert_float, docstring_decorator
-from npyx.gl import get_units, get_npyx_memory, check_periods
+from npyx.gl import check_periods, get_npyx_memory, get_units
 from npyx.inout import read_metadata
+from npyx.utils import (assert_float, assert_int, docstring_decorator, npa,
+                        smooth, thresh_consec)
+from scipy.optimize import curve_fit
+from scipy.stats import iqr, norm
 
 
 def ids(dp, unit, sav=True, verbose=False, periods='all', again=False, enforced_rp=-1):
     '''
     ********
     routine from routines_spikes
     computes spike indices (1, Nspikes) - int64, in samples
@@ -145,15 +147,15 @@
         spike_samples = np.load(Path(dp,'spike_times.npy'), mmap_mode='r')
         train = spike_samples[spike_clusters==unit].ravel()
 
         # Filter out spike duplicates (spikes following an ISI shorter than enforced_rp)
         # by default, only pure duplicates (yeah they happen!!)
         assert len(train)!=0, f'unit {unit} not found in spike_clusters.npy - probably a merger bug.'
         duplicates_m = duplicates_mask(train, enforced_rp, fs)
-        train=train[~duplicates_m]
+        train = train[~duplicates_m]
         # Save it
         if sav:
             np.save(dpnm/fn, train)
 
     # Optional selection of a section of the recording.
     # Always computed because cannot reasonably be part of file name.
     periods = check_periods(periods)
@@ -331,54 +333,124 @@
     periods = firing_periods(t, fs, t_end, b=1, sd=1000, th=0.02)
 
     if sav:
         np.save(Path(dpnm,fn), periods)
 
     return periods
 
-def firing_periods(t, fs, t_end, b=1, sd=1000, th=0.02, again=False, dp=None, u=None):
+def firing_periods(t, fs, t_end, b=1, sd=1000, th=0.02,
+                   again=False, dp=None, u=None, return_smoothed_rate = False):
     '''
     Arguments:
         - t: array of spike times, in samples
         - fs: sampling rate of spike times, in Hz
         - t_end: recording end time, in samples
         - b: float, bin size i.e. temporal resolution of presence periods, in ms | Default 1
         - sd: float, standard deviation of gaussian smoothing window, in ms | Default 1000
         - th: threshold to define presence, in fraction of mean firing rate
+    Returns:
+        - periods, in samples
     '''
     sav=False
     if u is not None:
         sav=True
         assert dp is not None
         assert len(trn(dp,u,0))==len(t), 'There seems to be a mismatch between the provided spike trains and the unit index.'
         fn=f'firing_periods_{u}_{b}_{sd}_{th}.npy'
         dpnm = get_npyx_memory(dp)
         if op.exists(Path(dpnm,fn)) and not again:
             return np.load(Path(dpnm,fn))
 
-    assert 1<sd<10000
+    assert 1<sd<100000
     assert 0<=th<1
     assert t.ndim==1
-    t=np.asarray(t)
+    t     = np.asarray(t)
 
     assert b>=1000/fs
-    tb = binarize(t, b, fs, t_end)
-    sd=int(sd/b) # convert from ms to bin units
-    b_s=b/1000 # bin seconds
-    tbs=smooth(tb, 'gaussian', sd=sd)/b_s # result is inst. firing rate in Hz - speed bottleneck
-    fr_th=mean_firing_rate(t, 0.005, fs)*th
+    tb    = binarize(t, b, fs, t_end)
+    sd    = int(sd/b) # convert from ms to bin units
+    b_s   = b/1000 # bin seconds
+    tbs   = smooth(tb, 'gaussian', sd=sd)/b_s # result is inst. firing rate in Hz - speed bottleneck
+    fr_th = mean_firing_rate(t, 0.005, fs)*th
 
     periods = thresh_consec(tbs, fr_th, sgn=1, n_consec=0, exclude_edges=False, only_max=False, ret_values=False)
     if not any(periods): periods=[[0,len(tbs)-1]]
-    periods=(np.array(periods)*(b_s*fs)).astype(np.int64) # conversion from bins to samples
+    periods = (np.array(periods)*(b_s*fs)).astype(np.int64) # conversion from bins to samples
 
     if sav: np.save(Path(dpnm,fn), periods)
 
+    if return_smoothed_rate:
+        return periods, tbs
+
     return periods
 
+def find_stable_recording_period(t, fs, t_end, target_period = 30,
+                                 b=1000, sd=10000, minimum_fr = 0.4,
+                                 return_rate=False):
+    
+    """
+    Finds a locally optimal recording period (in terms of stability i.e. low std) of at least 'target_period' seconds.
+    Arguments:
+        - t: array of spike times, in samples
+        - fs: sampling rate of spike times, in Hz
+        - t_end: recording end time, in samples
+        - target_period: float, minimum length of stable period, in seconds | Default 30.
+                        If the algorithm does not find any period lasting at least this amount of time
+                        for at least minimum_fr fraction of the mean firing rate,
+                        it ties to decrease this period.
+        - b: float, bin size i.e. temporal resolution of presence periods, in ms | Default 1
+        - sd: float, standard deviation of gaussian smoothing window, in ms | Default 1000
+        - th: threshold to define presence, in fraction of mean firing rate
+    Returns:
+        - periods: (2,) array of stable period on/offset, in samples
+    """
+    if not np.any(t):
+        if return_rate:
+            return np.array([np.nan, np.nan]), np.nan
+        return np.array([np.nan, np.nan])       
+
+    target_period = target_period*fs
+
+    # find candidate periods
+    fr_th = 0.9
+    periods, tbs = firing_periods(t, fs, t_end, b, sd, th=fr_th, return_smoothed_rate=True)
+    periods_t = np.diff(periods, axis=1).ravel()
+    while not np.any(periods_t>target_period):
+        periods, tbs = firing_periods(t, fs, t_end, b, sd, th=fr_th, return_smoothed_rate=True)
+        periods_t = np.diff(periods, axis=1).ravel()
+        fr_th -= 0.05
+        if fr_th<=minimum_fr: # do not tolerate less then x% of mfr
+            target_period -= 2
+            fr_th = 0.9
+            if target_period<=1:
+                print("Could not find a long enough stable recording period!")
+                break
+
+    # if none was found, return nans
+    if not np.any(periods_t>target_period):
+        if return_rate:
+            return np.array([np.nan, np.nan]), tbs
+        return np.array([np.nan, np.nan])
+    
+    # find the most stable period
+    candidate_periods = periods[periods_t>target_period]
+    variances = np.zeros(len(candidate_periods))
+    for i, p in enumerate(candidate_periods):
+        period_ms = p * 1000 / fs
+        period_bins = (period_ms / b).astype(int)
+        variances[i] = np.std(tbs[period_bins[0]:period_bins[1]])
+    
+    most_stable_period = candidate_periods[np.argmin(variances)]
+
+    most_stable_period_trimmed = np.array([most_stable_period[0], most_stable_period[0]+target_period])
+
+    if return_rate:
+        return most_stable_period_trimmed, tbs
+    return most_stable_period_trimmed
+
 
 def train_quality(dp, unit, period_m=[0,20],
                   fp_chunk_span=3, fp_chunk_size = 10,
                   fn_chunk_span = 3, fn_chunk_size = 10,
                   use_or_operator = True,
                   violations_ms = 0.8, fp_threshold = 0.05, fn_threshold = 0.05,
                   again = False, save = True, verbose = False, plot_debug = False,
@@ -858,11 +930,12 @@
     # Square-root choice
     elif rule == 'Sqrt':
         b = int(np.sqrt(n))
         return b
 
 
 
-from  npyx.corr import acg
-from npyx.merger import assert_multi, get_dataset_id, get_ds_table, get_source_dp_u
+from npyx.corr import acg
+from npyx.merger import (assert_multi, get_dataset_id, get_ds_table,
+                         get_source_dp_u)
+from npyx.metrics import isi_violations
 from npyx.plot import plot_fp_fn_rates
-from npyx.metrics import isi_violations
```

### Comparing `npyx-2.7.1/npyx/spk_wvf.py` & `npyx-2.8.0/npyx/spk_wvf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 """
 2018-07-20
 @author: Maxime Beau, Neural Computations Lab, University College London
 """
 
+import multiprocessing
 import os
-import os.path as op; opj=op.join
-import psutil
+from collections.abc import Iterable
 from pathlib import Path
+
+import psutil
 from tqdm.notebook import tqdm
 
-from collections.abc import Iterable
+import os.path as op; opj=op.join
+
 
-import multiprocessing
 num_cores = multiprocessing.cpu_count()
 
-import numpy as np
 from math import ceil
 
 import matplotlib.pyplot as plt
+import numpy as np
 
+from npyx.gl import get_npyx_memory, get_units
+from npyx.inout import chan_map, get_binary_file_path, read_metadata
+from npyx.preprocess import apply_filter, bandpass_filter, med_substract, whitening
 from npyx.utils import npa, split, xcorr_1d_loop
-from npyx.inout import read_metadata, get_binary_file_path, chan_map
-from npyx.preprocess import whitening, bandpass_filter, apply_filter, med_substract
-from npyx.gl import get_units, get_npyx_memory
+
 
 def wvf(dp, u=None, n_waveforms=100, t_waveforms=82, selection='regular', periods='all',
         spike_ids=None, wvf_batch_size=10, ignore_nwvf=True,
         save=True, verbose=False, again=False,
         whiten=False, med_sub=False, hpfilt=False, hpfiltf=300,
         nRangeWhiten=None, nRangeMedSub=None, ignore_ks_chanfilt=True):
     '''
@@ -40,15 +43,15 @@
         - u:                  int, unit index.
         - n_waveforms:        int, number of waveform to return, selected according to the periods parameter | Default 100
         - t_waveforms:        int, temporal span of waveforms | Default 82 (about 3ms)
         - selection:          str, way to select subset of n_waveforms spikes to return the waveforms of.
                               Either 'regular' (homogeneous selection or in batches) or 'random'.
         - periods:            recording periods to sample waveforms from. Either 'all' (default)
                               or [(t1, t2), (t3, t4), ...] with t1, t2 in seconds.
-        - spike_ids:          list/array, relative indices of spikes in the whole recording.
+        - spike_ids:          list/array, absolute indices of spikes in the whole recording.
                                           Takes precedence over every other parameter: if provided, u, n_waveforms and periods will be ignored.
         - wvf_batch_size:     int, if >1 and 'regular' selection, selects ids as batches of spikes. | Default 10
         - save:               bool, whether to save to NeuroPyxels cache. | Default True
         - verbose:            bool, whether to print informaiton. | Default False
         - again:              bool, whether to recompute waveforms even if ofund in routines memory. | Default False
         - ignore_nwvf:        bool, whether to ignore n_waveforms parameter when a list of times is provided as periods,
                                     to return all the spikes in the window instead. | Default True
@@ -105,52 +108,53 @@
 #     elif slc.stop >= traces.shape[0] - 1: extract = _pad(extract, _n_samples_extract, 'right')
 #     # Add this waveform, all good!
 #     return extract.T
 
 def get_waveforms(dp, u, n_waveforms=100, t_waveforms=82, selection='regular', periods='all',
                   spike_ids=None, wvf_batch_size=10, ignore_nwvf=True,
                   whiten=0, med_sub=0, hpfilt=0, hpfiltf=300,
-                  nRangeWhiten=None, nRangeMedSub=None, ignore_ks_chanfilt=0, verbose=False):
+                  nRangeWhiten=None, nRangeMedSub=None, ignore_ks_chanfilt=0, verbose=False,
+                  med_sub_in_time=True):
     f"{wvf.__doc__}"
 
     # Extract and process metadata
-    dp = Path(dp)
-    meta = read_metadata(dp)
-    dat_path = get_binary_file_path(dp, 'ap')
-
-    dp_source = get_source_dp_u(dp, u)[0]
-    meta=read_metadata(dp_source)
-    dtype=np.dtype(meta['highpass']['datatype'])
-    n_channels_dat=meta['highpass']['n_channels_binaryfile']
+    dp             = Path(dp)
+    meta           = read_metadata(dp)
+    dat_path       = get_binary_file_path(dp, 'ap')
+
+    dp_source      = get_source_dp_u(dp, u)[0]
+    meta           = read_metadata(dp_source)
+    dtype          = np.dtype(meta['highpass']['datatype'])
+    n_channels_dat = meta['highpass']['n_channels_binaryfile']
     n_channels_rec = n_channels_dat-1 if meta['acquisition_software']=='SpikeGLX' else n_channels_dat
-    sample_rate=meta['highpass']['sampling_rate']
-    item_size = dtype.itemsize
-    fileSizeBytes=meta['highpass']['binary_byte_size']
+    sample_rate    = meta['highpass']['sampling_rate']
+    item_size      = dtype.itemsize
+    fileSizeBytes  = meta['highpass']['binary_byte_size']
     assert not isinstance(fileSizeBytes, str), f"It seems like there isn't any binary file at {dp}."
     if meta['acquisition_software']=='SpikeGLX':
         if meta['highpass']['fileSizeBytes'] != fileSizeBytes:
             print((f"\033[91;1mMismatch between ap.meta and ap.bin file size"
             "(assumed encoding is {str(dtype)} and Nchannels is {n_channels_dat})!! "
             f"Probably wrong meta file - just edit fileSizeBytes in the .ap.meta file at {dp} "
             f"(replace {int(meta['highpass']['fileSizeBytes'])} with {fileSizeBytes}) "
             "and be aware that something went wrong in your data management...\033[0m"))
 
     # Select subset of spikes
     spike_samples = np.load(Path(dp, 'spike_times.npy'), mmap_mode='r').squeeze()
     if spike_ids is None:
-        spike_ids_subset=get_ids_subset(dp, u, n_waveforms, wvf_batch_size, selection, periods, ignore_nwvf, verbose)
+        spike_ids_subset = get_ids_subset(dp, u, n_waveforms, wvf_batch_size, selection, periods, ignore_nwvf, verbose)
     else:
         assert isinstance(spike_ids, Iterable), "WARNING spike_ids must be a list/array of ids!"
-        spike_ids_subset=np.array(spike_ids)
+        spike_ids_subset = np.array(spike_ids)
     n_spikes = len(spike_ids_subset)
 
     # Get waveforms times in bytes
     # and check that, for this waveform width,
     # they no not go beyond file limits
-    waveforms_t = spike_samples[spike_ids_subset].astype(np.int64)
+    waveforms_t  = spike_samples[spike_ids_subset].astype(np.int64)
     waveforms_t1 = (waveforms_t-t_waveforms//2)*n_channels_dat*item_size
     waveforms_t2 = (waveforms_t+t_waveforms//2)*n_channels_dat*item_size
     wcheck_m=(0<=waveforms_t1)&(waveforms_t2<fileSizeBytes)
     if not np.all(wcheck_m):
         print(f"Invalid times: {waveforms_t[~wcheck_m]}")
         waveforms_t1 = waveforms_t1[wcheck_m]
         waveforms_t2 = waveforms_t2[wcheck_m]
@@ -159,42 +163,44 @@
     waveforms = np.zeros((n_spikes, t_waveforms, n_channels_rec), dtype=np.float32)
     if verbose: print(f'Loading waveforms of unit {u} ({n_spikes})...')
     with open(dat_path, "rb") as f:
         for i,t1 in enumerate(waveforms_t1):
             if n_spikes>10:
                 if i%(n_spikes//10)==0 and verbose: print(f'{round((i/n_spikes)*100)}%...', end=' ')
             f.seek(t1, 0) # 0 for absolute file positioning
-            wave=f.read(n_channels_dat*t_waveforms*item_size)
-            wave=np.frombuffer(wave, dtype=dtype).reshape((t_waveforms,n_channels_dat))
-            wave = wave-np.median(wave, axis = 0)[np.newaxis,:] # center the waveforms on 0
+            wave = f.read(n_channels_dat*t_waveforms*item_size)
+            wave = np.frombuffer(wave, dtype=dtype).reshape((t_waveforms,n_channels_dat))
             # get rid of sync channel
             waveforms[i,:,:] = wave[:,:-1] if meta['acquisition_software']=='SpikeGLX' else wave
+    if med_sub_in_time:
+        medians = np.median(waveforms, axis = 1)
+        waveforms = waveforms - medians[:,np.newaxis,:]
     if verbose: print('\n')
 
     # Preprocess waveforms
     if hpfilt|med_sub|whiten:
-        waveforms=waveforms.reshape((n_spikes*t_waveforms, n_channels_rec))
+        waveforms     = waveforms.reshape((n_spikes*t_waveforms, n_channels_rec))
         if hpfilt:
-            waveforms=apply_filter(waveforms, bandpass_filter(rate=sample_rate, low=None, high=hpfiltf, order=3), axis=0)
+            waveforms = apply_filter(waveforms, bandpass_filter(rate=sample_rate, low=None, high=hpfiltf, order=3), axis=0)
         if med_sub:
-            waveforms=med_substract(waveforms, axis=1, nRange=nRangeMedSub)
+            waveforms = med_substract(waveforms, axis=1, nRange=nRangeMedSub)
         if whiten:
-            waveforms=whitening(waveforms.T, nRange=nRangeWhiten).T # whitens across channels so gotta transpose
-        waveforms=waveforms.reshape((n_spikes,t_waveforms, n_channels_rec))
+            waveforms = whitening(waveforms.T, nRange=nRangeWhiten).T # whitens across channels so gotta transpose
+        waveforms     = waveforms.reshape((n_spikes,t_waveforms, n_channels_rec))
 
     # Filter channels ignored by kilosort if necesssary
     if not ignore_ks_chanfilt:
         channel_ids_ks = np.load(Path(dp, 'channel_map.npy'), mmap_mode='r').squeeze()
-        channel_ids_ks=channel_ids_ks[channel_ids_ks!=384]
-        waveforms=waveforms[:,:,channel_ids_ks] # only AFTER processing, filter out channels
+        channel_ids_ks = channel_ids_ks[channel_ids_ks!=384]
+        waveforms      = waveforms[:,:,channel_ids_ks] # only AFTER processing, filter out channels
 
     # Correct voltage scaling
-    waveforms*=meta['bit_uV_conv_factor']
+    waveforms *= meta['bit_uV_conv_factor']
 
-    return  waveforms.astype(np.float32)
+    return waveforms.astype(np.float32)
 
 def wvf_dsmatch(dp, u, n_waveforms=100, t_waveforms=82, periods='all',
                 wvf_batch_size=10, ignore_nwvf=True, med_sub = False, spike_ids = None,
                 save=True, verbose=False, again=False,
                 whiten=False,  hpfilt=False, hpfiltf=300, nRangeWhiten=None, nRangeMedSub=None,
                 n_waves_used_for_matching = 5000, peakchan_allowed_range=6,
                 use_average_peakchan = False, max_allowed_amplitude = 1800, max_allowed_shift=3,
@@ -552,14 +558,83 @@
         ylim = fig.get_axes()[0].get_ylim()
         fig.get_axes()[0].plot([max_shift_allowed,max_shift_allowed], ylim, color='red', ls='--')
         fig.get_axes()[0].plot([-max_shift_allowed,-max_shift_allowed], ylim, color='red', ls='--')
         fig.get_axes()[0].set_ylim(ylim)
 
     return aligned_waves
 
+def across_channels_SNR(dp, u, n_waveforms=500, t_waveforms=90,
+                        periods='all', spike_ids=None,
+                        c = 1, chan_range = 3, return_distributions = False):
+    
+    dp = Path(dp)
+    
+    # load spike ids
+    if spike_ids is None:
+        spike_ids = get_ids_subset(dp, u, n_waveforms, 10, 'regular', periods, True)
+    n_spikes = len(spike_ids)
+    
+    # get waveforms
+    waves = get_waveforms(dp, u, n_waveforms, t_waveforms, 'regular',
+                          periods, spike_ids, ignore_ks_chanfilt=True)
+    
+    # get random selection of voltage snippets in the vicinity of the waveforms
+    meta           = read_metadata(dp)
+    dat_path       = get_binary_file_path(dp, 'ap')
+    n_channels_dat = meta['highpass']['n_channels_binaryfile']
+    n_channels_rec = n_channels_dat-1 if meta['acquisition_software']=='SpikeGLX' else n_channels_dat
+    dtype          = np.dtype(meta['highpass']['datatype'])
+    item_size      = dtype.itemsize
+    fileSizeBytes  = meta['highpass']['binary_byte_size']
+
+    spike_samples  = np.load(Path(dp, 'spike_times.npy'), mmap_mode='r').squeeze()
+    spike_times    = spike_samples[spike_ids].astype(np.int64)
+    random_times   = spike_times + np.random.randint(-30000, 30000, size=len(spike_times))
+
+    T1       = (random_times-t_waveforms//2)*n_channels_dat*item_size
+    T2       = (random_times+t_waveforms//2)*n_channels_dat*item_size
+    wcheck_m = (0<=T1)&(T2<fileSizeBytes)
+    if not np.all(wcheck_m):
+        T1   = T1[wcheck_m]
+        T2   = T2[wcheck_m]
+
+    noise = np.zeros((n_spikes, t_waveforms, n_channels_rec), dtype=np.float32)
+    with open(dat_path, "rb") as f:
+        for i,t1 in enumerate(T1):
+            f.seek(t1, 0) # 0 for absolute file positioning
+            snip = f.read(n_channels_dat*t_waveforms*item_size)
+            snip = np.frombuffer(snip, dtype=dtype).reshape((t_waveforms, n_channels_dat))
+            noise[i,:,:]     = snip[:,:-1] if meta['acquisition_software']=='SpikeGLX' else snip
+    # center on 0 like original waveform
+    medians = np.median(noise, axis = 1)
+    noise = noise - medians[:,np.newaxis,:]
+    # convert to microvolts
+    noise *= meta['bit_uV_conv_factor']
+
+    # compute SNR
+    s_mean     = waves.mean(0)
+    peak_chan  = np.argmax(np.ptp(s_mean, axis=0))
+    chan_range = np.arange(peak_chan-chan_range, peak_chan+chan_range+1)
+    used_channels = np.unique(np.clip(chan_range, 0, s_mean.shape[1]-1))
+
+    s = np.zeros(waves.shape[0])
+    for i, v in enumerate(waves):
+        s[i] = np.sum(s_mean[:,used_channels] * v[:,used_channels])
+
+    n = np.zeros(waves.shape[0])
+    for i, v in enumerate(noise):
+        n[i] = np.sum(s_mean[:,used_channels] * v[:,used_channels])
+
+    snr = (s.mean() - n.mean())/(c * n.std())
+
+    if return_distributions:
+        return snr, s, n, waves, noise
+
+    return snr
+
 def get_pc(waveforms):
     wvf_m = np.mean(waveforms, axis=0)
     max_min_wvf=np.max(wvf_m,0)-np.min(wvf_m,0)
     peak_chan = np.argmax(max_min_wvf)
     return peak_chan
 
 def get_peak_chan(dp, unit, use_template=True, again=False, ignore_ks_chanfilt=True, periods='all', save=True):
@@ -807,9 +882,9 @@
     assert n_excerpts >= 2
     step = max((n_samples - excerpt_size) // (n_excerpts - 1),
                excerpt_size)
     return step
 
 # Recurrent imports
 from npyx.merger import assert_multi, get_ds_ids, get_source_dp_u
-from npyx.spk_t import ids
 from npyx.plot import hist_MB, imshow_cbar, quickplot_n_waves
+from npyx.spk_t import ids
```

### Comparing `npyx-2.7.1/npyx/stats.py` & `npyx-2.8.0/npyx/stats.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/testing.py` & `npyx-2.8.0/npyx/testing.py`

 * *Files identical despite different names*

### Comparing `npyx-2.7.1/npyx/utils.py` & `npyx-2.8.0/npyx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,20 +39,20 @@
     4:(84./255, 255./255, 28./255),
     5:(255./255,165./255,0./255),
     -1:(0., 0., 0.),
     }
 
 mpl_colors=plt.rcParams['axes.prop_cycle'].by_key()['color']
 
-DistinctColors20 = [(127,127,127),(0,0,143),(182,0,0),(0,140,0),(195,79,255),(1,165,202),(236,157,0),(118,255,0),(255,127,0),
-    (255,117,152),(148,0,115),(0,243,204),(72,83,255),(0,127,255),(0,67,1),(237,183,255),(138,104,0),(97,0,163),(92,0,17),(255,245,133)]
-DistinctColors20 = [(c[0]/255, c[1]/255, c[2]/255) for c in DistinctColors20]
-DistinctColors15 = [(127,127,127),(255,255,0),(0,0,143),(255,0,0),(50,255,255),(255,0,255),(94,0,33),(0,67,0),
-    (255,218,248),(0,178,0),(124,72,255),(211,145,0),(5,171,253),(126,73,0),(147,0,153)]
-DistinctColors15 = [(c[0]/255, c[1]/255, c[2]/255) for c in DistinctColors15]
+DistinctColors20 = [[127,127,127],[0,0,143],[182,0,0],[0,140,0],[195,79,255],[1,165,202],[236,157,0],[118,255,0],[255,127,0],
+    [255,117,152],[148,0,115],[0,243,204],[72,83,255],[0,127,255],[0,67,1],[237,183,255],[138,104,0],[97,0,163],[92,0,17],[255,245,133]]
+DistinctColors20 = [[c[0]/255, c[1]/255, c[2]/255] for c in DistinctColors20]
+DistinctColors15 = [[127,127,127],[255,255,0],[0,0,143],[255,0,0],[50,255,255],[255,0,255],[94,0,33],[0,67,0],
+    [255,218,248],[0,178,0],[124,72,255],[211,145,0],[5,171,253],[126,73,0],[147,0,153]]
+DistinctColors15 = [[c[0]/255, c[1]/255, c[2]/255] for c in DistinctColors15]
 
 mark_dict = {
 ".":"point",
 ",":"pixel",
 "o":"circle",
 "v":"triangle_down",
 "^":"triangle_up",
```

### Comparing `npyx-2.7.1/npyx.egg-info/PKG-INFO` & `npyx-2.8.0/npyx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 2.7.1
+Version: 2.8.0
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 [![PyPI Version](https://img.shields.io/pypi/v/npyx.svg)](https://pypi.org/project/npyx/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5509776.svg)](https://doi.org/10.5281/zenodo.5509776)
 [![License](https://img.shields.io/pypi/l/npyx.svg)](https://github.com/m-beau/NeuroPyxels/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/npyx/month)](https://pepy.tech/project/npyx)
 
 [NeuroPyxels](https://github.com/m-beau/NeuroPyxels) (npyx) is a python library built for electrophysiologists using Neuropixels electrodes. This package stems from the need of a pythonist who really did not want to transition to MATLAB to work with Neuropixels: it features a suite of core utility functions for loading, processing and plotting Neuropixels data.
 
-There isn't any better doc atm - post an issue if you have any question, or email [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
+**Questions**: There isn't any better doc atm, but feel free to post an issue here (preferred option, so that everyone can benefit from it 🙂) or drop me an email at [Maxime Beau](maximebeaujeanroch047@gmail.com) (PhD Hausser lab, UCL). You can also use the [Neuropixels slack workgroup](neuropixelsgroup.slack.com).
 
 
 - **[Documentation](https://github.com/m-beau/NeuroPyxels#documentation)**
   - [Load synchronization channel](https://github.com/m-beau/NeuroPyxels#load-synchronization-channel)
   - [Get good units from dataset](https://github.com/m-beau/NeuroPyxels#get-good-units-from-dataset)
   - [Load spike times from unit u](https://github.com/m-beau/NeuroPyxels#load-spike-times-from-unit-u)
   - [Load waveforms from unit u](https://github.com/m-beau/NeuroPyxels#load-waveforms-from-unit-u)
@@ -37,27 +37,27 @@
   - [Bonus: cool npyx plotting utilities which could turn out useful](https://github.com/m-beau/NeuroPyxels#bonus-cool-matplotlib-plotting-utilities-which-could-turn-out-useful)
 - **[Installation](https://github.com/m-beau/NeuroPyxels#installation)**
 - **[Acknowledgement](https://github.com/m-beau/NeuroPyxels#acknowledgement)**
 - **[Developer cheatsheet](https://github.com/m-beau/NeuroPyxels#developer-cheatsheet)**
 
 
 ## Documentation:
-Npyx works in harmony with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html, results stored in `path/mydata/mydata.GUI`)). Any dataset you can run phy on can also be analyzed with npyx, in essence.
+Npyx works with the data formatting employed by [SpikeGLX](https://billkarsh.github.io/SpikeGLX/) and [OpenEphys](https://open-ephys.org/neuropixels) (binary data and meta data) used in combination with [Kilosort](https://github.com/MouseLand/Kilosort) or [SpyKING CIRCUS](https://spyking-circus.readthedocs.io/en/latest/) and [Phy](https://phy.readthedocs.io/en/latest/) ([after conversion for the phy gui](https://spyking-circus.readthedocs.io/en/latest/GUI/launching.html), results stored in `path/mydata/mydata.GUI`). **Any dataset compatible with phy can also be analyzed with npyx, in essence.**
 
-<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **kilosort_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
+<ins>Npyx is fast because it never computes the same thing twice</ins> - in the background, it saves most relevant outputs (spike trains, waveforms, correlograms...) at **npix_dataset/npyxMemory**, from where they are simply reloaded if called again. An important parameter controlling this behaviour is **`again`** (boolean), by default set to False: if True, the function will recompute the output rather than loading it from npyxMemory. This is important to be aware of this behaviour, as it can lead to mind boggling bugs. For instance, if you load the train of unit then re-spikesort your dataset, e.g. you split unit 56 in 504 and 505, the train of the old unit 56 will still exist at kilosort_dataset/npyxMemory and you will be able to load it even though the unit is gone!
 
-Most npyx functions take at least one input: **`dp`**, which is the path to your Kilosort-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on phy documentation.
+Most npyx functions take at least one input: **`dp`**, which is the path to your Neuropixels-phy dataset. You can find a [full description of the structure of such datasets](https://phy.readthedocs.io/en/latest/sorting_user_guide/#installation) on the phy documentation.
 
 Other typical parameters are: **`verbose`** (whether to print a bunch of informative messages, useful when debugging), **`saveFig`** (boolean) and **`saveDir`** (whether to save the figure in saveDir for plotting functions).
 
 Importantly, **`dp`** can also be the path to a **merged dataset**, generated with `npyx.merge_datasets()` - <ins>every function will run as smoothly on merged datasets as on any regular dataset</ins>. See below for more details.
 
-More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin``myrecording.dat`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `sync_chan` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
+More precisely, every function requires the files `myrecording.ap.meta`/`myrecording.oebin` (metadata from SpikeGLX/OpenEphys), `params.py`, `spike_times.npy` and `spike_clusters.npy`. If you have started spike sorting, `cluster_groups.tsv` will also be required obviously (will be created filled with 'unsorted' groups if none is found). Then particular functions will require particular files: loading waveforms with `npyx.spk_wvf.wvf` or extracting your sync channel with `npyx.io.get_npix_sync` require the raw data `myrecording.ap.bin`, `npyx.spk_wvf.templates` the files `templates.npy` and `spike_templates.npy`, and so on. This allows you to only transfer the strictly necassary files for your use case from a machine to the next: for instance, if you only want to make behavioural analysis of spike trains but do not care about the waveforms, you can run `get_npix_sync` on a first machine (which will generate a `sync_chan` folder containing extracted onsets/offsets from the sync channel(s)), then exclusively transfer the `dataset/sync_chan/` folder along with `spike_times.npy` and `spike_clusters.npy` (all very light files) on another computer and analyze your data there seemlessly.
 
-DISCLAIMER: some parts of the code (in particular contents of feat.py) are experimental - use at your own risk!
+DISCLAIMER: some parts of the code are experimental - use at your own risk!
 
 ### Directory structure
 
 The **`dp`** parameter of all npyx functions must be the **absolute path to `myrecording`** below.
 
 For SpikeGLX recordings:
 ```
```

### Comparing `npyx-2.7.1/setup.py` & `npyx-2.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     else:
         raise RuntimeError("Unable to find version string.")
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ['ipython', 'numpy', 'scipy', 'pandas', 'numba', 'statsmodels',
-                'matplotlib', 'cmcrameri', 'opencv-python', 'scikit-learn', 'networkx',
+                'matplotlib', 'cmcrameri', 'opencv-python', 'scikit-learn', 'imbalanced-learn', 'networkx',
                 'psutil', 'joblib', 'tqdm', 'h5py']
 
 setup(name='npyx',
       version=get_version("npyx/__init__.py"),
       author='Maxime Beau',
       author_email='maximebeaujeanroch047@gmail.com',
       description='Python routines dealing with Neuropixels data.',
```

