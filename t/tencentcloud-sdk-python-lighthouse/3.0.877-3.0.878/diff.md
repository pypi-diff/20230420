# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.877.tar", last modified: Wed Apr 19 09:20:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.878.tar", last modified: Thu Apr 20 00:36:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.877.tar` & `tencentcloud-sdk-python-lighthouse-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    23217 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88751 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230506 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:20:37.000000 tencentcloud-sdk-python-lighthouse-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    23217 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    88751 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230902 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:36:25.000000 tencentcloud-sdk-python-lighthouse-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,24 +642,33 @@
         r"""
         :param BlueprintName: 镜像名称。最大长度60。
         :type BlueprintName: str
         :param Description: 镜像描述。最大长度60。
         :type Description: str
         :param InstanceId: 需要制作镜像的实例ID。
         :type InstanceId: str
+        :param ForcePowerOff: 是否执行强制关机以制作镜像。
+取值范围：
+True：表示关机之后制作镜像
+False：表示开机状态制作镜像
+默认取值：True
+开机状态制作镜像，可能导致部分数据未备份，影响数据安全。
+        :type ForcePowerOff: bool
         """
         self.BlueprintName = None
         self.Description = None
         self.InstanceId = None
+        self.ForcePowerOff = None
 
 
     def _deserialize(self, params):
         self.BlueprintName = params.get("BlueprintName")
         self.Description = params.get("Description")
         self.InstanceId = params.get("InstanceId")
+        self.ForcePowerOff = params.get("ForcePowerOff")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5477,15 +5486,15 @@
 class ModifyInstancesBundleRequest(AbstractModel):
     """ModifyInstancesBundle请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceIds: 实例ID列表。一个或多个待操作的实例ID。可通过[DescribeInstances](https://cloud.tencent.com/document/api/1207/47573)接口返回值中的InstanceId获取。每次请求批量实例的上限为30。
+        :param InstanceIds: 实例ID列表。一个或多个待操作的实例ID。可通过[DescribeInstances](https://cloud.tencent.com/document/api/1207/47573)接口返回值中的InstanceId获取。每次请求批量实例的上限为15。
         :type InstanceIds: list of str
         :param BundleId: 待变更的套餐Id。可通过[DescribeBundles](https://cloud.tencent.com/document/api/1207/47575)接口返回值中的BundleId获取。
         :type BundleId: str
         :param AutoVoucher: 是否自动抵扣代金券。取值范围：
 true：表示自动抵扣代金券
 false：表示不自动抵扣代金券
 默认取值：false。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.878/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.877/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.878/setup.py`

 * *Files identical despite different names*

