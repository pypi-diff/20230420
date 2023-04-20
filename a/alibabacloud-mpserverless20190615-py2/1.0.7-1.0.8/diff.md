# Comparing `tmp/alibabacloud_mpserverless20190615_py2-1.0.7.tar.gz` & `tmp/alibabacloud_mpserverless20190615_py2-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mpserverless20190615_py2-1.0.7.tar", last modified: Mon Dec  5 03:52:16 2022, max compression
+gzip compressed data, was "dist/alibabacloud_mpserverless20190615_py2-1.0.8.tar", last modified: Thu Apr 20 09:47:39 2023, max compression
```

## Comparing `alibabacloud_mpserverless20190615_py2-1.0.7.tar` & `alibabacloud_mpserverless20190615_py2-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      210 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2526 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99233 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/client.py
--rw-r--r--   0 root         (0) root         (0)   380094 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2526 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2948 2022-12-05 03:52:16.000000 alibabacloud_mpserverless20190615_py2-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:47:39.000000 alibabacloud_mpserverless20190615_py2-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-20 09:47:39.000000 alibabacloud_mpserverless20190615_py2-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:47:39.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101058 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/client.py
+-rw-r--r--   0 root         (0) root         (0)   385699 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:47:39.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-20 09:47:39.000000 alibabacloud_mpserverless20190615_py2-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-04-20 09:47:38.000000 alibabacloud_mpserverless20190615_py2-1.0.8/setup.py
```

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/LICENSE` & `alibabacloud_mpserverless20190615_py2-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/PKG-INFO` & `alibabacloud_mpserverless20190615_py2-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mpserverless20190615_py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud MPServerless (20190615) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/README-CN.md` & `alibabacloud_mpserverless20190615_py2-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/README.md` & `alibabacloud_mpserverless20190615_py2-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/client.py` & `alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,14 +416,52 @@
             self.call_api(params, req, runtime)
         )
 
     def create_space(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_space_with_options(request, runtime)
 
+    def create_space_with_order_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.desc):
+            body['Desc'] = request.desc
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.package_version):
+            body['PackageVersion'] = request.package_version
+        if not UtilClient.is_unset(request.period):
+            body['Period'] = request.period
+        if not UtilClient.is_unset(request.subscription_type):
+            body['SubscriptionType'] = request.subscription_type
+        if not UtilClient.is_unset(request.use_coupon):
+            body['UseCoupon'] = request.use_coupon
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSpaceWithOrder',
+            version='2019-06-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            mpserverless_20190615_models.CreateSpaceWithOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_space_with_order(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_space_with_order_with_options(request, runtime)
+
     def delete_ant_open_platform_config_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.space_id):
             body['SpaceId'] = request.space_id
@@ -771,14 +809,16 @@
         return self.describe_fcopen_status_with_options(runtime)
 
     def describe_file_upload_signed_url_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.content_type):
             body['ContentType'] = request.content_type
+        if not UtilClient.is_unset(request.file_id):
+            body['FileId'] = request.file_id
         if not UtilClient.is_unset(request.filename):
             body['Filename'] = request.filename
         if not UtilClient.is_unset(request.size):
             body['Size'] = request.size
         if not UtilClient.is_unset(request.space_id):
             body['SpaceId'] = request.space_id
         req = open_api_models.OpenApiRequest(
@@ -1360,16 +1400,20 @@
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         body = {}
         if not UtilClient.is_unset(request.file_id):
             body['FileId'] = request.file_id
         if not UtilClient.is_unset(request.keyword):
             body['Keyword'] = request.keyword
+        if not UtilClient.is_unset(request.mode):
+            body['Mode'] = request.mode
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.prefix):
+            body['Prefix'] = request.prefix
         if not UtilClient.is_unset(request.space_id):
             body['SpaceId'] = request.space_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615/models.py` & `alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1331,14 +1331,142 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateSpaceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateSpaceWithOrderRequest(TeaModel):
+    def __init__(self, desc=None, name=None, package_version=None, period=None, subscription_type=None,
+                 use_coupon=None):
+        self.desc = desc  # type: str
+        self.name = name  # type: str
+        self.package_version = package_version  # type: str
+        self.period = period  # type: int
+        self.subscription_type = subscription_type  # type: str
+        self.use_coupon = use_coupon  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSpaceWithOrderRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.desc is not None:
+            result['Desc'] = self.desc
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.package_version is not None:
+            result['PackageVersion'] = self.package_version
+        if self.period is not None:
+            result['Period'] = self.period
+        if self.subscription_type is not None:
+            result['SubscriptionType'] = self.subscription_type
+        if self.use_coupon is not None:
+            result['UseCoupon'] = self.use_coupon
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Desc') is not None:
+            self.desc = m.get('Desc')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('PackageVersion') is not None:
+            self.package_version = m.get('PackageVersion')
+        if m.get('Period') is not None:
+            self.period = m.get('Period')
+        if m.get('SubscriptionType') is not None:
+            self.subscription_type = m.get('SubscriptionType')
+        if m.get('UseCoupon') is not None:
+            self.use_coupon = m.get('UseCoupon')
+        return self
+
+
+class CreateSpaceWithOrderResponseBody(TeaModel):
+    def __init__(self, instance_id=None, order_id=None, request_id=None, space_id=None):
+        self.instance_id = instance_id  # type: str
+        self.order_id = order_id  # type: str
+        self.request_id = request_id  # type: str
+        self.space_id = space_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSpaceWithOrderResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.space_id is not None:
+            result['SpaceId'] = self.space_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SpaceId') is not None:
+            self.space_id = m.get('SpaceId')
+        return self
+
+
+class CreateSpaceWithOrderResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateSpaceWithOrderResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateSpaceWithOrderResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateSpaceWithOrderResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteAntOpenPlatformConfigRequest(TeaModel):
     def __init__(self, app_id=None, space_id=None):
         self.app_id = app_id  # type: str
         self.space_id = space_id  # type: str
 
     def validate(self):
         pass
@@ -2417,16 +2545,17 @@
         if m.get('body') is not None:
             temp_model = DescribeFCOpenStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeFileUploadSignedUrlRequest(TeaModel):
-    def __init__(self, content_type=None, filename=None, size=None, space_id=None):
+    def __init__(self, content_type=None, file_id=None, filename=None, size=None, space_id=None):
         self.content_type = content_type  # type: str
+        self.file_id = file_id  # type: str
         self.filename = filename  # type: str
         self.size = size  # type: long
         self.space_id = space_id  # type: str
 
     def validate(self):
         pass
 
@@ -2434,26 +2563,30 @@
         _map = super(DescribeFileUploadSignedUrlRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.content_type is not None:
             result['ContentType'] = self.content_type
+        if self.file_id is not None:
+            result['FileId'] = self.file_id
         if self.filename is not None:
             result['Filename'] = self.filename
         if self.size is not None:
             result['Size'] = self.size
         if self.space_id is not None:
             result['SpaceId'] = self.space_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ContentType') is not None:
             self.content_type = m.get('ContentType')
+        if m.get('FileId') is not None:
+            self.file_id = m.get('FileId')
         if m.get('Filename') is not None:
             self.filename = m.get('Filename')
         if m.get('Size') is not None:
             self.size = m.get('Size')
         if m.get('SpaceId') is not None:
             self.space_id = m.get('SpaceId')
         return self
@@ -5436,19 +5569,22 @@
         if m.get('body') is not None:
             temp_model = ListExtensionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListFileRequest(TeaModel):
-    def __init__(self, file_id=None, keyword=None, next_token=None, page_size=None, space_id=None):
+    def __init__(self, file_id=None, keyword=None, mode=None, next_token=None, page_size=None, prefix=None,
+                 space_id=None):
         self.file_id = file_id  # type: str
         self.keyword = keyword  # type: str
+        self.mode = mode  # type: str
         self.next_token = next_token  # type: str
         self.page_size = page_size  # type: int
+        self.prefix = prefix  # type: str
         self.space_id = space_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListFileRequest, self).to_map()
@@ -5456,32 +5592,40 @@
             return _map
 
         result = dict()
         if self.file_id is not None:
             result['FileId'] = self.file_id
         if self.keyword is not None:
             result['Keyword'] = self.keyword
+        if self.mode is not None:
+            result['Mode'] = self.mode
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.prefix is not None:
+            result['Prefix'] = self.prefix
         if self.space_id is not None:
             result['SpaceId'] = self.space_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('FileId') is not None:
             self.file_id = m.get('FileId')
         if m.get('Keyword') is not None:
             self.keyword = m.get('Keyword')
+        if m.get('Mode') is not None:
+            self.mode = m.get('Mode')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        if m.get('Prefix') is not None:
+            self.prefix = m.get('Prefix')
         if m.get('SpaceId') is not None:
             self.space_id = m.get('SpaceId')
         return self
 
 
 class ListFileResponseBodyDataList(TeaModel):
     def __init__(self, gmt_create=None, gmt_modified=None, id=None, name=None, size=None, type=None, url=None):
@@ -8720,17 +8864,19 @@
             self.cdn_traffic = m.get('CdnTraffic')
         if m.get('StorageSize') is not None:
             self.storage_size = m.get('StorageSize')
         return self
 
 
 class QuerySpaceUsageResponseBodySpaceUsageDataList(TeaModel):
-    def __init__(self, cs_usage=None, db_usage=None, fc_usage=None, timestamp=None, wh_usage=None):
+    def __init__(self, cs_usage=None, db_usage=None, effective_bill_flag=None, fc_usage=None, timestamp=None,
+                 wh_usage=None):
         self.cs_usage = cs_usage  # type: QuerySpaceUsageResponseBodySpaceUsageDataListCsUsage
         self.db_usage = db_usage  # type: QuerySpaceUsageResponseBodySpaceUsageDataListDbUsage
+        self.effective_bill_flag = effective_bill_flag  # type: bool
         self.fc_usage = fc_usage  # type: QuerySpaceUsageResponseBodySpaceUsageDataListFcUsage
         self.timestamp = timestamp  # type: str
         self.wh_usage = wh_usage  # type: QuerySpaceUsageResponseBodySpaceUsageDataListWhUsage
 
     def validate(self):
         if self.cs_usage:
             self.cs_usage.validate()
@@ -8747,14 +8893,16 @@
             return _map
 
         result = dict()
         if self.cs_usage is not None:
             result['CsUsage'] = self.cs_usage.to_map()
         if self.db_usage is not None:
             result['DbUsage'] = self.db_usage.to_map()
+        if self.effective_bill_flag is not None:
+            result['EffectiveBillFlag'] = self.effective_bill_flag
         if self.fc_usage is not None:
             result['FcUsage'] = self.fc_usage.to_map()
         if self.timestamp is not None:
             result['Timestamp'] = self.timestamp
         if self.wh_usage is not None:
             result['WhUsage'] = self.wh_usage.to_map()
         return result
@@ -8763,14 +8911,16 @@
         m = m or dict()
         if m.get('CsUsage') is not None:
             temp_model = QuerySpaceUsageResponseBodySpaceUsageDataListCsUsage()
             self.cs_usage = temp_model.from_map(m['CsUsage'])
         if m.get('DbUsage') is not None:
             temp_model = QuerySpaceUsageResponseBodySpaceUsageDataListDbUsage()
             self.db_usage = temp_model.from_map(m['DbUsage'])
+        if m.get('EffectiveBillFlag') is not None:
+            self.effective_bill_flag = m.get('EffectiveBillFlag')
         if m.get('FcUsage') is not None:
             temp_model = QuerySpaceUsageResponseBodySpaceUsageDataListFcUsage()
             self.fc_usage = temp_model.from_map(m['FcUsage'])
         if m.get('Timestamp') is not None:
             self.timestamp = m.get('Timestamp')
         if m.get('WhUsage') is not None:
             temp_model = QuerySpaceUsageResponseBodySpaceUsageDataListWhUsage()
```

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/PKG-INFO` & `alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mpserverless20190615-py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud MPServerless (20190615) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/alibabacloud_mpserverless20190615_py2.egg-info/SOURCES.txt` & `alibabacloud_mpserverless20190615_py2-1.0.8/alibabacloud_mpserverless20190615_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpserverless20190615_py2-1.0.7/setup.py` & `alibabacloud_mpserverless20190615_py2-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mpserverless20190615_py2.
 
-Created on 05/12/2022
+Created on 20/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mpserverless20190615"
 NAME = "alibabacloud_mpserverless20190615_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MPServerless (20190615) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

