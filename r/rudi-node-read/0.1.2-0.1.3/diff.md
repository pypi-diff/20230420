# Comparing `tmp/rudi-node-read-0.1.2.tar.gz` & `tmp/rudi-node-read-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudi-node-read-0.1.2.tar", last modified: Wed Apr 19 13:37:28 2023, max compression
+gzip compressed data, was "rudi-node-read-0.1.3.tar", last modified: Thu Apr 20 14:22:59 2023, max compression
```

## Comparing `rudi-node-read-0.1.2.tar` & `rudi-node-read-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.929045 rudi-node-read-0.1.2/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.2/LICENCE.md
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1871 2023-04-19 13:37:28.928741 rudi-node-read-0.1.2/PKG-INFO
--rw-r--r--   0 omartine (660741) dept-aac (29120)      792 2023-04-19 13:28:20.000000 rudi-node-read-0.1.2/README.md
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1269 2023-04-19 13:35:42.000000 rudi-node-read-0.1.2/pyproject.toml
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-04-19 13:37:28.929126 rudi-node-read-0.1.2/setup.cfg
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.918375 rudi-node-read-0.1.2/src/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.920251 rudi-node-read-0.1.2/src/rudi_node_read/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.923473 rudi-node-read-0.1.2/src/rudi_node_read/connectors/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     5148 2023-04-19 12:30:07.000000 rudi-node-read-0.1.2/src/rudi_node_read/connectors/io_connector.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     3993 2023-04-19 12:57:38.000000 rudi-node-read-0.1.2/src/rudi_node_read/connectors/io_rudi_api.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)    19661 2023-04-19 12:52:26.000000 rudi-node-read-0.1.2/src/rudi_node_read/rudi_node_reader.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.928110 rudi-node-read-0.1.2/src/rudi_node_read/utils/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     2037 2023-04-19 12:31:16.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/err.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      834 2023-03-31 08:32:41.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/jwt.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-04-19 12:57:54.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/log.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      308 2023-04-04 08:52:42.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/serializable.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     8436 2023-04-19 12:31:29.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/type_dict.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     2548 2023-04-19 12:31:32.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/type_string.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1495 2023-04-19 12:31:35.000000 rudi-node-read-0.1.2/src/rudi_node_read/utils/types.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:37:28.922581 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1871 2023-04-19 13:37:28.000000 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/PKG-INFO
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      623 2023-04-19 13:37:28.000000 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/SOURCES.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-04-19 13:37:28.000000 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/dependency_links.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       56 2023-04-19 13:37:28.000000 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/requires.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-04-19 13:37:28.000000 rudi-node-read-0.1.2/src/rudi_node_read.egg-info/top_level.txt
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.063051 rudi-node-read-0.1.3/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.3/LICENCE.md
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2068 2023-04-20 14:22:59.062530 rudi-node-read-0.1.3/PKG-INFO
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      924 2023-04-20 08:32:38.000000 rudi-node-read-0.1.3/README.md
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1450 2023-04-20 14:22:49.000000 rudi-node-read-0.1.3/pyproject.toml
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-04-20 14:22:59.063189 rudi-node-read-0.1.3/setup.cfg
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.049723 rudi-node-read-0.1.3/src/
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.051912 rudi-node-read-0.1.3/src/rudi_node_read/
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.055203 rudi-node-read-0.1.3/src/rudi_node_read/connectors/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     5148 2023-04-19 12:30:07.000000 rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_connector.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     3993 2023-04-19 12:57:38.000000 rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_rudi_api.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)    19661 2023-04-19 12:52:26.000000 rudi-node-read-0.1.3/src/rudi_node_read/rudi_node_reader.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.061018 rudi-node-read-0.1.3/src/rudi_node_read/utils/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     2010 2023-04-20 12:06:46.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/err.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      851 2023-04-20 12:31:59.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/jwt.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-04-20 08:56:10.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/log.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      308 2023-04-20 12:40:43.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/serializable.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     5185 2023-04-20 14:19:11.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/type_dict.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1570 2023-04-20 13:26:33.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/type_string.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      829 2023-04-20 14:20:44.000000 rudi-node-read-0.1.3/src/rudi_node_read/utils/types.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.054200 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2068 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      654 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/SOURCES.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/dependency_links.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       70 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/requires.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-04-20 14:22:59.000000 rudi-node-read-0.1.3/src/rudi_node_read.egg-info/top_level.txt
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-20 14:22:59.061724 rudi-node-read-0.1.3/tests/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     3171 2023-04-20 09:46:35.000000 rudi-node-read-0.1.3/tests/test_rudi_node_reader.py
```

### Comparing `rudi-node-read-0.1.2/LICENCE.md` & `rudi-node-read-0.1.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.2/PKG-INFO` & `rudi-node-read-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
+Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
 Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -45,7 +46,15 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+## Testing
