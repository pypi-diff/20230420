# Comparing `tmp/apinator-databricks-0.0.2.tar.gz` & `tmp/apinator-databricks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-databricks-0.0.2.tar", last modified: Thu Apr 20 17:05:10 2023, max compression
+gzip compressed data, was "apinator-databricks-0.0.3.tar", last modified: Thu Apr 20 17:15:47 2023, max compression
```

## Comparing `apinator-databricks-0.0.2.tar` & `apinator-databricks-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      153 2023-04-20 17:04:55.251232 apinator-databricks-0.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0      584 2023-04-19 20:33:39.872507 apinator-databricks-0.0.2/.github/workflows/dagger.yml
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-databricks-0.0.2/.gitignore
--rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-databricks-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-databricks-0.0.2/.ruff.toml
--rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-databricks-0.0.2/LICENSE
--rw-r--r--   0        0        0      655 2023-04-19 21:42:10.375582 apinator-databricks-0.0.2/README.md
--rw-r--r--   0        0        0       66 2023-04-20 17:04:55.251232 apinator-databricks-0.0.2/apinator_databricks/__init__.py
--rw-r--r--   0        0        0      871 2023-04-19 21:05:45.761926 apinator-databricks-0.0.2/apinator_databricks/_common/api.py
--rw-r--r--   0        0        0      254 2023-04-19 20:59:10.639252 apinator-databricks-0.0.2/apinator_databricks/_common/model.py
--rw-r--r--   0        0        0      198 2023-04-19 21:05:45.775892 apinator-databricks-0.0.2/apinator_databricks/common.py
--rw-r--r--   0        0        0      153 2023-04-19 21:05:45.767812 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/__init__.py
--rw-r--r--   0        0        0      651 2023-04-19 21:01:13.109298 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/api.py
--rw-r--r--   0        0        0     2178 2023-04-19 21:35:17.137497 apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/model.py
--rw-r--r--   0        0        0      139 2023-04-19 21:04:33.333841 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/__init__.py
--rw-r--r--   0        0        0     2425 2023-04-20 17:02:14.494712 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/api.py
--rw-r--r--   0        0        0     3573 2023-04-20 17:00:47.987774 apinator-databricks-0.0.2/apinator_databricks/unity_catalog/model.py
--rw-r--r--   0        0        0      895 2023-04-19 20:28:33.161296 apinator-databricks-0.0.2/ci/main.py
--rw-r--r--   0        0        0      503 2023-04-19 20:48:53.408935 apinator-databricks-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      603 2023-04-20 17:04:55.250719 apinator-databricks-0.0.2/setup.cfg
--rw-r--r--   0        0        0        0 2023-04-18 01:05:39.006517 apinator-databricks-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1564 2023-04-19 21:40:03.159348 apinator-databricks-0.0.2/tests/test_marketplace_provider.py
--rw-r--r--   0        0        0     1452 2023-04-19 21:05:45.781659 apinator-databricks-0.0.2/tests/test_unity_catalog.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-04-20 17:15:40.442784 apinator-databricks-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      584 2023-04-19 20:33:39.872507 apinator-databricks-0.0.3/.github/workflows/dagger.yml
+-rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-databricks-0.0.3/.gitignore
+-rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-databricks-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-databricks-0.0.3/.ruff.toml
+-rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-databricks-0.0.3/LICENSE
+-rw-r--r--   0        0        0      655 2023-04-19 21:42:10.375582 apinator-databricks-0.0.3/README.md
+-rw-r--r--   0        0        0       66 2023-04-20 17:15:40.442267 apinator-databricks-0.0.3/apinator_databricks/__init__.py
+-rw-r--r--   0        0        0      871 2023-04-19 21:05:45.761926 apinator-databricks-0.0.3/apinator_databricks/_common/api.py
+-rw-r--r--   0        0        0      254 2023-04-19 20:59:10.639252 apinator-databricks-0.0.3/apinator_databricks/_common/model.py
+-rw-r--r--   0        0        0      198 2023-04-19 21:05:45.775892 apinator-databricks-0.0.3/apinator_databricks/common.py
+-rw-r--r--   0        0        0      153 2023-04-19 21:05:45.767812 apinator-databricks-0.0.3/apinator_databricks/marketplace_provider/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-19 21:01:13.109298 apinator-databricks-0.0.3/apinator_databricks/marketplace_provider/api.py
+-rw-r--r--   0        0        0     2178 2023-04-19 21:35:17.137497 apinator-databricks-0.0.3/apinator_databricks/marketplace_provider/model.py
+-rw-r--r--   0        0        0      139 2023-04-19 21:04:33.333841 apinator-databricks-0.0.3/apinator_databricks/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     2493 2023-04-20 17:06:31.009159 apinator-databricks-0.0.3/apinator_databricks/unity_catalog/api.py
+-rw-r--r--   0        0        0     3573 2023-04-20 17:00:47.987774 apinator-databricks-0.0.3/apinator_databricks/unity_catalog/model.py
+-rw-r--r--   0        0        0      895 2023-04-19 20:28:33.161296 apinator-databricks-0.0.3/ci/main.py
+-rw-r--r--   0        0        0      503 2023-04-19 20:48:53.408935 apinator-databricks-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-04-20 17:15:40.441733 apinator-databricks-0.0.3/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-18 01:05:39.006517 apinator-databricks-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-19 21:40:03.159348 apinator-databricks-0.0.3/tests/test_marketplace_provider.py
+-rw-r--r--   0        0        0     1452 2023-04-19 21:05:45.781659 apinator-databricks-0.0.3/tests/test_unity_catalog.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.3/PKG-INFO
```

### Comparing `apinator-databricks-0.0.2/.github/workflows/dagger.yml` & `apinator-databricks-0.0.3/.github/workflows/dagger.yml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/.gitignore` & `apinator-databricks-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/.pre-commit-config.yaml` & `apinator-databricks-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/.ruff.toml` & `apinator-databricks-0.0.3/.ruff.toml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/LICENSE` & `apinator-databricks-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/README.md` & `apinator-databricks-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/apinator_databricks/_common/api.py` & `apinator-databricks-0.0.3/apinator_databricks/_common/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/api.py` & `apinator-databricks-0.0.3/apinator_databricks/marketplace_provider/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/apinator_databricks/marketplace_provider/model.py` & `apinator-databricks-0.0.3/apinator_databricks/marketplace_provider/model.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/apinator_databricks/unity_catalog/api.py` & `apinator-databricks-0.0.3/apinator_databricks/unity_catalog/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,22 @@
             EndpointAction.partial_update(model.Share),
             EndpointAction.destroy(),
             EndpointAction(
                 action_name="get_permissions",
                 method="GET",
                 url="/shares/{id}/permissions",
                 response_model=model.SharePermissions,
+                arg_names=["id"],
             ),
             EndpointAction(
                 action_name="update_permissions",
                 method="PATCH",
                 url="/shares/{id}/permissions",
                 body_model=model.SharePermissionChanges,
+                arg_names=["id"],
             ),
         ],
     )
 
     catalogs = EndpointGroup(
         "/catalogs",
         actions=[
```

### Comparing `apinator-databricks-0.0.2/apinator_databricks/unity_catalog/model.py` & `apinator-databricks-0.0.3/apinator_databricks/unity_catalog/model.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/ci/main.py` & `apinator-databricks-0.0.3/ci/main.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/setup.cfg` & `apinator-databricks-0.0.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 302e 320d 0a6e 616d  ion = 0.0.2..nam
+00000010: 696f 6e20 3d20 302e 302e 330d 0a6e 616d  ion = 0.0.3..nam
 00000020: 6520 3d20 6170 696e 6174 6f72 2d64 6174  e = apinator-dat
 00000030: 6162 7269 636b 730d 0a64 6573 6372 6970  abricks..descrip
 00000040: 7469 6f6e 203d 2041 5049 6e61 746f 7220  tion = APInator 
 00000050: 6269 6e64 696e 6720 746f 2044 6174 6162  binding to Datab
 00000060: 7269 636b 7320 4150 490d 0a61 7574 686f  ricks API..autho
 00000070: 7220 3d20 5265 6172 6320 4461 7461 0d0a  r = Rearc Data..
 00000080: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
```

### Comparing `apinator-databricks-0.0.2/tests/test_marketplace_provider.py` & `apinator-databricks-0.0.3/tests/test_marketplace_provider.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/tests/test_unity_catalog.py` & `apinator-databricks-0.0.3/tests/test_unity_catalog.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.2/PKG-INFO` & `apinator-databricks-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apinator-databricks
-Version: 0.0.2
+Version: 0.0.3
 Summary: APInator bindings for Databricks API
 Author-email: Rearc Data <data@rearc.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: apinator~=0.0.2
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
```

