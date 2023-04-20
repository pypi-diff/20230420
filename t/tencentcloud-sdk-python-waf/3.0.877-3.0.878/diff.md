# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.877.tar", last modified: Wed Apr 19 09:44:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.878.tar", last modified: Thu Apr 20 00:56:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.877.tar` & `tencentcloud-sdk-python-waf-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    43894 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170365 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:44:55.000000 tencentcloud-sdk-python-waf-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:44:56.000000 tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46564 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177630 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:56:12.000000 tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.877/README.rst` & `tencentcloud-sdk-python-waf-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def AddCustomWhiteRule(self, request):
+        """增加精准白名单规则
+
+        :param request: Request instance for AddCustomWhiteRule.
+        :type request: :class:`tencentcloud.waf.v20180125.models.AddCustomWhiteRuleRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.AddCustomWhiteRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AddCustomWhiteRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.AddCustomWhiteRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def AddDomainWhiteRule(self, request):
         """增加域名规则白名单
 
         :param request: Request instance for AddDomainWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.AddDomainWhiteRuleRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.AddDomainWhiteRuleResponse`
 
@@ -183,14 +206,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteCustomWhiteRule(self, request):
+        """删除精准白名单规则
+
+        :param request: Request instance for DeleteCustomWhiteRule.
+        :type request: :class:`tencentcloud.waf.v20180125.models.DeleteCustomWhiteRuleRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.DeleteCustomWhiteRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteCustomWhiteRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteCustomWhiteRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteDomainWhiteRules(self, request):
         """删除域名规则白名单
 
 
         :param request: Request instance for DeleteDomainWhiteRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteDomainWhiteRulesRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.DeleteDomainWhiteRulesResponse`
@@ -895,14 +941,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyCustomWhiteRule(self, request):
+        """编辑精准白名单
+
+        :param request: Request instance for ModifyCustomWhiteRule.
+        :type request: :class:`tencentcloud.waf.v20180125.models.ModifyCustomWhiteRuleRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.ModifyCustomWhiteRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyCustomWhiteRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyCustomWhiteRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDomainWhiteRule(self, request):
         """更改某一条规则
 
         :param request: Request instance for ModifyDomainWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyDomainWhiteRuleRequest`
```

### Comparing `tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.877/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.878/tencentcloud/waf/v20180125/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,91 @@
         if params.get("Success") is not None:
             self.Success = ResponseCode()
             self.Success._deserialize(params.get("Success"))
         self.RuleId = params.get("RuleId")
         self.RequestId = params.get("RequestId")
 
 
+class AddCustomWhiteRuleRequest(AbstractModel):
+    """AddCustomWhiteRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 规则名称
+        :type Name: str
+        :param SortId: 优先级
+        :type SortId: str
+        :param ExpireTime: 过期时间
+        :type ExpireTime: str
+        :param Strategies: 策略详情
+        :type Strategies: list of Strategy
+        :param Domain: 需要添加策略的域名
+        :type Domain: str
+        :param Bypass: 放行的详情
+        :type Bypass: str
+        """
+        self.Name = None
+        self.SortId = None
+        self.ExpireTime = None
+        self.Strategies = None
+        self.Domain = None
+        self.Bypass = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.SortId = params.get("SortId")
+        self.ExpireTime = params.get("ExpireTime")
+        if params.get("Strategies") is not None:
+            self.Strategies = []
+            for item in params.get("Strategies"):
+                obj = Strategy()
+                obj._deserialize(item)
+                self.Strategies.append(obj)
+        self.Domain = params.get("Domain")
+        self.Bypass = params.get("Bypass")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddCustomWhiteRuleResponse(AbstractModel):
+    """AddCustomWhiteRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Success: 操作的状态码，如果所有的资源操作成功则返回的是成功的状态码，如果有资源操作失败则需要解析Message的内容来查看哪个资源失败
+        :type Success: :class:`tencentcloud.waf.v20180125.models.ResponseCode`
+        :param RuleId: 添加成功的规则ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuleId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Success = None
+        self.RuleId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Success") is not None:
+            self.Success = ResponseCode()
+            self.Success._deserialize(params.get("Success"))
+        self.RuleId = params.get("RuleId")
+        self.RequestId = params.get("RequestId")
+
+
 class AddDomainWhiteRuleRequest(AbstractModel):
     """AddDomainWhiteRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1171,14 +1248,65 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteCustomWhiteRuleRequest(AbstractModel):
