# Comparing `tmp/dop_integration_libs-0.1.5.tar.gz` & `tmp/dop_integration_libs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.5.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.6.tar", max compression
```

## Comparing `dop_integration_libs-0.1.5.tar` & `dop_integration_libs-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.5/README.md
--rw-r--r--   0        0        0     2264 2023-04-20 12:13:51.624660 dop_integration_libs-0.1.5/dop_integration_libs/Logger.py
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.5/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.5/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.5/dop_integration_libs/environment.py
--rw-r--r--   0        0        0      389 2023-04-20 12:14:08.255674 dop_integration_libs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.6/README.md
+-rw-r--r--   0        0        0     2287 2023-04-20 12:20:06.341415 dop_integration_libs-0.1.6/dop_integration_libs/Logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.6/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.6/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.6/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0      389 2023-04-20 12:20:14.561588 dop_integration_libs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.6/PKG-INFO
```

### Comparing `dop_integration_libs-0.1.5/dop_integration_libs/Logger.py` & `dop_integration_libs-0.1.6/dop_integration_libs/Logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Logger class for logging to log server
 """
 import logging
 import os
 import requests
 import json
+from typing import Any
 from environment import Environment
 
 
 class Logger(object):
     """
     Logger class for logging to log server
         .log(message) - log message
@@ -25,27 +26,27 @@
         fh = logging.FileHandler(f"{session_id}_log.log")
         fh.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
 
-    def log(self, message: str):
+    def log(self, message: Any):
         print(message)
         self.logger.info(message)
 
-    def error(self, message: str):
+    def error(self, message: Any):
         print(message)
         self.logger.error(message)
 
-    def warning(self, message: str):
+    def warning(self, message: Any):
         print(message)
         self.logger.warning(message)
 
-    def debug(self, message: str):
+    def debug(self, message: Any):
         print(message)
         self.logger.debug(message)
 
     def send_log_to_server(self, log: str):
         """
         This function is used to get the environment variables
         """
```

### Comparing `dop_integration_libs-0.1.5/dop_integration_libs/environment.py` & `dop_integration_libs-0.1.6/dop_integration_libs/environment.py`

 * *Files identical despite different names*

