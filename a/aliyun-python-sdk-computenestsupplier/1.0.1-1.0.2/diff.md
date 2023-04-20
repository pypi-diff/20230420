# Comparing `tmp/aliyun-python-sdk-computenestsupplier-1.0.1.tar.gz` & `tmp/aliyun-python-sdk-computenestsupplier-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.1.tar", last modified: Mon Feb  6 08:10:20 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.2.tar", last modified: Thu Apr 20 09:41:48 2023, max compression
```

## Comparing `aliyun-python-sdk-computenestsupplier-1.0.1.tar` & `aliyun-python-sdk-computenestsupplier-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1617 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1617 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1369 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/
--rw-r--r--   0 root         (0) root         (0)     2778 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2646 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2532 2023-02-06 08:10:20.000000 aliyun-python-sdk-computenestsupplier-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/setup.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/LICENSE` & `aliyun-python-sdk-computenestsupplier-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.1
+Version: 1.0.2
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/README.rst` & `aliyun-python-sdk-computenestsupplier-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.1
+Version: 1.0.2
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/endpoint.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class ListServiceInstancesRequest(RpcRequest):
+class ListServiceUsagesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceInstances')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceUsages')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
-	def get_Tags(self): # RepeatList
-		return self.get_query_params().get('Tag')
-
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_Filters(self): # RepeatList
 		return self.get_query_params().get('Filter')
 
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
 			if Filter[depth1].get('Value') is not None:
 				for depth2 in range(len(Filter[depth1].get('Value'))):
 					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # String
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,38 +16,52 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class ListServiceUsagesRequest(RpcRequest):
+class ListServiceInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceUsages')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceInstances')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_ShowDeleted(self): # Boolean
+		return self.get_query_params().get('ShowDeleted')
+
+	def set_ShowDeleted(self, ShowDeleted):  # Boolean
+		self.add_query_param('ShowDeleted', ShowDeleted)
 	def get_Filters(self): # RepeatList
 		return self.get_query_params().get('Filter')
 
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
 			if Filter[depth1].get('Value') is not None:
 				for depth2 in range(len(Filter[depth1].get('Value'))):
 					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # Integer
+	def get_MaxResults(self): # String
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # Integer
+	def set_MaxResults(self, MaxResults):  # String
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.1/setup.py` & `aliyun-python-sdk-computenestsupplier-1.0.2/setup.py`

 * *Files identical despite different names*

