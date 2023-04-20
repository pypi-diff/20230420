# Comparing `tmp/openfabric_pysdk-0.2.4.tar.gz` & `tmp/openfabric_pysdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfabric_pysdk-0.2.4.tar", max compression
+gzip compressed data, was "openfabric_pysdk-0.2.5.tar", max compression
```

## Comparing `openfabric_pysdk-0.2.4.tar` & `openfabric_pysdk-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.4/README.md
--rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.4/openfabric_pysdk/__init__.py
--rw-r--r--   0        0        0     5649 2023-03-30 07:45:52.716595 openfabric_pysdk-0.2.4/openfabric_pysdk/application.py
--rw-r--r--   0        0        0     3600 2023-03-30 07:45:52.768103 openfabric_pysdk-0.2.4/openfabric_pysdk/benchmark.py
--rw-r--r--   0        0        0      412 2023-03-14 13:25:56.167968 openfabric_pysdk-0.2.4/openfabric_pysdk/config.py
--rw-r--r--   0        0        0     5578 2023-04-11 19:44:10.159542 openfabric_pysdk-0.2.4/openfabric_pysdk/context.py
--rw-r--r--   0        0        0     7386 2023-03-30 07:45:52.744619 openfabric_pysdk-0.2.4/openfabric_pysdk/engine.py
--rw-r--r--   0        0        0     1993 2023-03-29 16:17:55.309405 openfabric_pysdk-0.2.4/openfabric_pysdk/loader.py
--rw-r--r--   0        0        0     1852 2023-03-30 07:45:52.736248 openfabric_pysdk-0.2.4/openfabric_pysdk/starter.py
--rw-r--r--   0        0        0     4463 2023-03-30 07:45:52.763114 openfabric_pysdk-0.2.4/openfabric_pysdk/store.py
--rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.4/openfabric_pysdk/task.py
--rw-r--r--   0        0        0    13433 2023-03-29 17:29:12.865670 openfabric_pysdk-0.2.4/openfabric_pysdk/templates/index.html
--rw-r--r--   0        0        0     3880 2023-03-16 19:44:08.374707 openfabric_pysdk-0.2.4/openfabric_pysdk/toolset.py
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.464562 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/__init__.py
--rw-r--r--   0        0        0     2609 2023-03-15 16:39:57.524646 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/queue.py
--rw-r--r--   0        0        0     1077 2023-03-15 16:31:53.418040 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/rest.py
--rw-r--r--   0        0        0     6224 2023-04-11 18:21:33.475130 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/socket.py
--rw-r--r--   0        0        0     2408 2023-03-14 13:25:56.172085 openfabric_pysdk-0.2.4/openfabric_pysdk/utility.py
--rw-r--r--   0        0        0      914 2023-04-11 14:42:48.562083 openfabric_pysdk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.5/README.md
+-rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.5/openfabric_pysdk/__init__.py
+-rw-r--r--   0        0        0     5973 2023-04-14 19:33:07.463488 openfabric_pysdk-0.2.5/openfabric_pysdk/application.py
+-rw-r--r--   0        0        0     3600 2023-03-30 07:45:52.768103 openfabric_pysdk-0.2.5/openfabric_pysdk/benchmark.py
+-rw-r--r--   0        0        0      412 2023-03-14 13:25:56.167968 openfabric_pysdk-0.2.5/openfabric_pysdk/config.py
+-rw-r--r--   0        0        0     5578 2023-04-11 19:44:10.159542 openfabric_pysdk-0.2.5/openfabric_pysdk/context.py
+-rw-r--r--   0        0        0     7445 2023-04-14 07:07:30.349151 openfabric_pysdk-0.2.5/openfabric_pysdk/engine.py
+-rw-r--r--   0        0        0     1993 2023-03-29 16:17:55.309405 openfabric_pysdk-0.2.5/openfabric_pysdk/loader.py
+-rw-r--r--   0        0        0     1847 2023-04-14 19:08:23.089026 openfabric_pysdk-0.2.5/openfabric_pysdk/starter.py
+-rw-r--r--   0        0        0     4463 2023-03-30 07:45:52.763114 openfabric_pysdk-0.2.5/openfabric_pysdk/store.py
+-rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.5/openfabric_pysdk/task.py
+-rw-r--r--   0        0        0    13433 2023-03-29 17:29:12.865670 openfabric_pysdk-0.2.5/openfabric_pysdk/templates/index.html
+-rw-r--r--   0        0        0     3927 2023-04-14 19:55:42.380807 openfabric_pysdk-0.2.5/openfabric_pysdk/toolset.py
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.464562 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/__init__.py
+-rw-r--r--   0        0        0     2609 2023-03-15 16:39:57.524646 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/queue.py
+-rw-r--r--   0        0        0     1077 2023-04-14 07:05:53.611228 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/rest.py
+-rw-r--r--   0        0        0     6224 2023-04-14 19:04:51.739451 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/socket.py
+-rw-r--r--   0        0        0     2404 2023-04-14 20:26:38.835024 openfabric_pysdk-0.2.5/openfabric_pysdk/utility.py
+-rw-r--r--   0        0        0      914 2023-04-20 14:46:51.646435 openfabric_pysdk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.5/PKG-INFO
```

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/application.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ----------------------------
+# Perform GEVENT monkey patch
+# ----------------------------
+from gevent import monkey
+monkey.patch_all()
+
 import logging
 
 from apispec import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin
 from flask import Flask, session
 from flask_apispec import FlaskApiSpec
 from flask_restful import Api
@@ -21,14 +27,15 @@
     __api: Api = None
     __app: Flask = None
     __socket: Socket = None
     __docs: FlaskApiSpec = None
 
     # ------------------------------------------------------------------------
     def __init__(self, app: Flask):
+        monkey.patch_all()
         self.__app = app
         self.__api = Api(app)
         self.__docs = FlaskApiSpec(app)
         self.state = State()
 
     # ------------------------------------------------------------------------
     def install_specs__rest(self, endpoint):
@@ -108,16 +115,19 @@
         logging.info(f"Openfabric - install Execution SOCKET endpoints on {endpoint}")
         self.__socket = Socket(endpoint, session, self.__app, self.state)
 
     # ------------------------------------------------------------------------
     def install_configuration(self):
         logging.info(f"Openfabric - install APP configuration")
         if config_callback_function:
-            items = state_config.all().items()
-            config = dict(map(lambda kv: (kv[0], ConfigSchema().load(kv[1])), items))
-            if config:
-                config_callback_function(config, self.state)
+            try:
+                items = state_config.all().items()
+                config = dict(map(lambda kv: (kv[0], ConfigSchema().load(kv[1])), items))
+                if config:
+                    config_callback_function(config, self.state)
+            except Exception as e:
+                logging.error(f"Openfabric - invalid configuration can\'t restored : {e}")
 
     # ------------------------------------------------------------------------
     def run(self, debug, host, port):
         self.__socket.run(debug=debug, host=host, port=port)
         # self.__app.run(debug=debug, host=host, port=port)
```

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/benchmark.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/benchmark.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/context.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/context.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/engine.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 import traceback
 import uuid
 from time import sleep
 from typing import Dict, Any, List
 
 from openfabric_pysdk.benchmark import MeasureBlockTime
