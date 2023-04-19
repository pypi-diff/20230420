# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev0.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1479.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev0.tar", last modified: Wed Apr 19 22:44:00 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1479.tar", last modified: Wed Apr 19 23:15:27 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/
--rw-r--r--   0 bverst     (501) staff       (20)    11377 2023-04-19 22:17:57.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/LICENSE
--rw-r--r--   0 bverst     (501) staff       (20)      973 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/PKG-INFO
--rw-r--r--   0 bverst     (501) staff       (20)      435 2023-04-19 22:31:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/README.rst
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/workflow/
--rw-r--r--   0 bverst     (501) staff       (20)      745 2023-04-19 22:36:51.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/workflow/__init__.py
--rw-r--r--   0 bverst     (501) staff       (20)      617 2023-04-19 22:41:11.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/workflow/version.py
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 bverst     (501) staff       (20)      973 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 bverst     (501) staff       (20)      343 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 bverst     (501) staff       (20)        1 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 bverst     (501) staff       (20)       23 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 bverst     (501) staff       (20)        5 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 bverst     (501) staff       (20)      887 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/setup.cfg
--rw-r--r--   0 bverst     (501) staff       (20)     2181 2023-04-19 22:33:40.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/setup.py
-drwxr-xr-x   0 bverst     (501) staff       (20)        0 2023-04-19 22:44:00.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/tests/
--rw-r--r--   0 bverst     (501) staff       (20)      741 2023-04-19 22:30:12.000000 dapr-ext-workflow-dev-0.0.1rc1.dev0/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-19 23:15:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 23:15:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-19 23:15:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 23:15:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/workflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 23:15:27.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-19 23:15:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1479/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev0
+Version: 0.0.1rc1.dev1479
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev0
+Version: 0.0.1rc1.dev1479
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev0/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1479/setup.py`

 * *Files identical despite different names*

