# Comparing `tmp/pdf.tocgen-1.3.0.tar.gz` & `tmp/pdf_tocgen-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf.tocgen-1.3.0.tar", last modified: Wed Nov 10 19:49:24 2021, max compression
+gzip compressed data, was "pdf_tocgen-1.3.1.tar", max compression
```

## Comparing `pdf.tocgen-1.3.0.tar` & `pdf_tocgen-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf.tocgen-1.3.0/LICENSE
--rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf.tocgen-1.3.0/LICENSE_AGPL
--rw-r--r--   0        0        0    13650 2021-05-09 08:08:57.010536 pdf.tocgen-1.3.0/README.md
--rw-r--r--   0        0        0      227 2021-01-12 05:43:12.956399 pdf.tocgen-1.3.0/fitzutils/__init__.py
--rw-r--r--   0        0        0     2565 2021-01-12 05:43:12.956399 pdf.tocgen-1.3.0/fitzutils/fitzutils.py
--rw-r--r--   0        0        0       87 2021-11-10 19:36:42.663214 pdf.tocgen-1.3.0/pdftocgen/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf.tocgen-1.3.0/pdftocgen/__main__.py
--rw-r--r--   0        0        0     4665 2021-11-10 10:52:45.466560 pdf.tocgen-1.3.0/pdftocgen/app.py
--rw-r--r--   0        0        0     5395 2021-11-10 10:51:01.789897 pdf.tocgen-1.3.0/pdftocgen/filter.py
--rw-r--r--   0        0        0     4963 2021-11-10 19:31:24.999892 pdf.tocgen-1.3.0/pdftocgen/recipe.py
--rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf.tocgen-1.3.0/pdftocgen/tocgen.py
--rw-r--r--   0        0        0       73 2021-11-10 19:36:47.946547 pdf.tocgen-1.3.0/pdftocio/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf.tocgen-1.3.0/pdftocio/__main__.py
--rw-r--r--   0        0        0     5320 2021-11-10 10:53:35.866558 pdf.tocgen-1.3.0/pdftocio/app.py
--rw-r--r--   0        0        0      481 2021-01-12 05:43:12.959732 pdf.tocgen-1.3.0/pdftocio/tocio.py
--rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf.tocgen-1.3.0/pdftocio/tocparser.py
--rw-r--r--   0        0        0      148 2021-11-10 19:36:53.809880 pdf.tocgen-1.3.0/pdfxmeta/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf.tocgen-1.3.0/pdfxmeta/__main__.py
--rw-r--r--   0        0        0     4107 2021-11-10 19:30:44.153227 pdf.tocgen-1.3.0/pdfxmeta/app.py
--rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf.tocgen-1.3.0/pdfxmeta/pdfxmeta.py
--rw-r--r--   0        0        0      947 2021-11-10 19:38:09.743211 pdf.tocgen-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    15082 2021-11-10 19:49:24.832852 pdf.tocgen-1.3.0/setup.py
--rw-r--r--   0        0        0    14506 2021-11-10 19:49:24.833644 pdf.tocgen-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.1/LICENSE
+-rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.1/LICENSE_AGPL
+-rw-r--r--   0        0        0    13650 2021-05-09 08:08:57.010536 pdf_tocgen-1.3.1/README.md
+-rw-r--r--   0        0        0      274 2023-04-20 06:06:03.536966 pdf_tocgen-1.3.1/fitzutils/__init__.py
+-rw-r--r--   0        0        0     2875 2023-04-20 06:05:46.873633 pdf_tocgen-1.3.1/fitzutils/fitzutils.py
+-rw-r--r--   0        0        0       87 2023-04-20 06:08:26.133627 pdf_tocgen-1.3.1/pdftocgen/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocgen/__main__.py
+-rw-r--r--   0        0        0     4880 2023-04-20 06:15:48.496945 pdf_tocgen-1.3.1/pdftocgen/app.py
+-rw-r--r--   0        0        0     5395 2021-11-10 10:51:01.789897 pdf_tocgen-1.3.1/pdftocgen/filter.py
+-rw-r--r--   0        0        0     4963 2021-11-10 19:31:24.999892 pdf_tocgen-1.3.1/pdftocgen/recipe.py
+-rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocgen/tocgen.py
+-rw-r--r--   0        0        0       73 2023-04-20 06:08:05.546961 pdf_tocgen-1.3.1/pdftocio/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocio/__main__.py
+-rw-r--r--   0        0        0     5563 2023-04-20 06:18:07.596940 pdf_tocgen-1.3.1/pdftocio/app.py
+-rw-r--r--   0        0        0      481 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdftocio/tocio.py
+-rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf_tocgen-1.3.1/pdftocio/tocparser.py
+-rw-r--r--   0        0        0      148 2023-04-20 06:08:00.250295 pdf_tocgen-1.3.1/pdfxmeta/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.1/pdfxmeta/__main__.py
+-rw-r--r--   0        0        0     4212 2023-04-20 06:10:42.420289 pdf_tocgen-1.3.1/pdfxmeta/app.py
+-rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf_tocgen-1.3.1/pdfxmeta/pdfxmeta.py
+-rw-r--r--   0        0        0      966 2023-04-20 06:03:36.103638 pdf_tocgen-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    14648 1970-01-01 00:00:00.000000 pdf_tocgen-1.3.1/PKG-INFO
```

### Comparing `pdf.tocgen-1.3.0/LICENSE` & `pdf_tocgen-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/LICENSE_AGPL` & `pdf_tocgen-1.3.1/LICENSE_AGPL`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/README.md` & `pdf_tocgen-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/fitzutils/fitzutils.py` & `pdf_tocgen-1.3.1/fitzutils/fitzutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, ContextManager, List, Tuple
 from fitz import Document
 
 import sys
 import fitz
 import io
 import csv
+import chardet
 
 
 @contextmanager
 def open_pdf(path: str,
              exit_on_error: bool = True
              ) -> ContextManager[Optional[Document]]:
     """A context manager for fitz Document
@@ -88,7 +89,23 @@
     Returns
       a multiline string
     """
     return '\n'.join([
         f"{(entry.level - 1) * '    '}{entry.title} ··· {entry.pagenum}"
         for entry in entries
     ])
+
+
+def get_file_encoding(path: str) -> str:
+    """Get encoding of file
+
+    Argument
+      path: file path
+    Returns
+      encoding string
+    """
+    try:
+        with open(path, "rb") as f:
+            enc = chardet.detect(f.read()).encoding
+    except:
+        enc = 'utf-8'
+    return enc
```

