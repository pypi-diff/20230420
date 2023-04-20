# Comparing `tmp/my-pipeline-package-1.1.8.tar.gz` & `tmp/my-pipeline-package-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-pipeline-package-1.1.8.tar", last modified: Thu Apr 20 12:34:29 2023, max compression
+gzip compressed data, was "my-pipeline-package-1.1.9.tar", last modified: Thu Apr 20 12:40:44 2023, max compression
```

## Comparing `my-pipeline-package-1.1.8.tar` & `my-pipeline-package-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:34:29.349076 my-pipeline-package-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:34:29.349076 my-pipeline-package-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 12:34:07.000000 my-pipeline-package-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:34:29.349076 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:34:29.000000 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 12:34:29.000000 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:34:29.000000 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 12:34:29.000000 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:34:29.000000 my-pipeline-package-1.1.8/my_pipeline_package.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:34:29.349076 my-pipeline-package-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 12:34:07.000000 my-pipeline-package-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:40:44.131705 my-pipeline-package-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:40:44.131705 my-pipeline-package-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 12:40:25.000000 my-pipeline-package-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:40:44.131705 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:40:44.000000 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 12:40:44.000000 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:40:44.000000 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 12:40:44.000000 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:40:43.000000 my-pipeline-package-1.1.9/my_pipeline_package.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:40:44.131705 my-pipeline-package-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 12:40:25.000000 my-pipeline-package-1.1.9/setup.py
```

### Comparing `my-pipeline-package-1.1.8/PKG-INFO` & `my-pipeline-package-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.8
+Version: 1.1.9
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

### Comparing `my-pipeline-package-1.1.8/README.md` & `my-pipeline-package-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `my-pipeline-package-1.1.8/my_pipeline_package.egg-info/PKG-INFO` & `my-pipeline-package-1.1.9/my_pipeline_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.8
+Version: 1.1.9
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

