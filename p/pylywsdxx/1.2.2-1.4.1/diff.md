# Comparing `tmp/pylywsdxx-1.2.2.tar.gz` & `tmp/pylywsdxx-1.4.1.tar.gz`

## Comparing `pylywsdxx-1.2.2.tar` & `pylywsdxx-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/.editorconfig
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/BUILDING.md
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/build
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/tox.ini
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/.github/dependabot.yml
--rwxr-xr-x   0        0        0     1228 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/examples/pylywsd02.py
--rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/examples/pylywsd03mmc.py
--rwxr-xr-x   0        0        0     1083 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/examples/pylywsd03mmc2csv.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/src/pylywsdxx/__init__.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/src/pylywsdxx/client.py
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/LICENSE
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/README.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 pylywsdxx-1.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/.editorconfig
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/BUILDING.md
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/build
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/tox.ini
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1228 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/examples/pylywsd02.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/examples/pylywsd03mmc.py
+-rwxr-xr-x   0        0        0     1083 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/examples/pylywsd03mmc2csv.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/src/pylywsdxx/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/src/pylywsdxx/bt_hardware.py
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/src/pylywsdxx/client.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/README.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 pylywsdxx-1.4.1/PKG-INFO
```

### Comparing `pylywsdxx-1.2.2/BUILDING.md` & `pylywsdxx-1.4.1/BUILDING.md`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/build` & `pylywsdxx-1.4.1/build`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/tox.ini` & `pylywsdxx-1.4.1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is used to override pycodestyle settings
 [pycodestyle]
-max-line-length=120
+max-line-length=96
 ignore=E402,W503
 
 [pydocstyle]
 convention = google
 
 [pylama]
 format = pylint
@@ -17,14 +17,14 @@
 [pylama:pyflakes]
 builtins = _
 
 [pylama:pydocstyle]
 convention = google
 
 [pylama:pycodestyle]
-max_line_length = 120
+max_line_length = 96
 ignore=E203,E402,W503
 
 [pylama:pylint]
-max_line_length = 120
+max_line_length = 96
 rcfile = .pylintrc
 disable = C0103,C0114,C0116,E0401,E1136,R0913,R0914,R0915,W0105,W0703,W1203
```

### Comparing `pylywsdxx-1.2.2/.github/dependabot.yml` & `pylywsdxx-1.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/examples/pylywsd02.py` & `pylywsdxx-1.4.1/examples/pylywsd02.py`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/examples/pylywsd03mmc.py` & `pylywsdxx-1.4.1/examples/pylywsd03mmc.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
         print(f"Fetching data from {mac}")
         data = client.data
         print(f"Temperature: {data.temperature}°C")
         print(f"Humidity: {data.humidity}%")
         print(f"Battery: {data.battery}% ({data.voltage} V)")
         print()
     except (Exception,) as e:
+        print(f"An exception of type {type(e).__name__} occured")
         print(e)
```

### Comparing `pylywsdxx-1.2.2/examples/pylywsd03mmc2csv.py` & `pylywsdxx-1.4.1/examples/pylywsd03mmc2csv.py`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/src/pylywsdxx/client.py` & `pylywsdxx-1.4.1/src/pylywsdxx/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 UUID_TIME = "EBE0CCB7-7A0A-4B0C-8A1A-6FF2997DA3A6"  # _        5 or 4 bytes          READ WRITE
 UUID_DATA = "EBE0CCC1-7A0A-4B0C-8A1A-6FF2997DA3A6"  # _        3 bytes               READ NOTIFY
 UUID_BATTERY = "EBE0CCC4-7A0A-4B0C-8A1A-6FF2997DA3A6"  # _     1 byte                READ
 UUID_NUM_RECORDS = "EBE0CCB9-7A0A-4B0C-8A1A-6FF2997DA3A6"  # _ 8 bytes               READ
 UUID_RECORD_IDX = "EBE0CCBA-7A0A-4B0C-8A1A-6FF2997DA3A6"  # _  4 bytes               READ WRITE
 
 
-class SensorData(collections.namedtuple("SensorDataBase", ["temperature", "humidity", "battery", "voltage"])):
+class SensorData(
+    collections.namedtuple("SensorDataBase", ["temperature", "humidity", "battery", "voltage"])
+):
     """Class to store sensor data..
     For LYWSD03MMC devices also battery information is available.
     """
 
     __slots__ = ()
 
 
@@ -56,17 +58,22 @@
     @contextlib.contextmanager
     def connect(self):
         """Handle device connecting and disconnecting"""
         if self._context_depth == 0:
             if self.debug:
                 print(f"|-> Connecting to {self._mac}")
             self._peripheral.connect(addr=self._mac, timeout=self._notification_timeout)
