# Comparing `tmp/aliyun-python-sdk-amqp-open-1.1.1.tar.gz` & `tmp/aliyun-python-sdk-amqp-open-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-amqp-open-1.1.1.tar", last modified: Wed Jul  1 08:07:40 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-amqp-open-1.1.2.tar", last modified: Thu Apr 20 02:32:09 2023, max compression
```

## Comparing `aliyun-python-sdk-amqp-open-1.1.1.tar` & `aliyun-python-sdk-amqp-open-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/
--rw-rw-r--   0 admin     (1017) admin     (1017)       21 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/
--rw-rw-r--   0 admin     (1017) admin     (1017)     1817 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteExchangeRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2182 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListExchangeUpStreamBindingsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2120 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListQueueConsumersRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2170 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListDownStreamBindingsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1460 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/GetMetadataAmountRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3385 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateQueueRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2577 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateExchangeRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1793 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteQueueRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2379 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteBindingRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1796 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListVirtualHostsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1966 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListBindingsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1962 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListQueuesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2539 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateBindingRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1639 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateVirtualHostRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1618 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListInstancesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1968 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListExchangesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2158 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListQueueUpStreamBindingsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1639 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteVirtualHostRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1088 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/endpoint.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/MANIFEST.in
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/
--rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       19 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/requires.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1583 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1567 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/setup.cfg
--rw-rw-r--   0 admin     (1017) admin     (1017)      539 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/README.rst
--rw-rw-r--   0 admin     (1017) admin     (1017)     1567 2020-07-01 08:07:40.000000 aliyun-python-sdk-amqp-open-1.1.1/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)     2482 2020-07-01 08:07:39.000000 aliyun-python-sdk-amqp-open-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateExchangeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateQueueRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateVirtualHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteExchangeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteQueueRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteVirtualHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/GetMetadataAmountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListDownStreamBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListExchangeUpStreamBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListExchangesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListQueueConsumersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListQueueUpStreamBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListQueuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListVirtualHostsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/UpdateInstanceNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-20 02:32:09.000000 aliyun-python-sdk-amqp-open-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-20 02:32:08.000000 aliyun-python-sdk-amqp-open-1.1.2/setup.py
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteExchangeRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateVirtualHostRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class DeleteExchangeRequest(RpcRequest):
+class CreateVirtualHostRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteExchange','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateVirtualHost')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ExchangeName(self):
-		return self.get_body_params().get('ExchangeName')
-
-	def set_ExchangeName(self,ExchangeName):
-		self.add_body_params('ExchangeName', ExchangeName)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListExchangeUpStreamBindingsRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteVirtualHostRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,47 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class ListExchangeUpStreamBindingsRequest(RpcRequest):
+class DeleteVirtualHostRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListExchangeUpStreamBindings','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteVirtualHost')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_InstanceId(self): # String
+		return self.get_body_params().get('InstanceId')
 
-	def get_ExchangeName(self):
-		return self.get_query_params().get('ExchangeName')
-
-	def set_ExchangeName(self,ExchangeName):
-		self.add_query_param('ExchangeName',ExchangeName)
-
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
-
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
-
-	def get_VirtualHost(self):
-		return self.get_query_params().get('VirtualHost')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_body_params('InstanceId', InstanceId)
+	def get_VirtualHost(self): # String
+		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListQueueConsumersRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListQueueConsumersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,44 +19,40 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class ListQueueConsumersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListQueueConsumers','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListQueueConsumers')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_QueryCount(self):
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_QueryCount(self): # Integer
 		return self.get_query_params().get('QueryCount')
 
-	def set_QueryCount(self,QueryCount):
-		self.add_query_param('QueryCount',QueryCount)
-
-	def get_VirtualHost(self):
+	def set_QueryCount(self, QueryCount):  # Integer
+		self.add_query_param('QueryCount', QueryCount)
+	def get_VirtualHost(self): # String
 		return self.get_query_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
