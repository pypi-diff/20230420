# Comparing `tmp/zpretty-3.0.3.tar.gz` & `tmp/zpretty-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpretty-3.0.3.tar", last modified: Sun Mar 26 06:58:56 2023, max compression
+gzip compressed data, was "zpretty-3.0.4.tar", last modified: Thu Apr 20 13:32:40 2023, max compression
```

## Comparing `zpretty-3.0.3.tar` & `zpretty-3.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/
--rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-03-26 06:58:55.000000 zpretty-3.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-03-26 06:58:55.000000 zpretty-3.0.3/.pre-commit-hooks.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)     3695 2023-03-26 06:58:55.000000 zpretty-3.0.3/HISTORY.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-03-26 06:58:55.000000 zpretty-3.0.3/LICENSE
--rw-rw-r--   0 ale       (1000) ale       (1000)      196 2023-03-26 06:58:55.000000 zpretty-3.0.3/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      808 2023-03-26 06:58:55.000000 zpretty-3.0.3/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)     8550 2023-03-26 06:58:56.625137 zpretty-3.0.3/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     3947 2023-03-26 06:58:55.000000 zpretty-3.0.3/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-03-26 06:58:55.000000 zpretty-3.0.3/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-03-26 06:58:55.000000 zpretty-3.0.3/requirements-dev.txt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/requirements.d/
--rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-03-26 06:58:55.000000 zpretty-3.0.3/requirements.d/requirements-dev-37.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-03-26 06:58:55.000000 zpretty-3.0.3/requirements.d/requirements-dev.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-03-26 06:58:56.625137 zpretty-3.0.3/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1563 2023-03-26 06:58:55.000000 zpretty-3.0.3/setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-03-26 06:58:55.000000 zpretty-3.0.3/tox.ini
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/zpretty/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7077 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4537 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4798 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/prettifier.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/zpretty/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/zpretty/tests/broken/
--rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/broken/broken.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/mock.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/zpretty/tests/original/
--rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_dtml.dtml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_html.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_html4.html
--rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1283 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_pt.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/sample_xml.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/original/text_with_markup.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3241 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_functions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_readme.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_zcml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6845 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/tests/test_zpretty.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/text.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-03-26 06:58:55.000000 zpretty-3.0.3/zpretty/zcml.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-03-26 06:58:56.621137 zpretty-3.0.3/zpretty.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)     8550 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1290 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-03-26 06:58:56.000000 zpretty-3.0.3/zpretty.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-04-20 13:32:40.000000 zpretty-3.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-04-20 13:32:40.000000 zpretty-3.0.4/.pre-commit-hooks.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3785 2023-04-20 13:32:40.000000 zpretty-3.0.4/HISTORY.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-04-20 13:32:40.000000 zpretty-3.0.4/LICENSE
+-rw-rw-r--   0 ale       (1000) ale       (1000)      196 2023-04-20 13:32:40.000000 zpretty-3.0.4/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)      808 2023-04-20 13:32:40.000000 zpretty-3.0.4/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8453 2023-04-20 13:32:40.178341 zpretty-3.0.4/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3760 2023-04-20 13:32:40.000000 zpretty-3.0.4/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-04-20 13:32:40.000000 zpretty-3.0.4/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements-dev.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.174341 zpretty-3.0.4/requirements.d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements.d/requirements-dev-37.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements.d/requirements-dev.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-04-20 13:32:40.178341 zpretty-3.0.4/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1563 2023-04-20 13:32:40.000000 zpretty-3.0.4/setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-04-20 13:32:40.000000 zpretty-3.0.4/tox.ini
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7077 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4537 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5242 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/prettifier.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/broken/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/broken/broken.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/mock.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/original/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_dtml.dtml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html4.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1283 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_pt.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_xml.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/text_with_markup.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3241 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_functions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_readme.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_zcml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7763 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_zpretty.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/text.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/zcml.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8453 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1290 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/top_level.txt
```

### Comparing `zpretty-3.0.3/.pre-commit-config.yaml` & `zpretty-3.0.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/PyCQA/flake8
```

### Comparing `zpretty-3.0.3/HISTORY.md` & `zpretty-3.0.4/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog
 
