# Comparing `tmp/breathXplorer-0.1.2.tar.gz` & `tmp/breathXplorer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breathXplorer-0.1.2.tar", last modified: Wed Apr 12 17:26:40 2023, max compression
+gzip compressed data, was "breathXplorer-0.1.3.tar", last modified: Thu Apr 20 00:00:55 2023, max compression
```

## Comparing `breathXplorer-0.1.2.tar` & `breathXplorer-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-12 17:26:40.589269 breathXplorer-0.1.2/
--rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.2/LICENSE
--rw-r--r--   0 wangyk     (501) staff       (20)      858 2023-04-12 17:26:40.589085 breathXplorer-0.1.2/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)      156 2023-04-12 04:11:58.000000 breathXplorer-0.1.2/README.md
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-12 17:26:40.587126 breathXplorer-0.1.2/breathXplorer/
--rw-r--r--   0 wangyk     (501) staff       (20)       48 2023-04-12 04:20:40.000000 breathXplorer-0.1.2/breathXplorer/__init__.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.2/breathXplorer/cluster.py
--rw-r--r--   0 wangyk     (501) staff       (20)     1445 2023-04-12 04:27:25.000000 breathXplorer-0.1.2/breathXplorer/extract.py
--rw-r--r--   0 wangyk     (501) staff       (20)     5047 2023-04-12 17:21:22.000000 breathXplorer-0.1.2/breathXplorer/file_io.py
--rw-r--r--   0 wangyk     (501) staff       (20)     6018 2023-04-12 17:21:22.000000 breathXplorer-0.1.2/breathXplorer/find_peak.py
--rw-r--r--   0 wangyk     (501) staff       (20)      484 2023-04-12 04:08:06.000000 breathXplorer-0.1.2/breathXplorer/score.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-12 17:26:40.588479 breathXplorer-0.1.2/breathXplorer.egg-info/
--rw-r--r--   0 wangyk     (501) staff       (20)      858 2023-04-12 17:26:40.000000 breathXplorer-0.1.2/breathXplorer.egg-info/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)      383 2023-04-12 17:26:40.000000 breathXplorer-0.1.2/breathXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-04-12 17:26:40.000000 breathXplorer-0.1.2/breathXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-04-12 17:26:40.000000 breathXplorer-0.1.2/breathXplorer.egg-info/requires.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-04-12 17:26:40.000000 breathXplorer-0.1.2/breathXplorer.egg-info/top_level.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-04-12 17:26:40.589343 breathXplorer-0.1.2/setup.cfg
--rw-r--r--   0 wangyk     (501) staff       (20)      978 2023-04-12 05:05:16.000000 breathXplorer-0.1.2/setup.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-12 17:26:40.588653 breathXplorer-0.1.2/tests/
--rw-r--r--   0 wangyk     (501) staff       (20)      331 2023-04-12 04:20:40.000000 breathXplorer-0.1.2/tests/test_extract.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:00:55.143624 breathXplorer-0.1.3/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.3/LICENSE
+-rw-r--r--   0 wangyk     (501) staff       (20)     1888 2023-04-20 00:00:55.143469 breathXplorer-0.1.3/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)     1185 2023-04-19 23:51:39.000000 breathXplorer-0.1.3/README.md
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:00:55.142032 breathXplorer-0.1.3/breathXplorer/
+-rw-r--r--   0 wangyk     (501) staff       (20)       60 2023-04-19 22:11:13.000000 breathXplorer-0.1.3/breathXplorer/__init__.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.3/breathXplorer/cluster.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     1858 2023-04-19 23:07:11.000000 breathXplorer-0.1.3/breathXplorer/extract.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     5045 2023-04-19 22:06:06.000000 breathXplorer-0.1.3/breathXplorer/file_io.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     6018 2023-04-12 17:21:22.000000 breathXplorer-0.1.3/breathXplorer/find_peak.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2019 2023-04-19 23:28:10.000000 breathXplorer-0.1.3/breathXplorer/utils.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:00:55.142980 breathXplorer-0.1.3/breathXplorer.egg-info/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1888 2023-04-20 00:00:55.000000 breathXplorer-0.1.3/breathXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)      383 2023-04-20 00:00:55.000000 breathXplorer-0.1.3/breathXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-04-20 00:00:55.000000 breathXplorer-0.1.3/breathXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-04-20 00:00:55.000000 breathXplorer-0.1.3/breathXplorer.egg-info/requires.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-04-20 00:00:55.000000 breathXplorer-0.1.3/breathXplorer.egg-info/top_level.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-04-20 00:00:55.143677 breathXplorer-0.1.3/setup.cfg
+-rw-r--r--   0 wangyk     (501) staff       (20)      978 2023-04-19 23:51:39.000000 breathXplorer-0.1.3/setup.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 00:00:55.143143 breathXplorer-0.1.3/tests/
+-rw-r--r--   0 wangyk     (501) staff       (20)      895 2023-04-19 23:31:55.000000 breathXplorer-0.1.3/tests/test_extract.py
```

### Comparing `breathXplorer-0.1.2/LICENSE` & `breathXplorer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.2/breathXplorer/cluster.py` & `breathXplorer-0.1.3/breathXplorer/cluster.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.2/breathXplorer/extract.py` & `breathXplorer-0.1.3/breathXplorer/extract.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 from pathlib import Path
-from typing import Sequence, List
+from typing import Sequence, List, Union
 
 import pandas as pd
 
 from .cluster import cluster_merge