-
-	def get_Queue(self):
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_query_param('VirtualHost', VirtualHost)
+	def get_Queue(self): # String
 		return self.get_query_params().get('Queue')
 
-	def set_Queue(self,Queue):
-		self.add_query_param('Queue',Queue)
+	def set_Queue(self, Queue):  # String
+		self.add_query_param('Queue', Queue)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListDownStreamBindingsRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListAccountsRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,47 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class ListDownStreamBindingsRequest(RpcRequest):
+class ListAccountsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListDownStreamBindings','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListAccounts')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ExchangeName(self):
-		return self.get_query_params().get('ExchangeName')
-
-	def set_ExchangeName(self,ExchangeName):
-		self.add_query_param('ExchangeName',ExchangeName)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
-
-	def get_VirtualHost(self):
-		return self.get_query_params().get('VirtualHost')
-
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/GetMetadataAmountRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/GetMetadataAmountRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class GetMetadataAmountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'GetMetadataAmount','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'GetMetadataAmount')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateQueueRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateQueueRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,80 +19,70 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class CreateQueueRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateQueue','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateQueue')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_QueueName(self):
+	def get_QueueName(self): # String
 		return self.get_body_params().get('QueueName')
 
-	def set_QueueName(self,QueueName):
+	def set_QueueName(self, QueueName):  # String
 		self.add_body_params('QueueName', QueueName)
-
-	def get_DeadLetterRoutingKey(self):
+	def get_DeadLetterRoutingKey(self): # String
 		return self.get_body_params().get('DeadLetterRoutingKey')
 
-	def set_DeadLetterRoutingKey(self,DeadLetterRoutingKey):
+	def set_DeadLetterRoutingKey(self, DeadLetterRoutingKey):  # String
 		self.add_body_params('DeadLetterRoutingKey', DeadLetterRoutingKey)
-
-	def get_MaxLength(self):
+	def get_MaxLength(self): # Long
 		return self.get_body_params().get('MaxLength')
 
-	def set_MaxLength(self,MaxLength):
+	def set_MaxLength(self, MaxLength):  # Long
 		self.add_body_params('MaxLength', MaxLength)
-
-	def get_AutoExpireState(self):
+	def get_AutoExpireState(self): # Long
 		return self.get_body_params().get('AutoExpireState')
 
-	def set_AutoExpireState(self,AutoExpireState):
+	def set_AutoExpireState(self, AutoExpireState):  # Long
 		self.add_body_params('AutoExpireState', AutoExpireState)
-
-	def get_DeadLetterExchange(self):
+	def get_DeadLetterExchange(self): # String
 		return self.get_body_params().get('DeadLetterExchange')
 
-	def set_DeadLetterExchange(self,DeadLetterExchange):
+	def set_DeadLetterExchange(self, DeadLetterExchange):  # String
 		self.add_body_params('DeadLetterExchange', DeadLetterExchange)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_ExclusiveState(self):
+	def get_ExclusiveState(self): # Boolean
 		return self.get_body_params().get('ExclusiveState')
 
-	def set_ExclusiveState(self,ExclusiveState):
+	def set_ExclusiveState(self, ExclusiveState):  # Boolean
 		self.add_body_params('ExclusiveState', ExclusiveState)
-
-	def get_AutoDeleteState(self):
+	def get_AutoDeleteState(self): # Boolean
 		return self.get_body_params().get('AutoDeleteState')
 
-	def set_AutoDeleteState(self,AutoDeleteState):
+	def set_AutoDeleteState(self, AutoDeleteState):  # Boolean
 		self.add_body_params('AutoDeleteState', AutoDeleteState)
-
-	def get_MessageTTL(self):
+	def get_MessageTTL(self): # Long
 		return self.get_body_params().get('MessageTTL')
 
-	def set_MessageTTL(self,MessageTTL):
+	def set_MessageTTL(self, MessageTTL):  # Long
 		self.add_body_params('MessageTTL', MessageTTL)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
