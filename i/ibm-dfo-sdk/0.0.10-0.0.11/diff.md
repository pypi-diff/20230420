# Comparing `tmp/ibm-dfo-sdk-0.0.10.tar.gz` & `tmp/ibm-dfo-sdk-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-dfo-sdk-0.0.10.tar", last modified: Wed Apr  5 06:19:07 2023, max compression
+gzip compressed data, was "ibm-dfo-sdk-0.0.11.tar", last modified: Thu Apr 20 07:54:24 2023, max compression
```

## Comparing `ibm-dfo-sdk-0.0.10.tar` & `ibm-dfo-sdk-0.0.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-05 06:19:07.864855 ibm-dfo-sdk-0.0.10/
--rw-r--r--   0 pugang     (501) staff       (20)    11357 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/LICENSE
--rw-r--r--   0 pugang     (501) staff       (20)       70 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/MANIFEST.in
--rw-r--r--   0 pugang     (501) staff       (20)     4339 2023-04-05 06:19:07.864698 ibm-dfo-sdk-0.0.10/PKG-INFO
--rw-r--r--   0 pugang     (501) staff       (20)     3387 2023-04-05 06:17:45.000000 ibm-dfo-sdk-0.0.10/README.md
-drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-05 06:19:07.863219 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/
--rw-r--r--   0 pugang     (501) staff       (20)     1078 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/__init__.py
--rw-r--r--   0 pugang     (501) staff       (20)     2300 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/common.py
--rw-r--r--   0 pugang     (501) staff       (20)    25153 2023-03-24 09:33:28.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/extended_api.py
--rw-r--r--   0 pugang     (501) staff       (20)    23449 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/get_service.py
--rw-r--r--   0 pugang     (501) staff       (20)    65012 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1.py
--rw-r--r--   0 pugang     (501) staff       (20)    24612 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1_dummy.py
--rw-r--r--   0 pugang     (501) staff       (20)      502 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/token_auth_handler.py
--rw-r--r--   0 pugang     (501) staff       (20)      657 2023-03-22 09:49:12.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/version.py
-drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-05 06:19:07.864300 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/
--rw-r--r--   0 pugang     (501) staff       (20)     4339 2023-04-05 06:19:07.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pugang     (501) staff       (20)      553 2023-04-05 06:19:07.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pugang     (501) staff       (20)        1 2023-04-05 06:19:07.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pugang     (501) staff       (20)      126 2023-04-05 06:19:07.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/requires.txt
--rw-r--r--   0 pugang     (501) staff       (20)       12 2023-04-05 06:19:07.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/top_level.txt
--rw-r--r--   0 pugang     (501) staff       (20)        1 2023-03-13 04:20:49.000000 ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/zip-safe
--rw-r--r--   0 pugang     (501) staff       (20)       64 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/pyproject.toml
--rw-r--r--   0 pugang     (501) staff       (20)      167 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.10/requirements-dev.txt
--rw-r--r--   0 pugang     (501) staff       (20)      126 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.10/requirements.txt
--rw-r--r--   0 pugang     (501) staff       (20)       38 2023-04-05 06:19:07.864906 ibm-dfo-sdk-0.0.10/setup.cfg
--rw-r--r--   0 pugang     (501) staff       (20)     2612 2023-04-05 03:43:18.000000 ibm-dfo-sdk-0.0.10/setup.py
+drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-20 07:54:24.554781 ibm-dfo-sdk-0.0.11/
+-rw-r--r--   0 pugang     (501) staff       (20)    11357 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/LICENSE
+-rw-r--r--   0 pugang     (501) staff       (20)       70 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/MANIFEST.in
+-rw-r--r--   0 pugang     (501) staff       (20)     4339 2023-04-20 07:54:24.554624 ibm-dfo-sdk-0.0.11/PKG-INFO
+-rw-r--r--   0 pugang     (501) staff       (20)     3387 2023-04-05 06:17:45.000000 ibm-dfo-sdk-0.0.11/README.md
+drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-20 07:54:24.553182 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/
+-rw-r--r--   0 pugang     (501) staff       (20)     1078 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/__init__.py
+-rw-r--r--   0 pugang     (501) staff       (20)     2300 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/common.py
+-rw-r--r--   0 pugang     (501) staff       (20)    25153 2023-03-24 09:33:28.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/extended_api.py
+-rw-r--r--   0 pugang     (501) staff       (20)    23449 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/get_service.py
+-rw-r--r--   0 pugang     (501) staff       (20)    66109 2023-04-18 05:54:21.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1.py
+-rw-r--r--   0 pugang     (501) staff       (20)    24612 2023-03-22 09:39:50.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1_dummy.py
+-rw-r--r--   0 pugang     (501) staff       (20)      502 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/token_auth_handler.py
+-rw-r--r--   0 pugang     (501) staff       (20)      657 2023-04-20 07:51:25.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/version.py
+drwxr-xr-x   0 pugang     (501) staff       (20)        0 2023-04-20 07:54:24.554354 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/
+-rw-r--r--   0 pugang     (501) staff       (20)     4339 2023-04-20 07:54:24.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pugang     (501) staff       (20)      553 2023-04-20 07:54:24.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pugang     (501) staff       (20)        1 2023-04-20 07:54:24.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pugang     (501) staff       (20)      126 2023-04-20 07:54:24.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/requires.txt
+-rw-r--r--   0 pugang     (501) staff       (20)       12 2023-04-20 07:54:24.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pugang     (501) staff       (20)        1 2023-03-13 04:20:49.000000 ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/zip-safe
+-rw-r--r--   0 pugang     (501) staff       (20)       64 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/pyproject.toml
+-rw-r--r--   0 pugang     (501) staff       (20)      167 2023-03-02 06:48:39.000000 ibm-dfo-sdk-0.0.11/requirements-dev.txt
+-rw-r--r--   0 pugang     (501) staff       (20)      126 2023-04-18 05:54:21.000000 ibm-dfo-sdk-0.0.11/requirements.txt
+-rw-r--r--   0 pugang     (501) staff       (20)       38 2023-04-20 07:54:24.554828 ibm-dfo-sdk-0.0.11/setup.cfg
+-rw-r--r--   0 pugang     (501) staff       (20)     2612 2023-04-20 07:51:55.000000 ibm-dfo-sdk-0.0.11/setup.py
```

### Comparing `ibm-dfo-sdk-0.0.10/LICENSE` & `ibm-dfo-sdk-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/PKG-INFO` & `ibm-dfo-sdk-0.0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-dfo-sdk
-Version: 0.0.10
+Version: 0.0.11
 Summary: IBM Data Fabric Orchestrator python SDK
 Home-page: https://github.com/IBM/dfo-python-sdk.git
 Author: IBM
 Author-email: pugangxa@cn.ibm.com
 License: Apache 2.0
 Keywords: ibm_dfo_sdk
 Classifier: Programming Language :: Python
