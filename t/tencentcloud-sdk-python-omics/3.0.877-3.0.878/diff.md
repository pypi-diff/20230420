# Comparing `tmp/tencentcloud-sdk-python-omics-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-omics-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.877.tar", last modified: Wed Apr 19 09:25:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.878.tar", last modified: Thu Apr 20 00:38:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-omics-3.0.877.tar` & `tencentcloud-sdk-python-omics-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)     6111 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29142 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 09:25:38.000000 tencentcloud-sdk-python-omics-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:25:39.000000 tencentcloud-sdk-python-omics-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29142 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:38:55.000000 tencentcloud-sdk-python-omics-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-omics-3.0.877/README.rst` & `tencentcloud-sdk-python-omics-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.877/tencentcloud_sdk_python_omics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.878/tencentcloud_sdk_python_omics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/omics_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.877/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-omics-3.0.878/tencentcloud/omics/v20221128/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-omics-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-omics-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.878/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.877/setup.py` & `tencentcloud-sdk-python-omics-3.0.878/setup.py`

 * *Files identical despite different names*