### Comparing `pdf.tocgen-1.3.0/pdftocgen/app.py` & `pdf_tocgen-1.3.1/pdftocgen/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """The executable of pdftocgen"""
 
 import toml
 import sys
 import getopt
 import pdftocgen
+import io
 
 from getopt import GetoptError
 from typing import TextIO
-from fitzutils import open_pdf, dump_toc, pprint_toc
+from fitzutils import open_pdf, dump_toc, pprint_toc, get_file_encoding
 from .tocgen import gen_toc
 
 usage_s = """
 usage: pdftocgen [options] doc.pdf < recipe.toml
 """.strip()
 
 help_s = """
@@ -85,35 +86,35 @@
             ["help", "recipe=", "human-readable", "vpos", "out=", "debug", "version"]
         )
     except GetoptError as e:
         print(e, file=sys.stderr)
         print(usage_s, file=sys.stderr)
         sys.exit(2)
 
-    recipe_file: TextIO = sys.stdin
+    recipe_file: TextIO = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8', errors='ignore')
     readable: bool = False
     vpos: bool = False
-    out: TextIO = sys.stdout
+    out: TextIO = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8', errors='ignore')
     debug: bool = False
 
     for o, a in opts:
         if o in ("-H", "--human-readable"):
             readable = True
         elif o in ("-v", "--vpos"):
             vpos = True
         elif o in ("-r", "--recipe"):
             try:
-                recipe_file = open(a, "r")
+                recipe_file = open(a, "r", encoding=get_file_encoding(a))
             except IOError as e:
                 print("error: can't open file for reading", file=sys.stderr)
                 print(e, file=sys.stderr)
                 sys.exit(1)
         elif o in ("-o", "--out"):
             try:
-                out = open(a, "w")
+                out = open(a, "w", encoding='utf-8', errors='ignore')
             except IOError as e:
                 print("error: can't open file for writing", file=sys.stderr)
                 print(e, file=sys.stderr)
                 sys.exit(1)
         elif o in ("-g", "--debug"):
             debug = True
         elif o in ("-V", "--version"):
```

### Comparing `pdf.tocgen-1.3.0/pdftocgen/filter.py` & `pdf_tocgen-1.3.1/pdftocgen/filter.py`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/pdftocgen/recipe.py` & `pdf_tocgen-1.3.1/pdftocgen/recipe.py`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/pdftocio/app.py` & `pdf_tocgen-1.3.1/pdftocio/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """The executable of pdftocio"""
 
 import sys
 import os.path
 import pdftocio
 import getopt
+import io
 
 from typing import Optional, TextIO
 from getopt import GetoptError
-from fitzutils import open_pdf, dump_toc, pprint_toc
+from fitzutils import open_pdf, dump_toc, pprint_toc, get_file_encoding
 from .tocparser import parse_toc
 from .tocio import write_toc, read_toc
 
 usage_s = """
 usage: pdftocio [options] in.pdf < toc
        pdftocio [options] in.pdf
 """.strip()
@@ -87,28 +88,28 @@
             ["help", "toc=", "print", "human-readable", "out=", "debug", "version"]
         )
     except GetoptError as e:
         print(e, file=sys.stderr)
         print(usage_s, file=sys.stderr)
         sys.exit(2)
 
-    toc_file: TextIO = sys.stdin
+    toc_file: TextIO = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8', errors='ignore')
     print_toc: bool = False
     readable: bool = False
     out: Optional[str] = None
     debug: bool = False
 
     for o, a in opts:
         if o in ("-H", "--human-readable"):
             readable = True
         elif o in ("-p", "--print"):
             print_toc = True
         elif o in ("-t", "--toc"):
             try:
-                toc_file = open(a, "r")
+                toc_file = open(a, "r", encoding=get_file_encoding(a))
             except IOError as e:
                 print("error: can't open file for reading", file=sys.stderr)
                 print(e, file=sys.stderr)
                 sys.exit(1)
         elif o in ("-o", "--out"):
             out = a
         elif o in ("-g", "--debug"):
@@ -134,18 +135,20 @@
                 # no input from user, switch to output mode and extract the toc
                 # of pdf
                 toc = read_toc(doc)
                 if len(toc) == 0:
                     print("error: no table of contents found", file=sys.stderr)
                     sys.exit(1)
 
+                stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8', errors='ignore')
+
                 if readable:
-                    print(pprint_toc(toc))
+                    print(pprint_toc(toc), file=stdout)
                 else:
-                    print(dump_toc(toc), end="")
+                    print(dump_toc(toc), end="", file=stdout)
                 sys.exit(0)
 
             # an input is given, so switch to input mode
             toc = parse_toc(toc_file)
             write_toc(doc, toc)
 
             if out is None:
```

### Comparing `pdf.tocgen-1.3.0/pdftocio/tocparser.py` & `pdf_tocgen-1.3.1/pdftocio/tocparser.py`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/pdfxmeta/app.py` & `pdf_tocgen-1.3.1/pdfxmeta/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The executable of pdfxmeta"""
 
 import getopt
 import sys
 import pdfxmeta
