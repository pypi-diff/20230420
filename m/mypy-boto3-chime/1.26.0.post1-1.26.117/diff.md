# Comparing `tmp/mypy-boto3-chime-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-chime-1.26.117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:09 2022, max compression
+gzip compressed data, was "mypy-boto3-chime-1.26.117.tar", last modified: Thu Apr 20 19:33:48 2023, max compression
```

## Comparing `mypy-boto3-chime-1.26.0.post1.tar` & `mypy-boto3-chime-1.26.117.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.880837 mypy-boto3-chime-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    32537 2022-11-01 21:43:09.880837 mypy-boto3-chime-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    31104 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.880837 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   121634 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (121)   121434 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12767 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12765 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-11-01 21:31:08.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   144519 2022-11-01 21:31:11.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   144358 2022-11-01 21:31:10.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.880837 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    32537 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-01 21:43:09.000000 mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:09.880837 mypy-boto3-chime-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-11-01 21:31:07.000000 mypy-boto3-chime-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.467264 mypy-boto3-chime-1.26.117/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121614 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121414 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-20 19:32:23.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-20 19:32:23.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144436 2023-04-20 19:32:27.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144277 2023-04-20 19:32:25.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:33:48.467264 mypy-boto3-chime-1.26.117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-20 19:32:20.000000 mypy-boto3-chime-1.26.117/setup.py
```

### Comparing `mypy-boto3-chime-1.26.0.post1/LICENSE` & `mypy-boto3-chime-1.26.117/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-chime-1.26.0.post1/PKG-INFO` & `mypy-boto3-chime-1.26.117/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Chime 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.117
+Summary: Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -818,42 +819,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-1.26.0.post1/README.md` & `mypy-boto3-chime-1.26.117/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -787,42 +787,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Chime 1.26.117\nVersion:         1.26.117\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.117")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,15 +670,15 @@
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
-        `sipMediaApplicationId` .
+        `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_sip_media_application_call)
         """
 
     def create_sip_rule(
         self,
@@ -754,23 +754,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_admin)
         """
 
     def delete_app_instance_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the streaming configurations of an `AppInstance` .
+        Deletes the streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_streaming_configurations)
         """
 
     def delete_app_instance_user(self, *, AppInstanceUserArn: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes an `AppInstanceUser` .
+        Deletes an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_user)
         """
 
     def delete_attendee(self, *, MeetingId: str, AttendeeId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -994,45 +994,45 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_voice_connector_termination_credentials)
         """
 
     def describe_app_instance(self, *, AppInstanceArn: str) -> DescribeAppInstanceResponseTypeDef:
         """
-        Returns the full details of an `AppInstance` .
+        Returns the full details of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance)
         """
 
     def describe_app_instance_admin(
         self, *, AppInstanceAdminArn: str, AppInstanceArn: str
     ) -> DescribeAppInstanceAdminResponseTypeDef:
         """
-        Returns the full details of an `AppInstanceAdmin` .
+        Returns the full details of an `AppInstanceAdmin`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance_admin)
         """
 
     def describe_app_instance_user(
         self, *, AppInstanceUserArn: str
     ) -> DescribeAppInstanceUserResponseTypeDef:
         """
-        Returns the full details of an `AppInstanceUser` .
+        Returns the full details of an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance_user)
         """
 
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelResponseTypeDef:
         """
-        Returns the full details of a channel in an Amazon Chime `AppInstance` .
+        Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel)
         """
 
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str = ...
@@ -1055,26 +1055,26 @@
         """
 
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
-        `AppInstanceUser` .
+        `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel_membership_for_app_instance_user)
         """
 
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
-        `AppInstanceUser` .
+        `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel_moderated_by_app_instance_user)
         """
 
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str = ...
@@ -1160,25 +1160,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_account_settings)
         """
 
     def get_app_instance_retention_settings(
         self, *, AppInstanceArn: str
     ) -> GetAppInstanceRetentionSettingsResponseTypeDef:
         """
-        Gets the retention settings for an `AppInstance` .
+        Gets the retention settings for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_app_instance_retention_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_app_instance_retention_settings)
         """
 
     def get_app_instance_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> GetAppInstanceStreamingConfigurationsResponseTypeDef:
         """
