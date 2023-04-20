# Comparing `tmp/my-pipeline-package-1.1.4.tar.gz` & `tmp/my-pipeline-package-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-pipeline-package-1.1.4.tar", last modified: Thu Apr 20 03:57:30 2023, max compression
+gzip compressed data, was "my-pipeline-package-1.1.5.tar", last modified: Thu Apr 20 04:01:07 2023, max compression
```

## Comparing `my-pipeline-package-1.1.4.tar` & `my-pipeline-package-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:57:30.329590 my-pipeline-package-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 03:57:30.329590 my-pipeline-package-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 03:57:13.000000 my-pipeline-package-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:57:30.325590 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 03:57:30.000000 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 03:57:30.000000 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:57:30.000000 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 03:57:30.000000 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:57:30.000000 my-pipeline-package-1.1.4/my_pipeline_package.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 03:57:30.329590 my-pipeline-package-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 03:57:13.000000 my-pipeline-package-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:01:07.742261 my-pipeline-package-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 04:01:07.742261 my-pipeline-package-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 04:00:49.000000 my-pipeline-package-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:01:07.742261 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 04:01:07.000000 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 04:01:07.000000 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:01:07.000000 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 04:01:07.000000 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:01:07.000000 my-pipeline-package-1.1.5/my_pipeline_package.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 04:01:07.742261 my-pipeline-package-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 04:00:49.000000 my-pipeline-package-1.1.5/setup.py
```

### Comparing `my-pipeline-package-1.1.4/PKG-INFO` & `my-pipeline-package-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.4
+Version: 1.1.5
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

### Comparing `my-pipeline-package-1.1.4/README.md` & `my-pipeline-package-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `my-pipeline-package-1.1.4/my_pipeline_package.egg-info/PKG-INFO` & `my-pipeline-package-1.1.5/my_pipeline_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.4
+Version: 1.1.5
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

