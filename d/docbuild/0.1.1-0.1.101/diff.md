# Comparing `tmp/docbuild-0.1.1.tar.gz` & `tmp/docbuild-0.1.101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.1.tar", last modified: Wed Apr 19 14:38:00 2023, max compression
+gzip compressed data, was "docbuild-0.1.101.tar", last modified: Thu Apr 20 11:06:47 2023, max compression
```

## Comparing `docbuild-0.1.1.tar` & `docbuild-0.1.101.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.504817 docbuild-0.1.1/
--rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 14:38:00.504651 docbuild-0.1.1/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.1/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.500513 docbuild-0.1.1/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-19 14:36:50.000000 docbuild-0.1.1/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      408 2023-04-19 09:10:09.000000 docbuild-0.1.1/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.1/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.1/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     6942 2023-04-19 09:11:18.000000 docbuild-0.1.1/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.503093 docbuild-0.1.1/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.1/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.1/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-19 06:25:05.000000 docbuild-0.1.1/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.1/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.1/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-19 06:25:19.000000 docbuild-0.1.1/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.1/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.504291 docbuild-0.1.1/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.1/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.1/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      158 2023-04-19 09:10:38.000000 docbuild-0.1.1/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16376 2023-04-19 09:12:11.000000 docbuild-0.1.1/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-19 14:38:00.501829 docbuild-0.1.1/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      564 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-19 14:38:00.000000 docbuild-0.1.1/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-19 14:38:00.504858 docbuild-0.1.1/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      830 2023-04-19 14:37:56.000000 docbuild-0.1.1/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.017799 docbuild-0.1.101/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-20 11:06:47.017466 docbuild-0.1.101/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.101/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.011799 docbuild-0.1.101/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-20 11:06:41.000000 docbuild-0.1.101/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.101/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.101/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.101/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7030 2023-04-20 11:06:00.000000 docbuild-0.1.101/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.014684 docbuild-0.1.101/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.101/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.101/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.101/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.101/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.101/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-19 06:25:19.000000 docbuild-0.1.101/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.101/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.016699 docbuild-0.1.101/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.101/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.101/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      158 2023-04-19 09:10:38.000000 docbuild-0.1.101/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16376 2023-04-19 09:12:11.000000 docbuild-0.1.101/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.013171 docbuild-0.1.101/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-20 11:06:47.017860 docbuild-0.1.101/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-20 11:06:30.000000 docbuild-0.1.101/setup.py
```

### Comparing `docbuild-0.1.1/PKG-INFO` & `docbuild-0.1.101/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.1
+Version: 0.1.101
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.1/docbuild/graph.py` & `docbuild-0.1.101/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/hocr_parser.py` & `docbuild-0.1.101/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/page_creator.py` & `docbuild-0.1.101/docbuild/page_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .textract_parser import TextractParser
 from .paragraph_detection.paragraph_extractor import ParagraphExtractor
 from .paragraph_detection.paragraph_sorter import sort_areas
 from .visual_detection.bordered_table_extraction import BorderedTableExtractor
 from .visual_detection.vis_line_detection import VisLineDetector
 from .utils import get_average_character_height, get_average_character_width
-
+from .constants import SORT_LINE_VERTICAL_SCALE
 
 class PageCreator:
     def __init__(
         self,
         image_path: str,
         textract_response: dict = None,
         words: list[Word] = None,
@@ -143,15 +143,15 @@
             words = self.words
             avg_char_width = get_average_character_width(words)
             lines = self.get_lines(words, space_threshold=3 * avg_char_width)
 
         else:
             parser = TextractParser(self.textract_response)
             lines = parser.parse_response()
-            lines = TextBlock.sort(lines)
+            lines = TextBlock.sort(lines, height_scale = SORT_LINE_VERTICAL_SCALE)
             words = [word for line in lines for word in line.children]
         if not words:
             return Page()
         tables = self.get_tables(words)
         table_words = list(
             itertools.chain(*(table.get_all(Word) for table in tables))
         )
```

### Comparing `docbuild-0.1.1/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.101/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.101/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.101/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/textract_parser.py` & `docbuild-0.1.101/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/utils.py` & `docbuild-0.1.101/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.101/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.101/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.101/docbuild.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.1
+Version: 0.1.101
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.1/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.101/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.1/setup.py` & `docbuild-0.1.101/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.1",
+    version="0.1.101",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

