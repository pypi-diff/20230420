# Comparing `tmp/tpfunc-1.2.3.tar.gz` & `tmp/tpfunc-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfunc-1.2.3.tar", last modified: Mon Jul 26 00:17:35 2021, max compression
+gzip compressed data, was "tpfunc-1.2.4.tar", last modified: Thu Apr 20 07:36:00 2023, max compression
```

## Comparing `tpfunc-1.2.3.tar` & `tpfunc-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.089716 tpfunc-1.2.3/
--rw-r--r--   0 root         (0) root         (0)     1256 2021-07-26 00:17:35.089716 tpfunc-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      615 2021-07-26 00:17:21.000000 tpfunc-1.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-26 00:17:35.089716 tpfunc-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      815 2021-07-26 00:17:21.000000 tpfunc-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.085716 tpfunc-1.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.085716 tpfunc-1.2.3/src/thingspro/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.085716 tpfunc-1.2.3/src/thingspro/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.085716 tpfunc-1.2.3/src/thingspro/edge/func_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/func_v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/func_v1/datadriven.py
--rw-rw-rw-   0 root         (0) root         (0)     2205 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/func_v1/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.089716 tpfunc-1.2.3/src/thingspro/edge/http_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/http_v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4424 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/http_v1/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.089716 tpfunc-1.2.3/src/thingspro/edge/tag_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/tag_v1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5782 2021-07-26 00:17:21.000000 tpfunc-1.2.3/src/thingspro/edge/tag_v1/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-26 00:17:35.089716 tpfunc-1.2.3/src/tpfunc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1256 2021-07-26 00:17:34.000000 tpfunc-1.2.3/src/tpfunc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2021-07-26 00:17:35.000000 tpfunc-1.2.3/src/tpfunc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-26 00:17:34.000000 tpfunc-1.2.3/src/tpfunc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-07-26 00:17:34.000000 tpfunc-1.2.3/src/tpfunc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-07-26 00:17:34.000000 tpfunc-1.2.3/src/tpfunc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-04-20 07:36:00.217606 tpfunc-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-20 07:35:51.000000 tpfunc-1.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 07:36:00.217606 tpfunc-1.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-20 07:35:51.000000 tpfunc-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/api_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/api_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/api_v1/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/func_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/datadriven.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/http_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/http_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7967 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/http_v1/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/tag_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/tag_v1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11410 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/tag_v1/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/tpfunc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/top_level.txt
```

### Comparing `tpfunc-1.2.3/PKG-INFO` & `tpfunc-1.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfunc
-Version: 1.2.3
+Version: 1.2.4
 Summary: ThingsPro Edge Function SDK
 Home-page: https://github.com/MOXA-ISD/edge-thingspro-function
 Author: Justin Tung
 Author-email: justincp.tung@moxa.com
 License: UNKNOWN
 Description: # ThingsPro Edge Function SDK