-from openfabric_pysdk.context import RayStatus, Ray, RaySchema, State
+from openfabric_pysdk.context import RayStatus, Ray, RaySchema, State, MessageType
 from openfabric_pysdk.loader import InputSchema, execution_callback_function, OutputSchema
 from openfabric_pysdk.store import Store
 from openfabric_pysdk.task import Task
 
 
 #######################################################
 #  Foreground Engine
@@ -66,20 +66,21 @@
                 if data is None:
                     return None
 
                 ray.status = RayStatus.RUNNING
                 self.write(qid, 'ray', ray, RaySchema().dump)
                 output = execution_callback_function(data, ray, self.__state)
                 ray.status = RayStatus.COMPLETED
-                ray.progress(step=100)
-            except Exception as e:
-                logging.error(f"Openfabric - failed executing: [{qid}]{e}")
-                traceback.print_exc()
+            except:
+                error = f"Openfabric - failed executing: [{qid}]\n{traceback.format_exc()}"
+                logging.error(error)
+                ray.message(MessageType.ERROR, error)
                 ray.status = RayStatus.FAILED
         ray.finished = True
+        ray.progress(step=100)
         self.write(qid, 'ray', ray, RaySchema().dump)
         self.write(qid, 'out', output, OutputSchema().dump)
 
         return output
 
     # ------------------------------------------------------------------------
     def read(self, qid: str, key: str, deserializer=None) -> Any:
