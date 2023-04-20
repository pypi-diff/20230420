# Comparing `tmp/octo_api_client-1.1.1.tar.gz` & `tmp/octo_api_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octo_api_client-1.1.1.tar", max compression
+gzip compressed data, was "octo_api_client-1.1.2.tar", max compression
```

## Comparing `octo_api_client-1.1.1.tar` & `octo_api_client-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      690 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/README.md
--rw-r--r--   0        0        0      111 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/octo_client/__init__.py
--rw-r--r--   0        0        0    18415 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/octo_client/client.py
--rw-r--r--   0        0        0     2391 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/octo_client/const.py
--rw-r--r--   0        0        0      426 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/octo_client/exceptions.py
--rw-r--r--   0        0        0    11968 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/octo_client/models.py
--rw-r--r--   0        0        0     1110 2023-04-04 09:25:16.852656 octo_api_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.1/setup.py
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      690 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/README.md
+-rw-r--r--   0        0        0      111 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/__init__.py
+-rw-r--r--   0        0        0    19069 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/client.py
+-rw-r--r--   0        0        0     2391 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/const.py
+-rw-r--r--   0        0        0      426 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/exceptions.py
+-rw-r--r--   0        0        0    11968 2023-04-20 11:04:52.871942 octo_api_client-1.1.2/octo_client/models.py
+-rw-r--r--   0        0        0     1110 2023-04-20 11:04:52.871942 octo_api_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.2/setup.py
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.2/PKG-INFO
```

### Comparing `octo_api_client-1.1.1/README.md` & `octo_api_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.1/octo_client/client.py` & `octo_api_client-1.1.2/octo_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,35 +55,60 @@
             403: exceptions.Unauthorized,
             404: exceptions.ApiError,
             500: exceptions.ApiError,
         }
         if status_code in CODE_EXCEPTION_MAP:
             raise CODE_EXCEPTION_MAP[status_code](response_text)
 
+    def _build_endpoint_url_for_request(self, supplier_id: str, path: str) -> str:
+        """Builds the endpoint's URL for making requests to a given supplier.
+
+        Args:
+            supplier_id: builds the URL for a supplier with this ID.
+            path: use this path to build the URL.
+
+        Returns: the full URL.
+        Raises:
+            - `exceptions.InvalidRequest` if the supplier ID is unknown.
+
+        """
+
+        if supplier_id not in self.supplier_url_map:
+            self.get_suppliers()
+
+        try:
+            endpoint_url = self.supplier_url_map[supplier_id]
+        except KeyError as e:
+            raise exceptions.InvalidRequest("Incorrect supplierId") from e
+
+        cleaned_endpoint = endpoint_url.rstrip("/")
+
+        return (
+            cleaned_endpoint
+            if cleaned_endpoint.endswith(path)
+            else f"{cleaned_endpoint}/{path}"
+        )
+
     def _make_request(
         self,
         http_method: Callable,
         path: str,
         supplier_id=None,
         json=None,
         params=None,
         headers=None,
     ):
         if headers is None:
             headers = {}
+
         if supplier_id:
-            if supplier_id not in self.supplier_url_map:
-                self.get_suppliers()
-            try:
-                endpoint_url = self.supplier_url_map[supplier_id]
-            except KeyError as e:
-                raise exceptions.InvalidRequest("Incorrect supplierId") from e
-            full_url = f"{endpoint_url}/{path}"
+            full_url: str = self._build_endpoint_url_for_request(str(supplier_id), path)
         else:
             full_url = f"{self.url}/{path}"
+
         self.logger.log(
             self.requests_loglevel,
             "Sending request to %s (%s)",
             full_url,
             http_method.__name__.upper(),
         )
         base_headers = self._get_headers()
```

### Comparing `octo_api_client-1.1.1/octo_client/const.py` & `octo_api_client-1.1.2/octo_client/const.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.1/octo_client/models.py` & `octo_api_client-1.1.2/octo_client/models.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.1/pyproject.toml` & `octo_api_client-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octo-api-client"
-version = "1.1.1"
+version = "1.1.2"
 description = "HTTP client for OCTo (Open Connection for Tourism) APIs."
 authors = ["Tiqets <connections@tiqets.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "octo_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `octo_api_client-1.1.1/setup.py` & `octo_api_client-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.20.0,<3', 'tonalite>=1.7.1,<2']
 
 setup_kwargs = {
     'name': 'octo-api-client',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'HTTP client for OCTo (Open Connection for Tourism) APIs.',
     'long_description': "# OCTO API client\n\nPython HTTP client for OCTO (Open Connection for Tourism) APIs.\n\nMore info at [octospec.com](https://octospec.com/)\n\nAPI Specification: https://docs.octo.travel/docs/octo/r6gduoa5ah5ne-octo-api\n\n## Installation\n\n    pip install octo-api-client\n\n## Requirements\n\n* Python v3.7+\n\n## Development\n\n### Getting started\n\n    $ pip install poetry\n    $ poetry install\n\n### Running tests and linters\n\nTo run linters:\n\n    $ poetry run ruff octo_client\n    $ poetry run mypy octo_client\n\nTo run tests:\n\n    $ poetry run pytest\n\n\n## Usage\n\n```\nfrom octo_client import OctoClient\n\nclient = OctoClient('https://octo-api.mysupplier.com', 'MY-SECRET_TOKEN')\nclient.get_suppliers()\n```\n",
     'author': 'Tiqets',
     'author_email': 'connections@tiqets.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `octo_api_client-1.1.1/PKG-INFO` & `octo_api_client-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octo-api-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: HTTP client for OCTo (Open Connection for Tourism) APIs.
 License: MIT
 Author: Tiqets
 Author-email: connections@tiqets.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

