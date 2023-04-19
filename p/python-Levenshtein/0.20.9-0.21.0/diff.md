# Comparing `tmp/python-Levenshtein-0.20.9.tar.gz` & `tmp/python-Levenshtein-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-Levenshtein-0.20.9.tar", last modified: Sun Dec 25 19:20:40 2022, max compression
+gzip compressed data, was "python-Levenshtein-0.21.0.tar", last modified: Wed Apr 19 23:02:01 2023, max compression
```

## Comparing `python-Levenshtein-0.20.9.tar` & `python-Levenshtein-0.21.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 19:20:40.868728 python-Levenshtein-0.20.9/
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2022-12-25 19:20:31.000000 python-Levenshtein-0.20.9/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2022-12-25 19:20:31.000000 python-Levenshtein-0.20.9/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-25 19:20:31.000000 python-Levenshtein-0.20.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2022-12-25 19:20:40.868728 python-Levenshtein-0.20.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2022-12-25 19:20:31.000000 python-Levenshtein-0.20.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-25 19:20:31.000000 python-Levenshtein-0.20.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 19:20:40.868728 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2022-12-25 19:20:40.000000 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-25 19:20:40.000000 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 19:20:40.000000 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-25 19:20:40.000000 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 19:20:40.000000 python-Levenshtein-0.20.9/python_Levenshtein.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-25 19:20:40.868728 python-Levenshtein-0.20.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/setup.cfg
```

### Comparing `python-Levenshtein-0.20.9/COPYING` & `python-Levenshtein-0.21.0/COPYING`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.20.9/HISTORY.md` & `python-Levenshtein-0.21.0/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## Changelog
 
+### v0.21.0
+#### Changed
+- relax dependency requirement on ``rapidfuzz``
+
 ### v0.20.9
 #### Fixed
 - fix function signature of `get_requires_for_build_wheel`
 
 ### v0.20.8
 #### Fixed
 - type hints for `editops`/`opcoded`/`matching_blocks` did not allow any
```

### Comparing `python-Levenshtein-0.20.9/PKG-INFO` & `python-Levenshtein-0.21.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.20.9
+Version: 0.21.0
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/maxbachmann/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.20.9 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.0 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/maxbachmann/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `python-Levenshtein-0.20.9/README.md` & `python-Levenshtein-0.21.0/README.md`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.20.9/python_Levenshtein.egg-info/PKG-INFO` & `python-Levenshtein-0.21.0/python_Levenshtein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.20.9
+Version: 0.21.0
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/maxbachmann/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.20.9 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.0 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/maxbachmann/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `python-Levenshtein-0.20.9/setup.cfg` & `python-Levenshtein-0.21.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-Levenshtein
-version = 0.20.9
+version = 0.21.0
 description = Python extension for computing string edit distances and similarities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Max Bachmann
 author_email = pypi@maxbachmann.de
 url = https://github.com/maxbachmann/python-Levenshtein
 license = GPL-2.0-or-later
@@ -18,13 +18,13 @@
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 keywords = string, Levenshtein, comparison, edit-distance
 
 [options]
 python_requires = >=3.6
 install_requires = 
-	Levenshtein==0.20.9
+	Levenshtein==0.21.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

