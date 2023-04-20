# Comparing `tmp/python-dbusmock-0.9.1.tar.gz` & `tmp/python-dbusmock-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-dbusmock-0.9.1.tar", last modified: Tue Dec 10 10:14:12 2013, max compression
+gzip compressed data, was "dist/python-dbusmock-0.9.2.tar", last modified: Fri Dec 13 06:12:46 2013, max compression
```

## Comparing `python-dbusmock-0.9.1.tar` & `python-dbusmock-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/dbusmock/
--rw-rw-r--   0 martin    (1000) martin    (1000)    25232 2013-11-28 09:11:07.000000 python-dbusmock-0.9.1/dbusmock/mockobject.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2013-12-10 10:14:11.000000 python-dbusmock-0.9.1/dbusmock/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9274 2013-11-27 18:02:52.000000 python-dbusmock-0.9.1/dbusmock/testcase.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3973 2013-11-27 18:02:52.000000 python-dbusmock-0.9.1/dbusmock/__main__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/dbusmock/templates/
--rw-rw-r--   0 martin    (1000) martin    (1000)    15851 2013-11-29 13:00:48.000000 python-dbusmock-0.9.1/dbusmock/templates/bluez5.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10866 2013-11-29 13:00:48.000000 python-dbusmock-0.9.1/dbusmock/templates/bluez5-obex.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10474 2013-11-28 08:18:11.000000 python-dbusmock-0.9.1/dbusmock/templates/logind.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2089 2013-02-03 20:29:03.000000 python-dbusmock-0.9.1/dbusmock/templates/polkitd.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9944 2013-11-08 05:35:21.000000 python-dbusmock-0.9.1/dbusmock/templates/upower.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      382 2012-11-08 08:25:13.000000 python-dbusmock-0.9.1/dbusmock/templates/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1250 2013-03-05 15:56:24.000000 python-dbusmock-0.9.1/dbusmock/templates/gnome_screensaver.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11416 2013-07-30 08:54:38.000000 python-dbusmock-0.9.1/dbusmock/templates/networkmanager.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2013-06-13 09:54:37.000000 python-dbusmock-0.9.1/dbusmock/templates/notification_daemon.py
--rwxr-xr-x   0 martin    (1000) martin    (1000)     1503 2013-12-10 10:11:34.000000 python-dbusmock-0.9.1/setup.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       59 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/python_dbusmock.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)      846 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/python_dbusmock.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/python_dbusmock.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/python_dbusmock.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)    15073 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/python_dbusmock.egg-info/PKG-INFO
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2295 2013-01-21 07:15:23.000000 python-dbusmock-0.9.1/tests/test_gnome_screensaver.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2685 2013-02-03 20:31:44.000000 python-dbusmock-0.9.1/tests/test_polkitd.py
--rw-r--r--   0 martin    (1000) martin    (1000)    11194 2013-11-11 08:28:05.000000 python-dbusmock-0.9.1/tests/test_upower.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4223 2013-06-13 09:57:31.000000 python-dbusmock-0.9.1/tests/test_notification_daemon.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6454 2013-07-30 08:52:56.000000 python-dbusmock-0.9.1/tests/test_networkmanager.py
--rw-r--r--   0 martin    (1000) martin    (1000)    29674 2013-11-28 09:04:14.000000 python-dbusmock-0.9.1/tests/test_api.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3726 2013-03-20 12:52:03.000000 python-dbusmock-0.9.1/tests/test_logind.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1588 2012-11-08 08:05:07.000000 python-dbusmock-0.9.1/tests/test_code.py
--rw-r--r--   0 martin    (1000) martin    (1000)     4241 2013-11-27 17:41:10.000000 python-dbusmock-0.9.1/tests/test_cli.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11469 2013-11-29 13:12:20.000000 python-dbusmock-0.9.1/tests/test_bluez.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3967 2012-11-08 11:36:42.000000 python-dbusmock-0.9.1/tests/test_consolekit.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    15073 2013-12-10 10:14:12.000000 python-dbusmock-0.9.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     7651 2012-10-01 13:35:04.000000 python-dbusmock-0.9.1/COPYING
--rw-rw-r--   0 martin    (1000) martin    (1000)       49 2012-11-02 21:07:22.000000 python-dbusmock-0.9.1/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)    11716 2013-03-20 10:13:39.000000 python-dbusmock-0.9.1/README.rst
--rw-rw-r--   0 martin    (1000) martin    (1000)     9477 2013-12-10 10:14:11.000000 python-dbusmock-0.9.1/NEWS
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/dbusmock/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25232 2013-11-28 09:11:07.000000 python-dbusmock-0.9.2/dbusmock/mockobject.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      855 2013-12-13 06:12:45.000000 python-dbusmock-0.9.2/dbusmock/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9274 2013-11-27 18:02:52.000000 python-dbusmock-0.9.2/dbusmock/testcase.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3973 2013-11-27 18:02:52.000000 python-dbusmock-0.9.2/dbusmock/__main__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/dbusmock/templates/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    15851 2013-11-29 13:00:48.000000 python-dbusmock-0.9.2/dbusmock/templates/bluez5.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10866 2013-11-29 13:00:48.000000 python-dbusmock-0.9.2/dbusmock/templates/bluez5-obex.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10474 2013-11-28 08:18:11.000000 python-dbusmock-0.9.2/dbusmock/templates/logind.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2089 2013-02-03 20:29:03.000000 python-dbusmock-0.9.2/dbusmock/templates/polkitd.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10124 2013-12-12 07:52:21.000000 python-dbusmock-0.9.2/dbusmock/templates/upower.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      382 2012-11-08 08:25:13.000000 python-dbusmock-0.9.2/dbusmock/templates/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1250 2013-03-05 15:56:24.000000 python-dbusmock-0.9.2/dbusmock/templates/gnome_screensaver.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11416 2013-07-30 08:54:38.000000 python-dbusmock-0.9.2/dbusmock/templates/networkmanager.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2013-06-13 09:54:37.000000 python-dbusmock-0.9.2/dbusmock/templates/notification_daemon.py
+-rwxr-xr-x   0 martin    (1000) martin    (1000)     1503 2013-12-10 10:11:34.000000 python-dbusmock-0.9.2/setup.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       59 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/python_dbusmock.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      846 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/python_dbusmock.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2013-12-13 06:12:45.000000 python-dbusmock-0.9.2/python_dbusmock.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2013-12-13 06:12:45.000000 python-dbusmock-0.9.2/python_dbusmock.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)    15073 2013-12-13 06:12:45.000000 python-dbusmock-0.9.2/python_dbusmock.egg-info/PKG-INFO
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2295 2013-01-21 07:15:23.000000 python-dbusmock-0.9.2/tests/test_gnome_screensaver.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2685 2013-02-03 20:31:44.000000 python-dbusmock-0.9.2/tests/test_polkitd.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    11968 2013-12-12 07:57:04.000000 python-dbusmock-0.9.2/tests/test_upower.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4223 2013-06-13 09:57:31.000000 python-dbusmock-0.9.2/tests/test_notification_daemon.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6454 2013-07-30 08:52:56.000000 python-dbusmock-0.9.2/tests/test_networkmanager.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    29866 2013-12-12 08:13:49.000000 python-dbusmock-0.9.2/tests/test_api.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3726 2013-03-20 12:52:03.000000 python-dbusmock-0.9.2/tests/test_logind.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1588 2012-11-08 08:05:07.000000 python-dbusmock-0.9.2/tests/test_code.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4361 2013-12-12 08:09:50.000000 python-dbusmock-0.9.2/tests/test_cli.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11469 2013-11-29 13:12:20.000000 python-dbusmock-0.9.2/tests/test_bluez.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3967 2012-11-08 11:36:42.000000 python-dbusmock-0.9.2/tests/test_consolekit.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    15073 2013-12-13 06:12:46.000000 python-dbusmock-0.9.2/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     7651 2012-10-01 13:35:04.000000 python-dbusmock-0.9.2/COPYING
+-rw-rw-r--   0 martin    (1000) martin    (1000)       49 2012-11-02 21:07:22.000000 python-dbusmock-0.9.2/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11716 2013-03-20 10:13:39.000000 python-dbusmock-0.9.2/README.rst
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9658 2013-12-13 06:12:45.000000 python-dbusmock-0.9.2/NEWS
```

### Comparing `python-dbusmock-0.9.1/dbusmock/mockobject.py` & `python-dbusmock-0.9.2/dbusmock/mockobject.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/__init__.py` & `python-dbusmock-0.9.2/dbusmock/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # later version.  See http://www.gnu.org/copyleft/lgpl.html for the full text
 # of the license.
 
 __author__ = 'Martin Pitt'
 __email__ = 'martin.pitt@ubuntu.com'
 __copyright__ = '(c) 2012 Canonical Ltd.'
 __license__ = 'LGPL 3+'
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 from dbusmock.mockobject import (DBusMockObject, MOCK_IFACE,
                                  OBJECT_MANAGER_IFACE, get_object, get_objects)
 from dbusmock.testcase import DBusTestCase
 
 __all__ = ['DBusMockObject', 'MOCK_IFACE', 'OBJECT_MANAGER_IFACE',
            'DBusTestCase', 'get_object', 'get_objects']
