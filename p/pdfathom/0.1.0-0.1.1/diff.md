# Comparing `tmp/pdfathom-0.1.0.tar.gz` & `tmp/pdfathom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfathom-0.1.0.tar", max compression
+gzip compressed data, was "pdfathom-0.1.1.tar", max compression
```

## Comparing `pdfathom-0.1.0.tar` & `pdfathom-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7048 2023-04-19 18:30:50.984373 pdfathom-0.1.0/LICENSE
--rw-r--r--   0        0        0     1333 2023-04-20 03:29:50.373801 pdfathom-0.1.0/README.md
--rw-r--r--   0        0        0      249 2023-04-19 23:23:43.416419 pdfathom-0.1.0/pdfathom/__main__.py
--rw-r--r--   0        0        0     1613 2023-04-20 15:52:32.065527 pdfathom-0.1.0/pdfathom/arguments.py
--rw-r--r--   0        0        0      598 2023-04-20 15:52:32.059466 pdfathom-0.1.0/pdfathom/config.py
--rw-r--r--   0        0        0     3069 2023-04-20 15:52:32.057086 pdfathom-0.1.0/pdfathom/db.py
--rw-r--r--   0        0        0     3849 2023-04-20 15:52:32.075357 pdfathom-0.1.0/pdfathom/repl.py
--rw-r--r--   0        0        0      537 2023-04-20 03:03:39.032890 pdfathom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 pdfathom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-19 18:30:50.984373 pdfathom-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1333 2023-04-20 03:29:50.373801 pdfathom-0.1.1/README.md
+-rw-r--r--   0        0        0      249 2023-04-19 23:23:43.416419 pdfathom-0.1.1/pdfathom/__main__.py
+-rw-r--r--   0        0        0     1613 2023-04-20 15:52:32.065527 pdfathom-0.1.1/pdfathom/arguments.py
+-rw-r--r--   0        0        0      598 2023-04-20 15:52:32.059466 pdfathom-0.1.1/pdfathom/config.py
+-rw-r--r--   0        0        0     3069 2023-04-20 15:52:32.057086 pdfathom-0.1.1/pdfathom/db.py
+-rw-r--r--   0        0        0     3849 2023-04-20 15:52:32.075357 pdfathom-0.1.1/pdfathom/repl.py
+-rw-r--r--   0        0        0      536 2023-04-20 16:05:22.312659 pdfathom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 pdfathom-0.1.1/PKG-INFO
```

### Comparing `pdfathom-0.1.0/LICENSE` & `pdfathom-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/README.md` & `pdfathom-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/pdfathom/arguments.py` & `pdfathom-0.1.1/pdfathom/arguments.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/pdfathom/config.py` & `pdfathom-0.1.1/pdfathom/config.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/pdfathom/db.py` & `pdfathom-0.1.1/pdfathom/db.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/pdfathom/repl.py` & `pdfathom-0.1.1/pdfathom/repl.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.0/pyproject.toml` & `pdfathom-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pdfathom"
-version = "0.1.0"
+version = "0.1.1"
 description = "Query PDFs in natural language from the command-line"
 authors = ["Liam <liam@scalzulli.com>"]
 license = "CC0-1.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 chromadb = "^0.3.21"
 langchain = "^0.0.144"
 openai = "^0.27.4"
 pypdf = "^3.8.0"
-python = "^3.10"
+python = "^3.8"
 rich = "^13.3.4"
 tiktoken = "^0.3.3"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 toml = "^0.10.2"
 yapf = "^0.33.0"
```

### Comparing `pdfathom-0.1.0/PKG-INFO` & `pdfathom-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pdfathom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Query PDFs in natural language from the command-line
 License: CC0-1.0
 Author: Liam
 Author-email: liam@scalzulli.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.21,<0.4.0)
 Requires-Dist: langchain (>=0.0.144,<0.0.145)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pypdf (>=3.8.0,<4.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
```

