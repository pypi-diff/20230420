# Comparing `tmp/ascii-cli-0.1.2.tar.gz` & `tmp/ascii-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.1.2.tar", last modified: Thu Apr 20 08:02:38 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.3.tar", last modified: Thu Apr 20 08:26:36 2023, max compression
```

## Comparing `ascii-cli-0.1.2.tar` & `ascii-cli-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.617198 ascii-cli-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2566 2023-04-20 08:02:38.609210 ascii-cli-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-04-20 07:43:25.000000 ascii-cli-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.593227 ascii-cli-0.1.2/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0     2566 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 08:02:38.617198 ascii-cli-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-04-20 08:02:31.000000 ascii-cli-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.609210 ascii-cli-0.1.2/src/
--rw-rw-rw-   0        0        0       20 2023-04-20 06:52:26.000000 ascii-cli-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-04-20 06:59:34.000000 ascii-cli-0.1.2/src/__main__.py
--rw-rw-rw-   0        0        0     4017 2023-04-20 07:00:43.000000 ascii-cli-0.1.2/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.560652 ascii-cli-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2566 2023-04-20 08:26:36.559648 ascii-cli-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-04-20 07:43:25.000000 ascii-cli-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.544648 ascii-cli-0.1.3/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0     2566 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:26:36.560652 ascii-cli-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-04-20 08:26:03.000000 ascii-cli-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.556647 ascii-cli-0.1.3/src/
+-rw-rw-rw-   0        0        0       20 2023-04-20 06:52:26.000000 ascii-cli-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-04-20 08:21:27.000000 ascii-cli-0.1.3/src/__main__.py
+-rw-rw-rw-   0        0        0     4017 2023-04-20 07:00:43.000000 ascii-cli-0.1.3/src/func.py
```

### Comparing `ascii-cli-0.1.2/LICENSE` & `ascii-cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.2/PKG-INFO` & `ascii-cli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.2/README.md` & `ascii-cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.2/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.1.3/ascii_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.2/setup.py` & `ascii-cli-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     package_data={'src': ['func.py']},
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `ascii-cli-0.1.2/src/__main__.py` & `ascii-cli-0.1.3/src/__main__.py`

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

### Comparing `ascii-cli-0.1.2/src/func.py` & `ascii-cli-0.1.3/src/func.py`

 * *Files identical despite different names*

