# Comparing `tmp/ec2-demo-0.1.5.tar.gz` & `tmp/ec2-demo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-demo-0.1.5.tar", last modified: Thu Apr 20 08:29:40 2023, max compression
+gzip compressed data, was "ec2-demo-0.1.6.tar", last modified: Thu Apr 20 08:36:38 2023, max compression
```

## Comparing `ec2-demo-0.1.5.tar` & `ec2-demo-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.139692 ec2-demo-0.1.5/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:29:40.139562 ec2-demo-0.1.5/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.5/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.138020 ec2-demo-0.1.5/ec2_demo/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:29:27.000000 ec2-demo-0.1.5/ec2_demo/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.5/ec2_demo/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:11:32.000000 ec2-demo-0.1.5/ec2_demo/instances.py
--rw-r--r--   0 pedro      (503) staff       (20)     1046 2023-04-20 08:11:24.000000 ec2-demo-0.1.5/ec2_demo/task.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.138966 ec2-demo-0.1.5/ec2_demo.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)       29 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:29:40.000000 ec2-demo-0.1.5/ec2_demo.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:29:40.139744 ec2-demo-0.1.5/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      986 2023-04-20 07:37:04.000000 ec2-demo-0.1.5/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:29:40.139259 ec2-demo-0.1.5/tests/
--rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.5/tests/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 07:45:45.000000 ec2-demo-0.1.5/tests/test_instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.218204 ec2-demo-0.1.6/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:36:38.218073 ec2-demo-0.1.6/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.6/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.216330 ec2-demo-0.1.6/ec2_demo/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 08:36:34.000000 ec2-demo-0.1.6/ec2_demo/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.6/ec2_demo/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:30:40.000000 ec2-demo-0.1.6/ec2_demo/instances.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1080 2023-04-20 08:35:42.000000 ec2-demo-0.1.6/ec2_demo/task.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.217500 ec2-demo-0.1.6/ec2_demo.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 08:36:38.000000 ec2-demo-0.1.6/ec2_demo.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 08:36:38.218250 ec2-demo-0.1.6/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)     1002 2023-04-20 08:36:29.000000 ec2-demo-0.1.6/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 08:36:38.217848 ec2-demo-0.1.6/tests/
+-rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.6/tests/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 08:32:30.000000 ec2-demo-0.1.6/tests/test_instances.py
```

### Comparing `ec2-demo-0.1.5/PKG-INFO` & `ec2-demo-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.5
+Version: 0.1.6
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
```

### Comparing `ec2-demo-0.1.5/ec2_demo/cli.py` & `ec2-demo-0.1.6/ec2_demo/cli.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.5/ec2_demo/instances.py` & `ec2-demo-0.1.6/ec2_demo/instances.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.5/ec2_demo/task.py` & `ec2-demo-0.1.6/ec2_demo/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import boto3
 import logging
+import time
 
 from .utils.tags import Tags
 
 
 class Task:
 
     def __init__(self, vars):
@@ -32,8 +33,9 @@
         logging.debug(f"Patched spec: {spec}")
         res = self.client.run_instances(**spec)
 
         for instance in res["Instances"]:
             logging.debug(f"InstanceId: {instance['InstanceId']}")
             self.instanceIds.append(instance["InstanceId"])
 
+        time.sleep(2)
         return self.instanceIds
```

### Comparing `ec2-demo-0.1.5/ec2_demo.egg-info/PKG-INFO` & `ec2-demo-0.1.6/ec2_demo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-demo
-Version: 0.1.5
+Version: 0.1.6
 Summary: EC2 demo
 Home-page: https://github.com/jpedro/ec2-demo
 Download-URL: https://github.com/jpedro/ec2-demo/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: ec2 create delete demo
```

### Comparing `ec2-demo-0.1.5/setup.py` & `ec2-demo-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "tests",
   ],
   install_requires=[
     "pyyaml",
     "jinja2",
     "requests",
     "boto3",
+    "tabulate",
   ],
   entry_points={
     "console_scripts": [
       "ec2-demo=ec2_demo.cli:main",
     ],
   },
 )
```

### Comparing `ec2-demo-0.1.5/tests/test_instances.py` & `ec2-demo-0.1.6/tests/test_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class TestInstances(TestCase):
 
     @mock.patch("ec2_demo.instances.Instances.create")
     def test_create(self, mocked):
         expected = ["i-created"]
         mocked.return_value = expected
         instances = Instances("dev")
-        returned = instances.create("instances/demo.yaml")
+        returned = instances.create("instances/test.yaml")
         self.assertEqual(expected, returned)
 
 
     @mock.patch("ec2_demo.instances.Instances.delete")
     def test_delete(self, mocked):
         expected = ["i-deleted"]
         mocked.return_value = expected
```

