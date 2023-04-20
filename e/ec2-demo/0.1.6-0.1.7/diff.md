# Comparing `tmp/ec2-demo-0.1.6.tar.gz` & `tmp/ec2-demo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-demo-0.1.6.tar", last modified: Thu Apr 20 08:36:38 2023, max compression
+gzip compressed data, was "ec2-demo-0.1.7.tar", last modified: Thu Apr 20 08:39:55 2023, max compression
```

## Comparing `ec2-demo-0.1.6.tar` & `ec2-demo-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.218204 ec2-demo-0.1.6/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:36:38.218073 ec2-demo-0.1.6/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.6/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.216330 ec2-demo-0.1.6/ec2_demo/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:36:34.000000 ec2-demo-0.1.6/ec2_demo/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.6/ec2_demo/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:30:40.000000 ec2-demo-0.1.6/ec2_demo/instances.py
--rw-r--r--   0 pedro      (503) staff       (20)     1080 2023-04-20 08:35:42.000000 ec2-demo-0.1.6/ec2_demo/task.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.217500 ec2-demo-0.1.6/ec2_demo.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:36:38.218250 ec2-demo-0.1.6/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)     1002 2023-04-20 08:36:29.000000 ec2-demo-0.1.6/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.217848 ec2-demo-0.1.6/tests/
--rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.6/tests/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 08:32:30.000000 ec2-demo-0.1.6/tests/test_instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:39:55.162898 ec2-demo-0.1.7/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:39:55.162730 ec2-demo-0.1.7/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.7/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:39:55.161344 ec2-demo-0.1.7/ec2_demo/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:39:45.000000 ec2-demo-0.1.7/ec2_demo/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.7/ec2_demo/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:30:40.000000 ec2-demo-0.1.7/ec2_demo/instances.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1080 2023-04-20 08:35:42.000000 ec2-demo-0.1.7/ec2_demo/task.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:39:55.162094 ec2-demo-0.1.7/ec2_demo.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:39:55.000000 ec2-demo-0.1.7/ec2_demo.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:39:55.162941 ec2-demo-0.1.7/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)     1002 2023-04-20 08:36:29.000000 ec2-demo-0.1.7/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:39:55.162479 ec2-demo-0.1.7/tests/
+-rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.7/tests/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 08:32:30.000000 ec2-demo-0.1.7/tests/test_instances.py
```

### Comparing `ec2-demo-0.1.6/PKG-INFO` & `ec2-demo-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.6
+Version: 0.1.7
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
```

### Comparing `ec2-demo-0.1.6/ec2_demo/cli.py` & `ec2-demo-0.1.7/ec2_demo/cli.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.6/ec2_demo/instances.py` & `ec2-demo-0.1.7/ec2_demo/instances.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.6/ec2_demo/task.py` & `ec2-demo-0.1.7/ec2_demo/task.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.6/ec2_demo.egg-info/PKG-INFO` & `ec2-demo-0.1.7/ec2_demo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.6
+Version: 0.1.7
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
```

### Comparing `ec2-demo-0.1.6/setup.py` & `ec2-demo-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.6/tests/test_instances.py` & `ec2-demo-0.1.7/tests/test_instances.py`

 * *Files identical despite different names*

