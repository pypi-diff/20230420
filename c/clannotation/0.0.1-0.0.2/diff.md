# Comparing `tmp/clannotation-0.0.1.tar.gz` & `tmp/clannotation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clannotation-0.0.1.tar", last modified: Thu Apr 20 08:54:18 2023, max compression
+gzip compressed data, was "clannotation-0.0.2.tar", last modified: Thu Apr 20 10:32:51 2023, max compression
```

## Comparing `clannotation-0.0.1.tar` & `clannotation-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:54:18.315003 clannotation-0.0.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.1/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     2840 2023-04-20 08:54:18.315003 clannotation-0.0.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      980 2023-04-20 08:53:48.000000 clannotation-0.0.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-04-20 08:42:10.000000 clannotation-0.0.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-04-20 08:54:18.315003 clannotation-0.0.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:54:18.315003 clannotation-0.0.1/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:54:18.315003 clannotation-0.0.1/src/clannotation/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.1/src/clannotation/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10726 2023-04-20 08:48:40.000000 clannotation-0.0.1/src/clannotation/annotator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:54:18.315003 clannotation-0.0.1/src/clannotation.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2840 2023-04-20 08:54:18.000000 clannotation-0.0.1/src/clannotation.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-04-20 08:54:18.000000 clannotation-0.0.1/src/clannotation.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-20 08:54:18.000000 clannotation-0.0.1/src/clannotation.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-04-20 08:54:18.000000 clannotation-0.0.1/src/clannotation.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-04-20 08:54:18.000000 clannotation-0.0.1/src/clannotation.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:54:18.315003 clannotation-0.0.1/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.1/tests/test_annotator_plugin.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 10:32:51.771948 clannotation-0.0.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.2/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-20 10:32:51.771948 clannotation-0.0.2/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      986 2023-04-20 09:30:48.000000 clannotation-0.0.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-04-20 10:27:48.000000 clannotation-0.0.2/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-04-20 10:32:51.771948 clannotation-0.0.2/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 10:32:51.771948 clannotation-0.0.2/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 10:32:51.771948 clannotation-0.0.2/src/clannotation/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.2/src/clannotation/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10752 2023-04-20 10:27:47.000000 clannotation-0.0.2/src/clannotation/annotator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 10:32:51.771948 clannotation-0.0.2/src/clannotation.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-04-20 10:32:51.000000 clannotation-0.0.2/src/clannotation.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-04-20 10:32:51.000000 clannotation-0.0.2/src/clannotation.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-20 10:32:51.000000 clannotation-0.0.2/src/clannotation.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-04-20 10:32:51.000000 clannotation-0.0.2/src/clannotation.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-04-20 10:32:51.000000 clannotation-0.0.2/src/clannotation.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 10:32:51.771948 clannotation-0.0.2/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.2/tests/test_annotator_plugin.py
```

### Comparing `clannotation-0.0.1/LICENSE.md` & `clannotation-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.1/PKG-INFO` & `clannotation-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # CLAnnotator: Crossref Labs Annotator 
 CLAnnotator is the module that Crossref Labs uses to decorate the experimental API.
 
-![license](https://img.shields.io/gitlab/license/crossref/labs/annotator) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/annotator)
+![license](https://img.shields.io/gitlab/license/crossref/labs/clannotation) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/clannotation)
 
 ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 This is a prototype Crossref Labs system. It is not guaranteed to be stable and the metadata schema and behaviour may be subject to change at any time.
 
 ## Installation
```

### Comparing `clannotation-0.0.1/README.md` & `clannotation-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CLAnnotator: Crossref Labs Annotator 
 CLAnnotator is the module that Crossref Labs uses to decorate the experimental API.
 
-![license](https://img.shields.io/gitlab/license/crossref/labs/annotator) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/annotator)
+![license](https://img.shields.io/gitlab/license/crossref/labs/clannotation) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/clannotation)
 
 ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 This is a prototype Crossref Labs system. It is not guaranteed to be stable and the metadata schema and behaviour may be subject to change at any time.
 
 ## Installation
```

### Comparing `clannotation-0.0.1/pyproject.toml` & `clannotation-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clannotation"
-version = "0.0.1"
+version = "0.0.2"
 description = "The Crossref Labs annotation tool."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["API", "Crossref", "annotation", "AWS", "Lambda"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `clannotation-0.0.1/setup.cfg` & `clannotation-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clannotation
-version = 0.0.1
+version = 0.0.2
 description = The Crossref Labs annotation tool.
 url = https://gitlab.com/crossref/labs/annotator
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `clannotation-0.0.1/src/clannotation/annotator.py` & `clannotation-0.0.2/src/clannotation/annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         for item in annotation_list:
             final_response["message"]["items"][item_count][
                 f"{self._settings.LABS_PREFIX}{Path(item).stem}"
             ] = {}
 
             # locate the right annotation
             for annotation in annotation_files:
-                if item in annotation:
+                if item in annotation and self._instrumentation:
                     self._instrumentation.logger.info(
                         f"Patching item {item_count} from ({item})"
                     )
 
                     final_response["message"]["items"][item_count][
                         f"{self._settings.LABS_PREFIX}{Path(item).stem}"
                     ] = json.loads(annotation[item])
```

### Comparing `clannotation-0.0.1/src/clannotation.egg-info/PKG-INFO` & `clannotation-0.0.2/src/clannotation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # CLAnnotator: Crossref Labs Annotator 
 CLAnnotator is the module that Crossref Labs uses to decorate the experimental API.
 
-![license](https://img.shields.io/gitlab/license/crossref/labs/annotator) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/annotator)
+![license](https://img.shields.io/gitlab/license/crossref/labs/clannotation) ![activity](https://img.shields.io/gitlab/last-commit/crossref/labs/clannotation)
 
 ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 This is a prototype Crossref Labs system. It is not guaranteed to be stable and the metadata schema and behaviour may be subject to change at any time.
 
 ## Installation
```

### Comparing `clannotation-0.0.1/tests/test_annotator_plugin.py` & `clannotation-0.0.2/tests/test_annotator_plugin.py`

 * *Files identical despite different names*

