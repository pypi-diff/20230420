# Comparing `tmp/pycellbase-5.3.0.tar.gz` & `tmp/pycellbase-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycellbase-5.3.0.tar", last modified: Mon Feb 20 09:45:09 2023, max compression
+gzip compressed data, was "pycellbase-5.4.0.tar", last modified: Thu Apr 20 14:55:27 2023, max compression
```

## Comparing `pycellbase-5.3.0.tar` & `pycellbase-5.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:45:09.528580 pycellbase-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-02-20 09:44:42.000000 pycellbase-5.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-20 09:44:42.000000 pycellbase-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-02-20 09:45:09.528580 pycellbase-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-02-20 09:44:42.000000 pycellbase-5.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:45:09.524579 pycellbase-5.3.0/pycellbase/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 09:44:43.000000 pycellbase-5.3.0/pycellbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-02-20 09:44:43.000000 pycellbase-5.3.0/pycellbase/cbclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-02-20 09:44:43.000000 pycellbase-5.3.0/pycellbase/cbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-02-20 09:44:43.000000 pycellbase-5.3.0/pycellbase/cbrestclients.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-02-20 09:44:43.000000 pycellbase-5.3.0/pycellbase/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:45:09.528580 pycellbase-5.3.0/pycellbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-02-20 09:45:09.000000 pycellbase-5.3.0/pycellbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-20 09:45:09.000000 pycellbase-5.3.0/pycellbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 09:45:09.000000 pycellbase-5.3.0/pycellbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 09:45:09.000000 pycellbase-5.3.0/pycellbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-20 09:45:09.000000 pycellbase-5.3.0/pycellbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-20 09:45:09.528580 pycellbase-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-20 09:44:43.000000 pycellbase-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:45:09.528580 pycellbase-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-20 09:44:43.000000 pycellbase-5.3.0/tests/test_cbcclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-20 09:44:43.000000 pycellbase-5.3.0/tests/test_cbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-02-20 09:44:43.000000 pycellbase-5.3.0/tests/test_cbrestclients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-02-20 09:44:43.000000 pycellbase-5.3.0/tests/test_commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:45:09.528580 pycellbase-5.3.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-02-20 09:44:44.000000 pycellbase-5.3.0/tools/cbtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:55:27.571627 pycellbase-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-20 14:54:54.000000 pycellbase-5.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 14:54:54.000000 pycellbase-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-04-20 14:55:27.571627 pycellbase-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-20 14:54:54.000000 pycellbase-5.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:55:27.571627 pycellbase-5.4.0/pycellbase/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 14:54:55.000000 pycellbase-5.4.0/pycellbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-20 14:54:55.000000 pycellbase-5.4.0/pycellbase/cbclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-20 14:54:55.000000 pycellbase-5.4.0/pycellbase/cbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-04-20 14:54:55.000000 pycellbase-5.4.0/pycellbase/cbrestclients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-04-20 14:54:55.000000 pycellbase-5.4.0/pycellbase/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:55:27.571627 pycellbase-5.4.0/pycellbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-04-20 14:55:27.000000 pycellbase-5.4.0/pycellbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 14:55:27.000000 pycellbase-5.4.0/pycellbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:55:27.000000 pycellbase-5.4.0/pycellbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 14:55:27.000000 pycellbase-5.4.0/pycellbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 14:55:27.000000 pycellbase-5.4.0/pycellbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 14:55:27.571627 pycellbase-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 14:54:55.000000 pycellbase-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:55:27.571627 pycellbase-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 14:54:55.000000 pycellbase-5.4.0/tests/test_cbcclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 14:54:55.000000 pycellbase-5.4.0/tests/test_cbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-04-20 14:54:55.000000 pycellbase-5.4.0/tests/test_cbrestclients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-20 14:54:55.000000 pycellbase-5.4.0/tests/test_commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:55:27.571627 pycellbase-5.4.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-04-20 14:54:56.000000 pycellbase-5.4.0/tools/cbtools.py
```

### Comparing `pycellbase-5.3.0/LICENSE.txt` & `pycellbase-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/PKG-INFO` & `pycellbase-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellbase
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python client for CellBase
 Home-page: https://github.com/opencb/cellbase/tree/develop/clients/python
 Author: Daniel Perez-Gil
 Author-email: dperezgil89@gmail.com
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/cellbase/RESTful+Web+Services
 Project-URL: Tutorial, http://docs.opencb.org/display/cellbase/Python+client+library
```

### Comparing `pycellbase-5.3.0/README.rst` & `pycellbase-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/pycellbase/cbclient.py` & `pycellbase-5.4.0/pycellbase/cbclient.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/pycellbase/cbconfig.py` & `pycellbase-5.4.0/pycellbase/cbconfig.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/pycellbase/cbrestclients.py` & `pycellbase-5.4.0/pycellbase/cbrestclients.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/pycellbase/commons.py` & `pycellbase-5.4.0/pycellbase/commons.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/pycellbase.egg-info/PKG-INFO` & `pycellbase-5.4.0/pycellbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellbase
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python client for CellBase
 Home-page: https://github.com/opencb/cellbase/tree/develop/clients/python
 Author: Daniel Perez-Gil
 Author-email: dperezgil89@gmail.com
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/cellbase/RESTful+Web+Services
 Project-URL: Tutorial, http://docs.opencb.org/display/cellbase/Python+client+library
```

### Comparing `pycellbase-5.3.0/setup.py` & `pycellbase-5.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'pycellbase',
-    'version': '5.3.0',
+    'version': '5.4.0',
     'description': 'Python client for CellBase',
     'long_description': long_description,
     'long_description_content_type': 'text/x-rst',
     'url': 'https://github.com/opencb/cellbase/tree/develop/clients/python',
     'author': 'Daniel Perez-Gil',
     'author_email': 'dperezgil89@gmail.com',
     'license': 'Apache Software License',
```

### Comparing `pycellbase-5.3.0/tests/test_cbcclient.py` & `pycellbase-5.4.0/tests/test_cbcclient.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/tests/test_cbconfig.py` & `pycellbase-5.4.0/tests/test_cbconfig.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/tests/test_cbrestclients.py` & `pycellbase-5.4.0/tests/test_cbrestclients.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/tests/test_commons.py` & `pycellbase-5.4.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `pycellbase-5.3.0/tools/cbtools.py` & `pycellbase-5.4.0/tools/cbtools.py`

 * *Files identical despite different names*