+    """DeleteCustomWhiteRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 删除的域名
+        :type Domain: str
+        :param RuleId: 删除的规则ID
+        :type RuleId: int
+        """
+        self.Domain = None
+        self.RuleId = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.RuleId = params.get("RuleId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteCustomWhiteRuleResponse(AbstractModel):
+    """DeleteCustomWhiteRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Success: 操作的状态码，如果所有的资源操作成功则返回的是成功的状态码，如果有资源操作失败则需要解析Message的内容来查看哪个资源失败
+        :type Success: :class:`tencentcloud.waf.v20180125.models.ResponseCode`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Success = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Success") is not None:
+            self.Success = ResponseCode()
+            self.Success._deserialize(params.get("Success"))
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteDomainWhiteRulesRequest(AbstractModel):
     """DeleteDomainWhiteRules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4114,14 +4242,90 @@
     def _deserialize(self, params):
         if params.get("Success") is not None:
             self.Success = ResponseCode()
             self.Success._deserialize(params.get("Success"))
         self.RequestId = params.get("RequestId")
 
 
+class ModifyCustomWhiteRuleRequest(AbstractModel):
+    """ModifyCustomWhiteRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 编辑的域名
+        :type Domain: str
+        :param RuleId: 编辑的规则ID
+        :type RuleId: int
+        :param RuleName: 编辑的规则名称
+        :type RuleName: str
+        :param Bypass: 放行时是否继续执行其它检查逻辑，继续执行地域封禁防护：geoip、继续执行CC策略防护：cc、继续执行WEB应用防护：owasp、继续执行AI引擎防护：ai、继续执行信息防泄漏防护：antileakage。如果多个勾选那么以,串接。
+        :type Bypass: str
+        :param SortId: 优先级，1~100的整数，数字越小，代表这条规则的执行优先级越高。
+        :type SortId: int
+        :param ExpireTime: 规则生效截止时间，0：永久生效，其它值为对应时间的时间戳。
+        :type ExpireTime: int
+        :param Strategies: 匹配条件数组
+        :type Strategies: list of Strategy
+        """
+        self.Domain = None
+        self.RuleId = None
+        self.RuleName = None
+        self.Bypass = None
+        self.SortId = None
+        self.ExpireTime = None
+        self.Strategies = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.RuleId = params.get("RuleId")
+        self.RuleName = params.get("RuleName")
+        self.Bypass = params.get("Bypass")
+        self.SortId = params.get("SortId")
+        self.ExpireTime = params.get("ExpireTime")
+        if params.get("Strategies") is not None:
+            self.Strategies = []
+            for item in params.get("Strategies"):
+                obj = Strategy()
+                obj._deserialize(item)
+                self.Strategies.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyCustomWhiteRuleResponse(AbstractModel):
+    """ModifyCustomWhiteRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Success: 操作的状态码，如果所有的资源操作成功则返回的是成功的状态码，如果有资源操作失败则需要解析Message的内容来查看哪个资源失败
+        :type Success: :class:`tencentcloud.waf.v20180125.models.ResponseCode`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Success = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Success") is not None:
+            self.Success = ResponseCode()
+            self.Success._deserialize(params.get("Success"))
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyDomainWhiteRuleRequest(AbstractModel):
     """ModifyDomainWhiteRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4973,15 +5177,15 @@
         r"""
         :param Domain: 域名
         :type Domain: str
         :param Items: ip 参数列表，json数组由ip，source，note，action，valid_ts组成。ip对应配置的ip地址，source固定为custom值，note为注释，action值42为黑名单，40为白名单，valid_ts为有效日期，值为秒级时间戳（（如1680570420代表2023-04-04 09:07:00））
         :type Items: list of str
         :param Edition: WAF实例类型，sparta-waf表示SAAS型WAF，clb-waf表示负载均衡型WAF
         :type Edition: str
-        :param SourceType: 是否为多域名黑白名单，当为多域名的黑白名单时，取值为batch，佛祖饿为空
+        :param SourceType: 是否为多域名黑白名单，当为多域名的黑白名单时，取值为batch，否则为空
         :type SourceType: str
         """
         self.Domain = None
         self.Items = None
         self.Edition = None
         self.SourceType = None
```

### Comparing `tencentcloud-sdk-python-waf-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.878/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.877/setup.py` & `tencentcloud-sdk-python-waf-3.0.878/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.877/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.878/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