```

### Comparing `tpfunc-1.2.3/README.md` & `tpfunc-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.3/setup.py` & `tpfunc-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tpfunc", # Replace with your own username
-    version="1.2.3",
+    version="1.2.4",
     author="Justin Tung",
     author_email="justincp.tung@moxa.com",
     description="ThingsPro Edge Function SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MOXA-ISD/edge-thingspro-function",
     classifiers=[
```

### Comparing `tpfunc-1.2.3/src/thingspro/edge/func_v1/datadriven.py` & `tpfunc-1.2.4/src/thingspro/edge/func_v1/datadriven.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
         with open("/var/run/mx-api-token") as f:
             token = f.readline()
             self._headers = {"Content-Type": "application/json", "mx-api-token": token.strip()}
 
 
 class Listener(Token):
-    """The listener object used by default in data driven function
-    """
 
     def __init__(self, callback):
         super().__init__()
         self.callback = callback
         self.__config = package.Configuration()
         self.__tag_url = "http://{}:{}/{}tags/monitor".format(self._ip, self._port, self._prefix)
         self.__event_url = "http://{}:{}/{}events".format(self._ip, self._port, self._prefix)
@@ -71,15 +69,14 @@
                             print("Err: {}, {}".format(err, line))
 
             except Exception as e:
                 print(e)
             time.sleep(1)
 
     def listen(self):
-        """ subscribe function (streaming) """
         urls = {}
         for tag_url in self.__get_tag_endpoint():
             urls[tag_url] = 'tag'
         evt_url = self.__get_event_endpoint()
         if evt_url != "":
             urls[evt_url] = 'event'
         for url, _type in urls.items():
```

### Comparing `tpfunc-1.2.3/src/thingspro/edge/func_v1/package.py` & `tpfunc-1.2.4/src/thingspro/edge/func_v1/package.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import json
 
 
 class Configuration():
     """
-    The configuration object used by default in function
+    Configuration class provides the properties value in package.json
     """
     def __init__(self):
         self.__load_configuration()
         self.__load_trigger_time()
 
     def __load_configuration(self):
         try:
@@ -31,51 +31,96 @@
         self._db['params'] = {}
 
     def __load_trigger_time(self):
         data = os.getenv('DATA')
         self.__trigger_time = data if data else ""
 
     def data_driven_tags(self):
-        """The target tags that will trigger your function up.
+        """
+        Return the value of key **tags** in package.json.
+
+        :Example:
+            .. code-block:: python
+            
+                {
+                    "system": {
+                        "status": [
+                            "cpuUsage"
+                        ]
+                    }
+                }
         """
         trigger = self._db['trigger'].get('dataDriven', None)
         if trigger is None:
             return {}
         return trigger.get('tags', {})
 
     def data_driven_events(self):
-        """The target events that will trigger your function up.
+        """
+        Return the value of key **events** in package.json.
+
+        :Example:
+            .. code-block:: python
+            
+                {
+                    "system": {
+                        "status": [
+                            "cpuUsage"
+                        ]
+                    }
+                }
+
         """
         trigger = self._db['trigger'].get('dataDriven', None)
         if trigger is None:
             return {}
         return trigger.get('events', {})
 
     def name(self):
-        """The name of your function package.
+        """
+        Return the name of your function package.
 
-        Returns:
-            name (string)
+        :Example: {YOUR FUNCTION NAME}
         """
         return self._db.get('name', '')
 
     def expose_tags(self):
-        """The virtual tags created/destoried by default as
-            your function up/down.
+        """
+        Return the value of key **expose** in package.json.
+
+        :Example:
+            .. code-block::
+
+                [
+                    {
+                        "prvdName": "user",
+                        "srcName": "define",
+                        "tagName": "tag",
+                        "dataType": "double",
+                        "access": "r"
+                    }
+                ]
         """
         return self._db['expose'].get('tags', [])
 
     def parameters(self):
-        """The pre-defined parameters of your function package.
+        """
+        Return pre-defined parameters.
 
-        Returns:
-            A dict mapping keys to the corresponding table of parameters.
+        :Example:
+            .. code-block:: python
+            
+                {
+                    'version': '1.0.0',
+                    'arch': 'amd64'
+                }
 
-            example:
-            {'version': '1.0.0', 'arch': 'amd64'}
         """
         return self._db.get('params', {})
 
     def boot_time(self):
-        """The start time of your function.
+        """
+        The start time of your function.
+        
+        :Example: string in ISO-8601 date format
         """
         return self.__trigger_time
```

### Comparing `tpfunc-1.2.3/src/tpfunc.egg-info/PKG-INFO` & `tpfunc-1.2.4/src/tpfunc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfunc
-Version: 1.2.3
+Version: 1.2.4
 Summary: ThingsPro Edge Function SDK
 Home-page: https://github.com/MOXA-ISD/edge-thingspro-function
 Author: Justin Tung
 Author-email: justincp.tung@moxa.com
 License: UNKNOWN
 Description: # ThingsPro Edge Function SDK
```

