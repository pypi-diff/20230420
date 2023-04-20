# Comparing `tmp/bloqade-0.2.0.tar.gz` & `tmp/bloqade-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloqade-0.2.0.tar", last modified: Thu Apr 20 18:42:46 2023, max compression
+gzip compressed data, was "bloqade-0.2.1.tar", last modified: Thu Apr 20 18:50:47 2023, max compression
```

## Comparing `bloqade-0.2.0.tar` & `bloqade-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.236289 bloqade-0.2.0/
--rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:42:46.236177 bloqade-0.2.0/PKG-INFO
--rw-r--r--   0 roger      (501) staff       (20)       49 2023-04-20 16:44:32.000000 bloqade-0.2.0/README.md
--rw-r--r--   0 roger      (501) staff       (20)      660 2023-04-20 18:42:43.000000 bloqade-0.2.0/pyproject.toml
--rw-r--r--   0 roger      (501) staff       (20)       38 2023-04-20 18:42:46.236320 bloqade-0.2.0/setup.cfg
-drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.235068 bloqade-0.2.0/src/
-drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.235420 bloqade-0.2.0/src/bloqade/
--rw-r--r--   0 roger      (501) staff       (20)      129 2023-04-20 18:39:21.000000 bloqade-0.2.0/src/bloqade/__init__.py
-drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.236008 bloqade-0.2.0/src/bloqade.egg-info/
--rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/PKG-INFO
--rw-r--r--   0 roger      (501) staff       (20)      222 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/SOURCES.txt
--rw-r--r--   0 roger      (501) staff       (20)        1 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/dependency_links.txt
--rw-r--r--   0 roger      (501) staff       (20)       86 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/requires.txt
--rw-r--r--   0 roger      (501) staff       (20)        8 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/top_level.txt
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:50:47.424232 bloqade-0.2.1/
+-rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:50:47.424117 bloqade-0.2.1/PKG-INFO
+-rw-r--r--   0 roger      (501) staff       (20)       49 2023-04-20 16:44:32.000000 bloqade-0.2.1/README.md
+-rw-r--r--   0 roger      (501) staff       (20)      680 2023-04-20 18:50:04.000000 bloqade-0.2.1/pyproject.toml
+-rw-r--r--   0 roger      (501) staff       (20)       38 2023-04-20 18:50:47.424270 bloqade-0.2.1/setup.cfg
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:50:47.423123 bloqade-0.2.1/src/
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:50:47.423411 bloqade-0.2.1/src/bloqade/
+-rw-r--r--   0 roger      (501) staff       (20)      129 2023-04-20 18:39:21.000000 bloqade-0.2.1/src/bloqade/__init__.py
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:50:47.423960 bloqade-0.2.1/src/bloqade.egg-info/
+-rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:50:47.000000 bloqade-0.2.1/src/bloqade.egg-info/PKG-INFO
+-rw-r--r--   0 roger      (501) staff       (20)      222 2023-04-20 18:50:47.000000 bloqade-0.2.1/src/bloqade.egg-info/SOURCES.txt
+-rw-r--r--   0 roger      (501) staff       (20)        1 2023-04-20 18:50:47.000000 bloqade-0.2.1/src/bloqade.egg-info/dependency_links.txt
+-rw-r--r--   0 roger      (501) staff       (20)       86 2023-04-20 18:50:47.000000 bloqade-0.2.1/src/bloqade.egg-info/requires.txt
+-rw-r--r--   0 roger      (501) staff       (20)        8 2023-04-20 18:50:47.000000 bloqade-0.2.1/src/bloqade.egg-info/top_level.txt
```

### Comparing `bloqade-0.2.0/pyproject.toml` & `bloqade-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "bloqade"
-version = "0.2.0"
+version = "0.2.1"
 description = "neutral atom software development kit"
 authors = [
     {name = "QuEra Computing Inc.", email = "info@quera.com"},
 ]
 dependencies = [
     "juliacall>=0.9.12",
     "matplotlib>=3.7.1",
     "numpy>=1.24.2",
     "pydantic>=1.10.7",
     "setuptools>=67.7.0",
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "MIT"}
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
@@ -26,8 +26,9 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
     "pytest>=7.3.1",
     "mypy>=1.2.0",
     "ipython>=8.12.0",
+    "twine>=4.0.2",
 ]
```

