# Comparing `tmp/voip-utils-0.0.2.tar.gz` & `tmp/voip-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voip-utils-0.0.2.tar", last modified: Mon Apr 10 20:29:30 2023, max compression
+gzip compressed data, was "voip-utils-0.0.3.tar", last modified: Thu Apr 20 17:22:34 2023, max compression
```

## Comparing `voip-utils-0.0.2.tar` & `voip-utils-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:30.002290 voip-utils-0.0.2/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.2/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-10 20:29:30.002290 voip-utils-0.0.2/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.2/README.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-10 20:29:17.000000 voip-utils-0.0.2/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-10 20:29:30.002290 voip-utils-0.0.2/setup.cfg
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:29.998290 voip-utils-0.0.2/voip_utils/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.2/voip_utils/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.2/voip_utils/error.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7678 2023-04-06 20:24:07.000000 voip-utils-0.0.2/voip_utils/rtp_audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-06 19:25:34.000000 voip-utils-0.0.2/voip_utils/sip.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.2/voip_utils/util.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5246 2023-04-06 19:28:21.000000 voip-utils-0.0.2/voip_utils/voip.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-10 20:29:30.002290 voip-utils-0.0.2/voip_utils.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-10 20:29:29.000000 voip-utils-0.0.2/voip_utils.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.2/voip_utils.egg-info/zip-safe
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.3/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 17:22:34.288439 voip-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.3/README.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-20 16:15:30.000000 voip-utils-0.0.3/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-20 17:22:34.288439 voip-utils-0.0.3/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/voip_utils/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.3/voip_utils/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.3/voip_utils/error.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7678 2023-04-06 20:24:07.000000 voip-utils-0.0.3/voip_utils/rtp_audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-20 17:19:08.000000 voip-utils-0.0.3/voip_utils/sip.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.3/voip_utils/util.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5583 2023-04-20 17:21:30.000000 voip-utils-0.0.3/voip_utils/voip.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/voip_utils.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 17:22:33.000000 voip-utils-0.0.3/voip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.3/voip_utils.egg-info/zip-safe
```

### Comparing `voip-utils-0.0.2/LICENSE.md` & `voip-utils-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.2/PKG-INFO` & `voip-utils-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `voip-utils-0.0.2/pyproject.toml` & `voip-utils-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "voip-utils"
-version     = "0.0.2"
+version     = "0.0.3"
 license     = {text = "Apache-2.0"}
 description = "Voice over IP Utilities"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "voip", "phone"]
```

### Comparing `voip-utils-0.0.2/voip_utils/rtp_audio.py` & `voip-utils-0.0.3/voip_utils/rtp_audio.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.2/voip_utils/sip.py` & `voip-utils-0.0.3/voip_utils/sip.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.2/voip_utils/voip.py` & `voip-utils-0.0.3/voip_utils/voip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 """Voice over IP (VoIP) implementation."""
 import asyncio
 import logging
 import socket
 from abc import ABC, abstractmethod
 from functools import partial
-from typing import Any, Callable, Set
+from typing import Any, Callable, Optional, Set
 
 from .rtp_audio import RtpOpusInput, RtpOpusOutput
 from .sip import CallInfo, SdpInfo, SipDatagramProtocol
 
 _LOGGER = logging.getLogger(__name__)
 
 CallProtocolFactory = Callable[[CallInfo], asyncio.Protocol]
 
 
 class VoipDatagramProtocol(SipDatagramProtocol):
     """UDP server for Voice over IP (VoIP)."""
 
     def __init__(
-        self, sdp_info: SdpInfo, protocol_factory: CallProtocolFactory
+        self,
+        sdp_info: SdpInfo,
+        valid_protocol_factory: CallProtocolFactory,
+        invalid_protocol_factory: Optional[CallProtocolFactory] = None,
     ) -> None:
         """Set up VoIP call handler."""
         super().__init__(sdp_info)
-        self.protocol_factory = protocol_factory
+        self.valid_protocol_factory = valid_protocol_factory
+        self.invalid_protocol_factory = invalid_protocol_factory
         self._tasks: Set[asyncio.Future[Any]] = set()
 
     def is_valid_call(self, call_info: CallInfo) -> bool:
         """Filter calls."""
         return True
 
     def on_call(self, call_info: CallInfo):
         """Answer incoming calls and start RTP server on a random port."""
-        if not self.is_valid_call(call_info):
-            _LOGGER.warning("Call rejected: %s", call_info)
+        protocol_factory = (
+            self.valid_protocol_factory
+            if self.is_valid_call(call_info)
+            else self.invalid_protocol_factory
+        )
+        if protocol_factory is None:
+            _LOGGER.debug("Call rejected: %s", call_info)
             return
 
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         sock.setblocking(False)
 
         # Bind to a random UDP port
         sock.bind((call_info.server_ip, 0))
@@ -47,15 +56,15 @@
             rtp_port,
         )
 
         # Handle RTP packets in RTP server
         loop = asyncio.get_running_loop()
         task = asyncio.create_task(
             loop.create_datagram_endpoint(
-                partial(self.protocol_factory, call_info),
+                partial(protocol_factory, call_info),
                 (rtp_ip, rtp_port),
             )
         )
         self._tasks.add(task)
         task.add_done_callback(self._tasks.remove)
 
         # Tell caller to start sending/receiving RTP audio
@@ -110,15 +119,15 @@
     async def send_audio(
         self,
         audio_bytes: bytes,
         rate: int,
         width: int,
         channels: int,
         addr: Any = None,
-        sleep_ratio: float = 0.99,
+        sleep_ratio: float = 0.98,
         silence_before: float = 0.0,
     ) -> None:
         """Send audio from WAV file in chunks over RTP."""
         if self.transport is None:
             raise ValueError("Transport not set")
 
         addr = addr or self.addr
```

### Comparing `voip-utils-0.0.2/voip_utils.egg-info/PKG-INFO` & `voip-utils-0.0.3/voip_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

