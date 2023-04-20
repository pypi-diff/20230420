# Comparing `tmp/pyiron_ontology-0.1.2.tar.gz` & `tmp/pyiron_ontology-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_ontology-0.1.2.tar", last modified: Wed Apr 19 21:32:32 2023, max compression
+gzip compressed data, was "pyiron_ontology-0.1.3.tar", last modified: Thu Apr 20 21:09:49 2023, max compression
```

## Comparing `pyiron_ontology-0.1.2.tar` & `pyiron_ontology-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/reasoning.py
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/example/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/pyiron_ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/pyiron_ontology/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/pyiron_ontology/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/atomistics/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/atomistics/reasoning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/pyiron_ontology/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/example/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/pyiron_ontology/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/pyiron_ontology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-20 21:09:49.609323 pyiron_ontology-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-20 21:09:49.000000 pyiron_ontology-0.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-20 21:09:42.000000 pyiron_ontology-0.1.3/versioneer.py
```

### Comparing `pyiron_ontology-0.1.2/LICENSE` & `pyiron_ontology-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/PKG-INFO` & `pyiron_ontology-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_ontology
-Version: 0.1.2
+Version: 0.1.3
 Summary: pyiron_ontology - module extension to pyiron.
 Home-page: https://github.com/pyiron/pyiron_ontology
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_ontology-0.1.2/README.md` & `pyiron_ontology-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/atomistics/constructor.py` & `pyiron_ontology-0.1.3/pyiron_ontology/atomistics/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/atomistics/reasoning.py` & `pyiron_ontology-0.1.3/pyiron_ontology/atomistics/reasoning.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/constructor.py` & `pyiron_ontology-0.1.3/pyiron_ontology/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/dynamic.py` & `pyiron_ontology-0.1.3/pyiron_ontology/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/example/constructor.py` & `pyiron_ontology-0.1.3/pyiron_ontology/example/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology/workflow.py` & `pyiron_ontology-0.1.3/pyiron_ontology/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology.egg-info/PKG-INFO` & `pyiron_ontology-0.1.3/pyiron_ontology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-ontology
-Version: 0.1.2
+Version: 0.1.3
 Summary: pyiron_ontology - module extension to pyiron.
 Home-page: https://github.com/pyiron/pyiron_ontology
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_ontology-0.1.2/pyiron_ontology.egg-info/SOURCES.txt` & `pyiron_ontology-0.1.3/pyiron_ontology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.2/setup.py` & `pyiron_ontology-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,11 @@
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'numpy',
         'owlready2',
         'pandas',
         'pint',
         'pyiron_atomistics>=0.2.63',
-        'sqlalchemy',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron_ontology-0.1.2/versioneer.py` & `pyiron_ontology-0.1.3/versioneer.py`

 * *Files identical despite different names*

