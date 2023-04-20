# Comparing `tmp/irobot_edu_sdk-0.2.0.tar.gz` & `tmp/irobot_edu_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irobot_edu_sdk-0.2.0.tar", max compression
+gzip compressed data, was "irobot_edu_sdk-0.3.0.tar", max compression
```

## Comparing `irobot_edu_sdk-0.2.0.tar` & `irobot_edu_sdk-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1471 2022-12-12 15:08:38.797628 irobot_edu_sdk-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     5632 2022-12-12 17:20:23.557046 irobot_edu_sdk-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/__init__.py
--rw-r--r--   0        0        0      769 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/backend.py
--rw-r--r--   0        0        0      310 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/bluetooth.py
--rw-r--r--   0        0        0     2983 2022-12-14 15:41:51.583554 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/bluetooth_desktop.py
--rw-r--r--   0        0        0     3799 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/bluetooth_web.py
--rw-r--r--   0        0        0     1425 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/serial.py
--rw-r--r--   0        0        0     1312 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/usb.py
--rw-r--r--   0        0        0      539 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/color.py
--rw-r--r--   0        0        0      939 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/completer.py
--rw-r--r--   0        0        0     6628 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/create3.py
--rw-r--r--   0        0        0     1463 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/event.py
--rw-r--r--   0        0        0     2070 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/getter_types.py
--rw-r--r--   0        0        0     1932 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/music.py
--rw-r--r--   0        0        0     2083 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/packet.py
--rw-r--r--   0        0        0    22356 2023-02-01 02:47:49.949018 irobot_edu_sdk-0.2.0/irobot_edu_sdk/robot.py
--rw-r--r--   0        0        0      366 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/robots.py
--rw-r--r--   0        0        0     5444 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/root.py
--rw-r--r--   0        0        0      579 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.2.0/irobot_edu_sdk/utils.py
--rw-r--r--   0        0        0      703 2023-02-01 02:47:49.949018 irobot_edu_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6459 2023-02-01 02:48:06.675704 irobot_edu_sdk-0.2.0/setup.py
--rw-r--r--   0        0        0     6407 2023-02-01 02:48:06.676268 irobot_edu_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1471 2022-12-12 15:08:38.797628 irobot_edu_sdk-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     5632 2022-12-12 17:20:23.557046 irobot_edu_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/__init__.py
+-rw-r--r--   0        0        0      769 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/backend.py
+-rw-r--r--   0        0        0      310 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/bluetooth.py
+-rw-r--r--   0        0        0     2983 2022-12-14 15:41:51.583554 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/bluetooth_desktop.py
+-rw-r--r--   0        0        0     3799 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/bluetooth_web.py
+-rw-r--r--   0        0        0     1425 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/serial.py
+-rw-r--r--   0        0        0     1312 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/usb.py
+-rw-r--r--   0        0        0      539 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/color.py
+-rw-r--r--   0        0        0      939 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/completer.py
+-rw-r--r--   0        0        0     7114 2023-04-20 20:32:56.799893 irobot_edu_sdk-0.3.0/irobot_edu_sdk/create3.py
+-rw-r--r--   0        0        0     1463 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/event.py
+-rw-r--r--   0        0        0     2070 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/getter_types.py
+-rw-r--r--   0        0        0     1932 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/music.py
+-rw-r--r--   0        0        0     2083 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/packet.py
+-rw-r--r--   0        0        0    22364 2023-04-20 20:32:56.799893 irobot_edu_sdk-0.3.0/irobot_edu_sdk/robot.py
+-rw-r--r--   0        0        0      366 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/robots.py
+-rw-r--r--   0        0        0     6581 2023-04-20 20:32:56.803893 irobot_edu_sdk-0.3.0/irobot_edu_sdk/root.py
+-rw-r--r--   0        0        0      579 2022-12-12 15:08:38.801628 irobot_edu_sdk-0.3.0/irobot_edu_sdk/utils.py
+-rw-r--r--   0        0        0      703 2023-04-20 20:32:56.803893 irobot_edu_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6459 2023-04-20 20:35:10.227320 irobot_edu_sdk-0.3.0/setup.py
+-rw-r--r--   0        0        0     6407 2023-04-20 20:35:10.227685 irobot_edu_sdk-0.3.0/PKG-INFO
```

### Comparing `irobot_edu_sdk-0.2.0/LICENSE.txt` & `irobot_edu_sdk-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/README.md` & `irobot_edu_sdk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/backend.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/backend.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/bluetooth_desktop.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/bluetooth_desktop.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/bluetooth_web.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/bluetooth_web.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/serial.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/serial.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/backend/usb.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/backend/usb.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/color.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/color.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/completer.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/completer.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/create3.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/create3.py`

 * *Files 7% similar despite different names*

```diff
@@ -156,7 +156,23 @@
         await self._backend.write_packet(Packet(dev, cmd, inc))
         packet = await completer.wait(self.DEFAULT_TIMEOUT)
         if packet:
             unpacked = unpack('>IBBBBHHHH', packet.payload)
             return {'timestamp': unpacked[0], 'contacts': unpacked[1], 'IR sensor 0': unpacked[2],
                     'IR sensor 1': unpacked[3], 'IR sensor 2': unpacked[4]}
         return None
