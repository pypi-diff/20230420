# Comparing `tmp/mypy-boto3-chime-sdk-meetings-1.26.117.tar.gz` & `tmp/mypy-boto3-chime-sdk-meetings-1.26.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.26.117.tar", last modified: Thu Apr 20 19:33:48 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-meetings-1.26.117.tar` & `mypy-boto3-chime-sdk-meetings-1.26.68.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.423264 mypy-boto3-chime-sdk-meetings-1.26.117/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-04-20 19:33:48.423264 mypy-boto3-chime-sdk-meetings-1.26.117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.423264 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-20 19:32:19.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-20 19:32:19.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-04-20 19:32:19.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-04-20 19:32:19.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-04-20 19:32:19.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.423264 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:33:48.423264 mypy-boto3-chime-sdk-meetings-1.26.117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-20 19:32:18.000000 mypy-boto3-chime-sdk-meetings-1.26.117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-02-09 20:26:11.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/setup.py
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/LICENSE` & `mypy-boto3-chime-sdk-meetings-1.26.68/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.26.68/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.26.117
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.68
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,42 +365,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/README.md` & `mypy-boto3-chime-sdk-meetings-1.26.68/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,42 +333,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/__main__.py` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMeetings 1.26.117\nVersion:         1.26.117\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMeetings 1.26.68\nVersion:         1.26.68\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.117")
+    print("1.26.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/client.py` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,12 +279,12 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#untag_resource)
         """
 
     def update_attendee_capabilities(
         self, *, MeetingId: str, AttendeeId: str, Capabilities: AttendeeCapabilitiesTypeDef
     ) -> UpdateAttendeeCapabilitiesResponseTypeDef:
         """
-        The capabilities that you want to update.
+        The capabilties that you want to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.update_attendee_capabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#update_attendee_capabilities)
         """
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/client.pyi` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -257,12 +257,12 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#untag_resource)
         """
     def update_attendee_capabilities(
         self, *, MeetingId: str, AttendeeId: str, Capabilities: AttendeeCapabilitiesTypeDef
     ) -> UpdateAttendeeCapabilitiesResponseTypeDef:
         """
-        The capabilities that you want to update.
+        The capabilties that you want to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.update_attendee_capabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#update_attendee_capabilities)
         """
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/literals.py` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,18 @@
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
-    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
-    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -231,15 +229,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -250,15 +247,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -409,20 +405,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/literals.pyi` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,20 +46,18 @@
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
-    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
-    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -229,15 +227,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -248,15 +245,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -407,20 +403,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/type_defs.py` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,14 @@
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": TranscribeLanguageCodeType,
-        "VocabularyNames": str,
-        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
 GetAttendeeRequestRequestTypeDef = TypedDict(
     "GetAttendeeRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings/type_defs.pyi` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,14 @@
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": TranscribeLanguageCodeType,
-        "VocabularyNames": str,
-        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
 GetAttendeeRequestRequestTypeDef = TypedDict(
     "GetAttendeeRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.26.117
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.68
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,42 +365,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.117/setup.py` & `mypy-boto3-chime-sdk-meetings-1.26.68/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-chime-sdk-meetings.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-chime-sdk-meetings",
-    version="1.26.117",
+    version="1.26.68",
     packages=["mypy_boto3_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMeetings 1.26.117 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with"
+        " mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