```

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/loader.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/loader.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/starter.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/starter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import pathlib
 import traceback
 
-from flask import Flask, app, render_template
+from flask import Flask, render_template
 from flask_cors import CORS
 
-from openfabric_pysdk.config import manifest
 from openfabric_pysdk.application import Application
+from openfabric_pysdk.config import manifest
 from openfabric_pysdk.context import StateStatus
 
 FlaskApp = Flask(__name__, template_folder=f"{pathlib.Path(__file__).parent}/templates")
 CORS(FlaskApp)
 
 
 @FlaskApp.route("/")
```

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/store.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/store.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/task.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/task.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/templates/index.html` & `openfabric_pysdk-0.2.5/openfabric_pysdk/templates/index.html`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/toolset.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/toolset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Union
-from flask_apispec import marshal_with, doc
+from flask_apispec import marshal_with, doc, use_kwargs
 from flask_apispec.views import MethodResource
 from flask_restful import Resource
 from marshmallow import fields, Schema, post_load
 from webargs.flaskparser import use_args
 from openfabric_pysdk import benchmark
 from openfabric_pysdk.config import manifest, state_config
 from openfabric_pysdk.context import State
@@ -31,32 +31,32 @@
     __state: State = None
 
     # ------------------------------------------------------------------------
     def __init__(self, state: State = None):
         self.__state = state
 
     @doc(description="Get APP configuration", tags=["Developer"])
-    @use_args(UserIdSchema, location='query')
+    @use_kwargs(UserIdSchema, location='query')
     @marshal_with(ConfigSchema)
     def get(self, uidc: UserIdClass) -> ConfigClass:
         with MeasureBlockTime("ConfigRestApi::get"):
             config = state_config.get(uidc.uid)
             if config is False:
                 return dict()
             return config
 
     @doc(description="Set APP configuration", tags=["Developer"])
-    @use_args(UserIdSchema, location='query')
-    @use_args(ConfigSchema, location='json')
+    @use_kwargs(UserIdSchema, location='query')
+    @use_kwargs(ConfigSchema, location='json')
     @marshal_with(ConfigSchema)
     def post(self, uidc: UserIdClass, config: Union[ConfigClass, List[ConfigClass]]) -> ConfigClass:
 
         with MeasureBlockTime("ConfigRestApi::post"):
-            if ConfigSchema().many is True:
-                config = list(config)
+            if ConfigSchema().many is True and not isinstance(config, list):
+                config = [config]
             else:
                 config = config[0] if type(config) == list else config
             state_config.set(uidc.uid, ConfigSchema().dump(config))
             if config_callback_function:
                 config = dict(map(lambda kv: (kv[0], ConfigSchema().load(kv[1])), state_config.all().items()))
                 config_callback_function(config, self.__state)
             return config
```

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/queue.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/transport/queue.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/rest.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/transport/rest.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/socket.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/transport/socket.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.4/openfabric_pysdk/utility.py` & `openfabric_pysdk-0.2.5/openfabric_pysdk/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         content_hash = cls.changes.get(name)
         new_content_hash = md5(str(content).encode('utf-8')).hexdigest()
         cls.changes.put(name, new_content_hash)
         return content_hash != new_content_hash
 
 
 #######################################################
-#  Change detector
+#  Schema util
 #######################################################
 class SchemaUtil:
 
     @staticmethod
     def create(instance: Any, data: Dict[Any, Any]):
         for key in data:
             instance.__setattr__(key, data[key])
```

### Comparing `openfabric_pysdk-0.2.4/pyproject.toml` & `openfabric_pysdk-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openfabric-pysdk"
-version = "0.2.4"
+version = "0.2.5"
 description = "Openfabric Python SDK"
 authors = ["Andrei Tara <andrei@openfabric.ai>"]
 readme = "README.md"
 homepage = "https://openfabric.ai"
 repository = "https://github.com/Openfabric/openfabic-pysdk"
 keywords = ["openfabric", "SDK", "IoAI"]
 classifiers = [
```

### Comparing `openfabric_pysdk-0.2.4/PKG-INFO` & `openfabric_pysdk-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfabric-pysdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Openfabric Python SDK
 Home-page: https://openfabric.ai
 Keywords: openfabric,SDK,IoAI
 Author: Andrei Tara
 Author-email: andrei@openfabric.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

