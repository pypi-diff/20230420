# Comparing `tmp/pulumiverse_time-0.0.8.tar.gz` & `tmp/pulumiverse_time-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_time-0.0.8.tar", last modified: Tue Aug 30 14:18:16 2022, max compression
+gzip compressed data, was "pulumiverse_time-0.0.9.tar", last modified: Fri Sep  2 16:46:22 2022, max compression
```

## Comparing `pulumiverse_time-0.0.8.tar` & `pulumiverse_time-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:18:16.638564 pulumiverse_time-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-08-30 14:18:16.638564 pulumiverse_time-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:18:16.638564 pulumiverse_time-0.0.8/pulumiverse_time/
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    33684 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/offset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    40338 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/rotating.py
--rw-r--r--   0 runner    (1001) docker     (121)    17168 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:18:16.638564 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/pulumiverse_time.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-30 14:18:16.638564 pulumiverse_time-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-08-30 14:18:16.000000 pulumiverse_time-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 16:46:22.425514 pulumiverse_time-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-09-02 16:46:22.425514 pulumiverse_time-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 16:46:22.425514 pulumiverse_time-0.0.9/pulumiverse_time/
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33684 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/offset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    40338 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/rotating.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17168 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time/static.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 16:46:22.425514 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/pulumiverse_time.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-02 16:46:22.425514 pulumiverse_time-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-09-02 16:46:22.000000 pulumiverse_time-0.0.9/setup.py
```

### Comparing `pulumiverse_time-0.0.8/PKG-INFO` & `pulumiverse_time-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_time
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Time resources
 Home-page: https://github.com/pulumiverse/pulumi-time
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-time
 Keywords: pulumi time category/utility
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_time-0.0.8/README.md` & `pulumiverse_time-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/__init__.py` & `pulumiverse_time-0.0.9/pulumiverse_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/_utilities.py` & `pulumiverse_time-0.0.9/pulumiverse_time/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/offset.py` & `pulumiverse_time-0.0.9/pulumiverse_time/offset.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/provider.py` & `pulumiverse_time-0.0.9/pulumiverse_time/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/rotating.py` & `pulumiverse_time-0.0.9/pulumiverse_time/rotating.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time/static.py` & `pulumiverse_time-0.0.9/pulumiverse_time/static.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_time-0.0.8/pulumiverse_time.egg-info/PKG-INFO` & `pulumiverse_time-0.0.9/pulumiverse_time.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-time
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Time resources
 Home-page: https://github.com/pulumiverse/pulumi-time
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-time
 Keywords: pulumi time category/utility
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_time-0.0.8/setup.py` & `pulumiverse_time-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.8"
-PLUGIN_VERSION = "0.0.8"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'time', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-time'])
         except OSError as error:
```

