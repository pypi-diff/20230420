# Comparing `tmp/ascii-cli-0.1.0.tar.gz` & `tmp/ascii-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.1.0.tar", last modified: Thu Apr 20 02:06:29 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.2.tar", last modified: Thu Apr 20 08:02:38 2023, max compression
```

## Comparing `ascii-cli-0.1.0.tar` & `ascii-cli-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.433775 ascii-cli-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-20 02:06:29.431138 ascii-cli-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.407668 ascii-cli-0.1.0/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 02:06:29.000000 ascii-cli-0.1.0/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 02:06:29.433775 ascii-cli-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-04-20 02:05:50.000000 ascii-cli-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.418082 ascii-cli-0.1.0/src/
--rw-rw-rw-   0        0        0       20 2023-04-20 01:59:29.000000 ascii-cli-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     1229 2023-04-20 02:05:40.000000 ascii-cli-0.1.0/src/__main__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:17:05.000000 ascii-cli-0.1.0/src/func.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:06:29.429122 ascii-cli-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:12:57.000000 ascii-cli-0.1.0/tests/test_func.py
--rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.1.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.617198 ascii-cli-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2566 2023-04-20 08:02:38.609210 ascii-cli-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-04-20 07:43:25.000000 ascii-cli-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.593227 ascii-cli-0.1.2/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0     2566 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-20 08:02:38.000000 ascii-cli-0.1.2/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:02:38.617198 ascii-cli-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-04-20 08:02:31.000000 ascii-cli-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:02:38.609210 ascii-cli-0.1.2/src/
+-rw-rw-rw-   0        0        0       20 2023-04-20 06:52:26.000000 ascii-cli-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-04-20 06:59:34.000000 ascii-cli-0.1.2/src/__main__.py
+-rw-rw-rw-   0        0        0     4017 2023-04-20 07:00:43.000000 ascii-cli-0.1.2/src/func.py
```

### Comparing `ascii-cli-0.1.0/LICENSE` & `ascii-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.0/setup.py` & `ascii-cli-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.1.0",
+    version="0.1.2",
     packages=find_packages(),
     package_data={'src': ['func.py']},
     install_requires=["Pillow"],
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+
     entry_points={
         "console_scripts": [
             "ascii-cli=src.__main__:main"
         ]
     },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/ascii-cli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
-    long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
 )
```

### Comparing `ascii-cli-0.1.0/src/__main__.py` & `ascii-cli-0.1.2/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from src.func import convert_to_ascii
+from func import convert_to_ascii
 
 
 def main():
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
         description="Converts an image to ASCII art.")
```

### Comparing `ascii-cli-0.1.0/src/func.py` & `ascii-cli-0.1.2/src/func.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def convert_to_ascii(args):
 
     # define characters used
     SET1 = ['/', '!', '=', '+', '|', '#', '%', '@', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '=', '?', '[', ']',
             '{', '}', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     SET2 = ["0", "O", "o", "8", "9", "6", "@", "&", ".", '"', ":"]
-    SET3 = ["░", "▒", "▓", "█"]
+    SET3 = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
 
     # input is set
     BRUSH = int(args.darkness)
     INVERT = bool(args.invert)
 
     # choose the character set  & shuffle
     if args.set == "1":
```

