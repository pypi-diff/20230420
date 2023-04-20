# Comparing `tmp/quakesaver_client-1.1.0.tar.gz` & `tmp/quakesaver_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quakesaver_client-1.1.0.tar", max compression
+gzip compressed data, was "quakesaver_client-1.1.1.tar", max compression
```

## Comparing `quakesaver_client-1.1.0.tar` & `quakesaver_client-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1497 2023-03-10 12:48:43.868669 quakesaver_client-1.1.0/LICENSE
--rw-r--r--   0        0        0     4233 2023-03-10 12:48:43.868669 quakesaver_client-1.1.0/README.md
--rw-r--r--   0        0        0     2291 2023-03-10 12:49:28.642262 quakesaver_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3966 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/__init__.py
--rw-r--r--   0        0        0      624 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/errors.py
--rw-r--r--   0        0        0       56 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/data_product_query.py
--rw-r--r--   0        0        0     4078 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/data_products.py
--rw-r--r--   0        0        0     2377 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/measurement.py
--rw-r--r--   0        0        0      365 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/permission.py
--rw-r--r--   0        0        0     9762 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/sensor.py
--rw-r--r--   0        0        0    69437 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/sensor_state.py
--rw-r--r--   0        0        0      205 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/token.py
--rw-r--r--   0        0        0      743 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/models/warnings.py
--rw-r--r--   0        0        0      387 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/types.py
--rw-r--r--   0        0        0     1718 2023-03-10 12:48:43.872669 quakesaver_client-1.1.0/quakesaver_client/util.py
--rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 quakesaver_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-20 10:23:55.210679 quakesaver_client-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4233 2023-04-20 10:23:55.210679 quakesaver_client-1.1.1/README.md
+-rw-r--r--   0        0        0     2291 2023-04-20 10:24:59.847141 quakesaver_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3869 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/errors.py
+-rw-r--r--   0        0        0       56 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/data_product_query.py
+-rw-r--r--   0        0        0     4078 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/data_products.py
+-rw-r--r--   0        0        0     2377 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/measurement.py
+-rw-r--r--   0        0        0      365 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/permission.py
+-rw-r--r--   0        0        0     9762 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/sensor.py
+-rw-r--r--   0        0        0    69437 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/sensor_state.py
+-rw-r--r--   0        0        0      205 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/token.py
+-rw-r--r--   0        0        0      743 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/warnings.py
+-rw-r--r--   0        0        0      387 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/types.py
+-rw-r--r--   0        0        0     1718 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/util.py
+-rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 quakesaver_client-1.1.1/PKG-INFO
```

### Comparing `quakesaver_client-1.1.0/LICENSE` & `quakesaver_client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/README.md` & `quakesaver_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/pyproject.toml` & `quakesaver_client-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quakesaver-client"
-version = "1.1.0"
+version = "1.1.1"
 description = "Client library for interacting with the QuakeSaver sensor fleet."
 authors = ["QuakeSaver <info@quakesaver.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "quakesaver_client"}]
 homepage = "https://quakesaver.net/"
 repository = "https://github.com/QuakeSaver/quakesaver-client"
```

### Comparing `quakesaver_client-1.1.0/quakesaver_client/__init__.py` & `quakesaver_client-1.1.1/quakesaver_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,38 @@
 from quakesaver_client.models.sensor import Sensor
 from quakesaver_client.models.token import Token
 from quakesaver_client.util import handle_response
 
 DecoratedFunction = TypeVar("DecoratedFunction", bound=Callable[..., Any])
 
 
+def _needs_token(function: DecoratedFunction) -> DecoratedFunction:
+    @wraps(function)
+    def request_token_if_needed(
+        self: QSClient, *args: list, **kwargs: dict
+    ) -> DecoratedFunction:
+        if not self._token:
+            logging.debug("QSClient requesting user _token.")
+            response = requests.post(
+                url=f"{self._api_base_url}/user/get_token",
+                data=f"username={self._email}&password={self._password}",
+                headers={"Content-Type": "application/x-www-form-urlencoded"},
+            )
+            response_data = handle_response(response)
+            try:
+                token = Token(**response_data)
+            except ValidationError as e:
+                raise CorruptedDataError() from e
+            self._token = token
+
+        return function(self, *args, **kwargs)
+
+    return request_token_if_needed
+
+
 class QSClient:
     """A class representing a client to the backend."""
 
     _base_domain: str
 
     _email: str
     _password: str
@@ -48,38 +72,14 @@
         self._token = None
 
         self._base_domain = base_domain
 
         self._api_base_url = f"https://api.{base_domain}/api/v1"
         self._fdsn_base_url = f"https://fdsnws.{base_domain}/fdsnws"
 
-    @staticmethod
-    def _needs_token(function: DecoratedFunction) -> DecoratedFunction:
-        @wraps(function)
-        def request_token_if_needed(
-            self: QSClient, *args: list, **kwargs: dict
-        ) -> DecoratedFunction:
-            if not self._token:
-                logging.debug("QSClient requesting user _token.")
-                response = requests.post(
-                    url=f"{self._api_base_url}/user/get_token",
-                    data=f"username={self._email}&password={self._password}",
-                    headers={"Content-Type": "application/x-www-form-urlencoded"},
-                )
-                response_data = handle_response(response)
-                try:
-                    token = Token(**response_data)
-                except ValidationError as e:
-                    raise CorruptedDataError() from e
-                self._token = token
-
-            return function(self, *args, **kwargs)
-
-        return request_token_if_needed
-
     @_needs_token
     def _get_authorization_headers(self: QSClient) -> dict:
         return {"Authorization": f"{self._token.token_type} {self._token.access_token}"}
 
     def get_sensor_ids(self: QSClient) -> list[str]:
         """Fetch all sensor UIDs the user has access to.
```

### Comparing `quakesaver_client-1.1.0/quakesaver_client/errors.py` & `quakesaver_client-1.1.1/quakesaver_client/errors.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/data_product_query.py` & `quakesaver_client-1.1.1/quakesaver_client/models/data_product_query.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/data_products.py` & `quakesaver_client-1.1.1/quakesaver_client/models/data_products.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/measurement.py` & `quakesaver_client-1.1.1/quakesaver_client/models/measurement.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/sensor.py` & `quakesaver_client-1.1.1/quakesaver_client/models/sensor.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/sensor_state.py` & `quakesaver_client-1.1.1/quakesaver_client/models/sensor_state.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/models/warnings.py` & `quakesaver_client-1.1.1/quakesaver_client/models/warnings.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/quakesaver_client/util.py` & `quakesaver_client-1.1.1/quakesaver_client/util.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.0/PKG-INFO` & `quakesaver_client-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quakesaver-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Client library for interacting with the QuakeSaver sensor fleet.
 Home-page: https://quakesaver.net/
 License: BSD-3-Clause
 Author: QuakeSaver
 Author-email: info@quakesaver.net
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quakesaver-client Version: 1.1.0 Summary: Client
+Metadata-Version: 2.1 Name: quakesaver-client Version: 1.1.1 Summary: Client
 library for interacting with the QuakeSaver sensor fleet. Home-page: https://
 quakesaver.net/ License: BSD-3-Clause Author: QuakeSaver Author-email:
 info@quakesaver.net Requires-Python: >=3.9,<3.12 Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.5,<1.11.0) Requires-Dist: requests
```

