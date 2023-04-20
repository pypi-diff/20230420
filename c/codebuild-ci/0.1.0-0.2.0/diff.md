# Comparing `tmp/codebuild_ci-0.1.0.tar.gz` & `tmp/codebuild_ci-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebuild_ci-0.1.0.tar", max compression
+gzip compressed data, was "codebuild_ci-0.2.0.tar", max compression
```

## Comparing `codebuild_ci-0.1.0.tar` & `codebuild_ci-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1153 2023-04-20 10:26:32.460886 codebuild_ci-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 09:13:36.816059 codebuild_ci-0.1.0/codebuild_ci/__init__.py
--rw-r--r--   0        0        0     1808 2023-04-20 09:55:46.797225 codebuild_ci-0.1.0/codebuild_ci/__main__.py
--rw-r--r--   0        0        0       95 2023-04-20 10:04:41.836764 codebuild_ci-0.1.0/codebuild_ci/clients.py
--rw-r--r--   0        0        0     1476 2023-04-20 10:05:00.668513 codebuild_ci-0.1.0/codebuild_ci/codebuild.py
--rw-r--r--   0        0        0     1896 2023-04-20 10:05:14.636912 codebuild_ci-0.1.0/codebuild_ci/logs.py
--rw-r--r--   0        0        0     3382 2023-04-20 09:09:53.746823 codebuild_ci-0.1.0/codebuild_ci/waiter.py
--rw-r--r--   0        0        0     2401 2023-04-20 09:51:18.751436 codebuild_ci-0.1.0/codebuild_ci/waiter_model.py
--rw-r--r--   0        0        0     1274 2023-04-20 10:24:07.403983 codebuild_ci-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 codebuild_ci-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-04-20 10:26:32.460886 codebuild_ci-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 09:13:36.816059 codebuild_ci-0.2.0/codebuild_ci/__init__.py
+-rw-r--r--   0        0        0     1808 2023-04-20 09:55:46.797225 codebuild_ci-0.2.0/codebuild_ci/__main__.py
+-rw-r--r--   0        0        0       95 2023-04-20 10:04:41.836764 codebuild_ci-0.2.0/codebuild_ci/clients.py
+-rw-r--r--   0        0        0     1476 2023-04-20 10:05:00.668513 codebuild_ci-0.2.0/codebuild_ci/codebuild.py
+-rw-r--r--   0        0        0     1896 2023-04-20 10:05:14.636912 codebuild_ci-0.2.0/codebuild_ci/logs.py
+-rw-r--r--   0        0        0     3382 2023-04-20 09:09:53.746823 codebuild_ci-0.2.0/codebuild_ci/waiter.py
+-rw-r--r--   0        0        0     2401 2023-04-20 09:51:18.751436 codebuild_ci-0.2.0/codebuild_ci/waiter_model.py
+-rw-r--r--   0        0        0     1275 2023-04-20 10:34:08.461753 codebuild_ci-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 codebuild_ci-0.2.0/PKG-INFO
```

### Comparing `codebuild_ci-0.1.0/README.md` & `codebuild_ci-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/codebuild_ci/__main__.py` & `codebuild_ci-0.2.0/codebuild_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/codebuild_ci/codebuild.py` & `codebuild_ci-0.2.0/codebuild_ci/codebuild.py`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/codebuild_ci/logs.py` & `codebuild_ci-0.2.0/codebuild_ci/logs.py`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/codebuild_ci/waiter.py` & `codebuild_ci-0.2.0/codebuild_ci/waiter.py`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/codebuild_ci/waiter_model.py` & `codebuild_ci-0.2.0/codebuild_ci/waiter_model.py`

 * *Files identical despite different names*

### Comparing `codebuild_ci-0.1.0/pyproject.toml` & `codebuild_ci-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codebuild_ci"
-version = "0.1.0"
+version = "0.2.0"
 description = "Command line utility to trigger and wait for Code build Pipeline to complete"
 authors = ["satyam soni"]
 readme = "README.md"
 packages = [
     { include = "codebuild_ci" },
 ]
 include = [
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9"
 boto3 = "^1.26.116"
 typer = {extras = ["all"], version = "^0.7.0"}
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
```

### Comparing `codebuild_ci-0.1.0/PKG-INFO` & `codebuild_ci-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: codebuild-ci
-Version: 0.1.0
+Version: 0.2.0
 Summary: Command line utility to trigger and wait for Code build Pipeline to complete
 Home-page: https://github.com/satyamsoni2211/codebuild_ci
 License: MIT
 Keywords: python,aws,codebuild,ci,devops,cli
 Author: satyam soni
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AWS CDK
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

