# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.877.tar", last modified: Wed Apr 19 09:39:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.878.tar", last modified: Thu Apr 20 00:53:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.877.tar` & `tencentcloud-sdk-python-tke-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   177308 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19361 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   640464 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:39:29.000000 tencentcloud-sdk-python-tke-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   177287 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19361 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   641750 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.877/README.rst` & `tencentcloud-sdk-python-tke-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateClusterRelease(self, request):
-        """在应用市场中给集群创建应用
+        """集群创建应用
 
         :param request: Request instance for CreateClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterReleaseRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.CreateClusterReleaseResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.877/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1993,15 +1993,20 @@
         :type SubnetId: str
         :param IsExtranet: 是否为外网访问（TRUE 外网访问 FALSE 内网访问，默认值： FALSE）
         :type IsExtranet: bool
         :param Domain: 设置域名
         :type Domain: str
         :param SecurityGroup: 使用的安全组，只有外网访问需要传递（开启外网访问时必传）
         :type SecurityGroup: str
-        :param ExtensiveParameters: 创建lb参数，只有外网访问需要设置
+        :param ExtensiveParameters: 创建lb参数，只有外网访问需要设置，是一个json格式化后的字符串：{"InternetAccessible":{"InternetChargeType":"TRAFFIC_POSTPAID_BY_HOUR","InternetMaxBandwidthOut":"200"},"VipIsp":"","BandwidthPackageId":""}。
+各个参数意义：
+InternetAccessible.InternetChargeType含义：TRAFFIC_POSTPAID_BY_HOUR按流量按小时后计费;BANDWIDTH_POSTPAID_BY_HOUR 按带宽按小时后计费;InternetAccessible.BANDWIDTH_PACKAGE 按带宽包计费。
+InternetMaxBandwidthOut含义：最大出带宽，单位Mbps，范围支持0到2048，默认值10。
+VipIsp含义：CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
+BandwidthPackageId含义：带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE。
         :type ExtensiveParameters: str
         """
         self.ClusterId = None
         self.SubnetId = None
         self.IsExtranet = None
         self.Domain = None
         self.SecurityGroup = None
@@ -2276,15 +2281,15 @@
         :type Name: str
         :param Namespace: 应用命名空间
         :type Namespace: str
         :param Chart: 制品名称或从第三方repo 安装chart时，制品压缩包下载地址, 不支持重定向类型chart 地址，结尾为*.tgz
         :type Chart: str
         :param Values: 自定义参数
         :type Values: :class:`tencentcloud.tke.v20180525.models.ReleaseValues`
-        :param ChartFrom: 制品来源，范围：tke 应用市场/第三方chart
+        :param ChartFrom: 制品来源，范围：tke-market 或 other
         :type ChartFrom: str
         :param ChartVersion: 制品版本
         :type ChartVersion: str
         :param ChartRepoURL: 制品仓库URL地址
         :type ChartRepoURL: str
         :param Username: 制品访问用户名
         :type Username: str
@@ -18053,15 +18058,15 @@
         :type Name: str
         :param Namespace: 应用命名空间
         :type Namespace: str
         :param Chart: 制品名称或从第三方repo 安装chart时，制品压缩包下载地址, 不支持重定向类型chart 地址，结尾为*.tgz
         :type Chart: str
         :param Values: 自定义参数，覆盖chart 中values.yaml 中的参数
         :type Values: :class:`tencentcloud.tke.v20180525.models.ReleaseValues`
-        :param ChartFrom: 制品来源，范围：tke-market/tcr/other
+        :param ChartFrom: 制品来源，范围：tke-market 或 other
         :type ChartFrom: str
         :param ChartVersion: 制品版本( 从第三安装时，不传这个参数）
         :type ChartVersion: str
         :param ChartRepoURL: 制品仓库URL地址
         :type ChartRepoURL: str
         :param Username: 制品访问用户名
         :type Username: str
@@ -18312,22 +18317,31 @@
 
     def __init__(self):
         r"""
         :param DisplayName: 节点展示名称
         :type DisplayName: str
         :param SubnetId: 子网ID
         :type SubnetId: str
+        :param Tags: 腾讯云标签
+        :type Tags: list of Tag
         """
         self.DisplayName = None
         self.SubnetId = None
+        self.Tags = None
 
 
     def _deserialize(self, params):
         self.DisplayName = params.get("DisplayName")
         self.SubnetId = params.get("SubnetId")
+        if params.get("Tags") is not None:
+            self.Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tke-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.878/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.877/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.877/setup.py` & `tencentcloud-sdk-python-tke-3.0.878/setup.py`

 * *Files identical despite different names*