+
+    async def get_version_string(self) -> str:
+        """Get version as a human-readable string."""
+        ver = await self.get_versions(0xA5)
+        try:
+            major = ver[1]
+            minor = ver[2]
+            patch = ver[9]
+            if major < 32 or major > 126:
+                major = str(major)
+            else:
+                major = chr(major)
+
+            return '.'.join([major, str(ver[2]), str(ver[9])])
+        except IndexError:
+            return None;
```

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/event.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/event.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/getter_types.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/getter_types.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/music.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/music.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/packet.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/packet.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/robot.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,21 +314,21 @@
         await self._backend.write_packet(Packet(5, 1, self.inc))
         self.sound_enabled = False
 
     async def wait(self, time: Union[int, float]):
         await asyncio.sleep(time)
 
     async def get_versions(self, board: int) -> List[int]:
-        """Get version numbers. Returns [board, fw maj, fw min, hw maj, hw min, boot maj, boot min, proto maj, proto min]."""
+        """Get version numbers. Returns [board, fw maj, fw min, hw maj, hw min, boot maj, boot min, proto maj, proto min, patch]."""
         dev, cmd, inc = 0, 0, self.inc
         completer = Completer()
         self._responses[(dev, cmd, inc)] = completer
         await self._backend.write_packet(Packet(dev, cmd, inc, bytes([board])))
         packet = await completer.wait(self.DEFAULT_TIMEOUT)
-        return packet.payload[: 9] if packet else []
+        return packet.payload[: 10] if packet else []
 
     async def set_name(self, name: str):
         """Set robot name."""
         utf = name.encode('utf-8')
         while len(utf) > Packet.PAYLOAD_LEN:
             name = name[: -1]
             utf = name.encode('utf-8')
```

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/root.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/root.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Licensed under 3-Clause BSD license available in the License file. Copyright (c) 2020-2022 iRobot Corporation. All rights reserved.
+# Licensed under 3-Clause BSD license available in the License file. Copyright (c) 2020-2023 iRobot Corporation. All rights reserved.
 #
 
 import math
 from typing import Union, Callable, Awaitable, List
 from struct import pack, unpack
 from .backend.backend import Backend
 from .event import Event
@@ -20,18 +20,18 @@
     # Marker/eraser.
     MARKER_UP = 0
     MARKER_DOWN = 1
     MARKER_ERASE = 2
 
     # Light sensor.
     LIGHT_UNKNOWN = 0
-    LIGHT_DARK = 4
+    LIGHT_DARKER = 4
     LIGHT_RIGHT_BRIGHTER_THAN_LEFT = 5
     LIGHT_LEFT_BRIGHTER_THAN_RIGHT = 6
-    LIGHT_BRIGHT = 7
+    LIGHT_BRIGHTER = 7
 
     # Gravity compensation.
     GRAVITY_OFF = 0
     GRAVITY_ON = 1
     GRAVITY_WHEN_MARKER = 2
 
     # Color sensor.
@@ -74,22 +74,22 @@
 
     async def _when_color_scanned_handler(self, packet: Packet):
         for event in self._when_color_scanned:
             self.color_sensor.colors = [c >> i & 0xF for c in packet.payload for i in range(4, -1, -4)]
             # TODO: Add trigger.
             await event.run(self)
 
-    # TODO: Test.
     async def _when_light_seen_handler(self, packet: Packet):
         for event in self._when_light_seen:
             self.light_sensors.state = packet.payload[4]
             self.light_sensors.left = unpack(">H", packet.payload[5:7])[0]
             self.light_sensors.right = unpack(">H", packet.payload[7:9])[0]
