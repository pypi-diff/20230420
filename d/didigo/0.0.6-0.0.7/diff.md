# Comparing `tmp/didigo-0.0.6.tar.gz` & `tmp/didigo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didigo-0.0.6.tar", last modified: Thu Apr 20 09:52:25 2023, max compression
+gzip compressed data, was "didigo-0.0.7.tar", last modified: Thu Apr 20 09:57:38 2023, max compression
```

## Comparing `didigo-0.0.6.tar` & `didigo-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 09:52:25.042303 didigo-0.0.6/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-04-20 09:52:25.042019 didigo-0.0.6/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-04-20 09:08:52.000000 didigo-0.0.6/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 09:52:25.041598 didigo-0.0.6/didigo.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-04-20 09:52:24.000000 didigo-0.0.6/didigo.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      186 2023-04-20 09:52:24.000000 didigo-0.0.6/didigo.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 09:52:24.000000 didigo-0.0.6/didigo.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       44 2023-04-20 09:52:24.000000 didigo-0.0.6/didigo.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 09:52:24.000000 didigo-0.0.6/didigo.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      275 2023-04-20 09:10:57.000000 didigo-0.0.6/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 09:52:25.042401 didigo-0.0.6/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1169 2023-04-20 09:46:16.000000 didigo-0.0.6/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 09:57:38.772918 didigo-0.0.7/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-04-20 09:57:38.772615 didigo-0.0.7/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-04-20 09:08:52.000000 didigo-0.0.7/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 09:57:38.771973 didigo-0.0.7/didigo.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-04-20 09:57:38.000000 didigo-0.0.7/didigo.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      186 2023-04-20 09:57:38.000000 didigo-0.0.7/didigo.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 09:57:38.000000 didigo-0.0.7/didigo.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-04-20 09:57:38.000000 didigo-0.0.7/didigo.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 09:57:38.000000 didigo-0.0.7/didigo.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      275 2023-04-20 09:10:57.000000 didigo-0.0.7/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 09:57:38.773051 didigo-0.0.7/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1170 2023-04-20 09:57:14.000000 didigo-0.0.7/setup.py
```

### Comparing `didigo-0.0.6/setup.py` & `didigo-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     # extras_require={
     #     'tests': utils.parse_requirements('requirements/tests.txt'),
     #     'build': utils.parse_requirements('requirements/build.txt'),
     #     'optional': utils.parse_requirements('requirements/optional.txt'),
     # },
     entry_points={
         'console_scripts': [
-              'didigo = didigo.cli:main'
+              'didigoy = didigo.cli:main'
           ]
     },
     ext_modules=[],
 )
```

