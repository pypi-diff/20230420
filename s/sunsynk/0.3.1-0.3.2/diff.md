# Comparing `tmp/sunsynk-0.3.1.tar.gz` & `tmp/sunsynk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.1.tar", last modified: Sun Mar 19 08:32:16 2023, max compression
+gzip compressed data, was "sunsynk-0.3.2.tar", last modified: Thu Apr 20 20:06:59 2023, max compression
```

## Comparing `sunsynk-0.3.1.tar` & `sunsynk-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.631889 sunsynk-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-19 08:32:05.000000 sunsynk-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-19 08:32:05.000000 sunsynk-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-03-19 08:32:16.631889 sunsynk-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-03-19 08:32:05.000000 sunsynk-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-19 08:32:16.631889 sunsynk-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-19 08:32:05.000000 sunsynk-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.623889 sunsynk-0.3.1/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12513 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6273 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-19 08:32:05.000000 sunsynk-0.3.1/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.627889 sunsynk-0.3.1/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 08:32:16.000000 sunsynk-0.3.1/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.627889 sunsynk-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk-dev.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.627889 sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/test_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:16.631889 sunsynk-0.3.1/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-03-19 08:32:05.000000 sunsynk-0.3.1/tests/sunsynk/test_sunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.554793 sunsynk-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 20:06:50.000000 sunsynk-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 20:06:50.000000 sunsynk-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 20:06:59.554793 sunsynk-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-20 20:06:50.000000 sunsynk-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-20 20:06:59.554793 sunsynk-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 20:06:50.000000 sunsynk-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12513 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6273 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-dev.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.554793 sunsynk-0.3.2/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_sunsynk.py
```

### Comparing `sunsynk-0.3.1/LICENSE` & `sunsynk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/setup.cfg` & `sunsynk-0.3.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 [metadata]
 name = sunsynk
 version = attr: sunsynk.VERSION
-description = Library to interface Sunsynk Hybrid Inverters
+description = Library to interface Deye/Sunsynk Hybrid Inverters
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/kellerza/sunsynk
+url = https://kellerza.github.io/sunsynk/
 author = Johann Kellerman
 author_email = kellerza@gmail.com
 license = MIT
 license_file = LICENSE
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 keywords = sunsynk, deye, inverter, modbus, asyncio
 
 [options]
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.9
 include_package_data = True
-tests_requires = file: requirements_test.txt
 install_requires = 
 	attrs>21
 zip_safe = true
 
 [options.extras_require]
 umodbus = 
 	async_modbus==0.2.1
 	umodbus==1.0.4
 	connio==0.2.0
 pymodbus = 
-	pymodbus==2.5.3
-	pyserial-asyncio
+	pymodbus[serial]==3.2.2
+tests = 
+	pytest
+	pytest-asyncio
+	pytest-cov
+	pytest-github-actions-annotate-failures
+	types-PyYAML
+	pylint
+	paho-mqtt~=1.5.0
+	pyyaml~=5.4.1
+	mqtt-entity
 
 [isort]
 profile = black
 
 [flake8]
 extend-ignore = E203, E501, W503
```

### Comparing `sunsynk-0.3.1/sunsynk/definitions.py` & `sunsynk-0.3.2/sunsynk/definitions.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/definitions3ph.py` & `sunsynk-0.3.2/sunsynk/definitions3ph.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/helpers.py` & `sunsynk-0.3.2/sunsynk/helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/pysunsynk.py` & `sunsynk-0.3.2/sunsynk/pysunsynk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,109 +1,107 @@
 """Sunsync Modbus interface."""
 import asyncio
 import logging
 from typing import Sequence
 from urllib.parse import urlparse
 
 import attr
