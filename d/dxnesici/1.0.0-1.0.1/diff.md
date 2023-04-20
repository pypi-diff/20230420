# Comparing `tmp/dxnesici-1.0.0.tar.gz` & `tmp/dxnesici-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxnesici-1.0.0.tar", last modified: Wed Apr 19 03:24:00 2023, max compression
+gzip compressed data, was "dxnesici-1.0.1.tar", last modified: Thu Apr 20 10:26:58 2023, max compression
```

## Comparing `dxnesici-1.0.0.tar` & `dxnesici-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-19 03:24:00.178692 dxnesici-1.0.0/
--rw-rw-r--   0 koki      (1000) koki      (1000)     1064 2023-04-18 12:27:26.000000 dxnesici-1.0.0/LICENSE
--rw-rw-r--   0 koki      (1000) koki      (1000)       89 2023-04-18 12:40:53.000000 dxnesici-1.0.0/MANIFEST.in
--rw-rw-r--   0 koki      (1000) koki      (1000)      886 2023-04-19 03:24:00.178692 dxnesici-1.0.0/PKG-INFO
-drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-19 03:24:00.178692 dxnesici-1.0.0/dxnesici/
--rw-rw-r--   0 koki      (1000) koki      (1000)       26 2023-04-18 12:31:31.000000 dxnesici-1.0.0/dxnesici/__init__.py
--rw-rw-r--   0 koki      (1000) koki      (1000)     8079 2023-04-18 12:31:31.000000 dxnesici-1.0.0/dxnesici/alg.py
-drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-19 03:24:00.178692 dxnesici-1.0.0/dxnesici.egg-info/
--rw-rw-r--   0 koki      (1000) koki      (1000)      886 2023-04-19 03:24:00.000000 dxnesici-1.0.0/dxnesici.egg-info/PKG-INFO
--rw-rw-r--   0 koki      (1000) koki      (1000)      224 2023-04-19 03:24:00.000000 dxnesici-1.0.0/dxnesici.egg-info/SOURCES.txt
--rw-rw-r--   0 koki      (1000) koki      (1000)        1 2023-04-19 03:24:00.000000 dxnesici-1.0.0/dxnesici.egg-info/dependency_links.txt
--rw-rw-r--   0 koki      (1000) koki      (1000)       12 2023-04-19 03:24:00.000000 dxnesici-1.0.0/dxnesici.egg-info/requires.txt
--rw-rw-r--   0 koki      (1000) koki      (1000)        9 2023-04-19 03:24:00.000000 dxnesici-1.0.0/dxnesici.egg-info/top_level.txt
--rw-rw-r--   0 koki      (1000) koki      (1000)       38 2023-04-19 03:24:00.178692 dxnesici-1.0.0/setup.cfg
--rw-rw-r--   0 koki      (1000) koki      (1000)     1423 2023-04-18 12:39:17.000000 dxnesici-1.0.0/setup.py
+drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-20 10:26:58.773309 dxnesici-1.0.1/
+-rw-rw-r--   0 koki      (1000) koki      (1000)     1064 2023-04-18 12:27:26.000000 dxnesici-1.0.1/LICENSE
+-rw-rw-r--   0 koki      (1000) koki      (1000)       89 2023-04-18 12:40:53.000000 dxnesici-1.0.1/MANIFEST.in
+-rw-rw-r--   0 koki      (1000) koki      (1000)     4023 2023-04-20 10:26:58.773309 dxnesici-1.0.1/PKG-INFO
+drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-20 10:26:58.773309 dxnesici-1.0.1/dxnesici/
+-rw-rw-r--   0 koki      (1000) koki      (1000)       26 2023-04-18 12:31:31.000000 dxnesici-1.0.1/dxnesici/__init__.py
+-rw-rw-r--   0 koki      (1000) koki      (1000)     9078 2023-04-20 09:55:12.000000 dxnesici-1.0.1/dxnesici/alg.py
+drwxrwxr-x   0 koki      (1000) koki      (1000)        0 2023-04-20 10:26:58.773309 dxnesici-1.0.1/dxnesici.egg-info/
+-rw-rw-r--   0 koki      (1000) koki      (1000)     4023 2023-04-20 10:26:58.000000 dxnesici-1.0.1/dxnesici.egg-info/PKG-INFO
+-rw-rw-r--   0 koki      (1000) koki      (1000)      224 2023-04-20 10:26:58.000000 dxnesici-1.0.1/dxnesici.egg-info/SOURCES.txt
+-rw-rw-r--   0 koki      (1000) koki      (1000)        1 2023-04-20 10:26:58.000000 dxnesici-1.0.1/dxnesici.egg-info/dependency_links.txt
+-rw-rw-r--   0 koki      (1000) koki      (1000)       12 2023-04-20 10:26:58.000000 dxnesici-1.0.1/dxnesici.egg-info/requires.txt
+-rw-rw-r--   0 koki      (1000) koki      (1000)        9 2023-04-20 10:26:58.000000 dxnesici-1.0.1/dxnesici.egg-info/top_level.txt
+-rw-rw-r--   0 koki      (1000) koki      (1000)       38 2023-04-20 10:26:58.773309 dxnesici-1.0.1/setup.cfg
+-rw-rw-r--   0 koki      (1000) koki      (1000)     1436 2023-04-20 10:25:03.000000 dxnesici-1.0.1/setup.py
```

### Comparing `dxnesici-1.0.0/LICENSE` & `dxnesici-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxnesici-1.0.0/setup.py` & `dxnesici-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="dxnesici",
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version="1.0.0",
+      version="1.0.1",
       description="DX-NES-ICI " +
                   "for numerical optimization in Python",
       author="Koki Ikeda",
       author_email="ikeda.k@ic.c.titech.ac.jp",
       maintainer="Koki Ikeda",
       maintainer_email="ikeda.k@ic.c.titech.ac.jp",
       url="https://github.com/ono-lab/dxnesici",
@@ -30,12 +30,12 @@
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Artificial Intelligence",
           "Operating System :: OS Independent",
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
       ],
-      keywords=["optimization", "DX-NES-ICI", "mixed-integer"],
+      keywords=["optimization", "DX-NES-ICI", "mixed-integer", "black-box"],
       packages=["dxnesici"],
       install_requires=["numpy", "scipy"],
       package_data={'': ['LICENSE']},
       )
```

