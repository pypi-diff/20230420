# Comparing `tmp/fasdr-0.0.5.tar.gz` & `tmp/fasdr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasdr-0.0.5.tar", last modified: Thu Apr 20 00:13:00 2023, max compression
+gzip compressed data, was "fasdr-0.0.6.tar", last modified: Thu Apr 20 18:43:58 2023, max compression
```

## Comparing `fasdr-0.0.5.tar` & `fasdr-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 00:13:00.006703 fasdr-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-20 00:12:43.000000 fasdr-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/fasdr/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/fasdr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/fasdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 00:13:00.000000 fasdr-0.0.5/fasdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:13:00.006703 fasdr-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-20 00:12:43.000000 fasdr-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-20 00:12:43.000000 fasdr-0.0.5/tests/test_fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:58.296835 fasdr-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 18:43:58.296835 fasdr-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-20 18:43:47.000000 fasdr-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:58.292835 fasdr-0.0.6/fasdr/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 18:43:47.000000 fasdr-0.0.6/fasdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 18:43:47.000000 fasdr-0.0.6/fasdr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-20 18:43:47.000000 fasdr-0.0.6/fasdr/fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:58.296835 fasdr-0.0.6/fasdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 18:43:58.000000 fasdr-0.0.6/fasdr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:43:58.296835 fasdr-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-20 18:43:47.000000 fasdr-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:58.296835 fasdr-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-20 18:43:47.000000 fasdr-0.0.6/tests/test_fasdr.py
```

### Comparing `fasdr-0.0.5/PKG-INFO` & `fasdr-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasdr-0.0.5/README.md` & `fasdr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fasdr-0.0.5/fasdr/cli.py` & `fasdr-0.0.6/fasdr/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import argparse
 import os
 import sys
+import logging
+import rich
+from rich.console import Console
+from rich.logging import RichHandler
 
 from fasdr import DocumentIndex
-from rich.console import Console
+
+FORMAT = "%(message)s"
+logging.basicConfig(
+    level="NOTSET", format=FORMAT, datefmt="[%X]", handlers=[RichHandler()]
+)
+
+logger = logging.getLogger("rich")
+logger.info("Hello, World!")
 
 def main():
     console = Console()
     parser = argparse.ArgumentParser(description="Fasdr: Fast Approximate String Distance Retrieval")
     parser.add_argument("path", help="Path to the index directory")
     args = parser.parse_args()
-
+    logger.debug(args)
     index_path = args.path
+    logger.debug(index_path)
+    logger.debug(sys.argv)
     if not os.path.exists(index_path):
         console.print(f"Error: Path '[red]{index_path}[/red]' does not exist.", style="bold red")
         sys.exit(1)
 
     with console.status("Building index..."):
         index = DocumentIndex(index_path)
 
@@ -34,8 +47,8 @@
     #     console.print(f"Error: Path '[red]{index_path}[/red]' does not exist.", style="bold red")
     #     sys.exit(1)
 
     # with console.status("Building index..."):
     #     index = DocumentIndex(index_path)
 
     # console.print("Done!", style="bold green")
-    # console.print(f"Index generated at [green]{index_path}/.embeddings[/green]", style="bold green")
+    # console.print(f"Index generated at [green]{index_path}/.embeddings[/green]", style="bold green")
```

### Comparing `fasdr-0.0.5/fasdr/fasdr.py` & `fasdr-0.0.6/fasdr/fasdr.py`

 * *Files identical despite different names*

### Comparing `fasdr-0.0.5/fasdr.egg-info/PKG-INFO` & `fasdr-0.0.6/fasdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasdr-0.0.5/setup.py` & `fasdr-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fasdr',
-    version='0.0.5',
+    version='0.0.6',
     author='David Marx',
     author_email='david.marx84@gmail.com',
     description='Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmarx/fast-and-simple-dense-retrieval/',
     packages=['fasdr'],
```

### Comparing `fasdr-0.0.5/tests/test_fasdr.py` & `fasdr-0.0.6/tests/test_fasdr.py`

 * *Files identical despite different names*