-        Gets the streaming settings for an `AppInstance` .
+        Gets the streaming settings for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_app_instance_streaming_configurations)
         """
 
     def get_attendee(self, *, MeetingId: str, AttendeeId: str) -> GetAttendeeResponseTypeDef:
         """
@@ -1381,15 +1381,15 @@
         """
 
     def get_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> GetVoiceConnectorGroupResponseTypeDef:
         """
         Retrieves details for the specified Amazon Chime Voice Connector group, such as
-        timestamps,name, and associated `VoiceConnectorItems` .
+        timestamps,name, and associated `VoiceConnectorItems`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_group)
         """
 
     def get_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str
@@ -1478,35 +1478,35 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_accounts)
         """
 
     def list_app_instance_admins(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstanceAdminsResponseTypeDef:
         """
-        Returns a list of the administrators in the `AppInstance` .
+        Returns a list of the administrators in the `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instance_admins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instance_admins)
         """
 
     def list_app_instance_users(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstanceUsersResponseTypeDef:
         """
-        List all `AppInstanceUsers` created under a single `AppInstance` .
+        List all `AppInstanceUsers` created under a single `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instance_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instance_users)
         """
 
     def list_app_instances(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstancesResponseTypeDef:
         """
-        Lists all Amazon Chime `AppInstance` s created under a single AWS account.
+        Lists all Amazon Chime `AppInstance`s created under a single AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instances)
         """
 
     def list_attendee_tags(
         self, *, MeetingId: str, AttendeeId: str
@@ -1639,15 +1639,15 @@
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
-        A list of the channels moderated by an `AppInstanceUser` .
+        A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_channels_moderated_by_app_instance_user)
         """
 
     def list_media_capture_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
@@ -1851,15 +1851,15 @@
     def put_app_instance_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
         AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef]
     ) -> PutAppInstanceStreamingConfigurationsResponseTypeDef:
         """
-        The data streaming configurations of an `AppInstance` .
+        The data streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_app_instance_streaming_configurations)
         """
 
     def put_events_configuration(
         self,
@@ -2027,15 +2027,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.reset_personal_pin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#reset_personal_pin)
         """
 
     def restore_phone_number(self, *, PhoneNumberId: str) -> RestorePhoneNumberResponseTypeDef:
         """
         Moves a phone number from the **Deletion queue** back into the phone number
-        **Inventory** .
+        **Inventory**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.restore_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#restore_phone_number)
         """
 
     def search_available_phone_numbers(
         self,
@@ -2074,23 +2074,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#send_channel_message)
         """
 
     def start_meeting_transcription(
         self, *, MeetingId: str, TranscriptionConfiguration: TranscriptionConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
-        Starts transcription for the specified `meetingId` .
+        Starts transcription for the specified `meetingId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.start_meeting_transcription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#start_meeting_transcription)
         """
 
     def stop_meeting_transcription(self, *, MeetingId: str) -> Dict[str, Any]:
         """
-        Stops transcription for the specified `meetingId` .
+        Stops transcription for the specified `meetingId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.stop_meeting_transcription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#stop_meeting_transcription)
         """
 
     def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -632,15 +632,15 @@
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
-        `sipMediaApplicationId` .
+        `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_sip_media_application_call)
         """
     def create_sip_rule(
         self,
         *,
@@ -708,22 +708,22 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_app_instance_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_admin)
         """
     def delete_app_instance_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the streaming configurations of an `AppInstance` .
+        Deletes the streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_streaming_configurations)
         """
     def delete_app_instance_user(self, *, AppInstanceUserArn: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes an `AppInstanceUser` .
+        Deletes an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_app_instance_user)
         """
     def delete_attendee(self, *, MeetingId: str, AttendeeId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an attendee from the specified Amazon Chime SDK meeting and deletes
@@ -923,42 +923,42 @@
         during call termination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#delete_voice_connector_termination_credentials)
         """
     def describe_app_instance(self, *, AppInstanceArn: str) -> DescribeAppInstanceResponseTypeDef:
         """
-        Returns the full details of an `AppInstance` .
+        Returns the full details of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance)
         """
     def describe_app_instance_admin(
         self, *, AppInstanceAdminArn: str, AppInstanceArn: str
     ) -> DescribeAppInstanceAdminResponseTypeDef:
         """
-        Returns the full details of an `AppInstanceAdmin` .
+        Returns the full details of an `AppInstanceAdmin`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance_admin)
         """
     def describe_app_instance_user(
         self, *, AppInstanceUserArn: str
     ) -> DescribeAppInstanceUserResponseTypeDef:
         """
-        Returns the full details of an `AppInstanceUser` .
+        Returns the full details of an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_app_instance_user)
         """
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelResponseTypeDef:
         """
-        Returns the full details of a channel in an Amazon Chime `AppInstance` .
+        Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel)
         """
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelBanResponseTypeDef:
@@ -978,25 +978,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel_membership)
         """
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
-        `AppInstanceUser` .
+        `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel_membership_for_app_instance_user)
         """
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
-        `AppInstanceUser` .
+        `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#describe_channel_moderated_by_app_instance_user)
         """
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str = ...
     ) -> DescribeChannelModeratorResponseTypeDef:
@@ -1073,24 +1073,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_account_settings)
         """
     def get_app_instance_retention_settings(
         self, *, AppInstanceArn: str
     ) -> GetAppInstanceRetentionSettingsResponseTypeDef:
         """