+	def set_VirtualHost(self, VirtualHost):  # String
 		self.add_body_params('VirtualHost', VirtualHost)
-
-	def get_MaximumPriority(self):
+	def get_MaximumPriority(self): # Integer
 		return self.get_body_params().get('MaximumPriority')
 
-	def set_MaximumPriority(self,MaximumPriority):
-		self.add_body_params('MaximumPriority', MaximumPriority)
+	def set_MaximumPriority(self, MaximumPriority):  # Integer
+		self.add_body_params('MaximumPriority', MaximumPriority)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateExchangeRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateExchangeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class CreateExchangeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateExchange','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateExchange')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Internal(self):
+	def get_Internal(self): # Boolean
 		return self.get_body_params().get('Internal')
 
-	def set_Internal(self,Internal):
+	def set_Internal(self, Internal):  # Boolean
 		self.add_body_params('Internal', Internal)
-
-	def get_ExchangeName(self):
+	def get_ExchangeName(self): # String
 		return self.get_body_params().get('ExchangeName')
 
-	def set_ExchangeName(self,ExchangeName):
+	def set_ExchangeName(self, ExchangeName):  # String
 		self.add_body_params('ExchangeName', ExchangeName)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_AlternateExchange(self):
+	def get_AlternateExchange(self): # String
 		return self.get_body_params().get('AlternateExchange')
 
-	def set_AlternateExchange(self,AlternateExchange):
+	def set_AlternateExchange(self, AlternateExchange):  # String
 		self.add_body_params('AlternateExchange', AlternateExchange)
-
-	def get_AutoDeleteState(self):
+	def get_AutoDeleteState(self): # Boolean
 		return self.get_body_params().get('AutoDeleteState')
 
-	def set_AutoDeleteState(self,AutoDeleteState):
+	def set_AutoDeleteState(self, AutoDeleteState):  # Boolean
 		self.add_body_params('AutoDeleteState', AutoDeleteState)
-
-	def get_ExchangeType(self):
+	def get_ExchangeType(self): # String
 		return self.get_body_params().get('ExchangeType')
 
-	def set_ExchangeType(self,ExchangeType):
+	def set_ExchangeType(self, ExchangeType):  # String
 		self.add_body_params('ExchangeType', ExchangeType)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteQueueRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteExchangeRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class DeleteQueueRequest(RpcRequest):
+class DeleteExchangeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteQueue','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteExchange')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ExchangeName(self): # String
+		return self.get_body_params().get('ExchangeName')
 
-	def get_QueueName(self):
-		return self.get_body_params().get('QueueName')
-
-	def set_QueueName(self,QueueName):
-		self.add_body_params('QueueName', QueueName)
-
-	def get_InstanceId(self):
+	def set_ExchangeName(self, ExchangeName):  # String
+		self.add_body_params('ExchangeName', ExchangeName)
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/DeleteBindingRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteBindingRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class DeleteBindingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteBinding','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteBinding')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_DestinationName(self):
+	def get_DestinationName(self): # String
 		return self.get_body_params().get('DestinationName')
 
-	def set_DestinationName(self,DestinationName):
+	def set_DestinationName(self, DestinationName):  # String
 		self.add_body_params('DestinationName', DestinationName)
-
-	def get_SourceExchange(self):
+	def get_SourceExchange(self): # String
 		return self.get_body_params().get('SourceExchange')
 
-	def set_SourceExchange(self,SourceExchange):
+	def set_SourceExchange(self, SourceExchange):  # String
 		self.add_body_params('SourceExchange', SourceExchange)
-
-	def get_BindingKey(self):
+	def get_BindingKey(self): # String
 		return self.get_body_params().get('BindingKey')
 
-	def set_BindingKey(self,BindingKey):
+	def set_BindingKey(self, BindingKey):  # String
 		self.add_body_params('BindingKey', BindingKey)
-
-	def get_BindingType(self):
+	def get_BindingType(self): # String
 		return self.get_body_params().get('BindingType')
 
