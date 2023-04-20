# Comparing `tmp/CoderElijah-0.3.6.tar.gz` & `tmp/CoderElijah-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoderElijah-0.3.6.tar", max compression
+gzip compressed data, was "CoderElijah-0.3.7.tar", max compression
```

## Comparing `CoderElijah-0.3.6.tar` & `CoderElijah-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    14248 2023-04-04 15:04:13.396875 CoderElijah-0.3.6/CoderElijah/E.py
--rw-r--r--   0        0        0       16 2023-02-06 16:48:51.371907 CoderElijah-0.3.6/CoderElijah/__init__.py
--rw-r--r--   0        0        0     9813 2023-02-07 19:18:35.632549 CoderElijah-0.3.6/CoderElijah/rickPy.py
--rw-r--r--   0        0        0     1073 2023-02-04 21:37:32.145807 CoderElijah-0.3.6/LICENSE
--rw-r--r--   0        0        0     1187 2023-04-04 15:04:17.032870 CoderElijah-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      739 2023-04-04 15:04:23.410564 CoderElijah-0.3.6/setup.py
--rw-r--r--   0        0        0      576 2023-04-04 15:04:23.410889 CoderElijah-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    14649 2023-04-20 13:13:51.279863 CoderElijah-0.3.7/CoderElijah/E.py
+-rw-r--r--   0        0        0       16 2023-02-06 16:48:51.371907 CoderElijah-0.3.7/CoderElijah/__init__.py
+-rw-r--r--   0        0        0     9813 2023-02-07 19:18:35.632549 CoderElijah-0.3.7/CoderElijah/rickPy.py
+-rw-r--r--   0        0        0     1073 2023-02-04 21:37:32.145807 CoderElijah-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1187 2023-04-20 13:14:58.419770 CoderElijah-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      739 2023-04-20 13:15:11.166613 CoderElijah-0.3.7/setup.py
+-rw-r--r--   0        0        0      576 2023-04-20 13:15:11.166996 CoderElijah-0.3.7/PKG-INFO
```

### Comparing `CoderElijah-0.3.6/CoderElijah/E.py` & `CoderElijah-0.3.7/CoderElijah/E.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,21 @@
   burntYellow = "\033[33m"
   yellow = "\033[93m"
   green = "\033[32m"
   blue = "\033[34m"
   purple = "\033[35m"
   white = "\033[37m"
 
+####################
+# ANSI Color Codes #
+####################
+class yes_no:
+  '''This contains a list of yes words (`yes`) and a list of no words (`no`).'''
+  yes = ['yes', 'yep', 'yup', 'y', 'ye', 'yuppers']
+  no = ['no', 'nope', 'nah', 'never', 'not right now']
 
 ###########################
 # Create a clear function #
 ###########################
 # Thanks to @bigminiboss on Replit.com for this clear command.
 # To use, type "clear()"
 clear = lambda: print("\033c", end="", flush=True)
@@ -199,18 +206,20 @@
   file = open(str(fileName))
   contents = file.readlines()
   return contents[lineNum].strip('\n')
   contents.close()
 ######################
 # Auto Docs Creation #
 ######################
+# Thanks to @bigminiboss on Replit.com for this function.
 def auto_docs(py_file, output_file:str='CoderElijah'):
   '''This function creates an MD file with documentation on a Python Library from the docstrings. DO NOT INCLUDE THE FILE NAME EXTENSIONS!
-  `py_file`: The name of the Py file you wish to create documentation for. Use `CoderElijah` to get docs on the CoderElijah library.
-  `output_file`: The name of your file. If left blank, it will create `CoderElijah.md`.'''
+`py_file`: The name of the Py file you wish to create documentation for. Use `CoderElijah` to get docs on the CoderElijah library.
+`output_file`: The name of your file. If left blank, it will create `CoderElijah.md`.
+Thanks to [@bigminiboss](https://replit.com/@bigminiboss] for the help with this!'''
   md = ""
   for i in dir(py_file):
       if (not i.startswith("__") and not i.endswith("__")):
           doc_string = getattr(py_file, i).__doc__
           try:
             doc_string = doc_string.split('\n')
             docs = ""
```

### Comparing `CoderElijah-0.3.6/CoderElijah/rickPy.py` & `CoderElijah-0.3.7/CoderElijah/rickPy.py`

 * *Files identical despite different names*

### Comparing `CoderElijah-0.3.6/LICENSE` & `CoderElijah-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CoderElijah-0.3.6/pyproject.toml` & `CoderElijah-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [project.urls]
 Homepage = "https://epy.coderelijah.repl.co"
 BugTracker = "https://replit.com/@coderelijah/epy?v=1"
 
 [tool.poetry]
 name = "CoderElijah"
 # name = "CoderElijahBeta"
-version = "0.3.6"
+version = "0.3.7"
 description = "This is the custom Python library of @CoderElijah on https://replit.com/."
 authors = ["CoderElijah <CoderElijah@outlook.com>"]
 packages = [{include = "CoderElijah"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 numpy = "^1.22.2"
```

### Comparing `CoderElijah-0.3.6/setup.py` & `CoderElijah-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Flask>=2.2.0,<3.0.0',
  'numpy>=1.22.2,<2.0.0',
  'replit>=3.2.4,<4.0.0',
  'urllib3>=1.26.12,<2.0.0']
 
 setup_kwargs = {
     'name': 'coderelijah',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': 'This is the custom Python library of @CoderElijah on https://replit.com/.',
     'long_description': None,
     'author': 'CoderElijah',
     'author_email': 'CoderElijah@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `CoderElijah-0.3.6/PKG-INFO` & `CoderElijah-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderelijah
-Version: 0.3.6
+Version: 0.3.7
 Summary: This is the custom Python library of @CoderElijah on https://replit.com/.
 Author: CoderElijah
 Author-email: CoderElijah@outlook.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

