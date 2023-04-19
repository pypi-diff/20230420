# Comparing `tmp/pyloobins-0.1.2.tar.gz` & `tmp/pyloobins-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.2.tar", max compression
+gzip compressed data, was "pyloobins-0.1.3.tar", max compression
```

## Comparing `pyloobins-0.1.2.tar` & `pyloobins-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.2/LICENSE
--rw-r--r--   0        0        0     1295 2023-04-12 01:43:08.133020 pyloobins-0.1.2/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.2/README.md
--rw-r--r--   0        0        0      877 2023-04-12 01:51:41.595228 pyloobins-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.2/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-11 23:56:04.085870 pyloobins-0.1.2/src/pyloobins/cli.py
--rw-r--r--   0        0        0     3582 2023-04-11 23:56:04.086003 pyloobins-0.1.2/src/pyloobins/models.py
--rw-r--r--   0        0        0     1177 2023-04-12 00:48:36.484104 pyloobins-0.1.2/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2610 2023-04-11 23:58:27.122687 pyloobins-0.1.2/src/pyloobins/util.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1295 2023-04-19 23:03:54.627657 pyloobins-0.1.3/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.3/README.md
+-rw-r--r--   0        0        0      877 2023-04-19 23:11:53.845950 pyloobins-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.3/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-19 23:11:53.846281 pyloobins-0.1.3/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     3582 2023-04-19 22:59:33.848606 pyloobins-0.1.3/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1177 2023-04-12 00:48:36.484104 pyloobins-0.1.3/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2610 2023-04-19 22:59:31.417375 pyloobins-0.1.3/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.3/PKG-INFO
```

### Comparing `pyloobins-0.1.2/LICENSE` & `pyloobins-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.2/LOOBins/pbpaste.yml` & `pyloobins-0.1.3/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.2/pyproject.toml` & `pyloobins-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
```

### Comparing `pyloobins-0.1.2/src/pyloobins/cli.py` & `pyloobins-0.1.3/src/pyloobins/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,18 @@
     required=True,
     help="File location of the LOOBin YAML file to validate.",
 )
 def validate(file: str) -> None:
     """Validate a LOOBin object."""
     if validate_loobin(yml_path=file):
         print(f"LOOBin at {file} is valid.")
+        sys.exit(0)
     else:
         print(f"LOOBin at {file} is NOT valid.")
+        sys.exit(1)
 
 
 @cli.command()
 @click.option("--name", type=str, required=False, help="Enter the name of the binary")
 @click.option(
     "--path",
     type=str,
```

### Comparing `pyloobins-0.1.2/src/pyloobins/models.py` & `pyloobins-0.1.3/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.2/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.3/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.2/src/pyloobins/util.py` & `pyloobins-0.1.3/src/pyloobins/util.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.2/PKG-INFO` & `pyloobins-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
```

