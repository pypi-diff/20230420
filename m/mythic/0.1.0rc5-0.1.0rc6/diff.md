# Comparing `tmp/mythic-0.1.0rc5.tar.gz` & `tmp/mythic-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc5.tar", last modified: Mon Apr 17 17:04:10 2023, max compression
+gzip compressed data, was "mythic-0.1.0rc6.tar", last modified: Thu Apr 20 16:27:24 2023, max compression
```

## Comparing `mythic-0.1.0rc5.tar` & `mythic-0.1.0rc6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 17:04:10.090827 mythic-0.1.0rc5/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-17 17:04:10.090439 mythic-0.1.0rc5/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc5/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 17:04:10.088221 mythic-0.1.0rc5/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc5/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc5/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    94316 2023-04-17 17:03:21.000000 mythic-0.1.0rc5/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3623 2023-04-17 17:01:54.000000 mythic-0.1.0rc5/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc5/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc5/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 17:04:10.089962 mythic-0.1.0rc5/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-17 17:04:10.000000 mythic-0.1.0rc5/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-17 17:04:10.000000 mythic-0.1.0rc5/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-17 17:04:10.000000 mythic-0.1.0rc5/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-17 17:04:10.000000 mythic-0.1.0rc5/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-17 17:04:10.000000 mythic-0.1.0rc5/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-17 17:04:10.090955 mythic-0.1.0rc5/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-17 17:01:59.000000 mythic-0.1.0rc5/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.871290 mythic-0.1.0rc6/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-20 16:27:24.870866 mythic-0.1.0rc6/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc6/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.868345 mythic-0.1.0rc6/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc6/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc6/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    95248 2023-04-20 16:26:24.000000 mythic-0.1.0rc6/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-20 16:27:07.000000 mythic-0.1.0rc6/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc6/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc6/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.870391 mythic-0.1.0rc6/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-20 16:27:24.871411 mythic-0.1.0rc6/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-20 16:26:50.000000 mythic-0.1.0rc6/setup.py
```

### Comparing `mythic-0.1.0rc5/PKG-INFO` & `mythic-0.1.0rc6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc5/README.md` & `mythic-0.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc5/mythic/graphql_queries.py` & `mythic-0.1.0rc6/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc5/mythic/mythic.py` & `mythic-0.1.0rc6/mythic/mythic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2079,24 +2079,47 @@
     return list(unique_results)
 
 
 # ####### Event Feed functions ############
 async def send_event_log_message(
         mythic: mythic_classes.Mythic,
         message: str,
-        level: str = "info"
+        level: str = "info",
+        source: str = "",
 ) -> dict:
     query = """
-    mutation SendEventLog($message: String!, $level: String!){
-        insert_operationeventlog_one(object: {level: $level, message: $message}) {
-            id
+    mutation SendEventLog($message: String!, $level: String!, $source: String){
+        createOperationEventLog(level: $level, message: $message, source: $source) {
+            status
+            error
         }
     }
     """
-    return await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={"level": level, "message": message})
+    return await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={"level": level,
+                                                                                      "message": message,
+                                                                                      "source": source})
+
+
+# ####### webhook ############
+async def send_custom_webhook_message(
+        mythic: mythic_classes.Mythic,
+        webhook_data: dict,
+        webhook_type: str = "new_custom",
+) -> dict:
+    query = """
+    mutation sendMyExternalWebhook($webhook_type: String!, $webhook_data: jsonb!){
+        sendExternalWebhook(webhook_type: $webhook_type, webhook_data: $webhook_data) {
+            status
+            error
+        }
+    }
+    """
+
+    return await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={"webhook_data": webhook_data,
+                                                                                      "webhook_type": webhook_type})
 
 # ####### Tag Functions ############
 
 
 async def create_tag_type(
         mythic: mythic_classes.Mythic,
         color: str = "#71a0d0",
```

### Comparing `mythic-0.1.0rc5/mythic/mythic_classes.py` & `mythic-0.1.0rc6/mythic/mythic_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,50 +8,44 @@
         password: str = None,
         apitoken: str = None,
         access_token: str = None,
         refresh_token: str = None,
         server_ip: str = None,
         ssl: bool = False,
         server_port: int = None,
-        server_api_version: float = 1.4,
         global_timeout: int = None,
         schema: str = None,
     ):
         self.username = username
         self.password = password
         self.apitoken = apitoken
         self.access_token = access_token
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
-        self.server_api_version = server_api_version
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.0rc5"
+        self.scripting_version = "0.1.0rc6"
         self.current_operation_id = 0
-        self.operator_id = None
-        self.operator = None
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
                 "password": self.password,
                 "apitoken": self.apitoken,
                 "access_token": self.access_token,
                 "refresh_token": self.refresh_token,
                 "server_ip": self.server_ip,
                 "server_port": self.server_port,
                 "ssl": self.ssl,
                 "current_operation_id": self.current_operation_id,
-                "operator": self.operator,
-                "operator_id": self.operator_id,
             },
             indent=4,
         )
 
 
 class MythicStatus:
     Error = "error"
```

### Comparing `mythic-0.1.0rc5/mythic/mythic_utilities.py` & `mythic-0.1.0rc6/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc5/mythic.egg-info/PKG-INFO` & `mythic-0.1.0rc6/mythic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc5/setup.py` & `mythic-0.1.0rc6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc5",
+    version="0.1.0rc6",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

