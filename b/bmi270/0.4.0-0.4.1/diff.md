# Comparing `tmp/bmi270-0.4.0.tar.gz` & `tmp/bmi270-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmi270-0.4.0.tar", last modified: Tue Apr 18 08:35:16 2023, max compression
+gzip compressed data, was "bmi270-0.4.1.tar", last modified: Thu Apr 20 09:21:00 2023, max compression
```

## Comparing `bmi270-0.4.0.tar` & `bmi270-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-18 08:35:16.082871 bmi270-0.4.0/
--rw-rw-r--   0 somml     (1000) somml     (1000)     1073 2023-03-24 10:40:45.000000 bmi270-0.4.0/LICENSE
--rw-rw-r--   0 somml     (1000) somml     (1000)     2743 2023-04-18 08:35:16.082871 bmi270-0.4.0/PKG-INFO
--rw-rw-r--   0 somml     (1000) somml     (1000)     2009 2023-04-18 08:31:36.000000 bmi270-0.4.0/README.md
--rw-rw-r--   0 somml     (1000) somml     (1000)      887 2023-04-18 08:32:14.000000 bmi270-0.4.0/pyproject.toml
--rw-rw-r--   0 somml     (1000) somml     (1000)       38 2023-04-18 08:35:16.082871 bmi270-0.4.0/setup.cfg
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-18 08:35:16.078871 bmi270-0.4.0/src/
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-18 08:35:16.082871 bmi270-0.4.0/src/bmi270/
--rw-rw-r--   0 somml     (1000) somml     (1000)    19742 2023-04-18 08:25:43.000000 bmi270-0.4.0/src/bmi270/BMI270.py
--rw-rw-r--   0 somml     (1000) somml     (1000)    51029 2023-04-05 14:15:45.000000 bmi270-0.4.0/src/bmi270/config_file.py
--rw-rw-r--   0 somml     (1000) somml     (1000)     2306 2023-04-05 14:15:45.000000 bmi270-0.4.0/src/bmi270/definitions.py
--rw-rw-r--   0 somml     (1000) somml     (1000)      976 2023-04-05 14:16:20.000000 bmi270-0.4.0/src/bmi270/registers.py
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-18 08:35:16.082871 bmi270-0.4.0/src/bmi270.egg-info/
--rw-rw-r--   0 somml     (1000) somml     (1000)     2743 2023-04-18 08:35:16.000000 bmi270-0.4.0/src/bmi270.egg-info/PKG-INFO
--rw-rw-r--   0 somml     (1000) somml     (1000)      298 2023-04-18 08:35:16.000000 bmi270-0.4.0/src/bmi270.egg-info/SOURCES.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)        1 2023-04-18 08:35:16.000000 bmi270-0.4.0/src/bmi270.egg-info/dependency_links.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)       14 2023-04-18 08:35:16.000000 bmi270-0.4.0/src/bmi270.egg-info/requires.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)        7 2023-04-18 08:35:16.000000 bmi270-0.4.0/src/bmi270.egg-info/top_level.txt
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/
+-rw-rw-r--   0 somml     (1000) somml     (1000)     1073 2023-03-24 10:40:45.000000 bmi270-0.4.1/LICENSE
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-20 09:21:00.375079 bmi270-0.4.1/PKG-INFO
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2054 2023-04-20 07:49:16.000000 bmi270-0.4.1/README.md
+-rw-rw-r--   0 somml     (1000) somml     (1000)      887 2023-04-20 07:49:30.000000 bmi270-0.4.1/pyproject.toml
+-rw-rw-r--   0 somml     (1000) somml     (1000)       38 2023-04-20 09:21:00.375079 bmi270-0.4.1/setup.cfg
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/bmi270/
+-rw-rw-r--   0 somml     (1000) somml     (1000)    19603 2023-04-20 09:09:13.000000 bmi270-0.4.1/src/bmi270/BMI270.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)    51029 2023-04-05 14:15:45.000000 bmi270-0.4.1/src/bmi270/config_file.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2306 2023-04-05 14:15:45.000000 bmi270-0.4.1/src/bmi270/definitions.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)     1003 2023-04-20 07:52:26.000000 bmi270-0.4.1/src/bmi270/registers.py
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/bmi270.egg-info/
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/PKG-INFO
+-rw-rw-r--   0 somml     (1000) somml     (1000)      298 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/SOURCES.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)        1 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/dependency_links.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)       14 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/requires.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)        7 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/top_level.txt
```

### Comparing `bmi270-0.4.0/LICENSE` & `bmi270-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.0/PKG-INFO` & `bmi270-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi270
-Version: 0.4.0
+Version: 0.4.1
 Summary: BMI270 I2C Python library (bare bones)
 Author-email: Kevin Sommler <sommler@live.de>
 License: MIT
 Project-URL: Homepage, https://github.com/CoRoLab-Berlin/bmi270_python
 Project-URL: Bug Tracker, https://github.com/CoRoLab-Berlin/bmi270_python/issues
 Keywords: BMI270,I2C,IMU,sensor,driver,accelerometer,gyroscope,gyro,bosch,sensortech,smbus2,library
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BMI270 I2C Python Implementation - Version: 0.4.0
 
-Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University.
+Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
 
 `pip3 install bmi270`
```

### Comparing `bmi270-0.4.0/README.md` & `bmi270-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BMI270 I2C Python Implementation - Version: 0.4.0
 
-Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University.
+Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
 
 `pip3 install bmi270`
```

### Comparing `bmi270-0.4.0/pyproject.toml` & `bmi270-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bmi270"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{name = "Kevin Sommler", email = "sommler@live.de"}]
 description = "BMI270 I2C Python library (bare bones)"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["BMI270", "I2C", "IMU", "sensor", "driver", "accelerometer", "gyroscope", "gyro", "bosch", "sensortech", "smbus2", "library"]
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `bmi270-0.4.0/src/bmi270/BMI270.py` & `bmi270-0.4.1/src/bmi270/BMI270.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,32 +355,30 @@
         gyr_value_z_lsb = self.read_register(GYR_Z_7_0)
         gyr_value_z_msb = self.read_register(GYR_Z_15_8)
         gyr_value_z = (gyr_value_z_msb << 8) | gyr_value_z_lsb
 
         return np.array([gyr_value_x, gyr_value_y, gyr_value_z]).astype(np.int16)
     
     def get_raw_temp_data(self) -> int:
-        temp_value_lsb = self.read_register(TEMPERATURE_0)
-        temp_value_msb = self.read_register(TEMPERATURE_1)
+        temp_value_lsb = self.read_register(TEMP_7_0)
+        temp_value_msb = self.read_register(TEMP_15_8)
         temp_value = (temp_value_msb << 8) | temp_value_lsb
 
         return self.__unsignedToSigned__(temp_value, 2)
     
     def get_acc_data(self) -> np.ndarray:
         raw_acc_data = self.get_raw_acc_data()
-        acceleration = raw_acc_data / 32767 * self.acc_range                        # in m/s²
+        acceleration = raw_acc_data / 32768 * self.acc_range                        # in m/s²
 
         return acceleration
 
     def get_gyr_data(self) -> np.ndarray:
         raw_gyr_data = self.get_raw_gyr_data()
-        angular_velocity = np.deg2rad(1) * raw_gyr_data / 32767 * self.gyr_range    # in rad/s
+        angular_velocity = np.deg2rad(1) * raw_gyr_data / 32768 * self.gyr_range    # in rad/s
 
         return angular_velocity
     
     def get_temp_data(self) -> float:
         raw_data = self.get_raw_temp_data()
         temp_celsius = raw_data * 0.001952594 + 23.0
-        drift_correction = temp_celsius * 0.02 / 100.0
-        corrected_temp_celsius = temp_celsius + drift_correction
         
-        return corrected_temp_celsius
+        return temp_celsius
```

### Comparing `bmi270-0.4.0/src/bmi270/config_file.py` & `bmi270-0.4.1/src/bmi270/config_file.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.0/src/bmi270/definitions.py` & `bmi270-0.4.1/src/bmi270/definitions.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.0/src/bmi270/registers.py` & `bmi270-0.4.1/src/bmi270/registers.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 DATA_REG        = 0x0C
 FIFO_CONFIG_0   = 0x48
 FIFO_CONFIG_1   = 0x49
 INIT_CTRL       = 0x59
 INIT_ADDR_0     = 0x5B
 INIT_ADDR_1     = 0x5C
 INIT_DATA       = 0x5E
+CMD             = 0x7E
 PWR_CONF        = 0x7C
 PWR_CTRL        = 0x7D
 
 # Accelerometer
 ACC_CONF        = 0x40
 ACC_RANGE       = 0x41
 ACC_X_7_0       = 0x0C
@@ -40,9 +41,9 @@
 GYR_X_15_8      = 0x13
 GYR_Y_7_0       = 0x14
 GYR_Y_15_8      = 0x15
 GYR_Z_7_0       = 0x16
 GYR_Z_15_8      = 0x17
 
 # Temperature
-TEMPERATURE_0 = 0x22
-TEMPERATURE_1 = 0x23
+TEMP_7_0        = 0x22
+TEMP_15_8       = 0x23
```

### Comparing `bmi270-0.4.0/src/bmi270.egg-info/PKG-INFO` & `bmi270-0.4.1/src/bmi270.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi270
-Version: 0.4.0
+Version: 0.4.1
 Summary: BMI270 I2C Python library (bare bones)
 Author-email: Kevin Sommler <sommler@live.de>
 License: MIT
 Project-URL: Homepage, https://github.com/CoRoLab-Berlin/bmi270_python
 Project-URL: Bug Tracker, https://github.com/CoRoLab-Berlin/bmi270_python/issues
 Keywords: BMI270,I2C,IMU,sensor,driver,accelerometer,gyroscope,gyro,bosch,sensortech,smbus2,library
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BMI270 I2C Python Implementation - Version: 0.4.0
 
-Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University.
+Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
 
 `pip3 install bmi270`
```

