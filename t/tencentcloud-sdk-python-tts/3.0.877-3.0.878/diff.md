# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.877.tar", last modified: Wed Apr 19 09:40:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.878.tar", last modified: Thu Apr 20 00:55:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.877.tar` & `tencentcloud-sdk-python-tts-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)     5481 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18535 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:40:52.000000 tencentcloud-sdk-python-tts-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19249 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tts-3.0.877/README.rst` & `tencentcloud-sdk-python-tts-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -297,27 +297,33 @@
         :type SampleRate: int
         :param Codec: 返回音频格式，可取值：wav（默认），mp3，pcm
         :type Codec: str
         :param EnableSubtitle: 是否开启时间戳功能，默认为false。
         :type EnableSubtitle: bool
         :param SegmentRate: 断句敏感阈值，默认值为：0，取值范围：[0,1,2]。该值越大越不容易断句，模型会更倾向于仅按照标点符号断句。此参数建议不要随意调整，可能会影响合成效果。
         :type SegmentRate: int
+        :param EmotionCategory: 控制合成音频的情感，仅支持情绪音色使用。取值: peaceful、exciting、thrill、neutral、sad、angry、cute、fear、poetry、happy、regretful、exciting_strong、aojiao、sajiao、story、raido、call、jieshuo等等；
+        :type EmotionCategory: str
+        :param EmotionIntensity: 控制合成音频情感程度，取值范围为[50,200],默认为100，不填写为默认值；只有EmotionCategory不为空时生效；
+        :type EmotionIntensity: int
         """
         self.Text = None
         self.SessionId = None
         self.Volume = None
         self.Speed = None
         self.ProjectId = None
         self.ModelType = None
         self.VoiceType = None
         self.PrimaryLanguage = None
         self.SampleRate = None
         self.Codec = None
         self.EnableSubtitle = None
         self.SegmentRate = None
+        self.EmotionCategory = None
+        self.EmotionIntensity = None
 
 
     def _deserialize(self, params):
         self.Text = params.get("Text")
         self.SessionId = params.get("SessionId")
         self.Volume = params.get("Volume")
         self.Speed = params.get("Speed")
@@ -325,14 +331,16 @@
         self.ModelType = params.get("ModelType")
         self.VoiceType = params.get("VoiceType")
         self.PrimaryLanguage = params.get("PrimaryLanguage")
         self.SampleRate = params.get("SampleRate")
         self.Codec = params.get("Codec")
         self.EnableSubtitle = params.get("EnableSubtitle")
         self.SegmentRate = params.get("SegmentRate")
+        self.EmotionCategory = params.get("EmotionCategory")
+        self.EmotionIntensity = params.get("EmotionIntensity")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tts-3.0.877/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.877/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.877/setup.py` & `tencentcloud-sdk-python-tts-3.0.878/setup.py`

 * *Files identical despite different names*

