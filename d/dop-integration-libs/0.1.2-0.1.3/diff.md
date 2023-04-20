# Comparing `tmp/dop_integration_libs-0.1.2.tar.gz` & `tmp/dop_integration_libs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.2.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.3.tar", max compression
```

## Comparing `dop_integration_libs-0.1.2.tar` & `dop_integration_libs-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.2/README.md
--rw-r--r--   0        0        0     1267 2023-04-20 11:43:21.697033 dop_integration_libs-0.1.2/dop_integration_libs/Logger.py
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.2/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.2/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.2/dop_integration_libs/environment.py
--rw-r--r--   0        0        0      389 2023-04-20 11:44:04.042946 dop_integration_libs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.3/README.md
+-rw-r--r--   0        0        0     1357 2023-04-20 11:46:23.435022 dop_integration_libs-0.1.3/dop_integration_libs/Logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.3/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.3/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.3/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0      389 2023-04-20 11:45:51.922248 dop_integration_libs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.3/PKG-INFO
```

### Comparing `dop_integration_libs-0.1.2/dop_integration_libs/Logger.py` & `dop_integration_libs-0.1.3/dop_integration_libs/Logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,11 @@
     def send_log(self):
         """
         Send log to log server
         """
         with open(f"{self.session_id}_log.log", "r") as log_file:
             lines = log_file.readlines()
             print(lines)
+
+    @staticmethod
+    def get_logger(session_id: str):
+        return Logger(session_id)
```

### Comparing `dop_integration_libs-0.1.2/dop_integration_libs/environment.py` & `dop_integration_libs-0.1.3/dop_integration_libs/environment.py`

 * *Files identical despite different names*

