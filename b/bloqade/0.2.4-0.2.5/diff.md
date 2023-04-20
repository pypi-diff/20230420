# Comparing `tmp/bloqade-0.2.4.tar.gz` & `tmp/bloqade-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloqade-0.2.4.tar", last modified: Thu Apr 20 20:20:49 2023, max compression
+gzip compressed data, was "bloqade-0.2.5.tar", last modified: Thu Apr 20 20:28:24 2023, max compression
```

## Comparing `bloqade-0.2.4.tar` & `bloqade-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       49 2023-04-20 19:18:21.970339 bloqade-0.2.4/README.md
--rw-r--r--   0        0        0      444 2023-04-20 20:15:06.312003 bloqade-0.2.4/build.py
--rw-r--r--   0        0        0      939 2023-04-20 20:20:49.648241 bloqade-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       17 2023-04-20 19:58:02.117607 bloqade-0.2.4/src/bloqade/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 20:02:39.462305 bloqade-0.2.4/src/bloqade/ir/__init__.py
--rw-r--r--   0        0        0       23 2023-04-20 20:02:45.744447 bloqade-0.2.4/src/bloqade/ir/scalar.py
--rw-r--r--   0        0        0      115 2023-04-20 20:20:49.648019 bloqade-0.2.4/src/bloqade/juliapkg.json
--rw-r--r--   0        0        0        0 2023-04-20 19:18:21.977393 bloqade-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 bloqade-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-04-20 19:18:21.970339 bloqade-0.2.5/README.md
+-rw-r--r--   0        0        0      427 2023-04-20 20:27:41.147571 bloqade-0.2.5/build.py
+-rw-r--r--   0        0        0      115 2023-04-20 20:28:24.236100 bloqade-0.2.5/juliapkg.json
+-rw-r--r--   0        0        0      939 2023-04-20 20:28:24.237057 bloqade-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       17 2023-04-20 20:22:38.842000 bloqade-0.2.5/src/bloqade/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:02:39.462305 bloqade-0.2.5/src/bloqade/ir/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-20 20:02:45.744447 bloqade-0.2.5/src/bloqade/ir/scalar.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:18:21.977393 bloqade-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 bloqade-0.2.5/PKG-INFO
```

### Comparing `bloqade-0.2.4/pyproject.toml` & `bloqade-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bloqade"
-version = "0.2.4"
+version = "0.2.5"
 description = "neutral atom software development kit"
 authors = [
     { name = "QuEra Computing Inc.", email = "info@quera.com" },
 ]
 dependencies = [
     "juliacall>=0.9.12",
     "matplotlib>=3.7.1",
```