```

### Comparing `python-dbusmock-0.9.1/dbusmock/testcase.py` & `python-dbusmock-0.9.2/dbusmock/testcase.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/__main__.py` & `python-dbusmock-0.9.2/dbusmock/__main__.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/bluez5.py` & `python-dbusmock-0.9.2/dbusmock/templates/bluez5.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/bluez5-obex.py` & `python-dbusmock-0.9.2/dbusmock/templates/bluez5-obex.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/logind.py` & `python-dbusmock-0.9.2/dbusmock/templates/logind.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/polkitd.py` & `python-dbusmock-0.9.2/dbusmock/templates/polkitd.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/upower.py` & `python-dbusmock-0.9.2/dbusmock/templates/upower.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
                    'org.freedesktop.UPower.Device',
                    {
                        'PowerSupply': dbus.Boolean(True, variant_level=1),
                        'Model': dbus.String(model_name, variant_level=1),
                        'Online': dbus.Boolean(True, variant_level=1),
                    },
                    [])
+    self.EmitSignal(MAIN_IFACE, 'DeviceAdded', 's', [path])
     return path
 
 
 @dbus.service.method(MOCK_IFACE,
                      in_signature='ssdx', out_signature='s')
 def AddDischargingBattery(self, device_name, model_name, percentage, seconds_to_empty):
     '''Convenience method to add a discharging battery object
@@ -143,14 +144,15 @@
                        'Energy': dbus.Double(percentage, variant_level=1),
                        # UP_DEVICE_STATE_DISCHARGING
                        'State': dbus.UInt32(2, variant_level=1),
                        # UP_DEVICE_KIND_BATTERY
                        'Type': dbus.UInt32(2, variant_level=1),
                    },
                    [])
+    self.EmitSignal(MAIN_IFACE, 'DeviceAdded', 's', [path])
     return path
 
 
 @dbus.service.method(MOCK_IFACE,
                      in_signature='ssdx', out_signature='s')
 def AddChargingBattery(self, device_name, model_name, percentage, seconds_to_full):
     '''Convenience method to add a charging battery object
