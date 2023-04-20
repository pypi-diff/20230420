# Comparing `tmp/simple_flask_restful-0.2.0.tar.gz` & `tmp/simple_flask_restful-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_flask_restful-0.2.0.tar", last modified: Sun Apr 16 21:18:08 2023, max compression
+gzip compressed data, was "simple_flask_restful-0.3.0.tar", last modified: Thu Apr 20 02:14:46 2023, max compression
```

## Comparing `simple_flask_restful-0.2.0.tar` & `simple_flask_restful-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.654151 simple_flask_restful-0.2.0/
--rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-04-16 02:39:40.000000 simple_flask_restful-0.2.0/LICENSE
--rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-16 21:18:08.654025 simple_flask_restful-0.2.0/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)     3913 2023-04-16 02:53:09.000000 simple_flask_restful-0.2.0/README.md
--rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-04-16 21:18:08.654196 simple_flask_restful-0.2.0/setup.cfg
--rw-r--r--   0 wwang2     (501) staff       (20)      858 2023-04-16 21:12:42.000000 simple_flask_restful-0.2.0/setup.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.651895 simple_flask_restful-0.2.0/src/
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.653104 simple_flask_restful-0.2.0/src/simple_flask_restful/
--rw-r--r--   0 wwang2     (501) staff       (20)      358 2023-04-16 21:04:02.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/__init__.py
--rw-r--r--   0 wwang2     (501) staff       (20)      733 2023-04-13 00:01:43.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/decorator_method.py
--rw-r--r--   0 wwang2     (501) staff       (20)     1912 2023-04-15 09:37:19.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/reqparse.py
--rw-r--r--   0 wwang2     (501) staff       (20)      296 2023-04-15 05:22:11.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/restful_exceptions.py
--rw-r--r--   0 wwang2     (501) staff       (20)     2370 2023-04-13 10:56:46.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/simple_restful.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.653824 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/
--rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/SOURCES.txt
--rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/dependency_links.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       27 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/requires.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/top_level.txt
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-20 02:14:46.430687 simple_flask_restful-0.3.0/
+-rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-04-16 02:39:40.000000 simple_flask_restful-0.3.0/LICENSE
+-rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-20 02:14:46.430537 simple_flask_restful-0.3.0/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)     3913 2023-04-16 02:53:09.000000 simple_flask_restful-0.3.0/README.md
+-rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-04-20 02:14:46.430734 simple_flask_restful-0.3.0/setup.cfg
+-rw-r--r--   0 wwang2     (501) staff       (20)      858 2023-04-20 00:36:36.000000 simple_flask_restful-0.3.0/setup.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-20 02:14:46.427591 simple_flask_restful-0.3.0/src/
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-20 02:14:46.429494 simple_flask_restful-0.3.0/src/simple_flask_restful/
+-rw-r--r--   0 wwang2     (501) staff       (20)      358 2023-04-20 00:36:36.000000 simple_flask_restful-0.3.0/src/simple_flask_restful/__init__.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      733 2023-04-13 00:01:43.000000 simple_flask_restful-0.3.0/src/simple_flask_restful/decorator_method.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     2447 2023-04-19 23:50:27.000000 simple_flask_restful-0.3.0/src/simple_flask_restful/reqparse.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      296 2023-04-15 05:22:11.000000 simple_flask_restful-0.3.0/src/simple_flask_restful/restful_exceptions.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     2370 2023-04-13 10:56:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful/simple_restful.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-20 02:14:46.430313 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/
+-rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-20 02:14:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-04-20 02:14:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/SOURCES.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-04-20 02:14:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/dependency_links.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       27 2023-04-20 02:14:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/requires.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-04-20 02:14:46.000000 simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/top_level.txt
```

### Comparing `simple_flask_restful-0.2.0/LICENSE` & `simple_flask_restful-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.2.0/PKG-INFO` & `simple_flask_restful-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_flask_restful
-Version: 0.2.0
+Version: 0.3.0
 Summary: wrap up flask for restful interface
 Home-page: https://github.com/AutomationLover/simple_flask_restful
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simple_flask_restful-0.2.0/README.md` & `simple_flask_restful-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.2.0/setup.py` & `simple_flask_restful-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='simple_flask_restful',
-    version='0.2.0',
+    version='0.3.0',
     author='William Wang',
     author_email='williamwangatsydney@gmail.com',
     description='wrap up flask for restful interface',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/AutomationLover/simple_flask_restful',
     packages=find_packages(where='src'),