-        Gets the retention settings for an `AppInstance` .
+        Gets the retention settings for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_app_instance_retention_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_app_instance_retention_settings)
         """
     def get_app_instance_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> GetAppInstanceStreamingConfigurationsResponseTypeDef:
         """
-        Gets the streaming settings for an `AppInstance` .
+        Gets the streaming settings for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_app_instance_streaming_configurations)
         """
     def get_attendee(self, *, MeetingId: str, AttendeeId: str) -> GetAttendeeResponseTypeDef:
         """
         Gets the Amazon Chime SDK attendee details for a specified meeting ID and
@@ -1271,15 +1271,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_emergency_calling_configuration)
         """
     def get_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> GetVoiceConnectorGroupResponseTypeDef:
         """
         Retrieves details for the specified Amazon Chime Voice Connector group, such as
-        timestamps,name, and associated `VoiceConnectorItems` .
+        timestamps,name, and associated `VoiceConnectorItems`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_group)
         """
     def get_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorLoggingConfigurationResponseTypeDef:
@@ -1359,33 +1359,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_accounts)
         """
     def list_app_instance_admins(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstanceAdminsResponseTypeDef:
         """
-        Returns a list of the administrators in the `AppInstance` .
+        Returns a list of the administrators in the `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instance_admins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instance_admins)
         """
     def list_app_instance_users(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstanceUsersResponseTypeDef:
         """
-        List all `AppInstanceUsers` created under a single `AppInstance` .
+        List all `AppInstanceUsers` created under a single `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instance_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instance_users)
         """
     def list_app_instances(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAppInstancesResponseTypeDef:
         """
-        Lists all Amazon Chime `AppInstance` s created under a single AWS account.
+        Lists all Amazon Chime `AppInstance`s created under a single AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_app_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_app_instances)
         """
     def list_attendee_tags(
         self, *, MeetingId: str, AttendeeId: str
     ) -> ListAttendeeTagsResponseTypeDef:
@@ -1508,15 +1508,15 @@
         *,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
-        A list of the channels moderated by an `AppInstanceUser` .
+        A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_channels_moderated_by_app_instance_user)
         """
     def list_media_capture_pipelines(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMediaCapturePipelinesResponseTypeDef:
@@ -1701,15 +1701,15 @@
     def put_app_instance_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
         AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef]
     ) -> PutAppInstanceStreamingConfigurationsResponseTypeDef:
         """
-        The data streaming configurations of an `AppInstance` .
+        The data streaming configurations of an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_app_instance_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_app_instance_streaming_configurations)
         """
     def put_events_configuration(
         self,
         *,
@@ -1861,15 +1861,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.reset_personal_pin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#reset_personal_pin)
         """
     def restore_phone_number(self, *, PhoneNumberId: str) -> RestorePhoneNumberResponseTypeDef:
         """
         Moves a phone number from the **Deletion queue** back into the phone number
-        **Inventory** .
+        **Inventory**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.restore_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#restore_phone_number)
         """
     def search_available_phone_numbers(
         self,
         *,
@@ -1905,22 +1905,22 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.send_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#send_channel_message)
         """
     def start_meeting_transcription(
         self, *, MeetingId: str, TranscriptionConfiguration: TranscriptionConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
-        Starts transcription for the specified `meetingId` .
+        Starts transcription for the specified `meetingId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.start_meeting_transcription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#start_meeting_transcription)
         """
     def stop_meeting_transcription(self, *, MeetingId: str) -> Dict[str, Any]:
         """
-        Stops transcription for the specified `meetingId` .
+        Stops transcription for the specified `meetingId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.stop_meeting_transcription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#stop_meeting_transcription)
         """
     def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,20 @@
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
+    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
+    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -213,14 +215,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -230,27 +233,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -279,14 +286,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -331,51 +339,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -407,28 +421,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -437,14 +455,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -455,55 +474,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -152,18 +152,20 @@
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
+    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
+    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -211,14 +213,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -228,27 +231,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -277,14 +284,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -329,51 +337,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -405,28 +419,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -435,14 +453,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -453,55 +472,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1792,44 +1792,37 @@
 
 class EngineTranscribeMedicalSettingsTypeDef(
     _RequiredEngineTranscribeMedicalSettingsTypeDef, _OptionalEngineTranscribeMedicalSettingsTypeDef
 ):
     pass
 
 
-_RequiredEngineTranscribeSettingsTypeDef = TypedDict(
-    "_RequiredEngineTranscribeSettingsTypeDef",
+EngineTranscribeSettingsTypeDef = TypedDict(
+    "EngineTranscribeSettingsTypeDef",
     {
         "LanguageCode": TranscribeLanguageCodeType,
-    },
-)
-_OptionalEngineTranscribeSettingsTypeDef = TypedDict(
-    "_OptionalEngineTranscribeSettingsTypeDef",
-    {
         "VocabularyFilterMethod": TranscribeVocabularyFilterMethodType,
         "VocabularyFilterName": str,
         "VocabularyName": str,
         "Region": TranscribeRegionType,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": TranscribePartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": TranscribeLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-
-class EngineTranscribeSettingsTypeDef(
-    _RequiredEngineTranscribeSettingsTypeDef, _OptionalEngineTranscribeSettingsTypeDef
-):
-    pass
-
-
 EventsConfigurationTypeDef = TypedDict(
     "EventsConfigurationTypeDef",
     {
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1735,42 +1735,37 @@
 )
 
 class EngineTranscribeMedicalSettingsTypeDef(
     _RequiredEngineTranscribeMedicalSettingsTypeDef, _OptionalEngineTranscribeMedicalSettingsTypeDef
 ):
     pass
 
-_RequiredEngineTranscribeSettingsTypeDef = TypedDict(
-    "_RequiredEngineTranscribeSettingsTypeDef",
+EngineTranscribeSettingsTypeDef = TypedDict(
+    "EngineTranscribeSettingsTypeDef",
     {
         "LanguageCode": TranscribeLanguageCodeType,
-    },
-)
-_OptionalEngineTranscribeSettingsTypeDef = TypedDict(
-    "_OptionalEngineTranscribeSettingsTypeDef",
-    {
         "VocabularyFilterMethod": TranscribeVocabularyFilterMethodType,
         "VocabularyFilterName": str,
         "VocabularyName": str,
         "Region": TranscribeRegionType,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": TranscribePartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": TranscribeLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-class EngineTranscribeSettingsTypeDef(
-    _RequiredEngineTranscribeSettingsTypeDef, _OptionalEngineTranscribeSettingsTypeDef
-):
-    pass
-
 EventsConfigurationTypeDef = TypedDict(
     "EventsConfigurationTypeDef",
     {
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Chime 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.117
+Summary: Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -818,42 +819,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-1.26.0.post1/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.0.post1/setup.py` & `mypy-boto3-chime-1.26.117/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-chime.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.26.0.post1",
+    version="1.26.117",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_chime": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_chime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