+
+```bash
+pip install pytest-cov
+
+python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+```
+
```

### Comparing `rudi-node-read-0.1.2/README.md` & `rudi-node-read-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -21,7 +21,15 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+## Testing
+
+```bash
+pip install pytest-cov
+
+python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+```
+
```

### Comparing `rudi-node-read-0.1.2/pyproject.toml` & `rudi-node-read-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudi-node-read"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Olivier Martineau", email = "olivier.martineau@irisa.fr" }]
+maintainers = [{ name = "Olivier Martineau", email = "olivier.martineau@irisa.fr" }]
 description = "Use the external API of a RUDI Producer node"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "EUPL-1.2" }
 classifiers = ["Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -23,14 +24,17 @@
 
 [project.urls]
 repository = "https://github.com/OlivierMartineau/rudi-node-read"
 documentation = "https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER"
 changelog = "https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md"
 
 [project.optional-dependencies]
-packaging = ["build", "twine", "pip-autoremove"]
-tests = ["pytest"]
+packaging = ["build", "twine", "pip-chill", "pip-autoremove"]
+tests = ["pytest-cov"]
+
+[tool.pytest.ini_options]
+norecursedirs = ["*.egg", ".eggs", "dist", "build"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["rudi_node_read*"]
```

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/connectors/io_connector.py` & `rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_connector.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/connectors/io_rudi_api.py` & `rudi-node-read-0.1.3/src/rudi_node_read/connectors/io_rudi_api.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/rudi_node_reader.py` & `rudi-node-read-0.1.3/src/rudi_node_read/rudi_node_reader.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/utils/err.py` & `rudi-node-read-0.1.3/src/rudi_node_read/utils/err.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     def __init__(self, ini_section: str, ini_subsection: str, err_msg: str):
         super().__init__(f'Unexpected value in INI config file for parameter {ini_section}.{ini_subsection}: {err_msg}')
 
 
 class UnexpectedValueException(Exception):
     def __init__(self, param_name: str, expected_val, received_val):
         super().__init__(
-            f"Unexpected value for parameter '{param_name}': expected {expected_val}, got '{received_val}'")
+            f"Unexpected value for parameter '{param_name}': expected '{expected_val}', got '{received_val}'")
 
 
 class LiteralUnexpectedValueException(Exception):
     def __init__(self, err_msg, expected_literal, received_val):
-        super().__init__(f"{err_msg}. "
-                         f"Expected {get_args(expected_literal)}, got '{received_val}'")
+        super().__init__(f"{err_msg}. Expected {get_args(expected_literal)}, got '{received_val}'")
 
 
 def rudi_api_http_error_to_string(status, err_type, err_msg):
     return f"ERR {status} {err_type}: {err_msg}"
 
 
 class HttpError(Exception):
```

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/utils/jwt.py` & `rudi-node-read-0.1.3/src/rudi_node_read/utils/jwt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from base64 import urlsafe_b64decode, urlsafe_b64encode
 from json import loads
 from math import ceil
 from time import time
 
 
-def is_jwt_expired(jwt_b64: str) -> bool:
-    jwt_head_b64, jwt_body_b64, jwt_sign_b64 = jwt_b64.split('.')
-    jwt_body_b64_pad = pad_b64_str(jwt_body_b64)
-    jwt_str = urlsafe_b64decode(jwt_body_b64_pad).decode('utf-8')
-    jwt_json = loads(jwt_str)
-    exp = int(jwt_json['exp'])
-    now_epoch_s = ceil(time())
-    return exp < now_epoch_s
-
-
 def pad_b64_str(jwt_base64url: str):
     jwt_str_length = len(jwt_base64url)
     div, mod = divmod(jwt_str_length, 4)
     return jwt_base64url if mod == 0 else jwt_base64url.ljust(jwt_str_length + 4 - mod, '=')
 
 
 def get_jwt_basic_auth(usr: str, pwd: str):
-    token = urlsafe_b64encode(bytes(f'{usr}:{pwd}', 'utf-8')).decode('ascii')
+    token = urlsafe_b64encode(bytes(f'{usr}:{pwd}', 'utf-8')).decode('ascii').replace('=', '')
     return f'Basic {token}'
+
+
+def is_jwt_expired(jwt_b64: str) -> bool:
+    jwt_head_b64, jwt_body_b64, jwt_sign_b64 = jwt_b64.split('.')
+    jwt_body_b64_pad = pad_b64_str(jwt_body_b64)
+    jwt_str = urlsafe_b64decode(jwt_body_b64_pad).decode('utf-8')
+    jwt_json = loads(jwt_str)
+    exp = int(jwt_json['exp'])
+    now_epoch_s = ceil(time())
+    return exp < now_epoch_s
```

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read/utils/log.py` & `rudi-node-read-0.1.3/src/rudi_node_read/utils/log.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read.egg-info/PKG-INFO` & `rudi-node-read-0.1.3/src/rudi_node_read.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
+Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
 Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -45,7 +46,15 @@
 node_reader = RudiNodeReader('https://bacasable.fenix.rudi-univ-rennes1.fr')
 print(node_reader.metadata_count)
 print(len(node_reader.metadata_list))
 print(node_reader.organization_names)
 print(node_reader.find_metadata_with_media_name('toucan.jpg'))
 
 ```
+## Testing
+
+```bash
+pip install pytest-cov
+
+python3 -m pytest --cov=rudi_node_read --cov-report term-missing --cov-report html
+```
+
```

### Comparing `rudi-node-read-0.1.2/src/rudi_node_read.egg-info/SOURCES.txt` & `rudi-node-read-0.1.3/src/rudi_node_read.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 src/rudi_node_read/connectors/io_rudi_api.py
 src/rudi_node_read/utils/err.py
 src/rudi_node_read/utils/jwt.py
 src/rudi_node_read/utils/log.py
 src/rudi_node_read/utils/serializable.py
 src/rudi_node_read/utils/type_dict.py
 src/rudi_node_read/utils/type_string.py
-src/rudi_node_read/utils/types.py
+src/rudi_node_read/utils/types.py
+tests/test_rudi_node_reader.py
```