```

### Comparing `ibm-dfo-sdk-0.0.10/README.md` & `ibm-dfo-sdk-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/__init__.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/common.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/common.py`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/extended_api.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/extended_api.py`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/get_service.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/get_service.py`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# IBM OpenAPI SDK Code Generator Version: 3.62.0-a2a22f95-20221115-162524
+# IBM OpenAPI SDK Code Generator Version: 3.68.2-ac7def68-20230310-195410
 
 """
 IBM Data Fabric Orchestrator control plane API.
 
 API Version: 1.0.0
 See: https://fybrik.io
 """
@@ -109,15 +109,15 @@
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='list_instance')
         headers.update(sdk_headers)
 
         params = {
             'context_type': context_type,
-            'context_id': context_id
+            'context_id': context_id,
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
@@ -158,15 +158,15 @@
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='create_instance')
         headers.update(sdk_headers)
 
         data = {
             'context_type': context_type,
-            'context_id': context_id
+            'context_id': context_id,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
@@ -298,15 +298,15 @@
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='list_application')
         headers.update(sdk_headers)
 
         params = {
             'intent': intent,
-            'location': location
+            'location': location,
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
@@ -354,15 +354,15 @@
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='create_application')
         headers.update(sdk_headers)
 
         data = {
             'intent': intent,
-            'location': location
+            'location': location,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
@@ -601,15 +601,15 @@
         headers = {}
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='add_assets')
         headers.update(sdk_headers)
 
         data = {
-            'assets': assets
+            'assets': assets,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
@@ -861,15 +861,15 @@
         headers = {}
         sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
                                       service_version='V1',
                                       operation_id='update_wkc_asset')
         headers.update(sdk_headers)
 
         data = {
-            'profile_status': profile_status
+            'profile_status': profile_status,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
@@ -970,15 +970,15 @@
                                       operation_id='create_wkc_asset')
         headers.update(sdk_headers)
 
         data = {
             'connection_id': connection_id,
             'connection_path': connection_path,
             'description': description,
-            'name': name
+            'name': name,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
@@ -1101,49 +1101,55 @@
 
     :attr str asset_id: (optional) Identifier of the data asset.
     :attr str state: (optional) Status of the data asset in the data fabric
           orchestrator application.
     :attr str message: (optional) Reason for the error/failed state of the data
           asset in the data fabric orchestrator application.
     :attr str endpoint: (optional) Endpoint of the data asset.
+    :attr str access_type: (optional) Access Type of the data asset.
     """
 
     def __init__(self,
                  *,
                  asset_id: str = None,
                  state: str = None,
                  message: str = None,
-                 endpoint: str = None) -> None:
+                 endpoint: str = None,
+                 access_type: str = None) -> None:
         """
         Initialize a AssetResource object.
 
         :param str asset_id: (optional) Identifier of the data asset.
         :param str state: (optional) Status of the data asset in the data fabric
                orchestrator application.
         :param str message: (optional) Reason for the error/failed state of the
                data asset in the data fabric orchestrator application.
         :param str endpoint: (optional) Endpoint of the data asset.
+        :param str access_type: (optional) Access Type of the data asset.
         """
         self.asset_id = asset_id
         self.state = state
         self.message = message
         self.endpoint = endpoint
+        self.access_type = access_type
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'AssetResource':
         """Initialize a AssetResource object from a json dictionary."""
         args = {}
         if 'asset_id' in _dict:
             args['asset_id'] = _dict.get('asset_id')
         if 'state' in _dict:
             args['state'] = _dict.get('state')
         if 'message' in _dict:
             args['message'] = _dict.get('message')
         if 'endpoint' in _dict:
             args['endpoint'] = _dict.get('endpoint')
+        if 'access_type' in _dict:
+            args['access_type'] = _dict.get('access_type')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a AssetResource object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1154,14 +1160,16 @@
             _dict['asset_id'] = self.asset_id
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
         if hasattr(self, 'message') and self.message is not None:
             _dict['message'] = self.message
         if hasattr(self, 'endpoint') and self.endpoint is not None:
             _dict['endpoint'] = self.endpoint
+        if hasattr(self, 'access_type') and self.access_type is not None:
+            _dict['access_type'] = self.access_type
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
@@ -1243,44 +1251,50 @@
     """
     Data access information of a data asset to add to the data fabric orchestrator
     application.  Encapsulates information required to access a data asset.
 
     :attr str asset_id: Identifier of the data asset.
     :attr str protocol: (optional) Protocol used to access the data asset.
     :attr str format: (optional) Format of the data asset.
+    :attr str access_type: (optional) Access type of the data asset.
     """
 
     def __init__(self,
                  asset_id: str,
                  *,
                  protocol: str = None,
-                 format: str = None) -> None:
+                 format: str = None,
+                 access_type: str = None) -> None:
         """
         Initialize a DataAsset object.
 
         :param str asset_id: Identifier of the data asset.
         :param str protocol: (optional) Protocol used to access the data asset.
         :param str format: (optional) Format of the data asset.
+        :param str access_type: (optional) Access type of the data asset.
         """
         self.asset_id = asset_id
         self.protocol = protocol
         self.format = format
+        self.access_type = access_type
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'DataAsset':
         """Initialize a DataAsset object from a json dictionary."""
         args = {}
         if 'asset_id' in _dict:
             args['asset_id'] = _dict.get('asset_id')
         else:
             raise ValueError('Required property \'asset_id\' not present in DataAsset JSON')
         if 'protocol' in _dict:
             args['protocol'] = _dict.get('protocol')
         if 'format' in _dict:
             args['format'] = _dict.get('format')
+        if 'access_type' in _dict:
+            args['access_type'] = _dict.get('access_type')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a DataAsset object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1289,14 +1303,16 @@
         _dict = {}
         if hasattr(self, 'asset_id') and self.asset_id is not None:
             _dict['asset_id'] = self.asset_id
         if hasattr(self, 'protocol') and self.protocol is not None:
             _dict['protocol'] = self.protocol
         if hasattr(self, 'format') and self.format is not None:
             _dict['format'] = self.format
+        if hasattr(self, 'access_type') and self.access_type is not None:
+            _dict['access_type'] = self.access_type
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
@@ -1323,14 +1339,23 @@
     class FormatEnum(str, Enum):
         """
         Format of the data asset.
         """
         ARROW = 'arrow'
 
 
+    class AccessTypeEnum(str, Enum):
+        """
+        Access type of the data asset.
+        """
+        READ_ONLY = 'read-only'
+        WRITE_ONLY = 'write-only'
+        READ_WRITE = 'read-write'
+
+
 class InstanceResource():
     """
     Information about the data fabric orchestrator instance.
 
     :attr str instance_id: (optional) Identifier of the data fabric orchestrator
           instance.
     :attr str context_type: Type of the context to associate this data fabric
```

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1_dummy.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/ibm_data_fabric_orchestrator_v1_dummy.py`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk/version.py` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_dfo_sdk
 """
-__version__ = '0.0.10'
+__version__ = '0.0.11'
```

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/PKG-INFO` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-dfo-sdk
-Version: 0.0.10
+Version: 0.0.11
 Summary: IBM Data Fabric Orchestrator python SDK
 Home-page: https://github.com/IBM/dfo-python-sdk.git
 Author: IBM
 Author-email: pugangxa@cn.ibm.com
 License: Apache 2.0
 Keywords: ibm_dfo_sdk
 Classifier: Programming Language :: Python
```

### Comparing `ibm-dfo-sdk-0.0.10/ibm_dfo_sdk.egg-info/SOURCES.txt` & `ibm-dfo-sdk-0.0.11/ibm_dfo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-dfo-sdk-0.0.10/setup.py` & `ibm-dfo-sdk-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.0.10'
+__version__ = '0.0.11'
 PACKAGE_NAME = 'ibm_dfo_sdk'
 PACKAGE_DESC = 'IBM Data Fabric Orchestrator python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