-	def set_BindingType(self,BindingType):
+	def set_BindingType(self, BindingType):  # String
 		self.add_body_params('BindingType', BindingType)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListVirtualHostsRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListVirtualHostsRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,32 +19,30 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class ListVirtualHostsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListVirtualHosts','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListVirtualHosts')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListBindingsRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListDownStreamBindingsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class ListBindingsRequest(RpcRequest):
+class ListDownStreamBindingsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListBindings','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListDownStreamBindings')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ExchangeName(self): # String
+		return self.get_query_params().get('ExchangeName')
 
-	def get_InstanceId(self):
+	def set_ExchangeName(self, ExchangeName):  # String
+		self.add_query_param('ExchangeName', ExchangeName)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
-
-	def get_VirtualHost(self):
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
+	def get_VirtualHost(self): # String
 		return self.get_query_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_query_param('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListQueuesRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListBindingsRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class ListQueuesRequest(RpcRequest):
+class ListBindingsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListQueues','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListBindings')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
-
-	def get_VirtualHost(self):
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
+	def get_VirtualHost(self): # String
 		return self.get_query_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_query_param('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateBindingRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/CreateBindingRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class CreateBindingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateBinding','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateBinding')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Argument(self):
+	def get_Argument(self): # String
 		return self.get_body_params().get('Argument')
 
-	def set_Argument(self,Argument):
+	def set_Argument(self, Argument):  # String
 		self.add_body_params('Argument', Argument)
-
-	def get_DestinationName(self):
+	def get_DestinationName(self): # String
 		return self.get_body_params().get('DestinationName')
 
-	def set_DestinationName(self,DestinationName):
+	def set_DestinationName(self, DestinationName):  # String
 		self.add_body_params('DestinationName', DestinationName)
-
-	def get_SourceExchange(self):
+	def get_SourceExchange(self): # String
 		return self.get_body_params().get('SourceExchange')
 
-	def set_SourceExchange(self,SourceExchange):
+	def set_SourceExchange(self, SourceExchange):  # String
 		self.add_body_params('SourceExchange', SourceExchange)
-
-	def get_BindingKey(self):
+	def get_BindingKey(self): # String
 		return self.get_body_params().get('BindingKey')
 
-	def set_BindingKey(self,BindingKey):
+	def set_BindingKey(self, BindingKey):  # String
 		self.add_body_params('BindingKey', BindingKey)
-
-	def get_BindingType(self):
+	def get_BindingType(self): # String
 		return self.get_body_params().get('BindingType')
 
-	def set_BindingType(self,BindingType):
+	def set_BindingType(self, BindingType):  # String
 		self.add_body_params('BindingType', BindingType)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/CreateVirtualHostRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/DeleteQueueRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class CreateVirtualHostRequest(RpcRequest):
+class DeleteQueueRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'CreateVirtualHost','onsproxy')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'DeleteQueue')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_QueueName(self): # String
+		return self.get_body_params().get('QueueName')
 
-	def get_InstanceId(self):
+	def set_QueueName(self, QueueName):  # String
+		self.add_body_params('QueueName', QueueName)
+	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
+	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-
-	def get_VirtualHost(self):
+	def get_VirtualHost(self): # String
 		return self.get_body_params().get('VirtualHost')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_body_params('VirtualHost', VirtualHost)
+	def set_VirtualHost(self, VirtualHost):  # String
+		self.add_body_params('VirtualHost', VirtualHost)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListInstancesRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/ListInstancesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
 class ListInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListInstances','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListInstances')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_NextToken(self):
+	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/request/v20191212/ListExchangesRequest.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/request/v20191212/UpdateInstanceNameRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkamqp_open.endpoint import endpoint_data
 
-class ListExchangesRequest(RpcRequest):
+class UpdateInstanceNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'ListExchanges','onsproxy')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'amqp-open', '2019-12-12', 'UpdateInstanceName')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_MaxResults(self):
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
-
-	def get_VirtualHost(self):
-		return self.get_query_params().get('VirtualHost')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_InstanceName(self): # String
+		return self.get_query_params().get('InstanceName')
 
