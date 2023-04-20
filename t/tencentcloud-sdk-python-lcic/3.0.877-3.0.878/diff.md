# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.877.tar", last modified: Wed Apr 19 09:20:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.878.tar", last modified: Thu Apr 20 00:36:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.877.tar` & `tencentcloud-sdk-python-lcic-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135371 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    46709 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 09:20:29.000000 tencentcloud-sdk-python-lcic-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:20:30.000000 tencentcloud-sdk-python-lcic-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135371 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    46709 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/README.rst` & `tencentcloud-sdk-python-lcic-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
 class AnswerInfo(AbstractModel):
-    """房间问答问题详情
+    """房间问答答案详情
 
     """
 
     def __init__(self):
         r"""
         :param Name: 用户名
         :type Name: str
@@ -3563,15 +3563,15 @@
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
 class QuestionInfo(AbstractModel):
-    """房间问答答案详情
+    """房间问答问题详情
 
     """
 
     def __init__(self):
         r"""
         :param QuestionId: 问题ID
         :type QuestionId: str
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.877/setup.py` & `tencentcloud-sdk-python-lcic-3.0.878/setup.py`

 * *Files identical despite different names*

