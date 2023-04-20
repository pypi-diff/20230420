# Comparing `tmp/my-pipeline-package-1.1.6.tar.gz` & `tmp/my-pipeline-package-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-pipeline-package-1.1.6.tar", last modified: Thu Apr 20 04:10:39 2023, max compression
+gzip compressed data, was "my-pipeline-package-1.1.7.tar", last modified: Thu Apr 20 12:12:56 2023, max compression
```

## Comparing `my-pipeline-package-1.1.6.tar` & `my-pipeline-package-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:10:39.673776 my-pipeline-package-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 04:10:39.673776 my-pipeline-package-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 04:10:16.000000 my-pipeline-package-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:10:39.669776 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 04:10:39.000000 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 04:10:39.000000 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:10:39.000000 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 04:10:39.000000 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:10:39.000000 my-pipeline-package-1.1.6/my_pipeline_package.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 04:10:39.673776 my-pipeline-package-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 04:10:16.000000 my-pipeline-package-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:56.401542 my-pipeline-package-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:12:56.397542 my-pipeline-package-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 12:12:28.000000 my-pipeline-package-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:56.397542 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 12:12:56.000000 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 12:12:56.000000 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:12:56.000000 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 12:12:56.000000 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:12:56.000000 my-pipeline-package-1.1.7/my_pipeline_package.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:12:56.401542 my-pipeline-package-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 12:12:28.000000 my-pipeline-package-1.1.7/setup.py
```

### Comparing `my-pipeline-package-1.1.6/PKG-INFO` & `my-pipeline-package-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.6
+Version: 1.1.7
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

### Comparing `my-pipeline-package-1.1.6/README.md` & `my-pipeline-package-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `my-pipeline-package-1.1.6/my_pipeline_package.egg-info/PKG-INFO` & `my-pipeline-package-1.1.7/my_pipeline_package.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-pipeline-package
-Version: 1.1.6
+Version: 1.1.7
 Summary: Build package from python tests.
 Description-Content-Type: text/markdown
 
 # DevOps Homework
 
 Welcome to the Postscript DevOps take home task! This task should take you an hour or less to complete. You will be working with a simplified service with a minimal feature set.
```

