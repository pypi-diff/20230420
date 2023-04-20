# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.877.tar", last modified: Wed Apr 19 09:16:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.878.tar", last modified: Thu Apr 20 00:28:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.877.tar` & `tencentcloud-sdk-python-ess-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49192 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217979 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:16:40.000000 tencentcloud-sdk-python-ess-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49192 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   218030 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.877/README.rst` & `tencentcloud-sdk-python-ess-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.877/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1979,15 +1979,15 @@
 PASSPORT 护照
 HONGKONG_AND_MACAO 中国香港
 FOREIGN_ID_CARD 境外身份
 HONGKONG_MACAO_AND_TAIWAN 中国台湾
         :type IdCardType: str
         :param Mobile: 手机号码
         :type Mobile: str
-        :param EnableAutoSign: 是否需开通自动签
+        :param EnableAutoSign: 是否开通自动签，该功能需联系运营工作人员开通后使用
         :type EnableAutoSign: bool
         """
         self.UserName = None
         self.IdCardNumber = None
         self.SealImage = None
         self.SealName = None
         self.Operator = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.877/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.877/setup.py` & `tencentcloud-sdk-python-ess-3.0.878/setup.py`

 * *Files identical despite different names*

