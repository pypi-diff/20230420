# Comparing `tmp/pasqal-cloud-0.0.2.tar.gz` & `tmp/pasqal-cloud-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.0.2.tar", last modified: Thu Apr 20 07:55:15 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.2.tar", last modified: Thu Apr 20 08:55:03 2023, max compression
```

## Comparing `pasqal-cloud-0.0.2.tar` & `pasqal-cloud-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.724752 pasqal-cloud-0.0.2/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.724752 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-20 07:55:15.000000 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 07:55:15.000000 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:55:15.000000 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 07:55:15.000000 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 07:55:15.000000 pasqal-cloud-0.0.2/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.728752 pasqal-cloud-0.0.2/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:15.732752 pasqal-cloud-0.0.2/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-20 07:55:04.000000 pasqal-cloud-0.0.2/tests/test_doubles/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.732367 pasqal-cloud-0.2.2/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.732367 pasqal-cloud-0.2.2/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.732367 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-20 08:55:03.000000 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 08:55:03.000000 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:55:03.000000 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 08:55:03.000000 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 08:55:03.000000 pasqal-cloud-0.2.2/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:55:03.736367 pasqal-cloud-0.2.2/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-20 08:54:50.000000 pasqal-cloud-0.2.2/tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.0.2/LICENSE` & `pasqal-cloud-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/PKG-INFO` & `pasqal-cloud-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.0.2
+Version: 0.2.2
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.0.2/README.md` & `pasqal-cloud-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.2/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.2/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.2"
+__version__ = "0.2.2"
```

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.2/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.2/pasqal_cloud/batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/client.py` & `pasqal-cloud-0.2.2/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.2/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.2.2/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.2/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/job.py` & `pasqal-cloud-0.2.2/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.2/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.2/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.0.2
+Version: 0.2.2
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.0.2/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.2/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/sdk/setup.py` & `pasqal-cloud-0.2.2/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/setup.py` & `pasqal-cloud-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/conftest.py` & `pasqal-cloud-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_batch.py` & `pasqal-cloud-0.2.2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_client.py` & `pasqal-cloud-0.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.2/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_config.py` & `pasqal-cloud-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_device_specs.py` & `pasqal-cloud-0.2.2/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.0.2/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.2/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

