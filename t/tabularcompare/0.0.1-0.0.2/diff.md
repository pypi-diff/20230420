# Comparing `tmp/tabularcompare-0.0.1.tar.gz` & `tmp/tabularcompare-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularcompare-0.0.1.tar", last modified: Thu Apr 20 03:24:42 2023, max compression
+gzip compressed data, was "tabularcompare-0.0.2.tar", last modified: Thu Apr 20 08:25:28 2023, max compression
```

## Comparing `tabularcompare-0.0.1.tar` & `tabularcompare-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.393591 tabularcompare-0.0.1/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.383591 tabularcompare-0.0.1/.github/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.383591 tabularcompare-0.0.1/.github/workflows/
--rw-r--r--   0 erich     (1000) erich     (1000)      838 2023-04-20 01:47:12.000000 tabularcompare-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 erich     (1000) erich     (1000)     1901 2023-04-20 03:16:17.000000 tabularcompare-0.0.1/.gitignore
--rw-r--r--   0 erich     (1000) erich     (1000)    11357 2023-04-14 19:34:43.000000 tabularcompare-0.0.1/LICENSE
--rw-r--r--   0 erich     (1000) erich     (1000)      325 2023-04-20 02:55:53.000000 tabularcompare-0.0.1/Makefile
--rw-r--r--   0 erich     (1000) erich     (1000)    13915 2023-04-20 03:24:42.393591 tabularcompare-0.0.1/PKG-INFO
--rw-r--r--   0 erich     (1000) erich     (1000)      338 2023-04-20 02:02:38.000000 tabularcompare-0.0.1/README.md
--rw-r--r--   0 erich     (1000) erich     (1000)     1166 2023-04-20 03:24:30.000000 tabularcompare-0.0.1/pyproject.toml
--rw-r--r--   0 erich     (1000) erich     (1000)     3248 2023-04-20 00:43:34.000000 tabularcompare-0.0.1/requirements.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       38 2023-04-20 03:24:42.393591 tabularcompare-0.0.1/setup.cfg
--rw-r--r--   0 erich     (1000) erich     (1000)       68 2023-04-18 07:14:15.000000 tabularcompare-0.0.1/setup.py
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.383591 tabularcompare-0.0.1/src/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.383591 tabularcompare-0.0.1/src/tabularcompare/
--rw-r--r--   0 erich     (1000) erich     (1000)       69 2023-04-20 00:32:25.000000 tabularcompare-0.0.1/src/tabularcompare/__init__.py
--rw-r--r--   0 erich     (1000) erich     (1000)     4194 2023-04-18 08:13:40.000000 tabularcompare-0.0.1/src/tabularcompare/app.py
--rw-r--r--   0 erich     (1000) erich     (1000)    18609 2023-04-18 08:13:40.000000 tabularcompare-0.0.1/src/tabularcompare/compare.py
--rw-r--r--   0 erich     (1000) erich     (1000)     3397 2023-04-18 08:13:40.000000 tabularcompare-0.0.1/src/tabularcompare/utils.py
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.393591 tabularcompare-0.0.1/src/tabularcompare.egg-info/
--rw-r--r--   0 erich     (1000) erich     (1000)    13915 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/PKG-INFO
--rw-r--r--   0 erich     (1000) erich     (1000)      542 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/SOURCES.txt
--rw-r--r--   0 erich     (1000) erich     (1000)        1 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/dependency_links.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       58 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/entry_points.txt
--rw-r--r--   0 erich     (1000) erich     (1000)      246 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/requires.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       15 2023-04-20 03:24:42.000000 tabularcompare-0.0.1/src/tabularcompare.egg-info/top_level.txt
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 03:24:42.393591 tabularcompare-0.0.1/tests/
--rw-r--r--   0 erich     (1000) erich     (1000)        0 2023-04-18 07:21:18.000000 tabularcompare-0.0.1/tests/__init__.py
--rw-r--r--   0 erich     (1000) erich     (1000)      204 2023-04-18 08:05:33.000000 tabularcompare-0.0.1/tests/test_app.py
--rw-r--r--   0 erich     (1000) erich     (1000)     5638 2023-04-20 01:51:28.000000 tabularcompare-0.0.1/tests/test_compare.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/.github/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/.github/workflows/
+-rw-r--r--   0 erich     (1000) erich     (1000)      844 2023-04-20 04:57:46.000000 tabularcompare-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 erich     (1000) erich     (1000)     1901 2023-04-20 03:16:17.000000 tabularcompare-0.0.2/.gitignore
+-rw-r--r--   0 erich     (1000) erich     (1000)    11357 2023-04-14 19:34:43.000000 tabularcompare-0.0.2/LICENSE
+-rw-r--r--   0 erich     (1000) erich     (1000)      312 2023-04-20 04:59:23.000000 tabularcompare-0.0.2/Makefile
+-rw-r--r--   0 erich     (1000) erich     (1000)     7202 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/PKG-INFO
+-rw-r--r--   0 erich     (1000) erich     (1000)     6370 2023-04-20 08:20:58.000000 tabularcompare-0.0.2/README.md
+-rw-r--r--   0 erich     (1000) erich     (1000)     1358 2023-04-20 08:25:12.000000 tabularcompare-0.0.2/pyproject.toml
+-rw-r--r--   0 erich     (1000) erich     (1000)      840 2023-04-20 04:56:50.000000 tabularcompare-0.0.2/requirements.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       38 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/setup.cfg
+-rw-r--r--   0 erich     (1000) erich     (1000)       68 2023-04-18 07:14:15.000000 tabularcompare-0.0.2/setup.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/tabularcompare/
+-rw-r--r--   0 erich     (1000) erich     (1000)       69 2023-04-20 08:25:16.000000 tabularcompare-0.0.2/src/tabularcompare/__init__.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     4308 2023-04-20 08:08:11.000000 tabularcompare-0.0.2/src/tabularcompare/app.py
+-rw-r--r--   0 erich     (1000) erich     (1000)    19210 2023-04-20 06:58:42.000000 tabularcompare-0.0.2/src/tabularcompare/compare.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     3397 2023-04-18 08:13:40.000000 tabularcompare-0.0.2/src/tabularcompare/utils.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/tabularcompare.egg-info/
+-rw-r--r--   0 erich     (1000) erich     (1000)     7202 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/PKG-INFO
+-rw-r--r--   0 erich     (1000) erich     (1000)      542 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/SOURCES.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)        1 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/dependency_links.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       58 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/entry_points.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)      246 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/requires.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       15 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/top_level.txt
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/tests/
+-rw-r--r--   0 erich     (1000) erich     (1000)        0 2023-04-18 07:21:18.000000 tabularcompare-0.0.2/tests/__init__.py
+-rw-r--r--   0 erich     (1000) erich     (1000)      204 2023-04-18 08:05:33.000000 tabularcompare-0.0.2/tests/test_app.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     8295 2023-04-20 07:21:31.000000 tabularcompare-0.0.2/tests/test_compare.py
```

### Comparing `tabularcompare-0.0.1/.github/workflows/python-package.yml` & `tabularcompare-0.0.2/.github/workflows/python-package.yml`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install
       run: |
-        make install
+        pip install .[dev]
     - name: Lint with pylint
       run: |
         make lint
     - name: Test with pytest
       run: |
         make test
```

