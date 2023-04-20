# Comparing `tmp/alibabacloud_amqp-open20191212-1.0.2.tar.gz` & `tmp/alibabacloud_amqp-open20191212-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_amqp-open20191212-1.0.2.tar", last modified: Fri Dec  9 07:22:51 2022, max compression
+gzip compressed data, was "dist/alibabacloud_amqp-open20191212-1.0.3.tar", last modified: Thu Apr 20 03:57:44 2023, max compression
```

## Comparing `alibabacloud_amqp-open20191212-1.0.2.tar` & `alibabacloud_amqp-open20191212-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       98 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57849 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/client.py
--rw-r--r--   0 root         (0) root         (0)   105843 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2642 2022-12-09 07:22:51.000000 alibabacloud_amqp-open20191212-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66879 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/client.py
+-rw-r--r--   0 root         (0) root         (0)   122718 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-20 03:57:44.000000 alibabacloud_amqp-open20191212-1.0.3/setup.py
```

### Comparing `alibabacloud_amqp-open20191212-1.0.2/LICENSE` & `alibabacloud_amqp-open20191212-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_amqp-open20191212-1.0.2/PKG-INFO` & `alibabacloud_amqp-open20191212-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_amqp-open20191212
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud amqp-open (20191212) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_amqp-open20191212-1.0.2/README-CN.md` & `alibabacloud_amqp-open20191212-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_amqp-open20191212-1.0.2/README.md` & `alibabacloud_amqp-open20191212-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/client.py` & `alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,104 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def create_account_with_options(
+        self,
+        request: amqp_open_20191212_models.CreateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.CreateAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_access_key):
+            query['accountAccessKey'] = request.account_access_key
+        if not UtilClient.is_unset(request.create_timestamp):
+            query['createTimestamp'] = request.create_timestamp
+        if not UtilClient.is_unset(request.instance_id):
+            query['instanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.secret_sign):
+            query['secretSign'] = request.secret_sign
+        if not UtilClient.is_unset(request.signature):
+            query['signature'] = request.signature
+        if not UtilClient.is_unset(request.user_name):
+            query['userName'] = request.user_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAccount',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.CreateAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_account_with_options_async(
+        self,
+        request: amqp_open_20191212_models.CreateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.CreateAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_access_key):
+            query['accountAccessKey'] = request.account_access_key
+        if not UtilClient.is_unset(request.create_timestamp):
+            query['createTimestamp'] = request.create_timestamp
+        if not UtilClient.is_unset(request.instance_id):
+            query['instanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.secret_sign):
+            query['secretSign'] = request.secret_sign
+        if not UtilClient.is_unset(request.signature):
+            query['signature'] = request.signature
+        if not UtilClient.is_unset(request.user_name):
+            query['userName'] = request.user_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAccount',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.CreateAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_account(
+        self,
+        request: amqp_open_20191212_models.CreateAccountRequest,
+    ) -> amqp_open_20191212_models.CreateAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_account_with_options(request, runtime)
+
+    async def create_account_async(
+        self,
+        request: amqp_open_20191212_models.CreateAccountRequest,
+    ) -> amqp_open_20191212_models.CreateAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_account_with_options_async(request, runtime)
+
     def create_binding_with_options(
         self,
         request: amqp_open_20191212_models.CreateBindingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> amqp_open_20191212_models.CreateBindingResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -409,14 +499,88 @@
     async def create_virtual_host_async(
         self,
         request: amqp_open_20191212_models.CreateVirtualHostRequest,
     ) -> amqp_open_20191212_models.CreateVirtualHostResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_virtual_host_with_options_async(request, runtime)
 
+    def delete_account_with_options(
+        self,
+        request: amqp_open_20191212_models.DeleteAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.DeleteAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.create_timestamp):
+            query['CreateTimestamp'] = request.create_timestamp
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteAccount',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.DeleteAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_account_with_options_async(
+        self,
+        request: amqp_open_20191212_models.DeleteAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.DeleteAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.create_timestamp):
+            query['CreateTimestamp'] = request.create_timestamp
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteAccount',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.DeleteAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_account(
+        self,
+        request: amqp_open_20191212_models.DeleteAccountRequest,
+    ) -> amqp_open_20191212_models.DeleteAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_account_with_options(request, runtime)
+
+    async def delete_account_async(
+        self,
+        request: amqp_open_20191212_models.DeleteAccountRequest,
+    ) -> amqp_open_20191212_models.DeleteAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_account_with_options_async(request, runtime)
+
     def delete_binding_with_options(
         self,
         request: amqp_open_20191212_models.DeleteBindingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> amqp_open_20191212_models.DeleteBindingResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -795,14 +959,84 @@
     async def get_metadata_amount_async(
         self,
         request: amqp_open_20191212_models.GetMetadataAmountRequest,
     ) -> amqp_open_20191212_models.GetMetadataAmountResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_metadata_amount_with_options_async(request, runtime)
 
+    def list_accounts_with_options(
+        self,
+        request: amqp_open_20191212_models.ListAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.ListAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAccounts',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.ListAccountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_accounts_with_options_async(
+        self,
+        request: amqp_open_20191212_models.ListAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> amqp_open_20191212_models.ListAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAccounts',
+            version='2019-12-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            amqp_open_20191212_models.ListAccountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_accounts(
+        self,
+        request: amqp_open_20191212_models.ListAccountsRequest,
+    ) -> amqp_open_20191212_models.ListAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_accounts_with_options(request, runtime)
+
+    async def list_accounts_async(
+        self,
+        request: amqp_open_20191212_models.ListAccountsRequest,
+    ) -> amqp_open_20191212_models.ListAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_accounts_with_options_async(request, runtime)
+
     def list_bindings_with_options(
         self,
         request: amqp_open_20191212_models.ListBindingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> amqp_open_20191212_models.ListBindingsResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
```

### Comparing `alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212/models.py` & `alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,288 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class DataValue(TeaModel):
+    def __init__(
+        self,
+        master_uid: int = None,
+        c_instance_id: str = None,
+        access_key: str = None,
+        user_name: str = None,
+        password: str = None,
+        deleted: int = None,
+        create_timestamp: int = None,
+    ):
+        self.master_uid = master_uid
+        self.c_instance_id = c_instance_id
+        self.access_key = access_key
+        self.user_name = user_name
+        self.password = password
+        self.deleted = deleted
+        self.create_timestamp = create_timestamp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.master_uid is not None:
+            result['masterUid'] = self.master_uid
+        if self.c_instance_id is not None:
+            result['cInstanceId'] = self.c_instance_id
+        if self.access_key is not None:
+            result['accessKey'] = self.access_key
+        if self.user_name is not None:
+            result['userName'] = self.user_name
+        if self.password is not None:
+            result['password'] = self.password
+        if self.deleted is not None:
+            result['deleted'] = self.deleted
+        if self.create_timestamp is not None:
+            result['createTimestamp'] = self.create_timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('masterUid') is not None:
+            self.master_uid = m.get('masterUid')
+        if m.get('cInstanceId') is not None:
+            self.c_instance_id = m.get('cInstanceId')
+        if m.get('accessKey') is not None:
+            self.access_key = m.get('accessKey')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
+        if m.get('password') is not None:
+            self.password = m.get('password')
+        if m.get('deleted') is not None:
+            self.deleted = m.get('deleted')
+        if m.get('createTimestamp') is not None:
+            self.create_timestamp = m.get('createTimestamp')
+        return self
+
+
+class CreateAccountRequest(TeaModel):
+    def __init__(
+        self,
+        account_access_key: str = None,
+        create_timestamp: int = None,
+        instance_id: str = None,
+        secret_sign: str = None,
+        signature: str = None,
+        user_name: str = None,
+    ):
+        self.account_access_key = account_access_key
+        self.create_timestamp = create_timestamp
+        self.instance_id = instance_id
+        self.secret_sign = secret_sign
+        self.signature = signature
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_access_key is not None:
+            result['accountAccessKey'] = self.account_access_key
+        if self.create_timestamp is not None:
+            result['createTimestamp'] = self.create_timestamp
+        if self.instance_id is not None:
+            result['instanceId'] = self.instance_id
+        if self.secret_sign is not None:
+            result['secretSign'] = self.secret_sign
+        if self.signature is not None:
+            result['signature'] = self.signature
+        if self.user_name is not None:
+            result['userName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accountAccessKey') is not None:
+            self.account_access_key = m.get('accountAccessKey')
+        if m.get('createTimestamp') is not None:
+            self.create_timestamp = m.get('createTimestamp')
+        if m.get('instanceId') is not None:
+            self.instance_id = m.get('instanceId')
+        if m.get('secretSign') is not None:
+            self.secret_sign = m.get('secretSign')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
+        return self
+
+
+class CreateAccountResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        access_key: str = None,
+        create_time_stamp: int = None,
+        instance_id: str = None,
+        master_uid: int = None,
+        password: str = None,
+        user_name: str = None,
+    ):
+        # AccessKey ID。
+        self.access_key = access_key
+        self.create_time_stamp = create_time_stamp
+        self.instance_id = instance_id
+        self.master_uid = master_uid
+        self.password = password
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key is not None:
+            result['AccessKey'] = self.access_key
+        if self.create_time_stamp is not None:
+            result['CreateTimeStamp'] = self.create_time_stamp
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.master_uid is not None:
+            result['MasterUId'] = self.master_uid
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessKey') is not None:
+            self.access_key = m.get('AccessKey')
+        if m.get('CreateTimeStamp') is not None:
+            self.create_time_stamp = m.get('CreateTimeStamp')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MasterUId') is not None:
+            self.master_uid = m.get('MasterUId')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class CreateAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: CreateAccountResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = CreateAccountResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateBindingRequest(TeaModel):
     def __init__(
         self,
         argument: str = None,
         binding_key: str = None,
         binding_type: str = None,
         destination_name: str = None,
@@ -530,14 +805,142 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVirtualHostResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteAccountRequest(TeaModel):
+    def __init__(
+        self,
+        create_timestamp: int = None,
+        user_name: str = None,
+    ):
+        self.create_timestamp = create_timestamp
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_timestamp is not None:
+            result['CreateTimestamp'] = self.create_timestamp
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTimestamp') is not None:
+            self.create_timestamp = m.get('CreateTimestamp')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class DeleteAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: bool = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteBindingRequest(TeaModel):
     def __init__(
         self,
         binding_key: str = None,
         binding_type: str = None,
         destination_name: str = None,
         instance_id: str = None,
@@ -1145,14 +1548,151 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetMetadataAmountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class ListAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: Dict[str, List[DataValue]] = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            for v in self.data.values():
+                for k1 in v:
+                    if k1:
+                        k1.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['Data'] = {}
+        if self.data is not None:
+            for k, v in self.data.items():
+                l1 = []
+                for k1 in v:
+                    l1.append(k1.to_map() if k1 else None)
+                result['data'][k] = l1
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.data = {}
+        if m.get('Data') is not None:
+            for k, v in m.get('Data').items():
+                l1 = []
+                for k1 in v:
+                    temp_model = DataValue()
+                    l1.append(temp_model.from_map(k1))
+                self.data['k'] = l1
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ListAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListAccountsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListBindingsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         max_results: int = None,
         next_token: str = None,
         virtual_host: str = None,
@@ -1968,14 +2508,15 @@
 class ListExchangesResponseBodyData(TeaModel):
     def __init__(
         self,
         exchanges: List[ListExchangesResponseBodyDataExchanges] = None,
         max_results: int = None,
         next_token: str = None,
     ):
+        # Exchange。
         self.exchanges = exchanges
         self.max_results = max_results
         self.next_token = next_token
 
     def validate(self):
         if self.exchanges:
             for k in self.exchanges:
@@ -2924,14 +3465,15 @@
         self,
         max_results: int = None,
         next_token: str = None,
         queues: List[ListQueuesResponseBodyDataQueues] = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
+        # Queue。
         self.queues = queues
 
     def validate(self):
         if self.queues:
             for k in self.queues:
                 if k:
                     k.validate()
@@ -3116,14 +3658,15 @@
         self,
         max_results: int = None,
         next_token: str = None,
         virtual_hosts: List[ListVirtualHostsResponseBodyDataVirtualHosts] = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
+        # Vhost。
         self.virtual_hosts = virtual_hosts
 
     def validate(self):
         if self.virtual_hosts:
             for k in self.virtual_hosts:
                 if k:
                     k.validate()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_amqp-open20191212-1.0.2/alibabacloud_amqp_open20191212.egg-info/PKG-INFO` & `alibabacloud_amqp-open20191212-1.0.3/alibabacloud_amqp_open20191212.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-amqp-open20191212
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud amqp-open (20191212) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_amqp-open20191212-1.0.2/setup.py` & `alibabacloud_amqp-open20191212-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_amqp-open20191212.
 
-Created on 09/12/2022
+Created on 20/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_amqp_open20191212"
 NAME = "alibabacloud_amqp-open20191212" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud amqp-open (20191212) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

