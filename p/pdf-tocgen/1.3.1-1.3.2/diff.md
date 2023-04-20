# Comparing `tmp/pdf_tocgen-1.3.1.tar.gz` & `tmp/pdf_tocgen-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_tocgen-1.3.1.tar", max compression
+gzip compressed data, was "pdf_tocgen-1.3.2.tar", max compression
```

## Comparing `pdf_tocgen-1.3.1.tar` & `pdf_tocgen-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.1/LICENSE
--rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.1/LICENSE_AGPL
--rw-r--r--   0        0        0    13650 2021-05-09 08:08:57.010536 pdf_tocgen-1.3.1/README.md
--rw-r--r--   0        0        0      274 2023-04-20 06:06:03.536966 pdf_tocgen-1.3.1/fitzutils/__init__.py
--rw-r--r--   0        0        0     2875 2023-04-20 06:05:46.873633 pdf_tocgen-1.3.1/fitzutils/fitzutils.py
--rw-r--r--   0        0        0       87 2023-04-20 06:08:26.133627 pdf_tocgen-1.3.1/pdftocgen/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocgen/__main__.py
--rw-r--r--   0        0        0     4880 2023-04-20 06:15:48.496945 pdf_tocgen-1.3.1/pdftocgen/app.py
--rw-r--r--   0        0        0     5395 2021-11-10 10:51:01.789897 pdf_tocgen-1.3.1/pdftocgen/filter.py
--rw-r--r--   0        0        0     4963 2021-11-10 19:31:24.999892 pdf_tocgen-1.3.1/pdftocgen/recipe.py
--rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocgen/tocgen.py
--rw-r--r--   0        0        0       73 2023-04-20 06:08:05.546961 pdf_tocgen-1.3.1/pdftocio/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocio/__main__.py
--rw-r--r--   0        0        0     5563 2023-04-20 06:18:07.596940 pdf_tocgen-1.3.1/pdftocio/app.py
--rw-r--r--   0        0        0      481 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocio/tocio.py
--rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf_tocgen-1.3.1/pdftocio/tocparser.py
--rw-r--r--   0        0        0      148 2023-04-20 06:08:00.250295 pdf_tocgen-1.3.1/pdfxmeta/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdfxmeta/__main__.py
--rw-r--r--   0        0        0     4212 2023-04-20 06:10:42.420289 pdf_tocgen-1.3.1/pdfxmeta/app.py
--rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf_tocgen-1.3.1/pdfxmeta/pdfxmeta.py
--rw-r--r--   0        0        0      966 2023-04-20 06:03:36.103638 pdf_tocgen-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    14648 1970-01-01 00:00:00.000000 pdf_tocgen-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.2/LICENSE
+-rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.2/LICENSE_AGPL
+-rw-r--r--   0        0        0    13650 2021-05-09 08:08:57.010536 pdf_tocgen-1.3.2/README.md
+-rw-r--r--   0        0        0      274 2023-04-20 06:06:03.536966 pdf_tocgen-1.3.2/fitzutils/__init__.py
+-rw-r--r--   0        0        0     2875 2023-04-20 06:05:46.873633 pdf_tocgen-1.3.2/fitzutils/fitzutils.py
+-rw-r--r--   0        0        0       87 2023-04-20 07:11:03.110161 pdf_tocgen-1.3.2/pdftocgen/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocgen/__main__.py
+-rw-r--r--   0        0        0     4880 2023-04-20 06:15:48.496945 pdf_tocgen-1.3.2/pdftocgen/app.py
+-rw-r--r--   0        0        0     5395 2021-11-10 10:51:01.789897 pdf_tocgen-1.3.2/pdftocgen/filter.py
+-rw-r--r--   0        0        0     4963 2021-11-10 19:31:24.999892 pdf_tocgen-1.3.2/pdftocgen/recipe.py
+-rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocgen/tocgen.py
+-rw-r--r--   0        0        0       73 2023-04-20 07:11:06.263494 pdf_tocgen-1.3.2/pdftocio/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocio/__main__.py
+-rw-r--r--   0        0        0     5563 2023-04-20 06:18:07.596940 pdf_tocgen-1.3.2/pdftocio/app.py
+-rw-r--r--   0        0        0      481 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocio/tocio.py
+-rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf_tocgen-1.3.2/pdftocio/tocparser.py
+-rw-r--r--   0        0        0      148 2023-04-20 07:11:09.396827 pdf_tocgen-1.3.2/pdfxmeta/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdfxmeta/__main__.py
+-rw-r--r--   0        0        0     4212 2023-04-20 06:10:42.420289 pdf_tocgen-1.3.2/pdfxmeta/app.py
+-rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf_tocgen-1.3.2/pdfxmeta/pdfxmeta.py
+-rw-r--r--   0        0        0      970 2023-04-20 07:11:22.273494 pdf_tocgen-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14648 1970-01-01 00:00:00.000000 pdf_tocgen-1.3.2/PKG-INFO
```

### Comparing `pdf_tocgen-1.3.1/LICENSE` & `pdf_tocgen-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/LICENSE_AGPL` & `pdf_tocgen-1.3.2/LICENSE_AGPL`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/README.md` & `pdf_tocgen-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/fitzutils/fitzutils.py` & `pdf_tocgen-1.3.2/fitzutils/fitzutils.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdftocgen/app.py` & `pdf_tocgen-1.3.2/pdftocgen/app.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdftocgen/filter.py` & `pdf_tocgen-1.3.2/pdftocgen/filter.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdftocgen/recipe.py` & `pdf_tocgen-1.3.2/pdftocgen/recipe.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdftocio/app.py` & `pdf_tocgen-1.3.2/pdftocio/app.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdftocio/tocparser.py` & `pdf_tocgen-1.3.2/pdftocio/tocparser.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdfxmeta/app.py` & `pdf_tocgen-1.3.2/pdfxmeta/app.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pdfxmeta/pdfxmeta.py` & `pdf_tocgen-1.3.2/pdfxmeta/pdfxmeta.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.1/pyproject.toml` & `pdf_tocgen-1.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf.tocgen"
-version = "1.3.1"
+version = "1.3.2"
 description = "Automatically generate table of contents for pdf files"
 authors = ["krasjet"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://krasjet.com/voice/pdf.tocgen/"
 repository = "https://github.com/Krasjet/pdf.tocgen"
 keywords = ["pdf", "cli"]
@@ -35,9 +35,9 @@
 
 [tool.poetry.scripts]
 pdfxmeta = "pdfxmeta.app:main"
 pdftocgen = "pdftocgen.app:main"
 pdftocio = "pdftocio.app:main"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pdf_tocgen-1.3.1/PKG-INFO` & `pdf_tocgen-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-tocgen
-Version: 1.3.1
+Version: 1.3.2
 Summary: Automatically generate table of contents for pdf files
 Home-page: https://krasjet.com/voice/pdf.tocgen/
 License: GPL-3.0-or-later
 Keywords: pdf,cli
 Author: krasjet
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

