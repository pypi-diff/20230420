# Comparing `tmp/alacorder-79.5.1.tar.gz` & `tmp/alacorder-79.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.5.1.tar", max compression
+gzip compressed data, was "alacorder-79.5.2.tar", max compression
```

## Comparing `alacorder-79.5.1.tar` & `alacorder-79.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.5.1/LICENSE
--rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.5.1/README.md
--rw-r--r--   0        0        0      682 2023-04-19 22:07:29.140941 alacorder-79.5.1/pyproject.toml
--rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.5.1/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.5.1/src/alacorder/.python-version
--rw-r--r--   0        0        0     2157 2023-04-19 22:05:38.789380 alacorder-79.5.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   135628 2023-04-19 22:04:37.672558 alacorder-79.5.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   135628 2023-04-19 22:04:37.672558 alacorder-79.5.1/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.5.1/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 alacorder-79.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.5.2/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.5.2/README.md
+-rw-r--r--   0        0        0      682 2023-04-19 23:01:00.665786 alacorder-79.5.2/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.5.2/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.5.2/src/alacorder/.python-version
+-rw-r--r--   0        0        0     2157 2023-04-19 22:05:38.789380 alacorder-79.5.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   135689 2023-04-19 22:59:51.002756 alacorder-79.5.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   135689 2023-04-19 22:59:51.002756 alacorder-79.5.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.5.2/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 alacorder-79.5.2/PKG-INFO
```

### Comparing `alacorder-79.5.1/LICENSE` & `alacorder-79.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.1/README.md` & `alacorder-79.5.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.1/pyproject.toml` & `alacorder-79.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.5.1"
+version = "79.5.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.5.1/src/alacorder/__init__.py` & `alacorder-79.5.2/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.5.1/src/alacorder/__main__.py` & `alacorder-79.5.2/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.5.1"
+version = "79.5.2"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
@@ -1517,16 +1517,17 @@
     if cf["NO_WRITE"] == True:
         return outputs
     elif not cf["OVERWRITE"] and os.path.isfile(cf["OUTPUT_PATH"]):
         raise Exception(
             "Could not write to output path because overwrite mode is not enabled."
         )
     elif cf["OUTPUT_EXT"] in (".xlsx", ".xls"):
-        if "AllPagesTextNoNewLine" in outputs.columns:
-            outputs = outputs.select(pl.exclude("AllPagesTextNoNewLine"))
+        if isinstance(pl.dataframe.frame.DataFrame):
+            if "AllPagesTextNoNewLine" in outputs.columns:
+                outputs = outputs.select(pl.exclude("AllPagesTextNoNewLine"))
         with xlsxwriter.Workbook(cf["OUTPUT_PATH"]) as workbook:
             if not isinstance(outputs, list):
                 outputs = [outputs]
             if len(sheet_names) > 0:
                 for i, x in enumerate(outputs):
                     x.write_excel(
                         workbook=workbook,
```

### Comparing `alacorder-79.5.1/src/alacorder/alac.py` & `alacorder-79.5.2/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
 (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.5.1"
+version = "79.5.2"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
@@ -1517,16 +1517,17 @@
     if cf["NO_WRITE"] == True:
         return outputs
     elif not cf["OVERWRITE"] and os.path.isfile(cf["OUTPUT_PATH"]):
         raise Exception(
             "Could not write to output path because overwrite mode is not enabled."
         )
     elif cf["OUTPUT_EXT"] in (".xlsx", ".xls"):
-        if "AllPagesTextNoNewLine" in outputs.columns:
-            outputs = outputs.select(pl.exclude("AllPagesTextNoNewLine"))
+        if isinstance(pl.dataframe.frame.DataFrame):
+            if "AllPagesTextNoNewLine" in outputs.columns:
+                outputs = outputs.select(pl.exclude("AllPagesTextNoNewLine"))
         with xlsxwriter.Workbook(cf["OUTPUT_PATH"]) as workbook:
             if not isinstance(outputs, list):
                 outputs = [outputs]
             if len(sheet_names) > 0:
                 for i, x in enumerate(outputs):
                     x.write_excel(
                         workbook=workbook,
```

### Comparing `alacorder-79.5.1/PKG-INFO` & `alacorder-79.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.5.1
+Version: 79.5.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