-            # TODO: Add trigger
-            await event.run(self)
+            if len(event.condition) == 1:
+                if event.condition[0] == self.light_sensors.state:
+                    await event.run(self)
 
     # Event Callbacks.
 
     def when_color_scanned(self, condition: list[List[int]], callback: Callable[[ColorSensor], Awaitable[None]]):
         """Register when color callback of type async def fn(colors:
         List[Color])"""
         self._when_color_scanned.append(Event(condition, callback))
@@ -149,7 +149,34 @@
         pointing towards the direction of the line between the destination and the origin points."""
         movement = self.compute_movement_to(x, y)
         await self.turn_left(Movement.minimize_angle(movement.angle))
         await self.move(movement.distance)
         if heading is not None:
             # TODO: test.
             await self.turn_left(Movement.minimize_angle(heading - self.heading))
+
+    async def get_version_string(self) -> str:
+        """Get version as a human-readable string."""
+        main = await self.get_versions(0xA5)
+        color = await self.get_versions(0xC6)
+        try:
+            return f'Main: {str(main[1])}.{str(main[2])}\tColor: {str(color[1])}.{str(color[2])}'
+        except IndexError:
+            try:
+                return f'Main: {str(main[1])}.{str(main[2])}'
+            except IndexError:
+                return None;
+
+    async def get_light_values(self):
+        """Get instantaneous ambient light sensor values"""
+        dev, cmd, inc = 13, 1, self.inc
+        completer = Completer()
+        self._responses[(dev, cmd, inc)] = completer
+        await self._backend.write_packet(Packet(dev, cmd, inc))
+
+        packet = await completer.wait(self.DEFAULT_TIMEOUT)
+        if packet:
+            payload = packet.payload
+            timestamp = unpack('>I', payload[0:4])[0]
+            (l, r) = unpack('>HH', payload[4:8])
+            return (l / 1000, r / 1000) # normalize between 0 and 1
+        return None
```

### Comparing `irobot_edu_sdk-0.2.0/irobot_edu_sdk/utils.py` & `irobot_edu_sdk-0.3.0/irobot_edu_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `irobot_edu_sdk-0.2.0/pyproject.toml` & `irobot_edu_sdk-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "irobot_edu_sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python SDK for iRobot Edu robots"
 authors = ["iRobot Corporation <education@irobot.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://python.irobot.com"
 repository = "https://github.com/iRobotEducation/irobot-edu-python-sdk"
 packages = [
```

### Comparing `irobot_edu_sdk-0.2.0/setup.py` & `irobot_edu_sdk-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['bleak>=0.19.0,<0.20.0', 'pyserial>=3.4,<4.0']
 
 setup_kwargs = {
     'name': 'irobot-edu-sdk',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Python SDK for iRobot Edu robots',
     'long_description': "# iRobot® Education Python® SDK\n\nThis is an installable Python SDK for the iRobot Education robots.\nIt supports the iRobot® Root® rt0, Root® rt1 and Create® 3 educational robots.\n\nThis SDK uses a similar format as Learning Level 3 of the iRobot® Coding App ([code.irobot.com](https://code.irobot.com)) and the iRobot® Python Web Playground ([python.irobot.com](https://python.irobot.com)).\nAs such, it uses async execution and is compatible with Python® 3.9 or greater. MicroPython may work, but it is not tested.\n\nThis SDK is designed to communicate with robots via Bluetooth® Low Energy on Windows®, macOS®, and Linux® systems.\nExperimental backends are provided for communicating over USB serial and USB on MicroPython boards with native USB ports.\nThese are not currently supported.\n\n## Disclaimer: this is a BETA release.\nThe BETA version of the iRobot® Python SDK is provided “as is” to conduct testing and gather user feedback. There is no guarantee on its performance or compatibility, continued availability, or on a timeline for improvements.\n\nPlease do file [issues](https://github.com/iRobotEducation/irobot-edu-python-sdk/issues) as they are found, so that the team (or the community) can address them.\n\n\n## Installation using pip\n\n```\npip3 install irobot_edu_sdk\n```\n\n\n## Optional: Installation from Source\n\n```\ngit clone https://github.com/iRobotEducation/irobot-edu-python-sdk.git\n```\n\nFrom the newly cloned SDK's directory, run:\n\n```\npip3 install .\n```\n\n\n## Usage\n\nA robot object is created from one of the communication backends.\nThis robot object has a number of event callbacks that can be registered and commands that can be sent to the robot.\nAfter a program is setup, the `play()` method will start execution and block until the robot's nose or power button is pressed, the robot is disconnected, or `Ctrl-C` is pressed.\n\n\n## Examples\n\nA good way of getting started is by looking at the examples provided [here](https://github.com/iRobotEducation/irobot-edu-python-sdk/tree/main/examples).\n\nThese examples mirror the iRobot Education [Python Web Playground](http://python.irobot.com).\n\n## Backend\n\n### Bluetooth\n\niRobot Education's robots communicate using a common Bluetooth Low Energy serial protocol, the details of which can be found [here](https://github.com/iRobotEducation/root-robot-ble-protocol).\n\n```python\nfrom irobot_edu_sdk.backend.bluetooth import Bluetooth\n\n# Connect to robot over Bluetooth Low Energy.\nbackend0 = Bluetooth('') # Connects to the first BLE robot detected.\nbackend1 = Bluetooth('ROOT') # Use robot named 'ROOT'\n```\n\n## ALPHA features\n**The features detailed below are included as ALPHA versions, which provide limited functionality and are likely to contain several known or unknown bugs.**\n**Support is not provided for ALPHA features at this time.**\n\n### Serial\n\nSome Root® robots support a serial port over USB.\n\n```python\nfrom irobot_edu_sdk.backend.serial import Serial\n\n# Connect to robot over USB-C cable.\nbackend = Serial('COM1')                          # Windows\nbackend = Serial('/dev/cu.usbmodemRT0123F456789') # macOS\nbackend = Serial('/dev/ttyACM0')                  # Linux\n```\n\n### MicroPython\n\nThis SDK requires MicroPython firmware that includes the `uasyncio` library -- version 1.13 or greater.\nDownload the latest release for your board from http://micropython.org/download.\nThen, copy the `irobot_edu_sdk` directory and all contents to the `PYBFLASH` drive.\n\n```python\nfrom irobot_edu_sdk.backend.usb import USB\n\n# Connect to robot from MicroPython-compatible board over USB.\nbackend = USB() # MicroPython-compatible board is powered from USB-C port\n```\n\nNOTE: You may need to use a USB-C to USB-A adapter or a USB-C to micro USB cable.\n\n**© 2022 iRobot Corporation. All rights reserved.**\n* [Terms and Conditions](https://about.irobot.com/en-us/legal/terms-and-conditions)\n* [Privacy Policy](https://edu.irobot.com/privacy-policy)\n\n## Attributions\n* Python® 3 is governed by and a trademark of the Python Software Foundation.\n* The Bluetooth® word mark and logos are registered trademarks owned by Bluetooth SIG, Inc. and any use of such marks by iRobot is under license.\n* Windows® is a trademark of Microsoft Corporation, registered in the U.S. and other countries and regions.\n* macOS® is a trademark of Apple Inc., registered in the U.S. and other countries and regions.\n* Linux® is a trademark of Linus Torvalds, registered in the U.S. and other countries and regions.\n* USB-C™ is a trademark of USB Implementers Forum.\n* All other trademarks mentioned are the property of their respective owners.\n\n\nThis library is made possible thanks to other community software.\nThe following are direct required dependencies:\n* [Bleak](https://github.com/hbldh/bleak), licensed under the MIT license, available [here](https://github.com/hbldh/bleak/blob/develop/LICENSE)\n* [pySerial](https://github.com/pyserial/pyserial/), licensed under the BSD 3-Clause license, available [here](https://github.com/pyserial/pyserial/blob/master/LICENSE.txt)\n* [Root Robot Python Web App](https://github.com/mogenson/root-robot-python-web-app), licensed under the MIT license, available [here](https://github.com/mogenson/root-robot-python-web-app/blob/main/LICENSE)\n\nTo build, the following is recommended:\n* [Poetry](https://github.com/python-poetry/poetry), licensed under the MIT license, available [here](https://github.com/python-poetry/poetry/blob/master/LICENSE)\n\nThe iRobot Education Python SDK provided is licensed under the 3-Clause BSD license, found [here](https://github.com/iRobotEducation/irobot-edu-python-sdk/tree/main/LICENSE.txt)\n",
     'author': 'iRobot Corporation',
     'author_email': 'education@irobot.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://python.irobot.com',
```

### Comparing `irobot_edu_sdk-0.2.0/PKG-INFO` & `irobot_edu_sdk-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irobot-edu-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python SDK for iRobot Edu robots
 Home-page: https://python.irobot.com
 License: BSD-3-Clause
 Author: iRobot Corporation
 Author-email: education@irobot.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