-from pymodbus.client.asynchronous.async_io import (  # type: ignore
-    AsyncioModbusSerialClient,
-    AsyncioModbusTcpClient,
-    ModbusClientProtocol,
+from pymodbus import version
+from pymodbus.client import (
+    AsyncModbusSerialClient,
+    AsyncModbusTcpClient,
+    ModbusBaseClient,
 )
 
-# from pymodbus.client.asynchronous import schedulers  # type: ignore
-from pymodbus.client.asynchronous.serial import AsyncModbusSerialClient  # type: ignore
-from serial.serialutil import STOPBITS_ONE
-
-from sunsynk.sunsynk import Sunsynk  # type: ignore
+from sunsynk.sunsynk import Sunsynk
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @attr.define
 class pySunsynk(Sunsynk):  # pylint: disable=invalid-name
     """Sunsync Modbus class."""
 
     port: str = attr.ib(default="/dev/tty0")
-    client: ModbusClientProtocol = attr.ib(default=None)
+    client: ModbusBaseClient = attr.ib(default=None)
 
     async def connect(self) -> None:
         """Connect.
 
         https://pymodbus.readthedocs.io/en/latest/source/example/async_asyncio_serial_client.html
 
         """
-        # pylint: disable=protected-access
-        url = urlparse(f"//{self.port}")
-        client = None
+        if self.client and self.client.async_connected:
+            return
+        url = urlparse(f"{self.port}")
 
         if not url.netloc:
             # Cannot run from a coroutine currently
             # https://github.com/riptideio/pymodbus/pull/658/files#r718775308
+            _LOGGER.debug("Port: %s pymodbus %s", self.port, version.short())
+
+            self.client = AsyncModbusSerialClient(
+                port=self.port,
+                baudrate=self.baudrate,
+                # method="rtu",
+                stopbits=1,
+                bytesize=8,
+            )
+            # _loop, client = msc  # pylint: disable=unpacking-non-sequence
 
-            # msc = AsyncModbusSerialClient(
-            #     schedulers.ASYNC_IO,
+            # Alternative interim...
+            # client = AsyncioModbusSerialClient(
             #     port=self.port,
+            #     protocol_class=ModbusClientProtocol,
+            #     framer=AsyncModbusSerialClient._framer(method="rtu"),
+            #     loop=asyncio.get_running_loop(),
             #     baudrate=self.baudrate,
-            #     method="rtu",
             #     stopbits=STOPBITS_ONE,
             #     bytesize=8,
             # )
-            # loop, client = msc  # pylint: disable=unpacking-non-sequence
-
-            # Alternative interim...
-            client = AsyncioModbusSerialClient(
-                port=self.port,
-                protocol_class=ModbusClientProtocol,
-                framer=AsyncModbusSerialClient._framer(method="rtu"),
-                loop=asyncio.get_running_loop(),
-                baudrate=self.baudrate,
-                stopbits=STOPBITS_ONE,
-                bytesize=8,
-            )
         else:
-            client = AsyncioModbusTcpClient(
+            _LOGGER.debug(
+                "Host: %s : %s pymodbus %s", url.hostname, url.port, version.short()
+            )
+            self.client = AsyncModbusTcpClient(
                 host=url.hostname,
                 port=url.port or 502,
-                protocol_class=ModbusClientProtocol,
-                loop=asyncio.get_running_loop(),
+                # protocol_class=ModbusClientProtocol,
+                # loop=asyncio.get_running_loop(),
             )
 
-        await client.connect()
+        await self.client.connect()
 
-        if (hasattr(client, "connected") and not client.connected) or (
-            hasattr(client, "_connected") and not client._connected
-        ):
+        if not self.client.async_connected:
             raise ConnectionError
 
-        try:
-            client.protocol._timeout = self.timeout
-        except AttributeError as err:
-            _LOGGER.warning("%s", err)
+        # try:
+        #     client.protocol._timeout = self.timeout
+        # except AttributeError as err:
+        #     _LOGGER.warning("%s", err)
 
-        self.client = client.protocol
+        # self.client = client. .protocol
 
     async def write_register(self, *, address: int, value: int) -> bool:
         """Write to a register - Sunsynk supports modbus function 0x10."""
         try:
             w_r = await self.client.write_registers(
-                address=address, values=(value,), unit=self.server_id
+                address=address, values=(value,), slave=self.server_id
             )
             if w_r.function_code < 0x80:  # test that we are not an error
                 return True
             _LOGGER.error("failed to write register %s=%s", address, value)
         except asyncio.TimeoutError:
             _LOGGER.error("timeout writing register %s=%s", address, value)
         self.timeouts += 1
         return False
 
     async def read_holding_registers(self, start: int, length: int) -> Sequence[int]:
         """Read a holding register."""
         res = await self.client.read_holding_registers(
-            start, length, unit=self.server_id
+            address=start, count=length, slave=self.server_id
         )
         if res.function_code >= 0x80:  # test that we are not an error
             raise Exception(  # pylint: disable=broad-exception-raised
                 f"failed to read register {start} - function code: {res.function_code}"
             )
         return res.registers
```

### Comparing `sunsynk-0.3.1/sunsynk/rwsensors.py` & `sunsynk-0.3.2/sunsynk/rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/sensors.py` & `sunsynk-0.3.2/sunsynk/sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/state.py` & `sunsynk-0.3.2/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/sunsynk.py` & `sunsynk-0.3.2/sunsynk/sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk/usunsynk.py` & `sunsynk-0.3.2/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.3.2/sunsynk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/hass-addon-sunsynk-dev.zip
 tests/hass-addon-sunsynk.zip
 tests/hass-addon-sunsynk-multi/__init__.py
 tests/hass-addon-sunsynk-multi/test_filter.py
-tests/hass-addon-sunsynk-multi/test_mqtt.py
 tests/hass-addon-sunsynk-multi/test_run.py
 tests/sunsynk/__init__.py
 tests/sunsynk/conftest.py
 tests/sunsynk/test_helpers.py
 tests/sunsynk/test_register.py
 tests/sunsynk/test_rwsensors.py
 tests/sunsynk/test_sensors.py
```

### Comparing `sunsynk-0.3.1/tests/conftest.py` & `sunsynk-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.2/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/test_filter.py` & `sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/hass-addon-sunsynk-multi/test_run.py` & `sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_run.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.2/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.2/tests/sunsynk/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/sunsynk/test_register.py` & `sunsynk-0.3.2/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.2/tests/sunsynk/test_rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.2/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.1/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.2/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

