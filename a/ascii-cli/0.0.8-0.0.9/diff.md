# Comparing `tmp/ascii-cli-0.0.8.tar.gz` & `tmp/ascii-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.8.tar", last modified: Thu Apr 20 01:44:18 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.9.tar", last modified: Thu Apr 20 02:02:40 2023, max compression
```

## Comparing `ascii-cli-0.0.8.tar` & `ascii-cli-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 01:44:18.715362 ascii-cli-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-20 01:44:18.714338 ascii-cli-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 01:44:18.685840 ascii-cli-0.0.8/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 01:44:18.000000 ascii-cli-0.0.8/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 01:44:18.715362 ascii-cli-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-04-20 01:43:40.000000 ascii-cli-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 01:44:18.697766 ascii-cli-0.0.8/src/
--rw-rw-rw-   0        0        0        0 2023-04-20 00:49:19.000000 ascii-cli-0.0.8/src/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-04-20 01:27:20.000000 ascii-cli-0.0.8/src/__main__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:17:05.000000 ascii-cli-0.0.8/src/func.py
-drwxrwxrwx   0        0        0        0 2023-04-20 01:44:18.711325 ascii-cli-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 01:12:57.000000 ascii-cli-0.0.8/tests/test_func.py
--rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.0.8/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.816912 ascii-cli-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-20 02:02:40.815912 ascii-cli-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.776963 ascii-cli-0.0.9/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 02:02:40.000000 ascii-cli-0.0.9/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 02:02:40.816912 ascii-cli-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-04-20 02:01:45.000000 ascii-cli-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.798984 ascii-cli-0.0.9/src/
+-rw-rw-rw-   0        0        0       20 2023-04-20 01:59:29.000000 ascii-cli-0.0.9/src/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-04-20 01:27:20.000000 ascii-cli-0.0.9/src/__main__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:17:05.000000 ascii-cli-0.0.9/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:02:40.811186 ascii-cli-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 23:30:44.000000 ascii-cli-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 01:12:57.000000 ascii-cli-0.0.9/tests/test_func.py
+-rw-rw-rw-   0        0        0     1230 2023-04-20 01:08:07.000000 ascii-cli-0.0.9/tests/test_main.py
```

### Comparing `ascii-cli-0.0.8/LICENSE` & `ascii-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.8/PKG-INFO` & `ascii-cli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.8/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.9/ascii_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.8/setup.py` & `ascii-cli-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
+    package_data={'src': ['func.py']},
     install_requires=["Pillow"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `ascii-cli-0.0.8/src/__main__.py` & `ascii-cli-0.0.9/src/__main__.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.8/src/func.py` & `ascii-cli-0.0.9/src/func.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.8/tests/test_func.py` & `ascii-cli-0.0.9/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.8/tests/test_main.py` & `ascii-cli-0.0.9/tests/test_main.py`

 * *Files identical despite different names*

