# Comparing `tmp/dop_integration_libs-0.1.6.tar.gz` & `tmp/dop_integration_libs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.6.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.7.tar", max compression
```

## Comparing `dop_integration_libs-0.1.6.tar` & `dop_integration_libs-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.6/README.md
--rw-r--r--   0        0        0     2287 2023-04-20 12:20:06.341415 dop_integration_libs-0.1.6/dop_integration_libs/Logger.py
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.6/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.6/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.6/dop_integration_libs/environment.py
--rw-r--r--   0        0        0      389 2023-04-20 12:20:14.561588 dop_integration_libs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.7/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.7/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-20 12:24:22.512014 dop_integration_libs-0.1.7/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0     2288 2023-04-20 12:25:09.853013 dop_integration_libs-0.1.7/dop_integration_libs/logger.py
+-rw-r--r--   0        0        0      389 2023-04-20 12:25:17.860031 dop_integration_libs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.7/PKG-INFO
```

### Comparing `dop_integration_libs-0.1.6/dop_integration_libs/Logger.py` & `dop_integration_libs-0.1.7/dop_integration_libs/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Logger class for logging to log server
 """
 import logging
 import os
 import requests
 import json
 from typing import Any
-from environment import Environment
+from .environment import Environment
 
 
 class Logger(object):
     """
     Logger class for logging to log server
         .log(message) - log message
         .error(message) - log error message
```

### Comparing `dop_integration_libs-0.1.6/dop_integration_libs/environment.py` & `dop_integration_libs-0.1.7/dop_integration_libs/environment.py`

 * *Files identical despite different names*