-	def set_VirtualHost(self,VirtualHost):
-		self.add_query_param('VirtualHost',VirtualHost)
+	def set_InstanceName(self, InstanceName):  # String
+		self.add_query_param('InstanceName', InstanceName)
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyunsdkamqp_open/endpoint.py` & `aliyun-python-sdk-amqp-open-1.1.2/aliyunsdkamqp_open/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/SOURCES.txt` & `aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+LICENSE
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 aliyun_python_sdk_amqp_open.egg-info/PKG-INFO
 aliyun_python_sdk_amqp_open.egg-info/SOURCES.txt
 aliyun_python_sdk_amqp_open.egg-info/dependency_links.txt
 aliyun_python_sdk_amqp_open.egg-info/requires.txt
 aliyun_python_sdk_amqp_open.egg-info/top_level.txt
 aliyunsdkamqp_open/__init__.py
 aliyunsdkamqp_open/endpoint.py
 aliyunsdkamqp_open/request/__init__.py
+aliyunsdkamqp_open/request/v20191212/CreateAccountRequest.py
 aliyunsdkamqp_open/request/v20191212/CreateBindingRequest.py
 aliyunsdkamqp_open/request/v20191212/CreateExchangeRequest.py
 aliyunsdkamqp_open/request/v20191212/CreateQueueRequest.py
 aliyunsdkamqp_open/request/v20191212/CreateVirtualHostRequest.py
+aliyunsdkamqp_open/request/v20191212/DeleteAccountRequest.py
 aliyunsdkamqp_open/request/v20191212/DeleteBindingRequest.py
 aliyunsdkamqp_open/request/v20191212/DeleteExchangeRequest.py
 aliyunsdkamqp_open/request/v20191212/DeleteQueueRequest.py
 aliyunsdkamqp_open/request/v20191212/DeleteVirtualHostRequest.py
 aliyunsdkamqp_open/request/v20191212/GetMetadataAmountRequest.py
+aliyunsdkamqp_open/request/v20191212/ListAccountsRequest.py
 aliyunsdkamqp_open/request/v20191212/ListBindingsRequest.py
 aliyunsdkamqp_open/request/v20191212/ListDownStreamBindingsRequest.py
 aliyunsdkamqp_open/request/v20191212/ListExchangeUpStreamBindingsRequest.py
 aliyunsdkamqp_open/request/v20191212/ListExchangesRequest.py
 aliyunsdkamqp_open/request/v20191212/ListInstancesRequest.py
 aliyunsdkamqp_open/request/v20191212/ListQueueConsumersRequest.py
 aliyunsdkamqp_open/request/v20191212/ListQueueUpStreamBindingsRequest.py
 aliyunsdkamqp_open/request/v20191212/ListQueuesRequest.py
 aliyunsdkamqp_open/request/v20191212/ListVirtualHostsRequest.py
+aliyunsdkamqp_open/request/v20191212/UpdateInstanceNameRequest.py
 aliyunsdkamqp_open/request/v20191212/__init__.py
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/aliyun_python_sdk_amqp_open.egg-info/PKG-INFO` & `aliyun-python-sdk-amqp-open-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-amqp-open
-Version: 1.1.1
+Version: 1.1.2
 Summary: The amqp-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-amqp-open
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/README.rst` & `aliyun-python-sdk-amqp-open-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/PKG-INFO` & `aliyun-python-sdk-amqp-open-1.1.2/aliyun_python_sdk_amqp_open.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-amqp-open
-Version: 1.1.1
+Version: 1.1.2
 Summary: The amqp-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-amqp-open
```

### Comparing `aliyun-python-sdk-amqp-open-1.1.1/setup.py` & `aliyun-python-sdk-amqp-open-1.1.2/setup.py`

 * *Files identical despite different names*

