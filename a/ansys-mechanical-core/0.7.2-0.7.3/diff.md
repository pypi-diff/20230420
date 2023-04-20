# Comparing `tmp/ansys-mechanical-core-0.7.2.tar.gz` & `tmp/ansys-mechanical-core-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-core-0.7.2.tar", last modified: Thu Apr 13 16:27:32 2023, max compression
+gzip compressed data, was "ansys-mechanical-core-0.7.3.tar", last modified: Thu Apr 20 12:11:26 2023, max compression
```

## Comparing `ansys-mechanical-core-0.7.2.tar` & `ansys-mechanical-core-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-04-13 16:27:09.947751 ansys-mechanical-core-0.7.2/LICENSE
--rw-r--r--   0        0        0     5456 2023-04-13 16:27:09.947751 ansys-mechanical-core-0.7.2/README.rst
--rw-r--r--   0        0        0     3922 2023-04-13 16:27:09.955751 ansys-mechanical-core-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      167 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     1344 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     2022 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/logging.py
--rw-r--r--   0        0        0      852 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2992 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    83310 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25079 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-20 12:11:06.263142 ansys-mechanical-core-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5456 2023-04-20 12:11:06.263142 ansys-mechanical-core-0.7.3/README.rst
+-rw-r--r--   0        0        0     3922 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      167 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     5088 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     1344 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     2022 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/logging.py
+-rw-r--r--   0        0        0      852 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2992 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    83310 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25079 2023-04-20 12:11:06.271142 ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.3/PKG-INFO
```

### Comparing `ansys-mechanical-core-0.7.2/LICENSE` & `ansys-mechanical-core-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/README.rst` & `ansys-mechanical-core-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/pyproject.toml` & `ansys-mechanical-core-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.7.2"
+version = "0.7.3"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/__init__.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/_version.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/app.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,22 @@
     def __init__(self, db_file=None, **kwargs):
         """Construct an instance of the mechanical Application.
 
         db_file is an optional path to a mechanical database file (.mechdat or .mechdb)
         you may set a version number with the `version` keyword argument.
         """
         global INSTANCES
+        from ansys.mechanical.core import BUILDING_GALLERY
+
+        if BUILDING_GALLERY:
+            if len(INSTANCES) != 0:
+                self._app = INSTANCES[0]
+                self._version = self._app.version
+                self._disposed = True
+                return
         if len(INSTANCES) > 0:
             raise Exception("Cannot have more than one embedded mechanical instance")
         self._version = kwargs.get("version")
         if self._version == None:
             self._version = _get_default_version()
         initializer.initialize(self._version)
         import clr
```

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/config.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/imports.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/initializer.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/loader.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/logging.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/resolver.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/runtime.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/shims.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/errors.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/downloads.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/launcher.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/logging.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/mechanical.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/misc.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/pool.py` & `ansys-mechanical-core-0.7.3/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.2/PKG-INFO` & `ansys-mechanical-core-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.7.2
+Version: 0.7.3
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

