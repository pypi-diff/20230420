# Comparing `tmp/ec2-demo-0.1.2.tar.gz` & `tmp/ec2-demo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-demo-0.1.2.tar", last modified: Thu Apr 20 08:17:53 2023, max compression
+gzip compressed data, was "ec2-demo-0.1.3.tar", last modified: Thu Apr 20 08:18:51 2023, max compression
```

## Comparing `ec2-demo-0.1.2.tar` & `ec2-demo-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:17:53.761083 ec2-demo-0.1.2/
--rw-r--r--   0 pedro      (503) staff       (20)      842 2023-04-20 08:17:53.760947 ec2-demo-0.1.2/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      256 2023-04-20 05:38:46.000000 ec2-demo-0.1.2/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:17:53.759387 ec2-demo-0.1.2/ec2_demo/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:17:52.000000 ec2-demo-0.1.2/ec2_demo/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.2/ec2_demo/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:11:32.000000 ec2-demo-0.1.2/ec2_demo/instances.py
--rw-r--r--   0 pedro      (503) staff       (20)     1046 2023-04-20 08:11:24.000000 ec2-demo-0.1.2/ec2_demo/task.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:17:53.760410 ec2-demo-0.1.2/ec2_demo.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)      842 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)       29 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:17:53.000000 ec2-demo-0.1.2/ec2_demo.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:17:53.761124 ec2-demo-0.1.2/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      986 2023-04-20 07:37:04.000000 ec2-demo-0.1.2/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:17:53.760733 ec2-demo-0.1.2/tests/
--rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.2/tests/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 07:45:45.000000 ec2-demo-0.1.2/tests/test_instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:18:51.294401 ec2-demo-0.1.3/
+-rw-r--r--   0 pedro      (503) staff       (20)      892 2023-04-20 08:18:51.294227 ec2-demo-0.1.3/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      306 2023-04-20 08:18:43.000000 ec2-demo-0.1.3/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:18:51.292793 ec2-demo-0.1.3/ec2_demo/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:18:49.000000 ec2-demo-0.1.3/ec2_demo/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.3/ec2_demo/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:11:32.000000 ec2-demo-0.1.3/ec2_demo/instances.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1046 2023-04-20 08:11:24.000000 ec2-demo-0.1.3/ec2_demo/task.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:18:51.293695 ec2-demo-0.1.3/ec2_demo.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)      892 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       29 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:18:51.000000 ec2-demo-0.1.3/ec2_demo.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:18:51.294469 ec2-demo-0.1.3/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      986 2023-04-20 07:37:04.000000 ec2-demo-0.1.3/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:18:51.293979 ec2-demo-0.1.3/tests/
+-rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.3/tests/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 07:45:45.000000 ec2-demo-0.1.3/tests/test_instances.py
```

### Comparing `ec2-demo-0.1.2/PKG-INFO` & `ec2-demo-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.2
+Version: 0.1.3
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
@@ -14,23 +14,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # EC2 Demo
 
-A small cli util to create and delete EC2 instances.
+A small cli util to create, list and delete EC2 instances.
 
 
 ## Design
 
-ec2-demo create <env> <file.yaml>
-ec2-demo list <env>
-ec2-demo delete <env> <id>
+    ec2-demo create <env> <file.yaml>
+    ec2-demo list <env>
+    ec2-demo delete <env> <id>
 
 
 ## Implementation
 
 We will use:
 
-- click for the cli interface
-- boto3 for the API calls (SDK)
+- `click` for the cli interface, not `argparse` and related
+- `boto3` for the API calls (SDK)
```

### Comparing `ec2-demo-0.1.2/ec2_demo/cli.py` & `ec2-demo-0.1.3/ec2_demo/cli.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.2/ec2_demo/instances.py` & `ec2-demo-0.1.3/ec2_demo/instances.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.2/ec2_demo/task.py` & `ec2-demo-0.1.3/ec2_demo/task.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.2/ec2_demo.egg-info/PKG-INFO` & `ec2-demo-0.1.3/ec2_demo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.2
+Version: 0.1.3
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
@@ -14,23 +14,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # EC2 Demo
 
-A small cli util to create and delete EC2 instances.
+A small cli util to create, list and delete EC2 instances.
 
 
 ## Design
 
-ec2-demo create <env> <file.yaml>
-ec2-demo list <env>
-ec2-demo delete <env> <id>
+    ec2-demo create <env> <file.yaml>
+    ec2-demo list <env>
+    ec2-demo delete <env> <id>
 
 
 ## Implementation
 
 We will use:
 
-- click for the cli interface
-- boto3 for the API calls (SDK)
+- `click` for the cli interface, not `argparse` and related
+- `boto3` for the API calls (SDK)
```

### Comparing `ec2-demo-0.1.2/setup.py` & `ec2-demo-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.2/tests/test_instances.py` & `ec2-demo-0.1.3/tests/test_instances.py`

 * *Files identical despite different names*

