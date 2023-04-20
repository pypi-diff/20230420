# Comparing `tmp/ascii-cli-0.0.6.tar.gz` & `tmp/ascii-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.6.tar", last modified: Wed Apr 19 12:52:16 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.7.tar", last modified: Thu Apr 20 01:09:58 2023, max compression
```

## Comparing `ascii-cli-0.0.6.tar` & `ascii-cli-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:52:16.707888 ascii-cli-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 12:52:16.705889 ascii-cli-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:52:16.701889 ascii-cli-0.0.6/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 12:52:16.708890 ascii-cli-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-19 12:51:40.000000 ascii-cli-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:09:58.146701 ascii-cli-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-20 01:09:58.137583 ascii-cli-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 01:09:58.102584 ascii-cli-0.0.7/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-20 01:09:57.000000 ascii-cli-0.0.7/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-20 01:09:58.000000 ascii-cli-0.0.7/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 01:09:57.000000 ascii-cli-0.0.7/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-20 01:09:57.000000 ascii-cli-0.0.7/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 01:09:57.000000 ascii-cli-0.0.7/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 01:09:57.000000 ascii-cli-0.0.7/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 01:09:58.146701 ascii-cli-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-04-20 01:09:20.000000 ascii-cli-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:09:58.118596 ascii-cli-0.0.7/src/
+-rw-rw-rw-   0        0        0        0 2023-04-20 00:49:19.000000 ascii-cli-0.0.7/src/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-04-20 00:55:19.000000 ascii-cli-0.0.7/src/__main__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:01:30.000000 ascii-cli-0.0.7/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:09:58.137583 ascii-cli-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:00:52.000000 ascii-cli-0.0.7/tests/test_func.py
+-rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.0.7/tests/test_main.py
```

### Comparing `ascii-cli-0.0.6/LICENSE` & `ascii-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.6/PKG-INFO` & `ascii-cli-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.6/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.7/ascii_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.6/setup.py` & `ascii-cli-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     install_requires=["Pillow"],
-    entry_points={
-        "console_scripts": [
-            "ascii-cli = ascii",
-        ],
-    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    entry_points={
+        "console_scripts": [
+            "myproject=myproject.__main__:main"
+        ]
+    },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/ascii-cli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 )
```