-3.0.3 (2023-03-26)
+## 3.0.4 (2023-04-20)
+
+- Fix bogus ampersands in attributes
+  (Fixes #116)
+  [ale-rt]
+
+## 3.0.3 (2023-03-26)
 
 - Handle HTML files with an XML preamble before the doctype.
   (Fixes #118)
   [ale-rt]
 
 ## 3.0.2 (2023-02-26)
```

### Comparing `zpretty-3.0.3/LICENSE` & `zpretty-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/Makefile` & `zpretty-3.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/PKG-INFO` & `zpretty-3.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.0.3
+Version: 3.0.4
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -144,23 +144,23 @@
 
 # RUNNING TESTS
 
 ```bash
 make test
 ```
 
-# TODO
+# Changelog
 
-- [ ] Valueless attributes are not allowed in XML
-- [ ] Attributes are aligned in a strange way if previous sibling has no spaces
-- [ ] TBD: Style attributes should be multiline
+## 3.0.4 (2023-04-20)
 
-# Changelog
+- Fix bogus ampersands in attributes
+  (Fixes #116)
+  [ale-rt]
 
-3.0.3 (2023-03-26)
+## 3.0.3 (2023-03-26)
 
 - Handle HTML files with an XML preamble before the doctype.
   (Fixes #118)
   [ale-rt]
 
 ## 3.0.2 (2023-02-26)
```

### Comparing `zpretty-3.0.3/README.md` & `zpretty-3.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -118,13 +118,7 @@
 ```
 
 # RUNNING TESTS
 
 ```bash
 make test
 ```
-
-# TODO
-
-- [ ] Valueless attributes are not allowed in XML
-- [ ] Attributes are aligned in a strange way if previous sibling has no spaces
-- [ ] TBD: Style attributes should be multiline
```

### Comparing `zpretty-3.0.3/requirements.d/requirements-dev-37.txt` & `zpretty-3.0.4/requirements.d/requirements-dev-37.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 mccabe==0.6.1
 mypy-extensions==0.4.3
 packaging==20.8
 pathspec==0.8.1
 pep517==0.9.1
 pkginfo==1.6.1
 pluggy==0.13.1
-py==1.10.0
+py==1.11.0
 pycodestyle==2.6.0
 pycparser==2.20
 pyflakes==2.2.0
 Pygments==2.7.4
 pyparsing==2.4.7
 pyroma==2.6
 pytest==6.2.1
```

### Comparing `zpretty-3.0.3/requirements.d/requirements-dev.txt` & `zpretty-3.0.4/requirements.d/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/setup.py` & `zpretty-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name="zpretty",
-    version="3.0.3",
+    version="3.0.4",
     description="An opinionated HTML/XML soup formatter",
     keywords=["Formatter", "HTML", "Prettifier", "Pretty print", "TAL", "XML", "ZPT"],
     long_description="\n".join((read("README.md"), read("HISTORY.md"))),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `zpretty-3.0.3/tox.ini` & `zpretty-3.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/attributes.py` & `zpretty-3.0.4/zpretty/attributes.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/cli.py` & `zpretty-3.0.4/zpretty/cli.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/elements.py` & `zpretty-3.0.4/zpretty/elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/prettifier.py` & `zpretty-3.0.4/zpretty/prettifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,25 @@
         self.filename = filename
         if self.filename:
             text = "".join(fileinput.input([filename]))
         if not isinstance(text, str):
             text = text.decode(self.encoding)
         self.original_text = text
         self.text = self._prepare_text()
-        self.soup = self.get_soup(self.text)
+        soup = self.get_soup(self.text)
+        # Workaround for https://github.com/collective/zpretty/issues/116
+        # restore the ampersands
+        # in the attributes so that bogus ones can be escaped
+        for el in soup.descendants:
+            attrs = getattr(el, "attrs", {})
+            for key, value in attrs.items():
+                if self._ampersand_marker in value:
+                    attrs[key] = value.replace(self._ampersand_marker, "&")
+
+        self.soup = soup
 
         # Cleanup all spurious self._newlines_marker attributes, see #35
         key = self._newlines_marker.partition("=")[0]
         for el in self.soup.find_all(attrs={key: ""}):
             el.attrs.pop(key, None)
 
         self.root = self.pretty_element(self.soup, -1)
```

### Comparing `zpretty-3.0.3/zpretty/tests/original/sample.zcml` & `zpretty-3.0.4/zpretty/tests/original/sample.zcml`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/original/sample_html.html` & `zpretty-3.0.4/zpretty/tests/original/sample_html.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/original/sample_html4.html` & `zpretty-3.0.4/zpretty/tests/original/sample_html4.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/original/sample_pt.pt` & `zpretty-3.0.4/zpretty/tests/original/sample_pt.pt`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/original/sample_xml.xml` & `zpretty-3.0.4/zpretty/tests/original/sample_xml.xml`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_attributes.py` & `zpretty-3.0.4/zpretty/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_cli.py` & `zpretty-3.0.4/zpretty/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_elements.py` & `zpretty-3.0.4/zpretty/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_functions.py` & `zpretty-3.0.4/zpretty/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_readme.py` & `zpretty-3.0.4/zpretty/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_xml.py` & `zpretty-3.0.4/zpretty/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_zcml.py` & `zpretty-3.0.4/zpretty/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/tests/test_zpretty.py` & `zpretty-3.0.4/zpretty/tests/test_zpretty.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,14 +167,28 @@
 
     def test_entities(self):
         self.assertPrettified("<root>&nbsp;</root>", "<root>&nbsp;</root>\n")
 
     def test_single_quotes_in_attrs(self):
         self.assertPrettified('<root a="\'" />', '<root a="\'"></root>\n')
 
+    def test_ampersand_in_attrs(self):
+        self.assertPrettified('<root a="&" />', '<root a="&amp;"></root>\n')
+        self.assertPrettified('<root a="foo &" />', '<root a="foo &amp;"></root>\n')
+        self.assertPrettified('<root a="& bar" />', '<root a="&amp; bar"></root>\n')
+        self.assertPrettified('<root a=";&" />', '<root a=";&amp;"></root>\n')
+        self.assertPrettified('<root a="&;" />', '<root a="&amp;;"></root>\n')
+
+    def test_escaped_ampersand_in_attrs(self):
+        self.assertPrettified('<root a="&amp;" />', '<root a="&amp;"></root>\n')
+        self.assertPrettified('<root a="foo &amp;" />', '<root a="foo &amp;"></root>\n')
+        self.assertPrettified('<root a="&amp; bar" />', '<root a="&amp; bar"></root>\n')
+        self.assertPrettified('<root a=";&amp;" />', '<root a=";&amp;"></root>\n')
+        self.assertPrettified('<root a="&amp;;" />', '<root a="&amp;;"></root>\n')
+
     def test_sample_html(self):
         self.prettify("sample_html.html")
 
     def test_sample_html4(self):
         self.prettify("sample_html4.html")
 
     def test_sample_html_with_preprocessing_instruction(self):
```

### Comparing `zpretty-3.0.3/zpretty/text.py` & `zpretty-3.0.4/zpretty/text.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/xml.py` & `zpretty-3.0.4/zpretty/xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty/zcml.py` & `zpretty-3.0.4/zpretty/zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.3/zpretty.egg-info/PKG-INFO` & `zpretty-3.0.4/zpretty.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.0.3
+Version: 3.0.4
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -144,23 +144,23 @@
 
 # RUNNING TESTS
 
 ```bash
 make test
 ```
 
-# TODO
+# Changelog
 
-- [ ] Valueless attributes are not allowed in XML
-- [ ] Attributes are aligned in a strange way if previous sibling has no spaces
-- [ ] TBD: Style attributes should be multiline
+## 3.0.4 (2023-04-20)
 
-# Changelog
+- Fix bogus ampersands in attributes
+  (Fixes #116)
+  [ale-rt]
 
-3.0.3 (2023-03-26)
+## 3.0.3 (2023-03-26)
 
 - Handle HTML files with an XML preamble before the doctype.
   (Fixes #118)
   [ale-rt]
 
 ## 3.0.2 (2023-02-26)
```

### Comparing `zpretty-3.0.3/zpretty.egg-info/SOURCES.txt` & `zpretty-3.0.4/zpretty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

