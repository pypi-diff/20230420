# Comparing `tmp/ec2-demo-0.1.8.tar.gz` & `tmp/ec2-demo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-demo-0.1.8.tar", last modified: Thu Apr 20 09:05:00 2023, max compression
+gzip compressed data, was "ec2-demo-0.1.9.tar", last modified: Thu Apr 20 10:55:57 2023, max compression
```

## Comparing `ec2-demo-0.1.8.tar` & `ec2-demo-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 09:05:00.059356 ec2-demo-0.1.8/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 09:05:00.059221 ec2-demo-0.1.8/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      441 2023-04-20 08:28:22.000000 ec2-demo-0.1.8/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 09:05:00.057835 ec2-demo-0.1.8/ec2_demo/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 09:03:49.000000 ec2-demo-0.1.8/ec2_demo/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)     1958 2023-04-20 08:16:13.000000 ec2-demo-0.1.8/ec2_demo/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)     3199 2023-04-20 08:30:40.000000 ec2-demo-0.1.8/ec2_demo/instances.py
--rw-r--r--   0 pedro      (503) staff       (20)     1080 2023-04-20 08:35:42.000000 ec2-demo-0.1.8/ec2_demo/task.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 09:05:00.058728 ec2-demo-0.1.8/ec2_demo.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     1027 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      330 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 09:05:00.000000 ec2-demo-0.1.8/ec2_demo.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 09:05:00.059410 ec2-demo-0.1.8/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)     1002 2023-04-20 08:36:29.000000 ec2-demo-0.1.8/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 09:05:00.059011 ec2-demo-0.1.8/tests/
--rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 07:37:16.000000 ec2-demo-0.1.8/tests/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 08:32:30.000000 ec2-demo-0.1.8/tests/test_instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 10:55:57.013696 ec2-demo-0.1.9/
+-rw-r--r--   0 pedro      (503) staff       (20)     1449 2023-04-20 10:55:57.013552 ec2-demo-0.1.9/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      863 2023-04-20 10:39:27.000000 ec2-demo-0.1.9/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 10:55:57.012314 ec2-demo-0.1.9/ec2_demo/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-04-20 10:20:01.000000 ec2-demo-0.1.9/ec2_demo/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)     1599 2023-04-20 10:36:46.000000 ec2-demo-0.1.9/ec2_demo/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)     2474 2023-04-20 10:43:46.000000 ec2-demo-0.1.9/ec2_demo/instances.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 10:55:57.013160 ec2-demo-0.1.9/ec2_demo.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     1449 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      313 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       47 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       15 2023-04-20 10:55:56.000000 ec2-demo-0.1.9/ec2_demo.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-04-20 10:55:57.013739 ec2-demo-0.1.9/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)     1002 2023-04-20 10:20:01.000000 ec2-demo-0.1.9/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-04-20 10:55:57.013385 ec2-demo-0.1.9/tests/
+-rw-r--r--   0 pedro      (503) staff       (20)        0 2023-04-20 10:20:01.000000 ec2-demo-0.1.9/tests/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      767 2023-04-20 10:53:55.000000 ec2-demo-0.1.9/tests/test_instances.py
```

### Comparing `ec2-demo-0.1.8/ec2_demo/cli.py` & `ec2-demo-0.1.9/ec2_demo/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-import yaml
 import click
 import logging
 import tabulate
 
 from .instances import Instances
 from .utils.tags import Tags
 
@@ -26,15 +24,15 @@
 
 
 @ec2.command()
 @click.argument("env", type=str, required=True)
 def list(env):
     logging.debug(f"env: {env}")
     instances = Instances(env)
-    resources = instances.list()
+    resources = instances.ls()
     table = []
     headers = ["INSTANCE ID", "NAME", "STATE", "PRIVATE IP", "PUBLIC IP"]
     for instance in resources:
         name = Tags.find(instance.tags, "Name")
         table.append([
             instance.instance_id,
             name,
@@ -44,33 +42,20 @@
         ])
 
     print(tabulate.tabulate(table,headers, tablefmt="rounded_outline"))
 
 
 @ec2.command()
 @click.argument("env", type=str, required=True)
-@click.argument("ids", type=str, required=False, nargs=-1)
-@click.option("--all", is_flag=True, default=False, help="Deletes all instances")
-def delete(env, ids, all):
+@click.argument("ids", type=str, required=True, nargs=-1)
+def delete(env, ids):
     logging.debug(f"env: {env}")
     logging.debug(f"ids: {ids}")
-    logging.debug(f"all: {all}")
-
-    instances = Instances(env)
-
-    if all:
-        resources = instances.list()
-        ids = []
-        for resource in resources:
-            ids.append(resource.instance_id)
-        status = instances.delete(ids)
-
-    else:
-        status = instances.delete(ids)
-
+    inst = Instances(env)
+    status = inst.delete(ids)
     for id_, state in status.items():
         print(f"- Instance \033[32;1m{id_}\033[0m is now in state \033[32;1m{state}\033[0m.")
 
 
 def main():
     ec2()
