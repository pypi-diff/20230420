# Comparing `tmp/balena_sdk_python-12.6.11.tar.gz` & `tmp/balena_sdk_python-12.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877.tar", max compression
+gzip compressed data, was "balena_sdk_python-12.6.12.tar", max compression
```

## Comparing `balena_sdk_python-12.6.11.tar` & `balena_sdk_python-12.6.12.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     9724 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/LICENSE
--rwxr-xr-x   0        0        0     3726 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/README.md
--rw-r--r--   0        0        0     1496 2023-04-20 16:15:10.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/__init__.py
--rw-r--r--   0        0        0    10624 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/auth.py
--rw-r--r--   0        0        0     9808 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/base_request.py
--rw-r--r--   0        0        0    13211 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/exceptions.py
--rw-r--r--   0        0        0     5158 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/logs.py
--rw-r--r--   0        0        0     1199 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/__init__.py
--rw-r--r--   0        0        0     7500 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/api_key.py
--rw-r--r--   0        0        0    55896 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/application.py
--rw-r--r--   0        0        0     1005 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/config.py
--rw-r--r--   0        0        0     9774 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/config_variable.py
--rw-r--r--   0        0        0    66881 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device.py
--rw-r--r--   0        0        0    25902 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device_os.py
--rw-r--r--   0        0        0     3610 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device_type.py
--rw-r--r--   0        0        0    26583 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/environment_variables.py
--rw-r--r--   0        0        0     8331 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/history.py
--rw-r--r--   0        0        0     1903 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/hup.py
--rw-r--r--   0        0        0     2379 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/image.py
--rw-r--r--   0        0        0     2373 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/key.py
--rw-r--r--   0        0        0    22244 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/organization.py
--rw-r--r--   0        0        0    11469 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/release.py
--rw-r--r--   0        0        0     1061 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/service.py
--rw-r--r--   0        0        0     1180 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/service_install.py
--rw-r--r--   0        0        0    22351 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/supervisor.py
--rw-r--r--   0        0        0    16200 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/tag.py
--rw-r--r--   0        0        0     2886 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/resources.py
--rw-r--r--   0        0        0     6694 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/settings.py
--rw-r--r--   0        0        0     5626 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/twofactor_auth.py
--rw-r--r--   0        0        0      830 2023-04-20 16:14:56.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/utils.py
--rw-r--r--   0        0        0      784 2023-04-20 16:22:32.683726 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/pyproject.toml
--rw-r--r--   0        0        0     4573 1970-01-01 00:00:00.000000 balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/PKG-INFO
+-rw-r--r--   0        0        0     9724 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/LICENSE
+-rwxr-xr-x   0        0        0     3730 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/README.md
+-rw-r--r--   0        0        0     1496 2023-04-20 17:41:20.000000 balena_sdk_python-12.6.12/balena/__init__.py
+-rw-r--r--   0        0        0    10624 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/auth.py
+-rw-r--r--   0        0        0     9808 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/base_request.py
+-rw-r--r--   0        0        0    13211 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/exceptions.py
+-rw-r--r--   0        0        0     5158 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/logs.py
+-rw-r--r--   0        0        0     1199 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/__init__.py
+-rw-r--r--   0        0        0     7500 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/api_key.py
+-rw-r--r--   0        0        0    55896 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/application.py
+-rw-r--r--   0        0        0     1005 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/config.py
+-rw-r--r--   0        0        0     9774 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/config_variable.py
+-rw-r--r--   0        0        0    66881 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/device.py
+-rw-r--r--   0        0        0    25902 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/device_os.py
+-rw-r--r--   0        0        0     3610 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/device_type.py
+-rw-r--r--   0        0        0    26583 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/environment_variables.py
+-rw-r--r--   0        0        0     8331 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/history.py
+-rw-r--r--   0        0        0     1903 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/hup.py
+-rw-r--r--   0        0        0     2379 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/image.py
+-rw-r--r--   0        0        0     2373 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/key.py
+-rw-r--r--   0        0        0    22244 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/organization.py
+-rw-r--r--   0        0        0    11469 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/release.py
+-rw-r--r--   0        0        0     1061 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/service.py
+-rw-r--r--   0        0        0     1180 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/service_install.py
+-rw-r--r--   0        0        0    22351 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/supervisor.py
+-rw-r--r--   0        0        0    16200 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/models/tag.py
+-rw-r--r--   0        0        0     2886 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/resources.py
+-rw-r--r--   0        0        0     6694 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/settings.py
+-rw-r--r--   0        0        0     5626 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/twofactor_auth.py
+-rw-r--r--   0        0        0      830 2023-04-20 17:41:05.000000 balena_sdk_python-12.6.12/balena/utils.py
+-rw-r--r--   0        0        0      732 2023-04-20 17:41:20.000000 balena_sdk_python-12.6.12/pyproject.toml
+-rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 balena_sdk_python-12.6.12/PKG-INFO
```

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/LICENSE` & `balena_sdk_python-12.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/README.md` & `balena_sdk_python-12.6.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ```
 
 Documentation
 -------------
 
 We generate markdown documentation in [DOCUMENTATION.md](https://github.com/balena-io/balena-sdk-python/blob/master/DOCUMENTATION.md).
 
-To generate the documentation:
+To generate the documentation run:
 ```bash
 python docs_generator.py > DOCUMENTATION.md
 ```
 
 Deprecation policy
 ------------------
```

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/__init__.py` & `balena_sdk_python-12.6.12/balena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .auth import Auth
 from .logs import Logs
 from .settings import Settings
 from .models import Models
 from .twofactor_auth import TwoFactorAuth
 
 
-__version__ = "12.6.11"
+__version__ = "12.6.12"
 
 
 class Balena:
     """
     This class implements all functions supported by the python SDK.
     Attributes:
             settings (Settings): configuration settings for balena python SDK.
```

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/auth.py` & `balena_sdk_python-12.6.12/balena/auth.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/base_request.py` & `balena_sdk_python-12.6.12/balena/base_request.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/exceptions.py` & `balena_sdk_python-12.6.12/balena/exceptions.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/logs.py` & `balena_sdk_python-12.6.12/balena/logs.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/__init__.py` & `balena_sdk_python-12.6.12/balena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/api_key.py` & `balena_sdk_python-12.6.12/balena/models/api_key.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/application.py` & `balena_sdk_python-12.6.12/balena/models/application.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/config.py` & `balena_sdk_python-12.6.12/balena/models/config.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/config_variable.py` & `balena_sdk_python-12.6.12/balena/models/config_variable.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device.py` & `balena_sdk_python-12.6.12/balena/models/device.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device_os.py` & `balena_sdk_python-12.6.12/balena/models/device_os.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/device_type.py` & `balena_sdk_python-12.6.12/balena/models/device_type.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/environment_variables.py` & `balena_sdk_python-12.6.12/balena/models/environment_variables.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/history.py` & `balena_sdk_python-12.6.12/balena/models/history.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/hup.py` & `balena_sdk_python-12.6.12/balena/models/hup.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/image.py` & `balena_sdk_python-12.6.12/balena/models/image.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/key.py` & `balena_sdk_python-12.6.12/balena/models/key.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/organization.py` & `balena_sdk_python-12.6.12/balena/models/organization.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/release.py` & `balena_sdk_python-12.6.12/balena/models/release.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/service.py` & `balena_sdk_python-12.6.12/balena/models/service.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/service_install.py` & `balena_sdk_python-12.6.12/balena/models/service_install.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/supervisor.py` & `balena_sdk_python-12.6.12/balena/models/supervisor.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/models/tag.py` & `balena_sdk_python-12.6.12/balena/models/tag.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/resources.py` & `balena_sdk_python-12.6.12/balena/resources.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/settings.py` & `balena_sdk_python-12.6.12/balena/settings.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/twofactor_auth.py` & `balena_sdk_python-12.6.12/balena/twofactor_auth.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/balena/utils.py` & `balena_sdk_python-12.6.12/balena/utils.py`

 * *Files identical despite different names*

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/pyproject.toml` & `balena_sdk_python-12.6.12/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balena-sdk-python"
-version = "12.6.11-dev545216588577956377958917887085997974804250675877"
+version = "12.6.12"
 description = ""
 authors = ["Balena <info@balena.io>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "balena"}]
 
 [tool.poetry.dependencies]
```

### Comparing `balena_sdk_python-12.6.11.dev545216588577956377958917887085997974804250675877/PKG-INFO` & `balena_sdk_python-12.6.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balena-sdk-python
-Version: 12.6.11.dev545216588577956377958917887085997974804250675877
+Version: 12.6.12
 Summary: 
 License: Apache-2.0
 Author: Balena
 Author-email: info@balena.io
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -87,15 +87,15 @@
 ```
 
 Documentation
 -------------
 
 We generate markdown documentation in [DOCUMENTATION.md](https://github.com/balena-io/balena-sdk-python/blob/master/DOCUMENTATION.md).
 
-To generate the documentation:
+To generate the documentation run:
 ```bash
 python docs_generator.py > DOCUMENTATION.md
 ```
 
 Deprecation policy
 ------------------
```