@@ -177,14 +179,15 @@
                        'Energy': dbus.Double(percentage, variant_level=1),
                        # UP_DEVICE_STATE_CHARGING
                        'State': dbus.UInt32(1, variant_level=1),
                        # UP_DEVICE_KIND_BATTERY
                        'Type': dbus.UInt32(2, variant_level=1),
                    },
                    [])
+    self.EmitSignal(MAIN_IFACE, 'DeviceAdded', 's', [path])
     return path
 
 
 @dbus.service.method(MOCK_IFACE,
                      in_signature='uuddddxxbsu', out_signature='')
 def SetupDisplayDevice(self, type, state, percentage, energy, energy_full,
                        energy_rate, time_to_empty, time_to_full, is_present,
```

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/gnome_screensaver.py` & `python-dbusmock-0.9.2/dbusmock/templates/gnome_screensaver.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/networkmanager.py` & `python-dbusmock-0.9.2/dbusmock/templates/networkmanager.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/dbusmock/templates/notification_daemon.py` & `python-dbusmock-0.9.2/dbusmock/templates/notification_daemon.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/setup.py` & `python-dbusmock-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/python_dbusmock.egg-info/SOURCES.txt` & `python-dbusmock-0.9.2/python_dbusmock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/python_dbusmock.egg-info/PKG-INFO` & `python-dbusmock-0.9.2/python_dbusmock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-dbusmock
-Version: 0.9.1
+Version: 0.9.2
 Summary: Mock D-Bus objects
 Home-page: https://launchpad.net/python-dbusmock
 Author: Martin Pitt
 Author-email: martin.pitt@ubuntu.com
 License: LGPL 3+
 Download-URL: https://launchpad.net/python-dbusmock/+download
 Description: python-dbusmock
```

### Comparing `python-dbusmock-0.9.1/tests/test_gnome_screensaver.py` & `python-dbusmock-0.9.2/tests/test_gnome_screensaver.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_polkitd.py` & `python-dbusmock-0.9.2/tests/test_polkitd.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_upower.py` & `python-dbusmock-0.9.2/tests/test_upower.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __license__ = 'LGPL 3+'
 
 import unittest
 import sys
 import subprocess
 import time
 import os
+import fcntl
 
 import dbus
 
 import dbusmock
 
 UP_DEVICE_LEVEL_UNKNOWN = 0
 UP_DEVICE_LEVEL_NONE = 1
@@ -46,14 +47,17 @@
     def setUpClass(klass):
         klass.start_system_bus()
         klass.dbus_con = klass.get_dbus(True)
 
     def setUp(self):
         (self.p_mock, self.obj_upower) = self.spawn_server_template(
             'upower', {'OnBattery': True, 'HibernateAllowed': False}, stdout=subprocess.PIPE)
+        # set log to nonblocking
+        flags = fcntl.fcntl(self.p_mock.stdout, fcntl.F_GETFL)
+        fcntl.fcntl(self.p_mock.stdout, fcntl.F_SETFL, flags | os.O_NONBLOCK)
         self.dbusmock = dbus.Interface(self.obj_upower, dbusmock.MOCK_IFACE)
 
     def tearDown(self):
         self.p_mock.terminate()
         self.p_mock.wait()
 
     def test_no_devices(self):
@@ -69,14 +73,18 @@
         self.assertRegex(out, 'lid-is-present:\s+yes')
 
     def test_one_ac(self):
         path = self.dbusmock.AddAC('mock_AC', 'Mock AC')
         self.assertEqual(path, '/org/freedesktop/UPower/devices/mock_AC')
         ac_obj = self.dbus_con.get_object('org.freedesktop.UPower', path)
 
+        self.assertRegex(self.p_mock.stdout.read(),
+                         b'emit org.freedesktop.UPower.DeviceAdded '
+                         b'"/org/freedesktop/UPower/devices/mock_AC"\n')
+
         out = subprocess.check_output(['upower', '--dump'],
                                       universal_newlines=True)
         self.assertRegex(out, 'Device: ' + path)
         # note, Add* is not magic: this just adds an object, not change
         # properties
         self.assertRegex(out, 'on-battery:\s+yes')
         self.assertRegex(out, 'lid-is-present:\s+yes')
@@ -104,14 +112,18 @@
         self.assertRegex(out, 'device changed:\s+' + path)
         #print('--------- monitor out --------\n%s\n------------' % out)
 
     def test_discharging_battery(self):
         path = self.dbusmock.AddDischargingBattery('mock_BAT', 'Mock Battery', 30.0, 1200)
         self.assertEqual(path, '/org/freedesktop/UPower/devices/mock_BAT')
 
+        self.assertRegex(self.p_mock.stdout.read(),
+                         b'emit org.freedesktop.UPower.DeviceAdded '
+                         b'"/org/freedesktop/UPower/devices/mock_BAT"\n')
+
         out = subprocess.check_output(['upower', '--dump'],
                                       universal_newlines=True)
         self.assertRegex(out, 'Device: ' + path)
         # note, Add* is not magic: this just adds an object, not change
         # properties
         self.assertRegex(out, 'on-battery:\s+yes')
         self.assertRegex(out, 'lid-is-present:\s+yes')
@@ -120,14 +132,18 @@
         self.assertRegex(out, ' time to empty:\s+20.0 min')
         self.assertRegex(out, ' state:\s+discharging')
 
     def test_charging_battery(self):
         path = self.dbusmock.AddChargingBattery('mock_BAT', 'Mock Battery', 30.0, 1200)
         self.assertEqual(path, '/org/freedesktop/UPower/devices/mock_BAT')
 
+        self.assertRegex(self.p_mock.stdout.read(),
+                         b'emit org.freedesktop.UPower.DeviceAdded '
+                         b'"/org/freedesktop/UPower/devices/mock_BAT"\n')
+
         out = subprocess.check_output(['upower', '--dump'],
                                       universal_newlines=True)
         self.assertRegex(out, 'Device: ' + path)
         # note, Add* is not magic: this just adds an object, not change
         # properties
         self.assertRegex(out, 'on-battery:\s+yes')
         self.assertRegex(out, 'lid-is-present:\s+yes')
```

### Comparing `python-dbusmock-0.9.1/tests/test_notification_daemon.py` & `python-dbusmock-0.9.2/tests/test_notification_daemon.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_networkmanager.py` & `python-dbusmock-0.9.2/tests/test_networkmanager.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_api.py` & `python-dbusmock-0.9.2/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -551,14 +551,15 @@
     mock.AddMethods(MAIN_IFACE, [('Answer', '', 'i', 'ret = 42')])
 ''')
             my_template.flush()
             (p_mock, dbus_ultimate) = self.spawn_server_template(
                 my_template.name, stdout=subprocess.PIPE)
             self.addCleanup(p_mock.wait)
             self.addCleanup(p_mock.terminate)
+            self.addCleanup(p_mock.stdout.close)
 
         self.assertEqual(dbus_ultimate.Answer(), 42)
 
         # should appear in introspection
         xml = dbus_ultimate.Introspect()
         self.assertIn('<interface name="universe.Ultimate">', xml)
         self.assertIn('<method name="Answer">', xml)
@@ -587,14 +588,15 @@
     return 42
 ''')
             my_template.flush()
             (p_mock, dbus_ultimate) = self.spawn_server_template(
                 my_template.name, stdout=subprocess.PIPE)
             self.addCleanup(p_mock.wait)
             self.addCleanup(p_mock.terminate)