+import io
 
 from getopt import GetoptError
 from typing import Optional, TextIO
 from fitzutils import open_pdf
 from textwrap import indent
 from pdfxmeta import dump_meta, dump_toml, extract_meta
 
@@ -78,26 +79,26 @@
         print(e, file=sys.stderr)
         print(usage_s, file=sys.stderr)
         sys.exit(2)
 
     ignore_case: bool = False
     page: Optional[int] = None
     auto_level: Optional[int] = None
-    out: TextIO = sys.stdout
+    out: TextIO = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8', errors='ignore')
 
     for o, a in opts:
         if o in ("-i", "--ignore-case"):
             ignore_case = True
         elif o in ("-p", "--page"):
             page = int(a)
         elif o in ("-a", "--auto"):
             auto_level = int(a)
         elif o in ("-o", "--out"):
             try:
-                out = open(a, "w")
+                out = open(a, "w", encoding='utf-8', errors='ignore')
             except IOError as e:
                 print("error: can't open file for writing", file=sys.stderr)
                 print(e, file=sys.stderr)
                 sys.exit(1)
         elif o in ("-V", "--version"):
             print("pdfxmeta", pdfxmeta.__version__, file=sys.stderr)
             sys.exit()
```

### Comparing `pdf.tocgen-1.3.0/pdfxmeta/pdfxmeta.py` & `pdf_tocgen-1.3.1/pdfxmeta/pdfxmeta.py`

 * *Files identical despite different names*

### Comparing `pdf.tocgen-1.3.0/pyproject.toml` & `pdf_tocgen-1.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf.tocgen"
-version = "1.3.0"
+version = "1.3.1"
 description = "Automatically generate table of contents for pdf files"
 authors = ["krasjet"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://krasjet.com/voice/pdf.tocgen/"
 repository = "https://github.com/Krasjet/pdf.tocgen"
 keywords = ["pdf", "cli"]
@@ -22,14 +22,15 @@
   { include = "fitzutils" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 PyMuPDF = "^1.18.14"
 toml = "^0.10.2"
+chardet = "^5.1.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.5.3"
 jedi = "^0.17.2"
 mamba = "^0.11.1"
 
 [tool.poetry.scripts]
```

### Comparing `pdf.tocgen-1.3.0/setup.py` & `pdf_tocgen-1.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,524 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pdf-tocgen
+Version: 1.3.1
+Summary: Automatically generate table of contents for pdf files
+Home-page: https://krasjet.com/voice/pdf.tocgen/
+License: GPL-3.0-or-later
+Keywords: pdf,cli
+Author: krasjet
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyMuPDF (>=1.18.14,<2.0.0)
+Requires-Dist: chardet (>=5.1.0,<6.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/Krasjet/pdf.tocgen
+Description-Content-Type: text/markdown
 
-packages = \
-['fitzutils', 'pdftocgen', 'pdftocio', 'pdfxmeta']
+[pdf.tocgen][tocgen]
+==========
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/pdf.tocgen)](https://pypi.org/project/pdf.tocgen/)
+[![build](https://github.com/Krasjet/pdf.tocgen/workflows/build/badge.svg?branch=master)](https://github.com/Krasjet/pdf.tocgen/actions?query=workflow%3Abuild)
 
-install_requires = \
-['PyMuPDF>=1.18.14,<2.0.0', 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['pdftocgen = pdftocgen.app:main',
-                     'pdftocio = pdftocio.app:main',
-                     'pdfxmeta = pdfxmeta.app:main']}
-
-setup_kwargs = {
-    'name': 'pdf.tocgen',
-    'version': '1.3.0',
-    'description': 'Automatically generate table of contents for pdf files',
-    'long_description': '[pdf.tocgen][tocgen]\n==========\n\n[![PyPI](https://img.shields.io/pypi/v/pdf.tocgen)](https://pypi.org/project/pdf.tocgen/)\n[![build](https://github.com/Krasjet/pdf.tocgen/workflows/build/badge.svg?branch=master)](https://github.com/Krasjet/pdf.tocgen/actions?query=workflow%3Abuild)\n\n```\n                          in.pdf\n                            |\n                            |\n     +----------------------+--------------------+\n     |                      |                    |\n     V                      V                    V\n+----------+          +-----------+         +----------+\n|          |  recipe  |           |   ToC   |          |\n| pdfxmeta +--------->| pdftocgen +-------->| pdftocio +---> out.pdf\n|          |          |           |         |          |\n+----------+          +-----------+         +----------+\n```\n\n[pdf.tocgen][tocgen] is a set of command-line tools for automatically\nextracting and generating the table of contents (ToC) of a PDF file. It uses\nthe embedded font attributes and position of headings to deduce the basic\noutline of a PDF file.\n\nIt works best for PDF files produces from a TeX document using `pdftex` (and\nits friends `pdflatex`, `pdfxetex`, etc.), but it\'s designed to work with any\n**software-generated** PDF files (i.e. you shouldn\'t expect it to work with\nscanned PDFs). Some examples include `troff`/`groff`, Adobe InDesign, Microsoft\nWord, and probably more.\n\nPlease see the [**homepage**][tocgen] for a detailed introduction.\n\nInstallation\n------------\n\npdf.tocgen is written in Python 3. It is known to work with Python 3.7 to 3.9\non Linux, Windows, and macOS (On BSDs, you probably need to build PyMuPDF\nyourself). Use\n\n```sh\n$ pip install -U pdf.tocgen\n```\nto install the latest version systemwide. Alternatively, use [pipx][pipx] or\n\n```sh\n$ pip install -U --user pdf.tocgen\n```\nto install it for the current user. I would recommend the latter approach to\navoid messing up the package manager on your system.\n\nIf you are using an Arch-based Linux distro, the package is also available on\n[AUR][aur]. It can be installed using any AUR helper, for example [`yay`][yay]:\n\n```{.console .codein}\n$ yay -S pdf.tocgen\n```\n\n[pipx]: https://pipxproject.github.io/pipx/\n[aur]: https://aur.archlinux.org/packages/pdf.tocgen/\n[yay]: https://github.com/Jguer/yay\n\nWorkflow\n--------\n\nThe design of pdf.tocgen is influenced by the [Unix philosophy][unix]. I\nintentionally separated pdf.tocgen to 3 separate programs. They work together,\nbut each of them is useful on their own.\n\n1. `pdfxmeta`: extract the metadata (font attributes, positions) of headings to\n    build a **recipe** file.\n2. `pdftocgen`: generate a table of contents from the recipe.\n3. `pdftocio`: import the table of contents to the PDF document.\n\nYou should read [the example][ex] on the homepage for a proper introduction,\nbut the basic workflow follows like this.\n\nFirst, use `pdfxmeta` to search for the metadata of headings, and generate\n**heading filters** using the automatic setting\n\n```sh\n$ pdfxmeta -p page -a 1 in.pdf "Section" >> recipe.toml\n$ pdfxmeta -p page -a 2 in.pdf "Subsection" >> recipe.toml\n```\nThe output `recipe.toml` file would contain several heading filters, each of\nwhich specifies the attribute of a heading at a particular level should have.\n\nAn example recipe file would look like this:\n\n```toml\n[[heading]]\nlevel = 1\ngreedy = true\nfont.name = "Times-Bold"\nfont.size = 19.92530059814453\n\n[[heading]]\nlevel = 2\ngreedy = true\nfont.name = "Times-Bold"\nfont.size = 11.9552001953125\n```\n\nThen pass the recipe to `pdftocgen` to generate a table of contents,\n\n```console\n$ pdftocgen in.pdf < recipe.toml\n"Preface" 5\n    "Bottom-up Design" 5\n    "Plan of the Book" 7\n    "Examples" 9\n    "Acknowledgements" 9\n"Contents" 11\n"The Extensible Language" 14\n    "1.1 Design by Evolution" 14\n    "1.2 Programming Bottom-Up" 16\n    "1.3 Extensible Software" 18\n    "1.4 Extending Lisp" 19\n    "1.5 Why Lisp (or When)" 21\n"Functions" 22\n    "2.1 Functions as Data" 22\n    "2.2 Defining Functions" 23\n    "2.3 Functional Arguments" 26\n    "2.4 Functions as Properties" 28\n    "2.5 Scope" 29\n    "2.6 Closures" 30\n    "2.7 Local Functions" 34\n    "2.8 Tail-Recursion" 35\n    "2.9 Compilation" 37\n    "2.10 Functions from Lists" 40\n"Functional Programming" 41\n    "3.1 Functional Design" 41\n    "3.2 Imperative Outside-In" 46\n    "3.3 Functional Interfaces" 48\n    "3.4 Interactive Programming" 50\n[--snip--]\n```\nwhich can be directly imported to the PDF file using `pdftocio`,\n\n```sh\n$ pdftocgen in.pdf < recipe.toml | pdftocio -o out.pdf in.pdf\n```\n\nOr if you want to edit the table of contents before importing it,\n\n```sh\n$ pdftocgen in.pdf < recipe.toml > toc\n$ vim toc # edit\n$ pdftocio in.pdf < toc\n```\n\nEach of the three programs has some extra functionalities. Use the `-h` option\nto see all the options you could pass in.\n\nCommand examples\n----------------\n\nBecause of the modularity of design, each program is useful on its own, despite\nbeing part of the pipeline. This section will provide some more examples on how\nyou could use them. Feel free to come up with more.\n\n### `pdftocio`\n\n`pdftocio` should best demonstrate this point, this program can do a lot on its\nown.\n\nTo display existing table of contents in a PDF to `stdout`:\n\n```console\n$ pdftocio doc.pdf\n"Level 1 heading 1" 1\n    "Level 2 heading 1" 1\n        "Level 3 heading 1" 2\n        "Level 3 heading 2" 3\n    "Level 2 heading 2" 4\n"Level 1 heading 2" 5\n```\n\nTo write existing table of contents in a PDF to a file named `toc`:\n\n```console\n$ pdftocio doc.pdf > toc\n```\n\nTo write a `toc` file back to `doc.pdf`:\n\n```console\n$ pdftocio doc.pdf < toc\n```\n\nTo specify the name of output PDF:\n\n```console\n$ pdftocio -o out.pdf doc.pdf < toc\n```\n\nTo copy the table of contents from `doc1.pdf` to `doc2.pdf`:\n\n```console\n$ pdftocio doc1.pdf | pdftocio doc2.pdf\n```\n\nTo print the table of contents for reading:\n\n```console\n$ pdftocio -H doc.pdf\nLevel 1 heading 1 ··· 1\n    Level 2 heading 1 ··· 1\n        Level 3 heading 1 ··· 2\n        Level 3 heading 2 ··· 3\n    Level 2 heading 2 ··· 4\nLevel 1 heading 2 ··· 5\n```\n\n### `pdftocgen`\n\nIf you have obtained an existing recipe `rcp.toml` for `doc.pdf`, you could\napply it and print the outline to `stdout` by\n\n```console\n$ pdftocio doc.pdf < rcp.toml\n"Level 1 heading 1" 1\n    "Level 2 heading 1" 1\n        "Level 3 heading 1" 2\n        "Level 3 heading 2" 3\n    "Level 2 heading 2" 4\n"Level 1 heading 2" 5\n```\n\nTo output the table of contents to a file called `toc`:\n\n```console\n$ pdftocgen doc.pdf < rcp.toml > toc\n```\n\nTo import the generated table of contents to the PDF file, and output\nto `doc_out.pdf`:\n\n```console\n$ pdftocgen doc.pdf < rcp.toml | pdftocio -o doc_out.pdf doc.pdf\n```\n\nTo print the generated table of contents for reading:\n\n```console\n$ pdftocgen -H doc.pdf < rcp.toml\nLevel 1 heading 1 ··· 1\n    Level 2 heading 1 ··· 1\n        Level 3 heading 1 ··· 2\n        Level 3 heading 2 ··· 3\n    Level 2 heading 2 ··· 4\nLevel 1 heading 2 ··· 5\n```\n\nIf you want to include the vertical position in a page for each heading, use the\n`-v` flag\n\n```console\n$ pdftocgen -v doc.pdf < rcp.toml\n"Level 1 heading 1" 1 306.947998046875\n    "Level 2 heading 1" 1 586.3488159179688\n        "Level 3 heading 1" 2 586.5888061523438\n        "Level 3 heading 2" 3 155.66879272460938\n    "Level 2 heading 2" 4 435.8687744140625\n"Level 1 heading 2" 5 380.78875732421875\n```\n\n`pdftocio` can understand the vertical position in the output to generate table\nof contents entries that link to the exact position of the heading, instead of\nthe top of the page.\n\n```console\n$ pdftocgen -v doc.pdf < rcp.toml | pdftocio doc.pdf\n```\n\nNote that the default output of `pdftocio` here is `doc_out.pdf`.\n\n### `pdfxmeta`\n\nTo search for `Anaphoric` in the entire PDF:\n\n```console\n$ pdfxmeta onlisp.pdf "Anaphoric"\n14. Anaphoric Macros:\n    font.name = "Times-Bold"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = true\n    bbox.left = 308.6400146484375\n    bbox.top = 307.1490478515625\n    bbox.right = 404.33282470703125\n    bbox.bottom = 320.9472351074219\n[--snip--]\n```\n\nTo output the result as a heading filter with the automatic settings,\n\n```console\n$ pdfxmeta -a 1 onlisp.pdf "Anaphoric"\n[[heading]]\n# 14. Anaphoric Macros\nlevel = 1\ngreedy = true\nfont.name = "Times-Bold"\nfont.size = 9.962599754333496\n# font.size_tolerance = 1e-5\n# font.color = 0x000000\n# font.superscript = false\n# font.italic = false\n# font.serif = true\n# font.monospace = false\n# font.bold = true\n# bbox.left = 308.6400146484375\n# bbox.top = 307.1490478515625\n# bbox.right = 404.33282470703125\n# bbox.bottom = 320.9472351074219\n# bbox.tolerance = 1e-5\n[--snip--]\n```\nwhich can be directly write to a recipe file:\n\n```console\n$ pdfxmeta -a 1 onlisp.pdf "Anaphoric" >> recipe.toml\n```\n\nTo case-insensitive search for `Anaphoric` in the entire PDF:\n\n```console\n$ pdfxmeta -i onlisp.pdf "Anaphoric"\nto compile-time. Chapter 14 introduces anaphoric macros, which allow you to:\n    font.name = "Times-Roman"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = false\n    bbox.left = 138.60000610351562\n    bbox.top = 295.6583557128906\n    bbox.right = 459.0260009765625\n    bbox.bottom = 308.948486328125\n[--snip--]\n```\n\nUse regular expression to case-insensitive search search for `Anaphoric` in the\nentire PDF:\n\n```console\n$ pdfxmeta onlisp.pdf "[Aa]naphoric"\nto compile-time. Chapter 14 introduces anaphoric macros, which allow you to:\n    font.name = "Times-Roman"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = false\n    bbox.left = 138.60000610351562\n    bbox.top = 295.6583557128906\n    bbox.right = 459.0260009765625\n    bbox.bottom = 308.948486328125\n[--snip--]\n```\n\nTo search only on page 203:\n\n```console\n$ pdfxmeta -p 203 onlisp.pdf "anaphoric"\nanaphoric if, called:\n    font.name = "Times-Roman"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = false\n    bbox.left = 138.60000610351562\n    bbox.top = 283.17822265625\n    bbox.right = 214.81094360351562\n    bbox.bottom = 296.4683532714844\n[--snip--]\n```\n\nTo dump the entire page of 203:\n\n```console\n$ pdfxmeta -p 203 onlisp.pdf\n190:\n    font.name = "Times-Roman"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = false\n    bbox.left = 138.60000610351562\n    bbox.top = 126.09941101074219\n    bbox.right = 153.54388427734375\n    bbox.bottom = 139.38951110839844\n[--snip--]\n```\n\nTo dump the entire PDF document:\n\n```console\n$ pdfxmeta onlisp.pdf\ni:\n    font.name = "Times-Roman"\n    font.size = 9.962599754333496\n    font.color = 0x000000\n    font.superscript = false\n    font.italic = false\n    font.serif = true\n    font.monospace = false\n    font.bold = false\n    bbox.left = 458.0400085449219\n    bbox.top = 126.09941101074219\n    bbox.right = 460.8096008300781\n    bbox.bottom = 139.38951110839844\n[--snip--]\n```\n\nDevelopment\n-----------\n\nIf you want to modify the source code or contribute anything, first install\n[`poetry`][poetry], which is a dependency and package manager for Python used\nby pdf.tocgen. Then run\n\n```sh\n$ poetry install\n```\nin the root directory of this repository to set up development dependencies.\n\nIf you want to test the development version of pdf.tocgen, use the `poetry run` command:\n\n```sh\n$ poetry run pdfxmeta in.pdf "pattern"\n```\nAlternatively, you could also use the\n\n```sh\n$ poetry shell\n```\ncommand to open up a virtual environment and run the development version\ndirectly:\n\n```sh\n(pdf.tocgen) $ pdfxmeta in.pdf "pattern"\n```\n\nBefore you send a patch or pull request, make sure the unit test passes by\nrunning:\n\n```sh\n$ make test\n```\n\nGUI front end\n-------------\n\nIf you are a Emacs user, you could install Daniel Nicolai\'s [toc-mode][tocmode]\npackage as a GUI front end for pdf.tocgen, though it offers many more\nfunctionalities, such as extracting (printed) table of contents from a PDF\nfile. Note that it uses pdf.tocgen under the hood, so you still need to install\npdf.tocgen before using toc-mode as a front end for pdf.tocgen.\n\nLicense\n-------\n\npdf.tocgen itself a is free software. The source code of pdf.tocgen is licensed\nunder the GNU GPLv3 license. However, the recipes in the `recipes` directory is\nseparately licensed under the [CC BY-NC-SA 4.0 License][cc] to prevent any\ncommercial usage, and thus not included in the distribution.\n\npdf.tocgen is based on [PyMuPDF][pymupdf], licensed under the GNU GPLv3\nlicense, which is again based on [MuPDF][mupdf], licensed under the GNU AGPLv3\nlicense. A copy of the AGPLv3 license is included in the repository.\n\nIf you want to make any derivatives based on this project, please follow the\nterms of the GNU GPLv3 license.\n\n[tocgen]: https://krasjet.com/voice/pdf.tocgen/\n[unix]: https://en.wikipedia.org/wiki/Unix_philosophy\n[ex]: https://krasjet.com/voice/pdf.tocgen/#a-worked-example\n[poetry]: https://python-poetry.org/\n[pymupdf]: https://github.com/pymupdf/PyMuPDF\n[mupdf]: https://mupdf.com/docs/index.html\n[cc]: https://creativecommons.org/licenses/by-nc-sa/4.0/\n[tocmode]: https://github.com/dalanicolai/toc-mode\n',
-    'author': 'krasjet',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://krasjet.com/voice/pdf.tocgen/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+```
+                          in.pdf
+                            |
+                            |
+     +----------------------+--------------------+
+     |                      |                    |
+     V                      V                    V
++----------+          +-----------+         +----------+
+|          |  recipe  |           |   ToC   |          |
+| pdfxmeta +--------->| pdftocgen +-------->| pdftocio +---> out.pdf
+|          |          |           |         |          |
++----------+          +-----------+         +----------+
+```
 
+[pdf.tocgen][tocgen] is a set of command-line tools for automatically
+extracting and generating the table of contents (ToC) of a PDF file. It uses
+the embedded font attributes and position of headings to deduce the basic
+outline of a PDF file.
+
+It works best for PDF files produces from a TeX document using `pdftex` (and
+its friends `pdflatex`, `pdfxetex`, etc.), but it's designed to work with any
+**software-generated** PDF files (i.e. you shouldn't expect it to work with
+scanned PDFs). Some examples include `troff`/`groff`, Adobe InDesign, Microsoft
+Word, and probably more.
+
+Please see the [**homepage**][tocgen] for a detailed introduction.
+
+Installation
+------------
+
+pdf.tocgen is written in Python 3. It is known to work with Python 3.7 to 3.9
+on Linux, Windows, and macOS (On BSDs, you probably need to build PyMuPDF
+yourself). Use
+
+```sh
+$ pip install -U pdf.tocgen
+```
+to install the latest version systemwide. Alternatively, use [pipx][pipx] or
+
+```sh
+$ pip install -U --user pdf.tocgen
+```
+to install it for the current user. I would recommend the latter approach to
+avoid messing up the package manager on your system.
+
+If you are using an Arch-based Linux distro, the package is also available on
+[AUR][aur]. It can be installed using any AUR helper, for example [`yay`][yay]:
+
+```{.console .codein}
+$ yay -S pdf.tocgen
+```
+
+[pipx]: https://pipxproject.github.io/pipx/
+[aur]: https://aur.archlinux.org/packages/pdf.tocgen/
+[yay]: https://github.com/Jguer/yay
+
+Workflow
+--------
+
+The design of pdf.tocgen is influenced by the [Unix philosophy][unix]. I
+intentionally separated pdf.tocgen to 3 separate programs. They work together,
+but each of them is useful on their own.
+
+1. `pdfxmeta`: extract the metadata (font attributes, positions) of headings to
+    build a **recipe** file.
+2. `pdftocgen`: generate a table of contents from the recipe.
+3. `pdftocio`: import the table of contents to the PDF document.
+
+You should read [the example][ex] on the homepage for a proper introduction,
+but the basic workflow follows like this.
+
+First, use `pdfxmeta` to search for the metadata of headings, and generate
+**heading filters** using the automatic setting
+
+```sh
+$ pdfxmeta -p page -a 1 in.pdf "Section" >> recipe.toml
+$ pdfxmeta -p page -a 2 in.pdf "Subsection" >> recipe.toml
+```
+The output `recipe.toml` file would contain several heading filters, each of
+which specifies the attribute of a heading at a particular level should have.
+
+An example recipe file would look like this:
+
+```toml
+[[heading]]
+level = 1
+greedy = true
+font.name = "Times-Bold"
+font.size = 19.92530059814453
+
+[[heading]]
+level = 2
+greedy = true
+font.name = "Times-Bold"
+font.size = 11.9552001953125
+```
+
+Then pass the recipe to `pdftocgen` to generate a table of contents,
+
+```console
+$ pdftocgen in.pdf < recipe.toml
+"Preface" 5
+    "Bottom-up Design" 5
+    "Plan of the Book" 7
+    "Examples" 9
+    "Acknowledgements" 9
+"Contents" 11
+"The Extensible Language" 14
+    "1.1 Design by Evolution" 14
+    "1.2 Programming Bottom-Up" 16
+    "1.3 Extensible Software" 18
+    "1.4 Extending Lisp" 19
+    "1.5 Why Lisp (or When)" 21
+"Functions" 22
+    "2.1 Functions as Data" 22
+    "2.2 Defining Functions" 23
+    "2.3 Functional Arguments" 26
+    "2.4 Functions as Properties" 28
+    "2.5 Scope" 29
+    "2.6 Closures" 30
+    "2.7 Local Functions" 34
+    "2.8 Tail-Recursion" 35
+    "2.9 Compilation" 37
+    "2.10 Functions from Lists" 40
+"Functional Programming" 41
+    "3.1 Functional Design" 41
+    "3.2 Imperative Outside-In" 46
+    "3.3 Functional Interfaces" 48
+    "3.4 Interactive Programming" 50
+[--snip--]
+```
+which can be directly imported to the PDF file using `pdftocio`,
+
+```sh
+$ pdftocgen in.pdf < recipe.toml | pdftocio -o out.pdf in.pdf
+```
+
+Or if you want to edit the table of contents before importing it,
+
+```sh
+$ pdftocgen in.pdf < recipe.toml > toc
+$ vim toc # edit
+$ pdftocio in.pdf < toc
+```
+
+Each of the three programs has some extra functionalities. Use the `-h` option
+to see all the options you could pass in.
+
+Command examples
+----------------
+
+Because of the modularity of design, each program is useful on its own, despite
+being part of the pipeline. This section will provide some more examples on how
+you could use them. Feel free to come up with more.
+
+### `pdftocio`
+
+`pdftocio` should best demonstrate this point, this program can do a lot on its
+own.
+
+To display existing table of contents in a PDF to `stdout`:
+
+```console
+$ pdftocio doc.pdf
+"Level 1 heading 1" 1
+    "Level 2 heading 1" 1
+        "Level 3 heading 1" 2
+        "Level 3 heading 2" 3
+    "Level 2 heading 2" 4
+"Level 1 heading 2" 5
+```
+
+To write existing table of contents in a PDF to a file named `toc`:
+
+```console
+$ pdftocio doc.pdf > toc
+```
+
+To write a `toc` file back to `doc.pdf`:
+
+```console
+$ pdftocio doc.pdf < toc
+```
+
+To specify the name of output PDF:
+
+```console
+$ pdftocio -o out.pdf doc.pdf < toc
+```
+
+To copy the table of contents from `doc1.pdf` to `doc2.pdf`:
+
+```console
+$ pdftocio doc1.pdf | pdftocio doc2.pdf
+```
+
+To print the table of contents for reading:
+
+```console
+$ pdftocio -H doc.pdf
+Level 1 heading 1 ··· 1
+    Level 2 heading 1 ··· 1
+        Level 3 heading 1 ··· 2
+        Level 3 heading 2 ··· 3
+    Level 2 heading 2 ··· 4
+Level 1 heading 2 ··· 5
+```
+
+### `pdftocgen`
+
+If you have obtained an existing recipe `rcp.toml` for `doc.pdf`, you could
+apply it and print the outline to `stdout` by
+
+```console
+$ pdftocio doc.pdf < rcp.toml
+"Level 1 heading 1" 1
+    "Level 2 heading 1" 1
+        "Level 3 heading 1" 2
+        "Level 3 heading 2" 3
+    "Level 2 heading 2" 4
+"Level 1 heading 2" 5
+```
+
+To output the table of contents to a file called `toc`:
+
+```console
+$ pdftocgen doc.pdf < rcp.toml > toc
+```
+
+To import the generated table of contents to the PDF file, and output
+to `doc_out.pdf`:
+
+```console
+$ pdftocgen doc.pdf < rcp.toml | pdftocio -o doc_out.pdf doc.pdf
+```
+
+To print the generated table of contents for reading:
+
+```console
+$ pdftocgen -H doc.pdf < rcp.toml
+Level 1 heading 1 ··· 1
+    Level 2 heading 1 ··· 1
+        Level 3 heading 1 ··· 2
+        Level 3 heading 2 ··· 3
+    Level 2 heading 2 ··· 4
+Level 1 heading 2 ··· 5
+```
+
+If you want to include the vertical position in a page for each heading, use the
+`-v` flag
+
+```console
+$ pdftocgen -v doc.pdf < rcp.toml
+"Level 1 heading 1" 1 306.947998046875
+    "Level 2 heading 1" 1 586.3488159179688
+        "Level 3 heading 1" 2 586.5888061523438
+        "Level 3 heading 2" 3 155.66879272460938
+    "Level 2 heading 2" 4 435.8687744140625
+"Level 1 heading 2" 5 380.78875732421875
+```
+
+`pdftocio` can understand the vertical position in the output to generate table
+of contents entries that link to the exact position of the heading, instead of
+the top of the page.
+
+```console
+$ pdftocgen -v doc.pdf < rcp.toml | pdftocio doc.pdf
+```
+
+Note that the default output of `pdftocio` here is `doc_out.pdf`.
+
+### `pdfxmeta`
+
+To search for `Anaphoric` in the entire PDF:
+
+```console
+$ pdfxmeta onlisp.pdf "Anaphoric"
+14. Anaphoric Macros:
+    font.name = "Times-Bold"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = true
+    bbox.left = 308.6400146484375
+    bbox.top = 307.1490478515625
+    bbox.right = 404.33282470703125
+    bbox.bottom = 320.9472351074219
+[--snip--]
+```
+
+To output the result as a heading filter with the automatic settings,
+
+```console
+$ pdfxmeta -a 1 onlisp.pdf "Anaphoric"
+[[heading]]
+# 14. Anaphoric Macros
+level = 1
+greedy = true
+font.name = "Times-Bold"
+font.size = 9.962599754333496
+# font.size_tolerance = 1e-5
+# font.color = 0x000000
+# font.superscript = false
+# font.italic = false
+# font.serif = true
+# font.monospace = false
+# font.bold = true
+# bbox.left = 308.6400146484375
+# bbox.top = 307.1490478515625
+# bbox.right = 404.33282470703125
+# bbox.bottom = 320.9472351074219
+# bbox.tolerance = 1e-5
+[--snip--]
+```
+which can be directly write to a recipe file:
+
+```console
+$ pdfxmeta -a 1 onlisp.pdf "Anaphoric" >> recipe.toml
+```
+
+To case-insensitive search for `Anaphoric` in the entire PDF:
+
+```console
+$ pdfxmeta -i onlisp.pdf "Anaphoric"
+to compile-time. Chapter 14 introduces anaphoric macros, which allow you to:
+    font.name = "Times-Roman"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = false
+    bbox.left = 138.60000610351562
+    bbox.top = 295.6583557128906
+    bbox.right = 459.0260009765625
+    bbox.bottom = 308.948486328125
+[--snip--]
+```
+
+Use regular expression to case-insensitive search search for `Anaphoric` in the
+entire PDF:
+
+```console
+$ pdfxmeta onlisp.pdf "[Aa]naphoric"
+to compile-time. Chapter 14 introduces anaphoric macros, which allow you to:
+    font.name = "Times-Roman"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = false
+    bbox.left = 138.60000610351562
+    bbox.top = 295.6583557128906
+    bbox.right = 459.0260009765625
+    bbox.bottom = 308.948486328125
+[--snip--]
+```
+
+To search only on page 203:
+
+```console
+$ pdfxmeta -p 203 onlisp.pdf "anaphoric"
+anaphoric if, called:
+    font.name = "Times-Roman"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = false
+    bbox.left = 138.60000610351562
+    bbox.top = 283.17822265625
+    bbox.right = 214.81094360351562
+    bbox.bottom = 296.4683532714844
+[--snip--]
+```
+
+To dump the entire page of 203:
+
+```console
+$ pdfxmeta -p 203 onlisp.pdf
+190:
+    font.name = "Times-Roman"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = false
+    bbox.left = 138.60000610351562
+    bbox.top = 126.09941101074219
+    bbox.right = 153.54388427734375
+    bbox.bottom = 139.38951110839844
+[--snip--]
+```
+
+To dump the entire PDF document:
+
+```console
+$ pdfxmeta onlisp.pdf
+i:
+    font.name = "Times-Roman"
+    font.size = 9.962599754333496
+    font.color = 0x000000
+    font.superscript = false
+    font.italic = false
+    font.serif = true
+    font.monospace = false
+    font.bold = false
+    bbox.left = 458.0400085449219
+    bbox.top = 126.09941101074219
+    bbox.right = 460.8096008300781
+    bbox.bottom = 139.38951110839844
+[--snip--]
+```
+
+Development
+-----------
+
+If you want to modify the source code or contribute anything, first install
+[`poetry`][poetry], which is a dependency and package manager for Python used
+by pdf.tocgen. Then run
+
+```sh
+$ poetry install
+```
+in the root directory of this repository to set up development dependencies.
+
+If you want to test the development version of pdf.tocgen, use the `poetry run` command:
+
+```sh
+$ poetry run pdfxmeta in.pdf "pattern"
+```
+Alternatively, you could also use the
+
+```sh
+$ poetry shell
+```
+command to open up a virtual environment and run the development version
+directly:
+
+```sh
+(pdf.tocgen) $ pdfxmeta in.pdf "pattern"
+```
+
+Before you send a patch or pull request, make sure the unit test passes by
+running:
+
+```sh
+$ make test
+```
+
+GUI front end
+-------------
+
+If you are a Emacs user, you could install Daniel Nicolai's [toc-mode][tocmode]
+package as a GUI front end for pdf.tocgen, though it offers many more
+functionalities, such as extracting (printed) table of contents from a PDF
+file. Note that it uses pdf.tocgen under the hood, so you still need to install
+pdf.tocgen before using toc-mode as a front end for pdf.tocgen.
+
+License
+-------
+
+pdf.tocgen itself a is free software. The source code of pdf.tocgen is licensed
+under the GNU GPLv3 license. However, the recipes in the `recipes` directory is
+separately licensed under the [CC BY-NC-SA 4.0 License][cc] to prevent any
+commercial usage, and thus not included in the distribution.
+
+pdf.tocgen is based on [PyMuPDF][pymupdf], licensed under the GNU GPLv3
+license, which is again based on [MuPDF][mupdf], licensed under the GNU AGPLv3
+license. A copy of the AGPLv3 license is included in the repository.
+
+If you want to make any derivatives based on this project, please follow the
+terms of the GNU GPLv3 license.
+
+[tocgen]: https://krasjet.com/voice/pdf.tocgen/
+[unix]: https://en.wikipedia.org/wiki/Unix_philosophy
+[ex]: https://krasjet.com/voice/pdf.tocgen/#a-worked-example
+[poetry]: https://python-poetry.org/
+[pymupdf]: https://github.com/pymupdf/PyMuPDF
+[mupdf]: https://mupdf.com/docs/index.html
+[cc]: https://creativecommons.org/licenses/by-nc-sa/4.0/
+[tocmode]: https://github.com/dalanicolai/toc-mode
 
-setup(**setup_kwargs)
```