### Comparing `tabularcompare-0.0.1/.gitignore` & `tabularcompare-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.1/LICENSE` & `tabularcompare-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.1/pyproject.toml` & `tabularcompare-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tabularcompare"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Erich Henrique", email="erich.hs13@gmail.com" },
 ]
 description = "Tabular data comparison wrapper for DataComPy"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["Tabular", "Compare", "Data"]
-license = { file = "LICENSE" }
+license = { text = "Apache-2.0" }
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy<=1.24.2,>=1.11.3",
     "pandas<=1.5.3,>=0.25.0",
     "datacompy<=0.9.0,>=0.8.4",
     "pretty-html-table==0.9.16",
```

### Comparing `tabularcompare-0.0.1/src/tabularcompare/app.py` & `tabularcompare-0.0.2/src/tabularcompare/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,16 @@
         )
 
     # Join params
     if columns:
         join_columns = [col.strip() for col in columns.split(",")]
         on_index = False
     else:
+        if verbose:
+            print("join_columns not provided. Performing comparison on DataFrame indices.")
         join_columns = None
         on_index = True
 
     if ignore_columns:
         ignore_columns = [col.strip() for col in ignore_columns.split(",")]
 
     # Comparison object
```

### Comparing `tabularcompare-0.0.1/src/tabularcompare/compare.py` & `tabularcompare-0.0.2/src/tabularcompare/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import math
+import warnings
 import pandas as pd
 from typing import Union
 from datacompy import Compare
 from ordered_set import OrderedSet
 from pretty_html_table import build_table
 
 
@@ -89,17 +90,24 @@
         self._rel_tol = rel_tol
         self._ignore_spaces = ignore_spaces
         self._ignore_case = ignore_case
         self._cast_column_names_lower = cast_column_names_lower
         self._df1_intersect_cols = []
         self._df2_intersect_cols = []
         self._intersect_match_cols = []
+        self._handle_join()
         self._preprocess_int_missing()
         self._compare()
         self._enhanced_compare()
+    
+    # join_columns and on_index handling
+    def _handle_join(self):
+        if self.join_columns is None and not self._on_index:
+            warnings.warn("The join_columns parameter was not provided. Performing join on DataFrame indices. Set on_index=True to silence this warning.")
+            self._on_index = True
 
     def _preprocess_int_missing(self):
         """
         Preprocess int columns with null values typecasting them to nullable integer Int64.
         """
         intersect_columns = OrderedSet(self.df1.columns) & OrderedSet(self.df2.columns)
         if self.join_columns:
@@ -275,14 +283,20 @@
         return self._df2_unq_rows_df
 
     def intersect_columns(self) -> OrderedSet:
         """
         Returns a set of columns present in both df1 and df2.
         """
         return OrderedSet(self.df1.columns) & OrderedSet(self.df2.columns)
+    
+    def intersect_rows(self) -> pd.DataFrame:
+        """
+        Returns a pandas DataFrame with the subset of matching rows between df1 and df2.
+        """
+        return self._comparison_results.intersect_rows
 
     def report_to_txt(
         self,
         file_name: str,
         sample_count: int = 10,
         column_count: int = 10,
         file_location: str = ".",
```

### Comparing `tabularcompare-0.0.1/src/tabularcompare/utils.py` & `tabularcompare-0.0.2/src/tabularcompare/utils.py`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.1/src/tabularcompare.egg-info/SOURCES.txt` & `tabularcompare-0.0.2/src/tabularcompare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

