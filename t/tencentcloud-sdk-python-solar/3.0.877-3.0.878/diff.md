# Comparing `tmp/tencentcloud-sdk-python-solar-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-solar-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.877.tar", last modified: Wed Apr 19 09:32:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.878.tar", last modified: Thu Apr 20 00:41:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-solar-3.0.877.tar` & `tencentcloud-sdk-python-solar-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/
--rw-r--r--   0 root         (0) root         (0)    15814 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/solar_client.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53600 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:32:20.000000 tencentcloud-sdk-python-solar-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/
+-rw-r--r--   0 root         (0) root         (0)    15814 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/solar_client.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53600 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:41:38.000000 tencentcloud-sdk-python-solar-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-solar-3.0.877/README.rst` & `tencentcloud-sdk-python-solar-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/solar_client.py` & `tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/solar_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/errorcodes.py` & `tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.877/tencentcloud/solar/v20181011/models.py` & `tencentcloud-sdk-python-solar-3.0.878/tencentcloud/solar/v20181011/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-solar-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-solar-3.0.877/tencentcloud_sdk_python_solar.egg-info/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.878/tencentcloud_sdk_python_solar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.877/setup.py` & `tencentcloud-sdk-python-solar-3.0.878/setup.py`

 * *Files identical despite different names*