```

### Comparing `ec2-demo-0.1.8/ec2_demo/instances.py` & `ec2-demo-0.1.9/ec2_demo/instances.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 import yaml
 import boto3
 import logging
-import threading
 
-
-from .task import Task
-from .utils.template import Template
 from .utils.tags import Tags
+from .utils.template import Template
 from .utils.loader import Loader
 
 level = os.environ.get("EC2_DEMO_LOG", "info").upper()
 logging.basicConfig(level=level)
 
+
 class Instances:
 
     def __init__(self, env):
         self.client = boto3.client("ec2")
         self.env = env
         self.loadEnv()
 
@@ -25,94 +23,68 @@
         with open(f"config/{self.env}.yaml", "r") as f:
             self.vars = yaml.safe_load(f)
         logging.debug(f"self.vars: {self.vars}")
 
 
     def create(self, path: str) ->list[str]:
         ids = []
-        threads = []
-        tasks = {}
         logging.debug(f"path: {path}")
         rendered = Template.render(path, self.vars)
         data = Loader.load(rendered)
 
         for name, config in data["instances"].items():
-            task = Task(self.vars)
-            thread = threading.Thread(
-                name=f"Task {name}",
-                target=task.create,
-                args=[name, config],
-            )
-            tasks[name] = task
-            threads.append(thread)
-            thread.start()
-
-        for thread in threads:
-            thread.join()
-
-        for name, task in tasks.items():
-            for instanceId in task.instanceIds:
-                ids.append(instanceId)
-            # instaceIds = self.createInstance(name, config)
-            # for instaceId in instaceIds:
-            #     ids.append(instaceId)
-
-        return ids
-
+            envTags = self.vars["tags"]
+            envTags.update({"Name": name})
+            awsTags = Tags.build(envTags)
+
+            logging.debug(f"Name: {name}")
+            logging.debug(f"Config: {config}")
+            logging.debug(f"Spec: {config['spec']}")
+            spec = config["spec"]
+            spec["TagSpecifications"] = [
+                {
+                    "ResourceType": "instance",
+                    "Tags": awsTags,
+                },
+            ]
+            spec["MinCount"] = 1
+            spec["MaxCount"] = 1
 
-    def createInstance(self, name: str, config: dict) ->list[str]:
-        ids = []
-        envTags = self.vars["tags"]
-        envTags.update({"Name": name})
-        awsTags = Tags.build(envTags)
-
-        logging.debug(f"Name: {name}")
-        logging.debug(f"Config: {config}")
-        logging.debug(f"Spec: {config['spec']}")
-        spec = config["spec"]
-        spec["TagSpecifications"] = [
-            {
-                "ResourceType": "instance",
-                "Tags": awsTags,
-            },
-        ]
-        spec["MinCount"] = 1
-        spec["MaxCount"] = 1
-
-        logging.debug(f"Patched spec: {spec}")
-        res = self.client.run_instances(**spec)
-
-        for instance in res["Instances"]:
-            logging.debug(f"InstanceId: {instance['InstanceId']}")
-            ids.append(instance["InstanceId"])
+            logging.debug(f"Patched spec: {spec}")
+            res = self.client.run_instances(**spec)
 
-        return ids
+            for instance in res["Instances"]:
+                logging.debug(f"InstanceId: {instance['InstanceId']}")
+                ids.append(instance["InstanceId"])
 
+            return ids
 
-    def delete(self, ids: list[str]) -> dict:
-        status = {}
-        logging.debug(f"Deleting ids: {ids}")
-        res = self.client.terminate_instances(
-            InstanceIds=ids,
-        )
-        for instance in res["TerminatingInstances"]:
-            status[instance["InstanceId"]] = instance["CurrentState"]["Name"]
 
-        return status
-
-
-    def list(self) -> list:
+    def ls(self) -> list:
         # Boto3 resources returns the ip addresses
         self.ec2 = boto3.resource("ec2")
         resources = []
         logging.debug(f"Finding ec2-demo instances...")
         res = self.ec2.instances.filter(
             Filters=[
                 {
                     "Name": "tag:CreatedBy",
                     "Values": [
                         "ec2-demo",
                     ],
                 },
             ],
         )
+
         return res
+
+
+    def delete(self, ids: list[str]) -> dict:
+        status = {}
+        logging.debug(f"Deleting ids: {ids}")
+        res = self.client.terminate_instances(
+            InstanceIds=ids,
+        )
+        for instance in res["TerminatingInstances"]:
+            status[instance["InstanceId"]] = instance["CurrentState"]["Name"]
+
+        return status
```

### Comparing `ec2-demo-0.1.8/setup.py` & `ec2-demo-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ec2-demo-0.1.8/tests/test_instances.py` & `ec2-demo-0.1.9/tests/test_instances.py`

 * *Files identical despite different names*

