# Comparing `tmp/bloqade-0.2.3.tar.gz` & `tmp/bloqade-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloqade-0.2.3.tar", last modified: Thu Apr 20 20:13:20 2023, max compression
+gzip compressed data, was "bloqade-0.2.4.tar", last modified: Thu Apr 20 20:20:49 2023, max compression
```

## Comparing `bloqade-0.2.3.tar` & `bloqade-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       49 2023-04-20 19:18:21.970339 bloqade-0.2.3/README.md
--rw-r--r--   0        0        0      462 2023-04-20 20:08:43.788934 bloqade-0.2.3/build.py
--rw-r--r--   0        0        0      961 2023-04-20 20:13:20.214754 bloqade-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      115 2023-04-20 20:13:20.214448 bloqade-0.2.3/src/bloqade/juliapkg.json
--rw-r--r--   0        0        0        0 2023-04-20 19:18:21.977393 bloqade-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 bloqade-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-04-20 19:18:21.970339 bloqade-0.2.4/README.md
+-rw-r--r--   0        0        0      444 2023-04-20 20:15:06.312003 bloqade-0.2.4/build.py
+-rw-r--r--   0        0        0      939 2023-04-20 20:20:49.648241 bloqade-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       17 2023-04-20 19:58:02.117607 bloqade-0.2.4/src/bloqade/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:02:39.462305 bloqade-0.2.4/src/bloqade/ir/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-20 20:02:45.744447 bloqade-0.2.4/src/bloqade/ir/scalar.py
+-rw-r--r--   0        0        0      115 2023-04-20 20:20:49.648019 bloqade-0.2.4/src/bloqade/juliapkg.json
+-rw-r--r--   0        0        0        0 2023-04-20 19:18:21.977393 bloqade-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 bloqade-0.2.4/PKG-INFO
```

### Comparing `bloqade-0.2.3/pyproject.toml` & `bloqade-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bloqade"
-version = "0.2.3"
+version = "0.2.4"
 description = "neutral atom software development kit"
 authors = [
     { name = "QuEra Computing Inc.", email = "info@quera.com" },
 ]
 dependencies = [
     "juliacall>=0.9.12",
     "matplotlib>=3.7.1",
@@ -17,15 +17,15 @@
 
 [project.license]
 text = "MIT"
 
 [tool.pdm.build]
 package-dir = "src"
 includes = [
-    "src/bloqade/juliapkg.json",
+    "src",
 ]
 custom-hook = "build.py"
 
 [tool.pdm.scripts]
 upload = "python -m twine upload -r bloqade dist/*"
 
 [tool.pdm.scripts._]
```

