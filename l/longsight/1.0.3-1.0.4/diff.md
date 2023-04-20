# Comparing `tmp/longsight-1.0.3.tar.gz` & `tmp/longsight-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longsight-1.0.3.tar", last modified: Thu Apr  6 09:56:32 2023, max compression
+gzip compressed data, was "longsight-1.0.4.tar", last modified: Thu Apr 20 08:37:02 2023, max compression
```

## Comparing `longsight-1.0.3.tar` & `longsight-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-06 09:56:32.645798 longsight-1.0.3/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.3/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     7876 2023-04-06 09:56:32.645798 longsight-1.0.3/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6005 2023-04-06 09:56:07.000000 longsight-1.0.3/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1028 2023-04-06 09:23:32.000000 longsight-1.0.3/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1010 2023-04-06 09:56:32.645798 longsight-1.0.3/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-06 09:56:32.645798 longsight-1.0.3/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-06 09:56:32.645798 longsight-1.0.3/src/longsight/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.3/src/longsight/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11959 2023-04-06 09:50:50.000000 longsight-1.0.3/src/longsight/instrumentation.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-06 09:56:32.645798 longsight-1.0.3/src/longsight.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7876 2023-04-06 09:56:32.000000 longsight-1.0.3/src/longsight.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-06 09:56:32.000000 longsight-1.0.3/src/longsight.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-06 09:56:32.000000 longsight-1.0.3/src/longsight.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      130 2023-04-06 09:56:32.000000 longsight-1.0.3/src/longsight.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-06 09:56:32.000000 longsight-1.0.3/src/longsight.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-06 09:56:32.645798 longsight-1.0.3/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     6998 2023-03-31 15:41:47.000000 longsight-1.0.3/tests/test_instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:37:02.001078 longsight-1.0.4/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.4/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7787 2023-04-20 08:37:02.001078 longsight-1.0.4/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5916 2023-04-06 09:59:05.000000 longsight-1.0.4/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-20 08:35:53.000000 longsight-1.0.4/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-20 08:37:02.001078 longsight-1.0.4/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:37:01.997078 longsight-1.0.4/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:37:01.997078 longsight-1.0.4/src/longsight/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.4/src/longsight/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11959 2023-04-06 09:50:50.000000 longsight-1.0.4/src/longsight/instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:37:02.001078 longsight-1.0.4/src/longsight.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7787 2023-04-20 08:37:01.000000 longsight-1.0.4/src/longsight.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-20 08:37:01.000000 longsight-1.0.4/src/longsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-20 08:37:01.000000 longsight-1.0.4/src/longsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-20 08:37:01.000000 longsight-1.0.4/src/longsight.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-20 08:37:01.000000 longsight-1.0.4/src/longsight.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 08:37:02.001078 longsight-1.0.4/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6998 2023-03-31 15:41:47.000000 longsight-1.0.4/tests/test_instrumentation.py
```

### Comparing `longsight-1.0.3/LICENSE.md` & `longsight-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.3/PKG-INFO` & `longsight-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.3
+Version: 1.0.4
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -66,16 +66,15 @@
 
     @instrumentation.instrument(
     cloudwatch_push=True,
     log_stream_name="martin-test-stream-name",
     log_group_name="martin-test-group-name",
     namespace="martin-test-namespace",
     )
-    def a_function(instrumentation, log_stream_name="martin-test-stream-name",
-    log_group_name="martin-test-group-name",):
+    def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         instrumentation.logger.info("A second log line")
         instrumentation.add_metric_point(
             metric_name="test_metric",
             dimensions=[{"Name": "Environment", "Value": "Production"}],
             metric_value=1,
             unit="Count",
```

### Comparing `longsight-1.0.3/README.md` & `longsight-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
     @instrumentation.instrument(
     cloudwatch_push=True,
     log_stream_name="martin-test-stream-name",
     log_group_name="martin-test-group-name",
     namespace="martin-test-namespace",
     )
-    def a_function(instrumentation, log_stream_name="martin-test-stream-name",
-    log_group_name="martin-test-group-name",):
+    def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         instrumentation.logger.info("A second log line")
         instrumentation.add_metric_point(
             metric_name="test_metric",
             dimensions=[{"Name": "Environment", "Value": "Production"}],
             metric_value=1,
             unit="Count",
```

### Comparing `longsight-1.0.3/pyproject.toml` & `longsight-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longsight"
-version = "1.0.3"
+version = "1.0.4"
 description = "This library implements a range of common logging functions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
@@ -20,15 +20,15 @@
 
 dependencies = [
     "aws-lambda-powertools[all]==2.11.0",
     "uvicorn==0.21.1",
     "fastapi~=0.95.0",
     "httpx==0.23.3",
     "starlette==0.26.1",
-    "claws==0.0.7",
+    "claws==0.0.11",
     "watchtower==3.0.1"
 ]
 
 [project.urls]
 homepage = "https://labs.crossref.org"
 documentation = "https://labs.crossref.org"
 repository = "https://gitlab.com/crossref/labs/longsight"
```

### Comparing `longsight-1.0.3/setup.cfg` & `longsight-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = longsight
-version = 1.0.3
+version = 1.0.4
 description = This library implements a range of common logging functions.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
@@ -26,15 +26,15 @@
 python_requires = >=3.8
 install_requires = 
 	aws-lambda-powertools[all]==2.11.0
 	uvicorn==0.21.1
 	fastapi~=0.95.0
 	httpx==0.23.3
 	starlette==0.26.1
-	claws==0.0.7
+	claws==0.0.11
 	watchtower==3.0.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `longsight-1.0.3/src/longsight/instrumentation.py` & `longsight-1.0.4/src/longsight/instrumentation.py`

 * *Files identical despite different names*

### Comparing `longsight-1.0.3/src/longsight.egg-info/PKG-INFO` & `longsight-1.0.4/src/longsight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.3
+Version: 1.0.4
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -66,16 +66,15 @@
 
     @instrumentation.instrument(
     cloudwatch_push=True,
     log_stream_name="martin-test-stream-name",
     log_group_name="martin-test-group-name",
     namespace="martin-test-namespace",
     )
-    def a_function(instrumentation, log_stream_name="martin-test-stream-name",
-    log_group_name="martin-test-group-name",):
+    def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         instrumentation.logger.info("A second log line")
         instrumentation.add_metric_point(
             metric_name="test_metric",
             dimensions=[{"Name": "Environment", "Value": "Production"}],
             metric_value=1,
             unit="Count",
```

### Comparing `longsight-1.0.3/tests/test_instrumentation.py` & `longsight-1.0.4/tests/test_instrumentation.py`

 * *Files identical despite different names*

