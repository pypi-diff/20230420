# Comparing `tmp/pykrakenfiles-0.0.1.tar.gz` & `tmp/pykrakenfiles-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrakenfiles-0.0.1.tar", last modified: Thu Mar 30 16:32:55 2023, max compression
+gzip compressed data, was "pykrakenfiles-0.0.2.tar", last modified: Thu Apr 20 13:42:39 2023, max compression
```

## Comparing `pykrakenfiles-0.0.1.tar` & `pykrakenfiles-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-30 16:32:43.000000 pykrakenfiles-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-30 16:32:43.000000 pykrakenfiles-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-30 16:32:43.000000 pykrakenfiles-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/src/pykrakenfiles/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-30 16:32:43.000000 pykrakenfiles-0.0.1/src/pykrakenfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-30 16:32:43.000000 pykrakenfiles-0.0.1/src/pykrakenfiles/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:32:55.587468 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-30 16:32:55.000000 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-30 16:32:55.000000 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:32:55.000000 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 16:32:55.000000 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 16:32:55.000000 pykrakenfiles-0.0.1/src/pykrakenfiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/src/pykrakenfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/src/pykrakenfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/src/pykrakenfiles/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-20 13:42:28.000000 pykrakenfiles-0.0.2/src/pykrakenfiles/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:39.572239 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 13:42:39.000000 pykrakenfiles-0.0.2/src/pykrakenfiles.egg-info/top_level.txt
```

### Comparing `pykrakenfiles-0.0.1/LICENSE` & `pykrakenfiles-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykrakenfiles-0.0.1/setup.py` & `pykrakenfiles-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pykrakenfiles",
-    version="0.0.1",
+    version="0.0.2",
     author="bontoutou",
     description="Krakenfiles upload API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['krakenfiles', 'upload'],
     url="https://github.com/bontoutou00/pykrakenfiles",
     project_urls={
@@ -19,9 +19,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
-    install_requires=['requests', 'tqdm', 'requests_toolbelt']
+    install_requires=['requests', 'tqdm', 'requests_toolbelt', 'pyyAML'],
+    entry_points={
+        "console_scripts":
+            ["pykrakenfiles = pykrakenfiles.cli:main",
+             "pykrakenfiles-list = pykrakenfiles.cli:list"]
+    },
 )
```

