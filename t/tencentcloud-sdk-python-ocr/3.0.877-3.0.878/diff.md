# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.877.tar", last modified: Wed Apr 19 09:25:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.878.tar", last modified: Thu Apr 20 00:38:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.877.tar` & `tencentcloud-sdk-python-ocr-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   105698 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   406294 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:25:30.000000 tencentcloud-sdk-python-ocr-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   107564 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   413744 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:38:48.000000 tencentcloud-sdk-python-ocr-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.878/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/README.rst` & `tencentcloud-sdk-python-ocr-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1550,14 +1550,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RecognizePhilippinesSssIDOCR(self, request):
+        """菲律宾SSSID识别
+
+        :param request: Request instance for RecognizePhilippinesSssIDOCR.
+        :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesSssIDOCRRequest`
+        :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesSssIDOCRResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RecognizePhilippinesSssIDOCR", params, headers=headers)
+            response = json.loads(body)
+            model = models.RecognizePhilippinesSssIDOCRResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RecognizePhilippinesTinIDOCR(self, request):
+        """菲律宾TinID识别
+
+        :param request: Request instance for RecognizePhilippinesTinIDOCR.
+        :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesTinIDOCRRequest`
+        :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesTinIDOCRResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RecognizePhilippinesTinIDOCR", params, headers=headers)
+            response = json.loads(body)
+            model = models.RecognizePhilippinesTinIDOCRResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RecognizePhilippinesVoteIDOCR(self, request):
         """本接口支持菲律宾VoteID识别，识别字段包括姓名、姓氏、出生日期、婚姻状况、国籍、地址、地区、菲律宾VoteID的VIN等。
 
         默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for RecognizePhilippinesVoteIDOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesVoteIDOCRRequest`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/ocr/v20181119/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5902,14 +5902,186 @@
             self.AgencyCode._deserialize(params.get("AgencyCode"))
         if params.get("Birthday") is not None:
             self.Birthday = TextDetectionResult()
             self.Birthday._deserialize(params.get("Birthday"))
         self.RequestId = params.get("RequestId")
 
 
+class RecognizePhilippinesSssIDOCRRequest(AbstractModel):
+    """RecognizePhilippinesSssIDOCR请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ReturnHeadImage: 是否返回人像照片。
+        :type ReturnHeadImage: bool
+        :param ImageBase64: 图片的 Base64 值。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+        :type ImageBase64: str
+        :param ImageUrl: 图片的 Url 地址。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
+非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+        :type ImageUrl: str
+        """
+        self.ReturnHeadImage = None
+        self.ImageBase64 = None
+        self.ImageUrl = None
+
+
+    def _deserialize(self, params):
+        self.ReturnHeadImage = params.get("ReturnHeadImage")
+        self.ImageBase64 = params.get("ImageBase64")
+        self.ImageUrl = params.get("ImageUrl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RecognizePhilippinesSssIDOCRResponse(AbstractModel):
+    """RecognizePhilippinesSssIDOCR返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param HeadPortrait: 人像照片Base64后的结果
+        :type HeadPortrait: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param LicenseNumber: 编号
+        :type LicenseNumber: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param FullName: 姓名
+        :type FullName: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Birthday: 生日
+        :type Birthday: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.HeadPortrait = None
+        self.LicenseNumber = None
+        self.FullName = None
+        self.Birthday = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("HeadPortrait") is not None:
+            self.HeadPortrait = TextDetectionResult()
+            self.HeadPortrait._deserialize(params.get("HeadPortrait"))
+        if params.get("LicenseNumber") is not None:
+            self.LicenseNumber = TextDetectionResult()
+            self.LicenseNumber._deserialize(params.get("LicenseNumber"))
+        if params.get("FullName") is not None:
+            self.FullName = TextDetectionResult()
+            self.FullName._deserialize(params.get("FullName"))
+        if params.get("Birthday") is not None:
+            self.Birthday = TextDetectionResult()
+            self.Birthday._deserialize(params.get("Birthday"))
+        self.RequestId = params.get("RequestId")
+
+
+class RecognizePhilippinesTinIDOCRRequest(AbstractModel):
+    """RecognizePhilippinesTinIDOCR请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ReturnHeadImage: 是否返回人像照片。
+        :type ReturnHeadImage: bool
+        :param ImageBase64: 图片的 Base64 值。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+        :type ImageBase64: str
+        :param ImageUrl: 图片的 Url 地址。
+支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
+非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+        :type ImageUrl: str
+        """
+        self.ReturnHeadImage = None
+        self.ImageBase64 = None
+        self.ImageUrl = None
+
+
+    def _deserialize(self, params):
+        self.ReturnHeadImage = params.get("ReturnHeadImage")
+        self.ImageBase64 = params.get("ImageBase64")
+        self.ImageUrl = params.get("ImageUrl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RecognizePhilippinesTinIDOCRResponse(AbstractModel):
+    """RecognizePhilippinesTinIDOCR返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param HeadPortrait: 人像照片Base64后的结果
+        :type HeadPortrait: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param LicenseNumber: 编码
+        :type LicenseNumber: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param FullName: 姓名
+        :type FullName: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Address: 地址
+        :type Address: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Birthday: 生日
+        :type Birthday: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param IssueDate: 发证日期
+        :type IssueDate: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.HeadPortrait = None
+        self.LicenseNumber = None
+        self.FullName = None
+        self.Address = None
+        self.Birthday = None
+        self.IssueDate = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("HeadPortrait") is not None:
+            self.HeadPortrait = TextDetectionResult()
+            self.HeadPortrait._deserialize(params.get("HeadPortrait"))
+        if params.get("LicenseNumber") is not None:
+            self.LicenseNumber = TextDetectionResult()
+            self.LicenseNumber._deserialize(params.get("LicenseNumber"))
+        if params.get("FullName") is not None:
+            self.FullName = TextDetectionResult()
+            self.FullName._deserialize(params.get("FullName"))
+        if params.get("Address") is not None:
+            self.Address = TextDetectionResult()
+            self.Address._deserialize(params.get("Address"))
+        if params.get("Birthday") is not None:
+            self.Birthday = TextDetectionResult()
+            self.Birthday._deserialize(params.get("Birthday"))
+        if params.get("IssueDate") is not None:
+            self.IssueDate = TextDetectionResult()
+            self.IssueDate._deserialize(params.get("IssueDate"))
+        self.RequestId = params.get("RequestId")
+
+
 class RecognizePhilippinesVoteIDOCRRequest(AbstractModel):
     """RecognizePhilippinesVoteIDOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.878/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.877'
+__version__ = '3.0.878'
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.877/setup.py` & `tencentcloud-sdk-python-ocr-3.0.878/setup.py`

 * *Files identical despite different names*

