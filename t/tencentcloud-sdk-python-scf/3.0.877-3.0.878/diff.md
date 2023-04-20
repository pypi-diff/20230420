# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.877.tar", last modified: Wed Apr 19 09:27:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.878.tar", last modified: Thu Apr 20 00:40:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.877.tar` & `tencentcloud-sdk-python-scf-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42711 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190551 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:27:12.000000 tencentcloud-sdk-python-scf-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:27:13.000000 tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190870 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:40:44.000000 tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.877/README.rst` & `tencentcloud-sdk-python-scf-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.877/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.878/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2705,32 +2705,37 @@
         :type LicenseInfo: str
         :param LayerVersion: 版本号
         :type LayerVersion: int
         :param LayerName: 层名称
         :type LayerName: str
         :param Status: 层的具体版本当前状态，状态值[参考此处](https://cloud.tencent.com/document/product/583/47175#.E5.B1.82.EF.BC.88layer.EF.BC.89.E7.8A.B6.E6.80.81)
         :type Status: str
+        :param Stamp: Stamp
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Stamp: str
         """
         self.CompatibleRuntimes = None
         self.AddTime = None
         self.Description = None
         self.LicenseInfo = None
         self.LayerVersion = None
         self.LayerName = None
         self.Status = None
+        self.Stamp = None
 
 
     def _deserialize(self, params):
         self.CompatibleRuntimes = params.get("CompatibleRuntimes")
         self.AddTime = params.get("AddTime")
         self.Description = params.get("Description")
         self.LicenseInfo = params.get("LicenseInfo")
         self.LayerVersion = params.get("LayerVersion")
         self.LayerName = params.get("LayerName")
         self.Status = params.get("Status")
+        self.Stamp = params.get("Stamp")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4112,15 +4117,15 @@
         :type MemUsage: int
         :param Duration: 表示执行函数的耗时，单位是毫秒，异步调用返回为空
         :type Duration: float
         :param BillDuration: 表示函数的计费耗时，单位是毫秒，异步调用返回为空
         :type BillDuration: int
         :param FunctionRequestId: 此次函数执行的Id
         :type FunctionRequestId: str
-        :param InvokeResult: 0为正确，异步调用返回为空
+        :param InvokeResult: 请求 Invoke 接口，该参数已弃用。请求 InvokeFunction 接口，该参数值为请求执行[状态码](https://cloud.tencent.com/document/product/583/42611)。
         :type InvokeResult: int
         """
         self.Log = None
         self.RetMsg = None
         self.ErrMsg = None
         self.MemUsage = None
         self.Duration = None
```

### Comparing `tencentcloud-sdk-python-scf-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.877/setup.py` & `tencentcloud-sdk-python-scf-3.0.878/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.877/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.878/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