```

### Comparing `simple_flask_restful-0.2.0/src/simple_flask_restful/decorator_method.py` & `simple_flask_restful-0.3.0/src/simple_flask_restful/decorator_method.py`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.2.0/src/simple_flask_restful/reqparse.py` & `simple_flask_restful-0.3.0/src/simple_flask_restful/reqparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,72 @@
 from flask import request
 from .restful_exceptions import BadRequest
 
-    
+
 def get_args_from_request():
     if request.is_json:
         request_args = request.get_json()
     else:
         request_args = request.args.to_dict()
     return request_args
 
 
 class Parser:
     def __init__(self):
         self.args = []
+        self.errors = {}
     
     def add_argument(self, name, dest=None, required=False, type=None, choices=None, help=None, default=None):
         self.args.append({
             'name': name,
             'dest': dest or name,
             'required': required,
             'type': type,
             'choices': choices,
             'help': help,
             'default': default,
         })
-
-    def parse_args(self, request_args, strict):
+    
+    def parse_args(self, request_args, strict, bundle_errors):
         args = {}
+        self.errors = {}
+        
+        def error(message, para_name):
+            if bundle_errors is False:
+                raise BadRequest(message)
+            else:
+                self.errors[para_name] = message
+                
         if strict:
             extra_args = set(request_args.keys()) - set(arg['name'] for arg in self.args)
             if extra_args:
-                raise BadRequest(f"Got unexpected arguments: {', '.join(extra_args)}")
-    
+                message = f"Got unexpected arguments: {', '.join(extra_args)}"
+                error(message, '_error')
+ 
         for arg in self.args:
             value = request_args.get(arg['name'], arg.get('default', None))
             if value is None and arg['required']:
-                raise BadRequest(f"{arg['name']} is required.")
-        
+                message = f"{arg['name']} is required."
+                error(message, arg['name'])
+            
             if value is not None:
                 if arg['type']:
                     try:
                         value = arg['type'](value)
                     except Exception:
                         message = f"{arg['name']} should be {arg['type'].__name__}."
-                        raise BadRequest(message)
+                        error(message, arg['name'])
                 if arg.get('choices') and value not in arg['choices']:
-                    raise BadRequest(f"{arg['name']} must be one of {arg['choices']}.")
+                    message = f"{arg['name']} must be one of {arg['choices']}."
+                    error(message, arg['name'])
+                    
             args[arg['dest']] = value
+        
+        if bundle_errors and self.errors:
+            raise BadRequest(self.errors)
         return args
 
 
 class RequestParser(Parser):
-    def parse_args(self, strict=False):
+    def parse_args(self, strict=False, bundle_errors=False):
         request_args = get_args_from_request()
-        return super().parse_args(request_args, strict)
-    
+        return super().parse_args(request_args, strict, bundle_errors)
```

### Comparing `simple_flask_restful-0.2.0/src/simple_flask_restful/simple_restful.py` & `simple_flask_restful-0.3.0/src/simple_flask_restful/simple_restful.py`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/PKG-INFO` & `simple_flask_restful-0.3.0/src/simple_flask_restful.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-flask-restful
-Version: 0.2.0
+Version: 0.3.0
 Summary: wrap up flask for restful interface
 Home-page: https://github.com/AutomationLover/simple_flask_restful
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

