# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.878.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.877.tar", last modified: Wed Apr 19 09:40:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.878.tar", last modified: Thu Apr 20 00:54:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.877.tar` & `tencentcloud-sdk-python-trtc-3.0.878.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198930 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58128 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 09:40:20.000000 tencentcloud-sdk-python-trtc-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:40:21.000000 tencentcloud-sdk-python-trtc-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198924 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58202 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:54:48.000000 tencentcloud-sdk-python-trtc-3.0.878/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/README.rst` & `tencentcloud-sdk-python-trtc-3.0.878/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         :type RoomId: str
         :param UserId: 录制机器人用于进入TRTC房间拉流的[UserId](https://cloud.tencent.com/document/product/647/46351#userid)，注意这个UserId不能与其他TRTC房间内的主播或者其他录制任务等已经使用的UserId重复，建议可以把房间ID作为userId的标识的一部分，即录制机器人进入房间的userid应保证独立且唯一。
         :type UserId: str
         :param UserSig: 录制机器人用于进入TRTC房间拉流的用户签名，当前 UserId 对应的验证签名，相当于登录密码，具体计算方法请参考TRTC计算[UserSig](https://cloud.tencent.com/document/product/647/45910#UserSig)的方案。
         :type UserSig: str
         :param RecordParams: 云端录制控制参数。
         :type RecordParams: :class:`tencentcloud.trtc.v20190722.models.RecordParams`
-        :param StorageParams: 云端录制文件上传到云存储的参数(目前只支持使用腾讯云点播作为存储)。
+        :param StorageParams: 云端录制文件上传到云存储的参数(目前支持云点播VOD和对象存储COS)。
         :type StorageParams: :class:`tencentcloud.trtc.v20190722.models.StorageParams`
         :param RoomIdType: TRTC房间号的类型，必须和录制的房间所对应的RoomId类型相同:
 0: 字符串类型的RoomId
 1: 32位整型的RoomId（默认）
         :type RoomIdType: int
         :param MixTranscodeParams: 混流的转码参数，录制模式为混流的时候可以设置。
         :type MixTranscodeParams: :class:`tencentcloud.trtc.v20190722.models.MixTranscodeParams`
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
     def CreateCloudRecording(self, request):
         """接口说明：
         启动云端录制功能，完成房间内的音视频录制，并上传到指定的云存储。您可以通过此 API 接口把TRTC 房间中的每一路音视频流做单独的录制有或者多路视频画面混流一路。
 
         您可以通过此接口实现如下目标：
         * 指定订阅流参数（RecordParams）来指定需要录制的主播的黑名单或者白名单。
-        * 指定第三方存储的参数（StorageParams）来指定上传到您希望的云存储，目前仅支持云点播存储（CloudVod）
+        * 指定第三方存储的参数（StorageParams）来指定上传到您希望的云存储，目前支持云点播VOD和对象存储COS
         * 指定混流模式下的音视频转码详细参数（MixTranscodeParams），包括视频分辨率、视频码率、视频帧率、以及声音质量等
         * 指定混流模式各路画面的位置和布局或者也可以指定自动模板的方式来配置。
 
         关键名词：
-        * 单流录制：分别录制房间的订阅UserId的音频和视频。录制服务会实时将录制文件上传至云点播存储。
-        * 合流录制：将房间内订阅UserId的音视频混录成一个音视频文件，并将录制文件上传至云点播存储（录制结束后可前往云点播控制台查看录制文件：https://console.cloud.tencent.com/vod/media）。
+        * 单流录制：分别录制房间的订阅UserId的音频和视频，录制服务会实时将录制文件上传至您指定的云存储。
+        * 合流录制：将房间内订阅UserId的音视频混录成一个视频文件，并将录制文件上传至您指定的云存储。（录制结束后可前往云点播控制台https://console.cloud.tencent.com/vod/media 或 对象存储COS控制台https://console.cloud.tencent.com/cos/bucket查看文件）。
 
         :param request: Request instance for CreateCloudRecording.
         :type request: :class:`tencentcloud.trtc.v20190722.models.CreateCloudRecordingRequest`
         :rtype: :class:`tencentcloud.trtc.v20190722.models.CreateCloudRecordingResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.878/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.878/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.878/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.877
+Version: 3.0.878
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.877/setup.py` & `tencentcloud-sdk-python-trtc-3.0.878/setup.py`

 * *Files identical despite different names*

