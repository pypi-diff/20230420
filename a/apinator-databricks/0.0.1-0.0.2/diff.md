# Comparing `tmp/apinator-databricks-0.0.1.tar.gz` & `tmp/apinator-databricks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-databricks-0.0.1.tar", last modified: Wed Apr 19 21:39:19 2023, max compression
+gzip compressed data, was "apinator-databricks-0.0.2.tar", last modified: Thu Apr 20 17:05:10 2023, max compression
```

## Comparing `apinator-databricks-0.0.1.tar` & `apinator-databricks-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      153 2023-04-19 20:49:44.255704 apinator-databricks-0.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-databricks-0.0.1/.gitignore
--rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-databricks-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-databricks-0.0.1/.ruff.toml
--rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-databricks-0.0.1/LICENSE
--rw-r--r--   0        0        0      617 2023-04-19 21:05:45.756749 apinator-databricks-0.0.1/README.md
--rw-r--r--   0        0        0       66 2023-04-19 20:49:27.220310 apinator-databricks-0.0.1/apinator_databricks/__init__.py
--rw-r--r--   0        0        0      871 2023-04-19 21:05:45.761926 apinator-databricks-0.0.1/apinator_databricks/_common/api.py
--rw-r--r--   0        0        0      254 2023-04-19 20:59:10.639252 apinator-databricks-0.0.1/apinator_databricks/_common/model.py
--rw-r--r--   0        0        0      198 2023-04-19 21:05:45.775892 apinator-databricks-0.0.1/apinator_databricks/common.py
--rw-r--r--   0        0        0      153 2023-04-19 21:05:45.767812 apinator-databricks-0.0.1/apinator_databricks/marketplace_provider/__init__.py
--rw-r--r--   0        0        0      651 2023-04-19 21:01:13.109298 apinator-databricks-0.0.1/apinator_databricks/marketplace_provider/api.py
--rw-r--r--   0        0        0     2178 2023-04-19 21:35:17.137497 apinator-databricks-0.0.1/apinator_databricks/marketplace_provider/model.py
--rw-r--r--   0        0        0      139 2023-04-19 21:04:33.333841 apinator-databricks-0.0.1/apinator_databricks/unity_catalog/__init__.py
--rw-r--r--   0        0        0     1972 2023-04-19 21:01:13.117694 apinator-databricks-0.0.1/apinator_databricks/unity_catalog/api.py
--rw-r--r--   0        0        0     1981 2023-04-19 20:59:46.763084 apinator-databricks-0.0.1/apinator_databricks/unity_catalog/model.py
--rw-r--r--   0        0        0      503 2023-04-19 20:48:53.408935 apinator-databricks-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      603 2023-04-19 20:37:53.184612 apinator-databricks-0.0.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-04-18 01:05:39.006517 apinator-databricks-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1575 2023-04-19 21:35:25.369093 apinator-databricks-0.0.1/tests/test_marketplace_provider.py
--rw-r--r--   0        0        0     1452 2023-04-19 21:05:45.781659 apinator-databricks-0.0.1/tests/test_unity_catalog.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 apinator-databricks-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-04-20 17:04:55.251232 apinator-databricks-0.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      584 2023-04-19 20:33:39.872507 apinator-databricks-0.0.2/.github/workflows/dagger.yml
+-rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-databricks-0.0.2/.gitignore
+-rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-databricks-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-databricks-0.0.2/.ruff.toml
+-rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-databricks-0.0.2/LICENSE
+-rw-r--r--   0        0        0      655 2023-04-19 21:42:10.375582 apinator-databricks-0.0.2/README.md
+-rw-r--r--   0        0        0       66 2023-04-20 17:04:55.251232 apinator-databricks-0.0.2/apinator_databricks/__init__.py
+-rw-r--r--   0        0        0      871 2023-04-19 21:05:45.761926 apinator-databricks-0.0.2/apinator_databricks/_common/api.py
+-rw-r--r--   0        0        0      254 2023-04-19 20:59:10.639252 apinator-databricks-0.0.2/apinator_databricks/_common/model.py
+-rw-r--r--   0        0        0      198 2023-04-19 21:05:45.775892 apinator-databricks-0.0.2/apinator_databricks/common.py
+-rw-r--r--   0        0        0      153 2023-04-19 21:05:45.767812 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-19 21:01:13.109298 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/api.py
+-rw-r--r--   0        0        0     2178 2023-04-19 21:35:17.137497 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/model.py
+-rw-r--r--   0        0        0      139 2023-04-19 21:04:33.333841 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     2425 2023-04-20 17:02:14.494712 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/api.py
+-rw-r--r--   0        0        0     3573 2023-04-20 17:00:47.987774 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/model.py
+-rw-r--r--   0        0        0      895 2023-04-19 20:28:33.161296 apinator-databricks-0.0.2/ci/main.py
+-rw-r--r--   0        0        0      503 2023-04-19 20:48:53.408935 apinator-databricks-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-04-20 17:04:55.250719 apinator-databricks-0.0.2/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-18 01:05:39.006517 apinator-databricks-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-19 21:40:03.159348 apinator-databricks-0.0.2/tests/test_marketplace_provider.py
+-rw-r--r--   0        0        0     1452 2023-04-19 21:05:45.781659 apinator-databricks-0.0.2/tests/test_unity_catalog.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.2/PKG-INFO
```

### Comparing `apinator-databricks-0.0.1/.gitignore` & `apinator-databricks-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/.pre-commit-config.yaml` & `apinator-databricks-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/.ruff.toml` & `apinator-databricks-0.0.2/.ruff.toml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/LICENSE` & `apinator-databricks-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/README.md` & `apinator-databricks-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Apinator-Databricks
 
