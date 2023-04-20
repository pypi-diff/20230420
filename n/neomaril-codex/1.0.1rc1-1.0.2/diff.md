# Comparing `tmp/neomaril-codex-1.0.1rc1.tar.gz` & `tmp/neomaril-codex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomaril-codex-1.0.1rc1.tar", last modified: Wed Mar 15 20:27:49 2023, max compression
+gzip compressed data, was "neomaril-codex-1.0.2.tar", last modified: Thu Apr 20 18:31:18 2023, max compression
```

## Comparing `neomaril-codex-1.0.1rc1.tar` & `neomaril-codex-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-03-15 20:27:49.068556 neomaril-codex-1.0.1rc1/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.1rc1/LICENSE.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.1rc1/MANIFEST.in
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      365 2023-03-15 20:27:49.068556 neomaril-codex-1.0.1rc1/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.1rc1/README.md
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-02-08 17:56:54.000000 neomaril-codex-1.0.1rc1/requirements.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-03-15 20:27:49.068556 neomaril-codex-1.0.1rc1/setup.cfg
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      931 2023-03-15 19:34:38.000000 neomaril-codex-1.0.1rc1/setup.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-03-15 20:27:49.060556 neomaril-codex-1.0.1rc1/src/
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-03-15 20:27:49.064556 neomaril-codex-1.0.1rc1/src/neomaril_codex/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/__init__.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    11916 2023-03-08 12:49:14.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/base.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/exceptions.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/logging.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    38969 2023-03-15 18:52:32.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/model.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12504 2023-03-08 12:49:14.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/pipeline.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    28922 2023-03-14 19:55:40.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/training.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-03-07 18:36:14.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex/utils.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-03-15 20:27:49.068556 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      365 2023-03-15 20:27:48.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-03-15 20:27:49.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-03-15 20:27:48.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-02-07 14:57:39.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-03-15 20:27:48.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/requires.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-03-15 20:27:48.000000 neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.2/LICENSE.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.2/MANIFEST.in
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      359 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.2/README.md
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/requirements.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/setup.cfg
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      928 2023-04-20 18:30:27.000000 neomaril-codex-1.0.2/setup.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.288173 neomaril-codex-1.0.2/src/
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/src/neomaril_codex/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/__init__.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    11916 2023-03-08 12:49:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/base.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/exceptions.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.2/src/neomaril_codex/logging.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    38969 2023-03-15 18:52:32.000000 neomaril-codex-1.0.2/src/neomaril_codex/model.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12504 2023-03-08 12:49:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/pipeline.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    28919 2023-04-20 18:30:54.000000 neomaril-codex-1.0.2/src/neomaril_codex/training.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-03-07 18:36:14.000000 neomaril-codex-1.0.2/src/neomaril_codex/utils.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-04-20 18:31:18.292173 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      359 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-02-07 14:57:39.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/requires.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-04-20 18:31:18.000000 neomaril-codex-1.0.2/src/neomaril_codex.egg-info/top_level.txt
```

### Comparing `neomaril-codex-1.0.1rc1/LICENSE.txt` & `neomaril-codex-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/README.md` & `neomaril-codex-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/setup.py` & `neomaril-codex-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os.path import join
 
 from setuptools import setup, find_packages
 
 MODULE_NAME = 'neomaril-codex'
 MODULE_NAME_IMPORT = 'neomaril_codex'
 REPO_NAME = 'mlops-neomaril-codex'
-MODULE_VERSION='1.0.1rc1'
+MODULE_VERSION='1.0.2'
 
 def requirements_from_pip(filename='requirements.txt'):
     with open(filename, 'r') as pip:
         return [l.strip() for l in pip if not l.startswith('#') and l.strip()]
 
 
 setup(name=MODULE_NAME,
```

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/base.py` & `neomaril-codex-1.0.2/src/neomaril_codex/base.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/exceptions.py` & `neomaril-codex-1.0.2/src/neomaril_codex/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/logging.py` & `neomaril-codex-1.0.2/src/neomaril_codex/logging.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/model.py` & `neomaril-codex-1.0.2/src/neomaril_codex/model.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/pipeline.py` & `neomaril-codex-1.0.2/src/neomaril_codex/pipeline.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/training.py` & `neomaril-codex-1.0.2/src/neomaril_codex/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         form_data = {'name': model_name, 'operation': operation}
         upload_data = []
 
         if self.training_type == 'Custom':
             form_data['model_reference'] = model_reference
             form_data['input_type'] = input_type
         
-            file_extesions = {'py': 'script.py', 'ipynb': "notebook.ipynb"}
+            file_extesions = {'py': 'app.py', 'ipynb': "notebook.ipynb"}
         
 
             upload_data = [
                 ("source", (file_extesions[source_file.split('.')[-1]], open(source_file, "r")))
             ]
 
             if env:
```

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex/utils.py` & `neomaril-codex-1.0.2/src/neomaril_codex/utils.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.1rc1/src/neomaril_codex.egg-info/SOURCES.txt` & `neomaril-codex-1.0.2/src/neomaril_codex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

