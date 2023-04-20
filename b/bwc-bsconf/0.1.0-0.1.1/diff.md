# Comparing `tmp/bwc-bsconf-0.1.0.tar.gz` & `tmp/bwc-bsconf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwc-bsconf-0.1.0.tar", last modified: Thu Apr 20 13:02:29 2023, max compression
+gzip compressed data, was "bwc-bsconf-0.1.1.tar", last modified: Thu Apr 20 14:09:31 2023, max compression
```

## Comparing `bwc-bsconf-0.1.0.tar` & `bwc-bsconf-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 13:02:29.018808 bwc-bsconf-0.1.0/
--rw-rw-rw-   0        0        0     1053 2023-04-20 12:57:32.000000 bwc-bsconf-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      936 2023-04-20 13:02:29.016807 bwc-bsconf-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-04-20 13:01:03.000000 bwc-bsconf-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 13:02:28.980810 bwc-bsconf-0.1.0/bwc-bsconf/
--rw-rw-rw-   0        0        0       84 2023-04-20 13:00:29.000000 bwc-bsconf-0.1.0/bwc-bsconf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:02:29.015805 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/
--rw-rw-rw-   0        0        0      936 2023-04-20 13:02:28.000000 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-20 13:02:28.000000 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 13:02:28.000000 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-20 13:02:28.000000 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-20 13:02:28.000000 bwc-bsconf-0.1.0/bwc_bsconf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 13:02:29.020835 bwc-bsconf-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-04-20 12:57:07.000000 bwc-bsconf-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:31.802451 bwc-bsconf-0.1.1/
+-rw-rw-rw-   0        0        0     1053 2023-04-20 13:39:10.000000 bwc-bsconf-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1373 2023-04-20 14:09:31.800449 bwc-bsconf-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1043 2023-04-20 14:05:59.000000 bwc-bsconf-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:31.766451 bwc-bsconf-0.1.1/bwc-bsconf/
+-rw-rw-rw-   0        0        0       84 2023-04-20 13:39:10.000000 bwc-bsconf-0.1.1/bwc-bsconf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:31.798450 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/
+-rw-rw-rw-   0        0        0     1373 2023-04-20 14:09:31.000000 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-20 14:09:31.000000 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:09:31.000000 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-20 14:09:31.000000 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-20 14:09:31.000000 bwc-bsconf-0.1.1/bwc_bsconf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:09:31.802451 bwc-bsconf-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-04-20 14:05:49.000000 bwc-bsconf-0.1.1/setup.py
```

### Comparing `bwc-bsconf-0.1.0/LICENSE` & `bwc-bsconf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bwc-bsconf-0.1.0/PKG-INFO` & `bwc-bsconf-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,66 @@
 Metadata-Version: 2.1
 Name: bwc-bsconf
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library Python to configure, repair and install servers in an automated way.
 Home-page: UNKNOWN
 Author: Aníbal Barca, 
 Author-email: anibalbs@barca.com, 
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-### Pip [bwc-bsconf 0.1.0](https://pypi.org/project/bwc-bsconf/0.1.0/) 
+### [bwc-bsconf 0.1.1](https://pypi.org/project/bwc-bsconf/0.1.1/) 
 
 This project better define server configurations, repairs and installations in various operating environments.
 
+Developers can use the main features of the tool with this pip package.
+
+Facilitate the installation of web servers, games, email, etc.
 
 #### To Developers
 
 <br>
 
-1. Install the **wheel** module in your python environment
+### Installation
 
-`pip install wheel`
+Install the package with pip:
 
-<br>
+via PyPI:
+
+`pip install bwc-bsconf`
 
-2. Install **twine** which will be used to upload the tarball
+or via GitHub
 
-`pip install twine`
+`pip install git+https://github.com/BarcaWebCloud/bsconf-py.git`
 
 <br>
 
-3. Now compile the library setup of bsconf module
+Now Create a Python file to start using the **bwc-bsconf** package in your project. In the example below, the file named `main.py` was specified to run the bsconf module. Add the following content in the main file.
 
-`python .\setup.py sdist bdist_wheel`
+`main.py`
 
-...
+```py
+import importlib
+
+bwc_bsconf = importlib.import_module("bwc-bsconf")
+init = bwc_bsconf.bsconf
+
+init()
+```
 
 <br>
 
-4. Publish or update package in Pip Manager
+Run the main program
+
+```
+python3 main.py*
+```
+<br>
+
+Will display on your screen something like this:
 
 ```
-python3 -m twine upload dist/*
+Welcome to BSconf
 ```
```

### Comparing `bwc-bsconf-0.1.0/bwc_bsconf.egg-info/PKG-INFO` & `bwc-bsconf-0.1.1/bwc_bsconf.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,66 @@
 Metadata-Version: 2.1
 Name: bwc-bsconf
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library Python to configure, repair and install servers in an automated way.
 Home-page: UNKNOWN
 Author: Aníbal Barca, 
 Author-email: anibalbs@barca.com, 
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-### Pip [bwc-bsconf 0.1.0](https://pypi.org/project/bwc-bsconf/0.1.0/) 
+### [bwc-bsconf 0.1.1](https://pypi.org/project/bwc-bsconf/0.1.1/) 
 
 This project better define server configurations, repairs and installations in various operating environments.
 
+Developers can use the main features of the tool with this pip package.
+
+Facilitate the installation of web servers, games, email, etc.
 
 #### To Developers
 
 <br>
 
-1. Install the **wheel** module in your python environment
+### Installation
 
-`pip install wheel`
+Install the package with pip:
 
-<br>
+via PyPI:
+
+`pip install bwc-bsconf`
 
-2. Install **twine** which will be used to upload the tarball
+or via GitHub
 
-`pip install twine`
+`pip install git+https://github.com/BarcaWebCloud/bsconf-py.git`
 
 <br>
 
-3. Now compile the library setup of bsconf module
+Now Create a Python file to start using the **bwc-bsconf** package in your project. In the example below, the file named `main.py` was specified to run the bsconf module. Add the following content in the main file.
 
-`python .\setup.py sdist bdist_wheel`
+`main.py`
 
-...
+```py
+import importlib
+
+bwc_bsconf = importlib.import_module("bwc-bsconf")
+init = bwc_bsconf.bsconf
+
+init()
+```
 
 <br>
 
-4. Publish or update package in Pip Manager
+Run the main program
+
+```
+python3 main.py*
+```
+<br>
+
+Will display on your screen something like this:
 
 ```
-python3 -m twine upload dist/*
+Welcome to BSconf
 ```
```

