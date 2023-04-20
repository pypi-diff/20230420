# Comparing `tmp/ec2-demo-0.1.4.tar.gz` & `tmp/ec2-demo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-demo-0.1.4.tar", last modified: Thu Apr 20 08:27:40 2023, max compression
+gzip compressed data, was "ec2-demo-0.1.5.tar", last modified: Thu Apr 20 08:29:40 2023, max compression
```

## Comparing `ec2-demo-0.1.4.tar` & `ec2-demo-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:27:40.223257 ec2-demo-0.1.4/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:27:40.223105 ec2-demo-0.1.4/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:27:26.000000 ec2-demo-0.1.4/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:27:40.221548 ec2-demo-0.1.4/ec2_demo/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:27:37.000000 ec2-demo-0.1.4/ec2_demo/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.4/ec2_demo/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:11:32.000000 ec2-demo-0.1.4/ec2_demo/instances.py
--rw-r--r--   0 pedro      (503) staff       (20)     1046 2023-04-20 08:11:24.000000 ec2-demo-0.1.4/ec2_demo/task.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:27:40.222547 ec2-demo-0.1.4/ec2_demo.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)       29 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:27:40.000000 ec2-demo-0.1.4/ec2_demo.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:27:40.223307 ec2-demo-0.1.4/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      986 2023-04-20 07:37:04.000000 ec2-demo-0.1.4/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:27:40.222883 ec2-demo-0.1.4/tests/
--rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.4/tests/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 07:45:45.000000 ec2-demo-0.1.4/tests/test_instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.139692 ec2-demo-0.1.5/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:29:40.139562 ec2-demo-0.1.5/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.5/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.138020 ec2-demo-0.1.5/ec2_demo/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:29:27.000000 ec2-demo-0.1.5/ec2_demo/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.5/ec2_demo/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:11:32.000000 ec2-demo-0.1.5/ec2_demo/instances.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1046 2023-04-20 08:11:24.000000 ec2-demo-0.1.5/ec2_demo/task.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.138966 ec2-demo-0.1.5/ec2_demo.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       29 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:29:40.139744 ec2-demo-0.1.5/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      986 2023-04-20 07:37:04.000000 ec2-demo-0.1.5/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.139259 ec2-demo-0.1.5/tests/
+-rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.5/tests/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 07:45:45.000000 ec2-demo-0.1.5/tests/test_instances.py
```

### Comparing `ec2-demo-0.1.4/PKG-INFO` & `ec2-demo-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.4
+Version: 0.1.5
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # EC2 Demo
 
-[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_for demo_purposes_only_-red)](https://semver.org)
+[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_for_demo_purposes_only_-red)](https://semver.org)
 
 
 A small cli util to create, list and delete EC2 instances.
 
 
 ## Design
```

### Comparing `ec2-demo-0.1.4/ec2_demo/cli.py` & `ec2-demo-0.1.5/ec2_demo/cli.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.4/ec2_demo/instances.py` & `ec2-demo-0.1.5/ec2_demo/instances.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.4/ec2_demo/task.py` & `ec2-demo-0.1.5/ec2_demo/task.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.4/ec2_demo.egg-info/PKG-INFO` & `ec2-demo-0.1.5/ec2_demo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.4
+Version: 0.1.5
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # EC2 Demo
 
-[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_for demo_purposes_only_-red)](https://semver.org)
+[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_for_demo_purposes_only_-red)](https://semver.org)
 
 
 A small cli util to create, list and delete EC2 instances.
 
 
 ## Design
```

### Comparing `ec2-demo-0.1.4/setup.py` & `ec2-demo-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.4/tests/test_instances.py` & `ec2-demo-0.1.5/tests/test_instances.py`

 * *Files identical despite different names*

