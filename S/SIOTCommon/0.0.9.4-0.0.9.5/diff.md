# Comparing `tmp/SIOTCommon-0.0.9.4.tar.gz` & `tmp/SIOTCommon-0.0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.4.tar", last modified: Thu Apr 20 12:46:45 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.5.tar", last modified: Thu Apr 20 13:04:56 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.4.tar` & `SIOTCommon-0.0.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:46:45.001096 SIOTCommon-0.0.9.4/
--rw-rw-rw-   0        0        0      341 2023-04-20 12:46:44.999094 SIOTCommon-0.0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 12:46:44.970093 SIOTCommon-0.0.9.4/SIOTC/
--rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.4/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.4/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.4/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2453 2023-04-19 17:58:24.000000 SIOTCommon-0.0.9.4/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:46:44.997093 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      341 2023-04-20 12:46:44.000000 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-20 12:46:44.000000 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:46:44.000000 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-20 12:46:44.000000 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 12:46:44.000000 SIOTCommon-0.0.9.4/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 12:46:45.001096 SIOTCommon-0.0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-04-19 17:57:14.000000 SIOTCommon-0.0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.442831 SIOTCommon-0.0.9.5/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:04:56.442831 SIOTCommon-0.0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.421833 SIOTCommon-0.0.9.5/SIOTC/
+-rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.5/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.5/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.5/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2650 2023-04-20 13:04:33.000000 SIOTCommon-0.0.9.5/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.440834 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 13:04:56.443831 SIOTCommon-0.0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-20 13:04:46.000000 SIOTCommon-0.0.9.5/setup.py
```

### Comparing `SIOTCommon-0.0.9.4/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.5/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.4/SIOTC/Operations.py` & `SIOTCommon-0.0.9.5/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.4/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.5/SIOTC/helperhttps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from flask import request, jsonify 
 from functools import wraps
-from flask_jwt_extended import get_jwt_identity
+from flask_jwt_extended import get_jwt_identity, verify_jwt_in_request
 from enum import Enum
 import SIOTC.Operations as op
 import re
 
 # Checks what type of data is being sent and returns correct object
 def CheckContentType():
     content_type = request.headers.get('Content-Type')
@@ -36,34 +36,40 @@
         print('Content not abled to be verified or it does not match the intended format')
         return False
     
 def VerifyMacContent(content):
     regex_pattern = '^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$'
     return bool(re.match(regex_pattern, content))
 
-def admin_required(f):
-    @wraps(f)
+def admin_required(fn):
+    @wraps(fn)
     def wrapper(*args, **kwargs):
-        user = kwargs.get('id', None)
+        # Check if JWT exists and is valid
+        verify_jwt_in_request()
+
+        # Get the id from the JWT
+        jwt_id = get_jwt_identity()
+
+        user = jwt_id
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
 
         user_role = op.GetTable('users').query.filter_by(id=user).first().role.name
 
         if user_role != 'System Administrator':
             return jsonify({'message': 'You do not have permission to access this endpoint.'}), 403
-
-        return f(*args, **kwargs)
-
+        return fn(*args, **kwargs)
     return wrapper
 
-def ownership_required(f):
+
+def device_ownership_required(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
-        user = kwargs.get('id', None)
+        verify_jwt_in_request()
+        user = get_jwt_identity()
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
         deviceID = op.GetTable('devices').query.filter_by(id=user).first()
 
         if user != deviceID.user_id:
             return jsonify({'message': 'User does not own device.'}), 403
         return f(*args, **kwargs)
```

### Comparing `SIOTCommon-0.0.9.4/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.5/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.4/setup.py` & `SIOTCommon-0.0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9.4',
+    version='0.0.9.5',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

