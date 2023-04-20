# Comparing `tmp/aliendev_api-0.1.4.tar.gz` & `tmp/aliendev_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_api-0.1.4.tar", max compression
+gzip compressed data, was "aliendev_api-0.1.5.tar", max compression
```

## Comparing `aliendev_api-0.1.4.tar` & `aliendev_api-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/__init__.py
--rw-r--r--   0        0        0      824 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0      479 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/config/mongo.py
--rw-r--r--   0        0        0     2325 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/main.py
--rw-r--r--   0        0        0      377 2023-04-19 20:03:07.184370 aliendev_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435969 aliendev_api-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435917 aliendev_api-0.1.5/aliendev_api/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-19 19:11:20.493960 aliendev_api-0.1.5/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0      479 2023-04-19 18:47:44.244132 aliendev_api-0.1.5/aliendev_api/config/mongo.py
+-rw-r--r--   0        0        0     2898 2023-04-20 18:53:54.796929 aliendev_api-0.1.5/aliendev_api/main.py
+-rw-r--r--   0        0        0      377 2023-04-20 18:57:58.489136 aliendev_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 aliendev_api-0.1.5/setup.py
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.5/PKG-INFO
```

### Comparing `aliendev_api-0.1.4/aliendev_api/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_api-0.1.5/aliendev_api/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.4/aliendev_api/main.py` & `aliendev_api-0.1.5/aliendev_api/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from bson.objectid import ObjectId
 from aliendev_api.config import mongo
 from pydantic import BaseModel, Field
 from enum import Enum
+import os, json
 
 def _case(param: str):
     splitter = param.lower().replace(" ", "-")
     return splitter
 
 
 method_name = ["GET", "POST", "PUT", "DELETE"]
@@ -17,19 +18,30 @@
 class ParamData(BaseModel):
     key: str = Field(..., example="name")
     data_type: str = Field(..., example="string|int|any")
     required: bool
 
 
 class ApiGateway:
-    def __init__(self, username, title) -> None:
-        self.username = username
+    def __init__(self, title) -> None:
+        self.username = ""
+        self.account_id= ""
         self.title = title
         self.stack_name = _case(title)
         self.endpoint = []
+        print("Deploying API Gateway 🤩")
+        home_folder = os.path.expanduser("~")
+        path = f'{home_folder}/.aliendev'
+        if not os.path.exists(path+"/config.json"):
+            print("Please Login first 😊")
+        else:
+            with open(path+"/config.json", "r") as file:
+                json_file = json.load(file)
+                self.username = json_file.get("username")
+                self.account_id = json_file.get("_id")
 
     def addMethod(self, method, prefix, param_type:ParamType, data:ParamData):
         """
         Args:
             method (string): "GET|POST|PUT|DELETE"
             prefix (string): "/test-get"
             param_type (ParamType): "param|body"
@@ -55,23 +67,24 @@
             }
             self.endpoint.append(endpoint)
 
     def build(self):
         objId = ObjectId()
         result_data = {
             "_id": str(objId),
+            "account_id":self.account_id,
             "username": self.username,
             "title": self.title,
             "stack_name": self.stack_name,
             "endpoint": self.endpoint
         }
         client, db = mongo.connect()
         with client:
             finder = db['gateway'].find_one(
                 {"$and": [{"username": self.username}, {"stack_name": self.stack_name}]})
             if finder:
                 newvalues = {"$set": {"endpoint": self.endpoint}}
                 db['gateway'].update_one({"_id": finder['_id']}, newvalues)
             else:
                 db['gateway'].insert_one(result_data)
-
+        print("API Gateway has deployed 🎉")
         return result_data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aliendev_api-0.1.4/PKG-INFO` & `aliendev_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