+            self.addCleanup(p_mock.stdout.close)
 
         self.assertEqual(dbus_ultimate.Answer(), 42)
 
         # should appear in introspection
         xml = dbus_ultimate.Introspect()
         self.assertIn('<interface name="universe.Ultimate">', xml)
         self.assertIn('<method name="Answer">', xml)
@@ -618,14 +620,15 @@
     mock.AddObject('/org/test/Peer', 'org.test.Do', {'name': 'peer'}, [])
 ''')
             my_template.flush()
             (p_mock, dbus_objmgr) = self.spawn_server_template(
                 my_template.name, stdout=subprocess.PIPE)
             self.addCleanup(p_mock.wait)
             self.addCleanup(p_mock.terminate)
+            self.addCleanup(p_mock.stdout.close)
 
         # should have the two Things, but not the Peer
         self.assertEqual(dbus_objmgr.GetManagedObjects(),
                          {'/org/test/Things/Thing1': {'org.test.Do': {'name': 'one'}},
                           '/org/test/Things/Thing2': {'org.test.Do': {'name': 'two'}}})
 
         # should appear in introspection
@@ -638,14 +641,15 @@
     def test_reset(self):
         '''Reset() puts the template back to pristine state'''
 
         (p_mock, obj_logind) = self.spawn_server_template(
             'logind', stdout=subprocess.PIPE)
         self.addCleanup(p_mock.wait)
         self.addCleanup(p_mock.terminate)
+        self.addCleanup(p_mock.stdout.close)
 
         # do some property, method, and object changes
         obj_logind.Set('org.freedesktop.login1.Manager', 'IdleAction', 'frob')
         mock_logind = dbus.Interface(obj_logind, dbusmock.MOCK_IFACE)
         mock_logind.AddProperty('org.Test.Other', 'walk', 'silly')
         mock_logind.AddMethod('', 'DoWalk', '', '', '')
         mock_logind.AddObject('/obj1', '', {}, [])
```

### Comparing `python-dbusmock-0.9.1/tests/test_logind.py` & `python-dbusmock-0.9.2/tests/test_logind.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_code.py` & `python-dbusmock-0.9.2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_cli.py` & `python-dbusmock-0.9.2/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         klass.session_con = klass.get_dbus()
 
     def setUp(self):
         self.p_mock = None
 
     def tearDown(self):
         if self.p_mock:
+            if self.p_mock.stdout:
+                self.p_mock.stdout.close()
+            if self.p_mock.stderr:
+                self.p_mock.stdout.close()
             self.p_mock.terminate()
             self.p_mock.wait()
             self.p_mock = None
 
     def test_session_bus(self):
         self.p_mock = subprocess.Popen([sys.executable, '-m', 'dbusmock',
                                         'com.example.Test', '/', 'TestIface'])
@@ -66,16 +70,14 @@
             out = subprocess.check_output(['upower', '--dump'],
                                           universal_newlines=True)
             self.assertRegex(out, 'on-battery:\s+no')
 
             mock_out = self.p_mock.stdout.readline()
             self.assertTrue('EnumerateDevices' in mock_out, mock_out)
 
-        self.p_mock.stdout.close()
-
     def test_object_manager(self):
         self.p_mock = subprocess.Popen([sys.executable, '-m', 'dbusmock',
                                         '-m', 'com.example.Test', '/', 'TestIface'],
                                        stdout=subprocess.PIPE)
         self.wait_for_bus_object('com.example.Test', '/')
 
         obj = self.session_con.get_object('com.example.Test', '/')
```

### Comparing `python-dbusmock-0.9.1/tests/test_bluez.py` & `python-dbusmock-0.9.2/tests/test_bluez.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/tests/test_consolekit.py` & `python-dbusmock-0.9.2/tests/test_consolekit.py`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/PKG-INFO` & `python-dbusmock-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-dbusmock
-Version: 0.9.1
+Version: 0.9.2
 Summary: Mock D-Bus objects
 Home-page: https://launchpad.net/python-dbusmock
 Author: Martin Pitt
 Author-email: martin.pitt@ubuntu.com
 License: LGPL 3+
 Download-URL: https://launchpad.net/python-dbusmock/+download
 Description: python-dbusmock
```

### Comparing `python-dbusmock-0.9.1/COPYING` & `python-dbusmock-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/README.rst` & `python-dbusmock-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-dbusmock-0.9.1/NEWS` & `python-dbusmock-0.9.2/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.9.2 (2013-12-13)
+------------------
+ - upower template: Emit DeviceAdded when adding new a new AC adapter or
+   battery. Thanks Iain Lane!
+ - Fix ResourceWarnings in test suite.
+
 0.9.1 (2013-12-10)
 ------------------
  - Fix UnicodeDecodeError in NEWS parsing when trying to build with a C locale.
    Thanks Dmitry Shachnev.
 
 0.9 (2013-11-29)
 ----------------
```