+            # TO DO: consider to catch connection errors here
+            # kimnaty.kimnaty[1372]: *** While talking to room 1.1 (A4:C1:38:6F:E7:CA) an error occured on 2023-04-15 18:20:35
+            # kimnaty.kimnaty[1372]:      -btle- Timed out while trying to connect to peripheral A4:C1:38:6F:E7:CA, addr type: public, interface None, >
         self._context_depth += 1
         try:
             yield self
+        except Exception as her:
+            print(f"(pylywsdxx.client) An exception of type {type(her).__name__} occured")
         finally:
             self._context_depth -= 1
             if self._context_depth == 0:
                 if self.debug:
                     print(f"|-< Disconnecting from {self._mac}")
                 self._peripheral.disconnect()
 
@@ -165,15 +172,17 @@
         return self._history_data
 
     def _get_sensor_data(self):
         with self.connect():
             self._subscribe(UUID_DATA, self._process_sensor_data)
 
             if not self._peripheral.waitForNotifications(self._notification_timeout):
-                raise TimeoutError(f"No data from device for {self._notification_timeout} seconds")
+                raise TimeoutError(
+                    f"No data from device for {self._notification_timeout} seconds"
+                )
 
     def _get_history_data(self):
         with self.connect():
             self._subscribe(UUID_HISTORY, self._process_history_data)
 
             while True:
                 if not self._peripheral.waitForNotifications(self._notification_timeout):
@@ -193,15 +202,17 @@
         desc = ch.getDescriptors(forUUID=0x2902)[0]
 
         desc.write(0x01.to_bytes(2, byteorder="little"), withResponse=True)
 
     def _process_sensor_data(self, data):
         temperature, humidity = struct.unpack_from("hB", data)
         temperature /= 100
-        self._data = SensorData(temperature=temperature, humidity=humidity, battery=None, voltage=None)
+        self._data = SensorData(
+            temperature=temperature, humidity=humidity, battery=None, voltage=None
+        )
 
     def _process_history_data(self, data):
         (idx, ts, max_temp, max_hum, min_temp, min_hum) = struct.unpack_from("<IIhBhB", data)
 
         ts = datetime.fromtimestamp(ts)
         min_temp /= 100
         max_temp /= 100
@@ -242,15 +253,17 @@
         CR2025 / CR2032 maximum theoretical voltage = 3.4 V
         ref. Table 1;
          CR2025: https://www.farnell.com/datasheets/1496883.pdf
          CR2032: https://www.farnell.com/datasheets/1496885.pdf
         Lowest voltage for these batteries is 2.0 V but the BT radio
         on most devices will stop working when below 2.3 V (YMMV).
         """
-        self._data = SensorData(temperature=temperature, humidity=humidity, battery=battery, voltage=voltage)
+        self._data = SensorData(
+            temperature=temperature, humidity=humidity, battery=battery, voltage=voltage
+        )
 
     @property
     def battery(self):
         """
         Battery data comes along with the temperature and humidity data, so just get it from there.
 
         Returns:
@@ -305,15 +318,17 @@
         This is done by taking the current time, subtracting the time
         taken from the device (the run time), and adding the timezone offset.
 
         Returns:
             datetime: the start time of the device
         """
         if not self._start_time:
-            start_time_delta = self.time[0] - datetime(1970, 1, 1) - timedelta(hours=self.tz_offset)
+            start_time_delta = (
+                self.time[0] - datetime(1970, 1, 1) - timedelta(hours=self.tz_offset)
+            )
             self._start_time = datetime.now() - start_time_delta
         return self._start_time
 
     @property
     def time(self):
         """Fetch datetime and timezone of a LYWSD03MMC device
         Returns:
```

### Comparing `pylywsdxx-1.2.2/.gitignore` & `pylywsdxx-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/LICENSE` & `pylywsdxx-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/README.md` & `pylywsdxx-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pylywsdxx-1.2.2/pyproject.toml` & `pylywsdxx-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pylywsdxx"
 description = "A Python3 class to interrogate Xiaomi Mijia LYWSD* sensors."
-version = "1.2.2"
+version = "1.4.1"
 dependencies = [
     "bluepy3",
 ]
 license = "MIT"
 authors = [
   { name="Mausy5043" },
 ]
```

### Comparing `pylywsdxx-1.2.2/PKG-INFO` & `pylywsdxx-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylywsdxx
-Version: 1.2.2
+Version: 1.4.1
 Summary: A Python3 class to interrogate Xiaomi Mijia LYWSD* sensors.
 Project-URL: Homepage, https://github.com/Mausy5043/pylywsdxx
 Project-URL: Bug Tracker, https://github.com/Mausy5043/pylywsdxx/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

