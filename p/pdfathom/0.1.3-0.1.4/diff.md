# Comparing `tmp/pdfathom-0.1.3.tar.gz` & `tmp/pdfathom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfathom-0.1.3.tar", max compression
+gzip compressed data, was "pdfathom-0.1.4.tar", max compression
```

## Comparing `pdfathom-0.1.3.tar` & `pdfathom-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7048 2023-04-19 18:30:50.984373 pdfathom-0.1.3/LICENSE
--rw-r--r--   0        0        0     1333 2023-04-20 03:29:50.373801 pdfathom-0.1.3/README.md
--rw-r--r--   0        0        0      273 2023-04-20 16:25:02.676376 pdfathom-0.1.3/pdfathom/__main__.py
--rw-r--r--   0        0        0     1592 2023-04-20 16:24:58.587998 pdfathom-0.1.3/pdfathom/arguments.py
--rw-r--r--   0        0        0      598 2023-04-20 16:25:22.408923 pdfathom-0.1.3/pdfathom/config.py
--rw-r--r--   0        0        0     3069 2023-04-20 16:25:11.880571 pdfathom-0.1.3/pdfathom/db.py
--rw-r--r--   0        0        0     3850 2023-04-20 16:25:16.831240 pdfathom-0.1.3/pdfathom/repl.py
--rw-r--r--   0        0        0      595 2023-04-20 16:25:35.993457 pdfathom-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 pdfathom-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-19 18:30:50.984373 pdfathom-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1333 2023-04-20 03:29:50.373801 pdfathom-0.1.4/README.md
+-rw-r--r--   0        0        0      273 2023-04-20 16:25:53.664196 pdfathom-0.1.4/pdfathom/__main__.py
+-rw-r--r--   0        0        0     1592 2023-04-20 16:29:10.984342 pdfathom-0.1.4/pdfathom/arguments.py
+-rw-r--r--   0        0        0      598 2023-04-20 16:25:53.646933 pdfathom-0.1.4/pdfathom/config.py
+-rw-r--r--   0        0        0     3088 2023-04-20 16:28:56.951830 pdfathom-0.1.4/pdfathom/db.py
+-rw-r--r--   0        0        0     3851 2023-04-20 16:25:53.662819 pdfathom-0.1.4/pdfathom/repl.py
+-rw-r--r--   0        0        0      595 2023-04-20 16:29:43.591687 pdfathom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 pdfathom-0.1.4/PKG-INFO
```

### Comparing `pdfathom-0.1.3/LICENSE` & `pdfathom-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.3/README.md` & `pdfathom-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.3/pdfathom/arguments.py` & `pdfathom-0.1.4/pdfathom/arguments.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.3/pdfathom/config.py` & `pdfathom-0.1.4/pdfathom/config.py`

 * *Files identical despite different names*

### Comparing `pdfathom-0.1.3/pdfathom/db.py` & `pdfathom-0.1.4/pdfathom/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import Dict, List, Union
 from urllib.request import urlretrieve
 
 import chromadb
 from langchain.chains import RetrievalQA
 from langchain.chains.retrieval_qa.base import BaseRetrievalQA
 from langchain.document_loaders import PyPDFLoader
 from langchain.embeddings import OpenAIEmbeddings
@@ -36,20 +36,20 @@
     return self
 
   def documents(self) -> List[str]:
     """Get a list of PDFs."""
 
     return list(self.retrievers.keys())
 
-  def get_active_document(self) -> str | None:
+  def get_active_document(self) -> Union[str, None]:
     """Get the active PDF."""
 
     return self.active
 
-  def get_active_retriever(self) -> BaseRetrievalQA | None:
+  def get_active_retriever(self) -> Union[BaseRetrievalQA, None]:
     """Get the active retriever."""
 
     return None if not self.active else self.retrievers[self.active]
 
   def set_active_document(self, pdf_path: str) -> None:
     """Set the active PDF."""
```

### Comparing `pdfathom-0.1.3/pdfathom/repl.py` & `pdfathom-0.1.4/pdfathom/repl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import atexit
 import os
 import readline
 from dataclasses import dataclass
 from textwrap import dedent
 
-from .db import Db
 from rich import print
 from rich.prompt import Confirm
 
+from .db import Db
+
 @dataclass
 class Repl:
   HELP = dedent(
     '''
     Enter a query to search the active PDF document for relevant information.
 
     [bold]Available commands:[/bold]
```

### Comparing `pdfathom-0.1.3/pyproject.toml` & `pdfathom-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdfathom"
-version = "0.1.3"
+version = "0.1.4"
 description = "Query PDFs in natural language from the command-line"
 authors = ["Liam <liam@scalzulli.com>"]
 license = "CC0-1.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 chromadb = "^0.3.21"
```

### Comparing `pdfathom-0.1.3/PKG-INFO` & `pdfathom-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfathom
-Version: 0.1.3
+Version: 0.1.4
 Summary: Query PDFs in natural language from the command-line
 License: CC0-1.0
 Author: Liam
 Author-email: liam@scalzulli.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

