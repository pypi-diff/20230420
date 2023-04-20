# Comparing `tmp/octo_api_client-1.1.2.tar.gz` & `tmp/octo_api_client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octo_api_client-1.1.2.tar", max compression
+gzip compressed data, was "octo_api_client-1.1.3.tar", max compression
```

## Comparing `octo_api_client-1.1.2.tar` & `octo_api_client-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      690 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/README.md
--rw-r--r--   0        0        0      111 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/__init__.py
--rw-r--r--   0        0        0    19069 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/client.py
--rw-r--r--   0        0        0     2391 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/const.py
--rw-r--r--   0        0        0      426 2023-04-20 11:04:52.867942 octo_api_client-1.1.2/octo_client/exceptions.py
--rw-r--r--   0        0        0    11968 2023-04-20 11:04:52.871942 octo_api_client-1.1.2/octo_client/models.py
--rw-r--r--   0        0        0     1110 2023-04-20 11:04:52.871942 octo_api_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.2/setup.py
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      690 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/README.md
+-rw-r--r--   0        0        0      111 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/__init__.py
+-rw-r--r--   0        0        0    19611 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/client.py
+-rw-r--r--   0        0        0     2391 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/const.py
+-rw-r--r--   0        0        0      426 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/exceptions.py
+-rw-r--r--   0        0        0    11968 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/models.py
+-rw-r--r--   0        0        0     1110 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.3/setup.py
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.3/PKG-INFO
```

### Comparing `octo_api_client-1.1.2/README.md` & `octo_api_client-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.2/octo_client/client.py` & `octo_api_client-1.1.3/octo_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,27 +255,39 @@
     def get_calendar(
         self,
         supplier_id: str,
         product_id: str,
         option_id: str,
         local_date_start: date,
         local_date_end: date,
-        availability_ids: Optional[List[str]] = None,
         units: Optional[List[models.UnitQuantity]] = None,
     ) -> List[models.AvailabilityCalendarItem]:
+        """This method retrieve the availability calendar for a range of dates.
+
+        Args:
+            supplier_id: retrieve calendar data for the supplier with this ID.
+            product_id: retrieve calendar data for a product with this ID.
+            option_id: retrieve calendar data for the option with this ID.
+            local_date_start: retrieve calendar data from this date onwards.
+            local_date_end: retrieve calendar data until this date.
+            units: a list of units. Each unit requires:
+                - id
+                - quantity
+
+        Returns: a list of availability objects; one object per each day in the range of dates.
+        """
+
         payload: Dict[str, Any] = {
             "productId": product_id,
             "optionId": option_id,
         }
         if local_date_start:
             payload["localDateStart"] = local_date_start.isoformat()
         if local_date_end:
             payload["localDateEnd"] = local_date_end.isoformat()
-        if availability_ids:
-            payload["availabilityIds"] = availability_ids
         if units:
             payload["units"] = [unit.as_dict() for unit in units]
 
         response = self._http_post("availability/calendar", supplier_id=supplier_id, json=payload)
         daily_availability = [
             models.AvailabilityCalendarItem.from_dict(availability, strict=self.strict)
             for availability in response
```

### Comparing `octo_api_client-1.1.2/octo_client/const.py` & `octo_api_client-1.1.3/octo_client/const.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.2/octo_client/models.py` & `octo_api_client-1.1.3/octo_client/models.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.2/pyproject.toml` & `octo_api_client-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octo-api-client"
-version = "1.1.2"
+version = "1.1.3"
 description = "HTTP client for OCTo (Open Connection for Tourism) APIs."
 authors = ["Tiqets <connections@tiqets.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "octo_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `octo_api_client-1.1.2/setup.py` & `octo_api_client-1.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.20.0,<3', 'tonalite>=1.7.1,<2']
 
 setup_kwargs = {
     'name': 'octo-api-client',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'HTTP client for OCTo (Open Connection for Tourism) APIs.',
     'long_description': "# OCTO API client\n\nPython HTTP client for OCTO (Open Connection for Tourism) APIs.\n\nMore info at [octospec.com](https://octospec.com/)\n\nAPI Specification: https://docs.octo.travel/docs/octo/r6gduoa5ah5ne-octo-api\n\n## Installation\n\n    pip install octo-api-client\n\n## Requirements\n\n* Python v3.7+\n\n## Development\n\n### Getting started\n\n    $ pip install poetry\n    $ poetry install\n\n### Running tests and linters\n\nTo run linters:\n\n    $ poetry run ruff octo_client\n    $ poetry run mypy octo_client\n\nTo run tests:\n\n    $ poetry run pytest\n\n\n## Usage\n\n```\nfrom octo_client import OctoClient\n\nclient = OctoClient('https://octo-api.mysupplier.com', 'MY-SECRET_TOKEN')\nclient.get_suppliers()\n```\n",
     'author': 'Tiqets',
     'author_email': 'connections@tiqets.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `octo_api_client-1.1.2/PKG-INFO` & `octo_api_client-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octo-api-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: HTTP client for OCTo (Open Connection for Tourism) APIs.
 License: MIT
 Author: Tiqets
 Author-email: connections@tiqets.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

