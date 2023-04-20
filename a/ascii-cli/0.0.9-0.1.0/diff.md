# Comparing `tmp/ascii-cli-0.0.9.tar.gz` & `tmp/ascii-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.9.tar", last modified: Thu Apr 20 02:02:40 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.0.tar", last modified: Thu Apr 20 02:06:29 2023, max compression
```

## Comparing `ascii-cli-0.0.9.tar` & `ascii-cli-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.816912 ascii-cli-0.0.9/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-20 02:02:40.815912 ascii-cli-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.776963 ascii-cli-0.0.9/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 02:02:40.816912 ascii-cli-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-04-20 02:01:45.000000 ascii-cli-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.798984 ascii-cli-0.0.9/src/
--rw-rw-rw-   0        0        0       20 2023-04-20 01:59:29.000000 ascii-cli-0.0.9/src/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-04-20 01:27:20.000000 ascii-cli-0.0.9/src/__main__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:17:05.000000 ascii-cli-0.0.9/src/func.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.811186 ascii-cli-0.0.9/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:12:57.000000 ascii-cli-0.0.9/tests/test_func.py
--rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.0.9/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.433775 ascii-cli-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-20 02:06:29.431138 ascii-cli-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.407668 ascii-cli-0.1.0/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 02:06:29.433775 ascii-cli-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-04-20 02:05:50.000000 ascii-cli-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.418082 ascii-cli-0.1.0/src/
+-rw-rw-rw-   0        0        0       20 2023-04-20 01:59:29.000000 ascii-cli-0.1.0/src/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-04-20 02:05:40.000000 ascii-cli-0.1.0/src/__main__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:17:05.000000 ascii-cli-0.1.0/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.429122 ascii-cli-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:12:57.000000 ascii-cli-0.1.0/tests/test_func.py
+-rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.1.0/tests/test_main.py
```

### Comparing `ascii-cli-0.0.9/LICENSE` & `ascii-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.9/PKG-INFO` & `ascii-cli-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.9/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.1.0/ascii_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.9/setup.py` & `ascii-cli-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.9",
+    version="0.1.0",
     packages=find_packages(),
     package_data={'src': ['func.py']},
     install_requires=["Pillow"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ascii-cli-0.0.9/src/__main__.py` & `ascii-cli-0.1.0/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from func import convert_to_ascii
+from src.func import convert_to_ascii
 
 
 def main():
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
         description="Converts an image to ASCII art.")
```

### Comparing `ascii-cli-0.0.9/src/func.py` & `ascii-cli-0.1.0/src/func.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.9/tests/test_func.py` & `ascii-cli-0.1.0/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.9/tests/test_main.py` & `ascii-cli-0.1.0/tests/test_main.py`

 * *Files identical despite different names*