-`apinator` bindings for the [Databricks API](https://docs.databricks.com/api-explorer/).
+[`apinator` bindings](https://pypi.org/project/apinator/) for the [Databricks API](https://docs.databricks.com/api-explorer/).
 
 ## Example
 
 ```python
 from apinator_databricks.common import DatabricksContext
 from apinator_databricks.unity_catalog import DatabricksUnityCatalogApi, uc_model
```

### Comparing `apinator-databricks-0.0.1/apinator_databricks/_common/api.py` & `apinator-databricks-0.0.2/apinator_databricks/_common/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/apinator_databricks/marketplace_provider/api.py` & `apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/apinator_databricks/marketplace_provider/model.py` & `apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/model.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/apinator_databricks/unity_catalog/api.py` & `apinator-databricks-0.0.2/apinator_databricks/unity_catalog/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,26 @@
                 model.Share,
                 default_query={"include_shared_data": "true"},
             ),
             EndpointAction.create(model.Share),
             EndpointAction.update(model.Share),
             EndpointAction.partial_update(model.Share),
             EndpointAction.destroy(),
+            EndpointAction(
+                action_name="get_permissions",
+                method="GET",
+                url="/shares/{id}/permissions",
+                response_model=model.SharePermissions,
+            ),
+            EndpointAction(
+                action_name="update_permissions",
+                method="PATCH",
+                url="/shares/{id}/permissions",
+                body_model=model.SharePermissionChanges,
+            ),
         ],
     )
 
     catalogs = EndpointGroup(
         "/catalogs",
         actions=[
             EndpointAction.list(model.CatalogList),
```

### Comparing `apinator-databricks-0.0.1/setup.cfg` & `apinator-databricks-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 302e 310d 0a6e 616d  ion = 0.0.1..nam
+00000010: 696f 6e20 3d20 302e 302e 320d 0a6e 616d  ion = 0.0.2..nam
 00000020: 6520 3d20 6170 696e 6174 6f72 2d64 6174  e = apinator-dat
 00000030: 6162 7269 636b 730d 0a64 6573 6372 6970  abricks..descrip
 00000040: 7469 6f6e 203d 2041 5049 6e61 746f 7220  tion = APInator 
 00000050: 6269 6e64 696e 6720 746f 2044 6174 6162  binding to Datab
 00000060: 7269 636b 7320 4150 490d 0a61 7574 686f  ricks API..autho
 00000070: 7220 3d20 5265 6172 6320 4461 7461 0d0a  r = Rearc Data..
 00000080: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
```

### Comparing `apinator-databricks-0.0.1/tests/test_marketplace_provider.py` & `apinator-databricks-0.0.2/tests/test_marketplace_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     mp_model,
 )
 
 
 @pytest.fixture
 def databricks_context() -> DatabricksContext:
     return DatabricksContext(
-        access_token=SecretStr("TOKEN"),
+        access_token="TOKEN",
         account="account",
     )
 
 
 @pytest.fixture
 def mp_api(databricks_context) -> DatabricksMarketplaceProviderApi:
     return DatabricksMarketplaceProviderApi(context=databricks_context)
```

### Comparing `apinator-databricks-0.0.1/tests/test_unity_catalog.py` & `apinator-databricks-0.0.2/tests/test_unity_catalog.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.1/PKG-INFO` & `apinator-databricks-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: apinator-databricks
-Version: 0.0.1
+Version: 0.0.2
 Summary: APInator bindings for Databricks API
 Author-email: Rearc Data <data@rearc.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: apinator~=0.0.2
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
 Requires-Dist: responses ; extra == "tests"
 Project-URL: Home, https://github.com/rearc-data/apinator-databricks
 Provides-Extra: tests
 
 # Apinator-Databricks
 
-`apinator` bindings for the [Databricks API](https://docs.databricks.com/api-explorer/).
+[`apinator` bindings](https://pypi.org/project/apinator/) for the [Databricks API](https://docs.databricks.com/api-explorer/).
 
 ## Example
 
 ```python
 from apinator_databricks.common import DatabricksContext
 from apinator_databricks.unity_catalog import DatabricksUnityCatalogApi, uc_model
```