-from .file_io import cluster_ms, gen_csv
-from .score import score
+from .file_io import cluster_ms, gen_df
+from .utils import score, time_union, interpolate_time
 
 
 # a single task
-def find_feature(ms: Path, line: bool, quantity: float, method: str, n_peak=1) -> pd.DataFrame:
+def find_feature(ms: Union[Path, str], line: bool, quantity: float, method: str, n_peak: int = 1) -> pd.DataFrame:
     """
     Calculate the feature table of a single mzML file.
     :param ms:  Path of the mzML file.
     :param line:  Whether to use line mode.
     :param quantity: control the quality of peak
     :param method:  The method used to find peaks ('Topological' or 'Gaussian').
     :param n_peak:  Number of peaks to be picked
     :return:  Feature table
     """
+    ms = Path(ms)
     scanned = cluster_ms(str(ms.absolute()), line, quantity, method, n_peak)
     try:
         scores = score(scanned, scanned['peak_time'])
     except ZeroDivisionError:
         scores = score(scanned)
-    return gen_csv(scanned, [('intensity', scores)])
+    return gen_df(scanned, [('intensity', scores)])
 
 
 # merge all the result files of single tasks in the target folder
 def merge_result(tbs: Sequence[pd.DataFrame], names: List[str]) -> pd.DataFrame:
     """
     Merge the feature tables of multiple mzML files.
     :param tbs:  Feature tables
     :param names:  Names of the mzML files
     :return:  Merged feature table
     """
     sub_results = [dict(zip(tb.index, tb['intensity'])) for tb in tbs]
     result = cluster_merge(sub_results)
     return pd.DataFrame(data=list(result.values()), index=list(result.keys()), columns=names)
+
+
+def time_align(tbs: Sequence[pd.DataFrame]) -> Sequence[pd.DataFrame]:
+    """
+    Align the time of multiple feature tables.
+    :param tbs:  Feature tables
+    :return:  Aligned feature tables
+    """
+    if len(tbs) == 1:
+        return tbs
+    common_time = time_union(tbs)
+    return [interpolate_time(tb, common_time) for tb in tbs]
```

### Comparing `breathXplorer-0.1.2/breathXplorer/file_io.py` & `breathXplorer-0.1.3/breathXplorer/file_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,16 +106,16 @@
     for c in np.unique(labels[labels != -1]):
         this_mz = projected_mz[labels == c]
         new_mz.append(this_mz.mean())
         records.append(__drop_zero_near(tb.loc[np.unique(this_mz)].values, this_mz.mean(), np.unique(this_mz)))
     return {'time': times, "intensities": dict(zip(new_mz, records)), 'tic': tic, 'peak_time': total_time}
 
 
-def gen_csv(scanned_file: dict, new_inf: List[Tuple]) -> pd.DataFrame:
-    """Generate the result csv.
+def gen_df(scanned_file: dict, new_inf: List[Tuple]) -> pd.DataFrame:
+    """Generate the Dataframe.
     :param scanned_file: Dictionary read from scan_file
     :param new_inf: New information to append, such as class, mean m/z, correlation with CO2, etc.
                 [tuple1(name1, dc1), tuple2(name2, dc2<key: m/z>), ...]
     :return: DataFrame to be saved in result.csv
     """
     mat = np.array(list(scanned_file['intensities'].values()))
     otb = pd.DataFrame(data=mat, index=list(scanned_file['intensities'].keys()), columns=scanned_file['time'])
```

### Comparing `breathXplorer-0.1.2/breathXplorer/find_peak.py` & `breathXplorer-0.1.3/breathXplorer/find_peak.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.2/setup.py` & `breathXplorer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirement.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="breathXplorer",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=required_packages,
     author="wykswr",
     author_email="bifocal.above.0y@icloud.com",
     description="A tool to do peak picking and feature extraction on breath data",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

