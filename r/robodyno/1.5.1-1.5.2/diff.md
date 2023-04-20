# Comparing `tmp/robodyno-1.5.1.tar.gz` & `tmp/robodyno-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robodyno-1.5.1.tar", last modified: Fri Mar 31 09:51:09 2023, max compression
+gzip compressed data, was "robodyno-1.5.2.tar", last modified: Thu Apr 20 01:30:56 2023, max compression
```

## Comparing `robodyno-1.5.1.tar` & `robodyno-1.5.2.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.760501 robodyno-1.5.1/
--rw-rw-rw-   0        0        0     1124 2022-05-26 09:20:21.000000 robodyno-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     9483 2023-03-31 09:51:09.759501 robodyno-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     8415 2022-12-29 03:33:44.000000 robodyno-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.691169 robodyno-1.5.1/robodyno/
--rw-rw-rw-   0        0        0       91 2022-10-18 07:58:23.000000 robodyno-1.5.1/robodyno/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.701170 robodyno-1.5.1/robodyno/components/
--rw-rw-rw-   0        0        0     1300 2023-03-31 01:42:25.000000 robodyno-1.5.1/robodyno/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.706401 robodyno-1.5.1/robodyno/components/brands/
--rw-rw-rw-   0        0        0       44 2023-03-31 01:42:41.000000 robodyno-1.5.1/robodyno/components/brands/__init__.py
--rw-rw-rw-   0        0        0     2487 2023-03-31 01:42:56.000000 robodyno-1.5.1/robodyno/components/brands/robodyno.py
--rw-rw-rw-   0        0        0      736 2023-03-31 01:44:56.000000 robodyno-1.5.1/robodyno/components/brands/uuid.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.715911 robodyno-1.5.1/robodyno/components/can_bus/
--rw-rw-rw-   0        0        0        0 2023-01-05 01:31:03.000000 robodyno-1.5.1/robodyno/components/can_bus/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-30 00:39:27.000000 robodyno-1.5.1/robodyno/components/can_bus/adaptive_gripper.py
--rw-rw-rw-   0        0        0     1626 2023-03-31 01:47:06.000000 robodyno-1.5.1/robodyno/components/can_bus/can_bus_device.py
--rw-rw-rw-   0        0        0    23142 2023-03-31 02:23:42.000000 robodyno-1.5.1/robodyno/components/can_bus/motor.py
--rw-rw-rw-   0        0        0     3615 2023-03-31 01:32:54.000000 robodyno-1.5.1/robodyno/components/can_bus/slider_module.py
--rw-rw-rw-   0        0        0     2279 2023-03-31 01:45:58.000000 robodyno-1.5.1/robodyno/components/can_bus/vacuum_gripper.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.719913 robodyno-1.5.1/robodyno/components/webots/
--rw-rw-rw-   0        0        0        0 2023-01-05 01:31:03.000000 robodyno-1.5.1/robodyno/components/webots/__init__.py
--rw-rw-rw-   0        0        0    18915 2023-03-31 03:02:52.000000 robodyno-1.5.1/robodyno/components/webots/motor.py
--rw-rw-rw-   0        0        0     1627 2023-03-31 01:45:10.000000 robodyno-1.5.1/robodyno/components/webots/webots_device.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.725432 robodyno-1.5.1/robodyno/interfaces/
--rw-rw-rw-   0        0        0      502 2023-03-31 01:27:49.000000 robodyno-1.5.1/robodyno/interfaces/__init__.py
--rw-rw-rw-   0        0        0     8822 2023-01-05 04:13:36.000000 robodyno-1.5.1/robodyno/interfaces/can_bus.py
--rw-rw-rw-   0        0        0     3069 2023-03-31 09:36:22.000000 robodyno-1.5.1/robodyno/interfaces/webots.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.731433 robodyno-1.5.1/robodyno/tools/
--rw-rw-rw-   0        0        0    10261 2023-03-01 03:27:39.000000 robodyno-1.5.1/robodyno/tools/__init__.py
--rw-rw-rw-   0        0        0     1516 2023-01-05 01:31:03.000000 robodyno-1.5.1/robodyno/tools/list_devices.py
--rw-rw-rw-   0        0        0     1890 2022-10-19 01:56:31.000000 robodyno-1.5.1/robodyno/tools/monitor.py
--rw-rw-rw-   0        0        0      759 2022-10-19 01:56:19.000000 robodyno-1.5.1/robodyno/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.700169 robodyno-1.5.1/robodyno.egg-info/
--rw-rw-rw-   0        0        0     9483 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1707 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      869 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-31 09:51:09.000000 robodyno-1.5.1/robodyno.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.733148 robodyno-1.5.1/robodyno_robots/
--rw-rw-rw-   0        0        0      309 2023-01-05 02:44:11.000000 robodyno-1.5.1/robodyno_robots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.736959 robodyno-1.5.1/robodyno_robots/four_dof_palletizing_robot/
--rw-rw-rw-   0        0        0        0 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/four_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0        0        0     7510 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.740476 robodyno-1.5.1/robodyno_robots/four_dof_scara_robot/
--rw-rw-rw-   0        0        0       46 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/four_dof_scara_robot/__init__.py
--rw-rw-rw-   0        0        0     8374 2023-01-05 01:46:18.000000 robodyno-1.5.1/robodyno_robots/four_dof_scara_robot/four_dof_scara_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.743978 robodyno-1.5.1/robodyno_robots/six_dof_collaborative_robot/
--rw-rw-rw-   0        0        0       51 2022-10-12 03:40:06.000000 robodyno-1.5.1/robodyno_robots/six_dof_collaborative_robot/__init__.py
--rw-rw-rw-   0        0        0    10587 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/six_dof_collaborative_robot/six_dof_collab_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.747988 robodyno-1.5.1/robodyno_robots/three_dof_delta_robot/
--rw-rw-rw-   0        0        0       48 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/three_dof_delta_robot/__init__.py
--rw-rw-rw-   0        0        0     9755 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/three_dof_delta_robot/three_dof_delta_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.751988 robodyno-1.5.1/robodyno_robots/three_dof_palletizing_robot/
--rw-rw-rw-   0        0        0       50 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/three_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0        0        0     7494 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:51:09.757501 robodyno-1.5.1/robodyno_robots/utils/
--rw-rw-rw-   0        0        0        0 2022-10-12 03:40:06.000000 robodyno-1.5.1/robodyno_robots/utils/__init__.py
--rw-rw-rw-   0        0        0      626 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/utils/interpolations.py
--rw-rw-rw-   0        0        0    59526 2023-01-02 13:41:13.000000 robodyno-1.5.1/robodyno_robots/utils/transformations.py
--rw-rw-rw-   0        0        0       42 2023-03-31 09:51:09.760501 robodyno-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3329 2023-03-31 09:50:18.000000 robodyno-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.592635 robodyno-1.5.2/
+-rw-rw-rw-   0        0        0     1124 2022-05-26 09:20:21.000000 robodyno-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     9483 2023-04-20 01:30:56.591637 robodyno-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8415 2022-12-29 03:33:44.000000 robodyno-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.546635 robodyno-1.5.2/robodyno/
+-rw-rw-rw-   0        0        0       91 2022-10-18 07:58:23.000000 robodyno-1.5.2/robodyno/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.554636 robodyno-1.5.2/robodyno/components/
+-rw-rw-rw-   0        0        0     1300 2023-03-31 01:42:25.000000 robodyno-1.5.2/robodyno/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.557635 robodyno-1.5.2/robodyno/components/brands/
+-rw-rw-rw-   0        0        0       44 2023-03-31 01:42:41.000000 robodyno-1.5.2/robodyno/components/brands/__init__.py
+-rw-rw-rw-   0        0        0     2487 2023-03-31 01:42:56.000000 robodyno-1.5.2/robodyno/components/brands/robodyno.py
+-rw-rw-rw-   0        0        0      731 2023-04-20 01:26:17.000000 robodyno-1.5.2/robodyno/components/brands/uuid.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.565638 robodyno-1.5.2/robodyno/components/can_bus/
+-rw-rw-rw-   0        0        0        0 2023-01-05 01:31:03.000000 robodyno-1.5.2/robodyno/components/can_bus/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-30 00:39:27.000000 robodyno-1.5.2/robodyno/components/can_bus/adaptive_gripper.py
+-rw-rw-rw-   0        0        0     1626 2023-03-31 01:47:06.000000 robodyno-1.5.2/robodyno/components/can_bus/can_bus_device.py
+-rw-rw-rw-   0        0        0    23142 2023-03-31 02:23:42.000000 robodyno-1.5.2/robodyno/components/can_bus/motor.py
+-rw-rw-rw-   0        0        0     2079 2023-03-31 14:21:11.000000 robodyno-1.5.2/robodyno/components/can_bus/pwm_driver.py
+-rw-rw-rw-   0        0        0     3615 2023-03-31 01:32:54.000000 robodyno-1.5.2/robodyno/components/can_bus/slider_module.py
+-rw-rw-rw-   0        0        0     4612 2023-04-01 11:03:12.000000 robodyno-1.5.2/robodyno/components/can_bus/stepper_driver.py
+-rw-rw-rw-   0        0        0     2271 2023-03-31 13:48:28.000000 robodyno-1.5.2/robodyno/components/can_bus/vacuum_gripper.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.570635 robodyno-1.5.2/robodyno/components/webots/
+-rw-rw-rw-   0        0        0        0 2023-01-05 01:31:03.000000 robodyno-1.5.2/robodyno/components/webots/__init__.py
+-rw-rw-rw-   0        0        0    19929 2023-04-02 13:03:06.000000 robodyno-1.5.2/robodyno/components/webots/motor.py
+-rw-rw-rw-   0        0        0     3456 2023-04-02 13:25:06.000000 robodyno-1.5.2/robodyno/components/webots/slider_module.py
+-rw-rw-rw-   0        0        0     1543 2023-04-02 12:55:40.000000 robodyno-1.5.2/robodyno/components/webots/webots_device.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.572636 robodyno-1.5.2/robodyno/interfaces/
+-rw-rw-rw-   0        0        0      502 2023-03-31 01:27:49.000000 robodyno-1.5.2/robodyno/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     8822 2023-01-05 04:13:36.000000 robodyno-1.5.2/robodyno/interfaces/can_bus.py
+-rw-rw-rw-   0        0        0     3069 2023-03-31 09:36:22.000000 robodyno-1.5.2/robodyno/interfaces/webots.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.576636 robodyno-1.5.2/robodyno/tools/
+-rw-rw-rw-   0        0        0    10261 2023-03-01 03:27:39.000000 robodyno-1.5.2/robodyno/tools/__init__.py
+-rw-rw-rw-   0        0        0     1516 2023-01-05 01:31:03.000000 robodyno-1.5.2/robodyno/tools/list_devices.py
+-rw-rw-rw-   0        0        0     1890 2022-10-19 01:56:31.000000 robodyno-1.5.2/robodyno/tools/monitor.py
+-rw-rw-rw-   0        0        0      759 2022-10-19 01:56:19.000000 robodyno-1.5.2/robodyno/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.553637 robodyno-1.5.2/robodyno.egg-info/
+-rw-rw-rw-   0        0        0     9483 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1072 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 01:30:56.000000 robodyno-1.5.2/robodyno.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.577637 robodyno-1.5.2/robodyno_robots/
+-rw-rw-rw-   0        0        0      309 2023-01-05 02:44:11.000000 robodyno-1.5.2/robodyno_robots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.579637 robodyno-1.5.2/robodyno_robots/four_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0        0 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/four_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7510 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.581637 robodyno-1.5.2/robodyno_robots/four_dof_scara_robot/
+-rw-rw-rw-   0        0        0       46 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/four_dof_scara_robot/__init__.py
+-rw-rw-rw-   0        0        0     8374 2023-01-05 01:46:18.000000 robodyno-1.5.2/robodyno_robots/four_dof_scara_robot/four_dof_scara_robot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.583638 robodyno-1.5.2/robodyno_robots/six_dof_collaborative_robot/
+-rw-rw-rw-   0        0        0       51 2022-10-12 03:40:06.000000 robodyno-1.5.2/robodyno_robots/six_dof_collaborative_robot/__init__.py
+-rw-rw-rw-   0        0        0    10587 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/six_dof_collaborative_robot/six_dof_collab_robot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.585638 robodyno-1.5.2/robodyno_robots/three_dof_delta_robot/
+-rw-rw-rw-   0        0        0       48 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/three_dof_delta_robot/__init__.py
+-rw-rw-rw-   0        0        0     9755 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/three_dof_delta_robot/three_dof_delta_robot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.587637 robodyno-1.5.2/robodyno_robots/three_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0       50 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/three_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7494 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 01:30:56.590636 robodyno-1.5.2/robodyno_robots/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-12 03:40:06.000000 robodyno-1.5.2/robodyno_robots/utils/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/utils/interpolations.py
+-rw-rw-rw-   0        0        0    59526 2023-01-02 13:41:13.000000 robodyno-1.5.2/robodyno_robots/utils/transformations.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 01:30:56.592635 robodyno-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     3580 2023-04-02 13:15:45.000000 robodyno-1.5.2/setup.py
```

### Comparing `robodyno-1.5.1/LICENSE` & `robodyno-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/PKG-INFO` & `robodyno-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodyno
-Version: 1.5.1
+Version: 1.5.2
 Summary: The Robodyno Robot SDK for Python 3
 Home-page: https://github.com/robottime/Robodyno-Python-API
 Author: song
 Author-email: zhaosongy@126.com
 Maintainer: robottime
 Maintainer-email: lab@robottime.cn
 License: MIT License
```

### Comparing `robodyno-1.5.1/README.md` & `robodyno-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/__init__.py` & `robodyno-1.5.2/robodyno/components/__init__.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/brands/robodyno.py` & `robodyno-1.5.2/robodyno/components/brands/robodyno.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/brands/uuid.py` & `robodyno-1.5.2/robodyno/components/brands/uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ROBODYNO_PRO_100 = 0x03
     ROBODYNO_PRO_DIRECT = 0x0F
     ROBODYNO_PLUS_50  = 0x10
     ROBODYNO_PLUS_100 = 0x11
     ROBODYNO_PLUS_12  = 0x12
     ROBODYNO_PLUS_DIRECT = 0x1F
     ROBODYNO_NANO_100 = 0x20
-    ROBODYNO_GENERAL_GRIPPER = 0x61
+    ROBODYNO_PWM_DRIVER = 0x61
     ROBODYNO_STEPPER_DRIVER = 0x62
     ROBODYNO_VACUUM_GRIPPER = 0x63
     ROBODYNO_ADAPTIVE_GRIPPER = 0x64
     ROBODYNO_FLEXIBLE_GRIPPER = 0x65
     ROBODYNO_EXB_FCTY = 0x80
     ROBODYNO_THIRD_PARTY = 0xFF
```

### Comparing `robodyno-1.5.1/robodyno/components/can_bus/can_bus_device.py` & `robodyno-1.5.2/robodyno/components/can_bus/can_bus_device.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/can_bus/motor.py` & `robodyno-1.5.2/robodyno/components/can_bus/motor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/can_bus/slider_module.py` & `robodyno-1.5.2/robodyno/components/can_bus/slider_module.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/components/can_bus/vacuum_gripper.py` & `robodyno-1.5.2/robodyno/components/can_bus/vacuum_gripper.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 
     def __init__(self, iface, id = 0x21, type = None):
         """Init vacuum gripper from interface, id and type
         
         Args:
             iface: robodyno interface
             id: range from 0x01 to 0x40, default 0x21
-            type: vacuum gripper type(ROBODYNO_GENERAL_GRIPPER / ROBODYNO_VACUUM_GRIPPER)
+            type: vacuum gripper type(ROBODYNO_PWM_DRIVER / ROBODYNO_VACUUM_GRIPPER)
         """
         super().__init__(iface, id)
         self.get_version(timeout=0.15)
         if type:
             self.type = DeviceType[type]
-        if self.type not in [DeviceType.ROBODYNO_GENERAL_GRIPPER, DeviceType.ROBODYNO_VACUUM_GRIPPER]:
+        if self.type not in [DeviceType.ROBODYNO_PWM_DRIVER, DeviceType.ROBODYNO_VACUUM_GRIPPER]:
             raise ValueError('Vacuum gripper type is invalid and can not distinguish automatically.')
         self.status = False
         self.off()
 
     @CanBus.send_to_bus(CMD_SET_NODE_ID, '<B')
     def config_can_bus(self, new_id):
-        """Cange gripper device id.
+        """Change gripper device id.
         
         Args:
             new_id: gripper new device id
         """
         return (new_id,)
 
     @CanBus.send_to_bus(CMD_SET_PWM, '<B')
     def set_pwm(self, pwm):
-        """Cange gripper strength.
+        """Change gripper strength.
         
         Args:
             pwm: range from 0 to 255
         """
         return (pwm,)
 
     def on(self):
```

### Comparing `robodyno-1.5.1/robodyno/components/webots/motor.py` & `robodyno-1.5.2/robodyno/components/webots/motor.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,18 @@
             DeviceType.ROBODYNO_PRO_DIRECT,
             DeviceType.ROBODYNO_PLUS_50 ,
             DeviceType.ROBODYNO_PLUS_100,
             DeviceType.ROBODYNO_PLUS_12 ,
             DeviceType.ROBODYNO_PLUS_DIRECT,
             DeviceType.ROBODYNO_NANO_100,
         ]
-
+        try:
+            self.name = '0x{:02X}::motor'.format(id)
+        except:
+            self.name = id
         self._motor = self._iface.robot.getDevice(self.name)
         self._pos_sensor = self._motor.getPositionSensor()
         self._twin_motor = None
         if twin and GET_IFACE_TYPE(twin) == InterfaceType.CanBus:
             self._twin_motor = CanMotor(twin, id, type)
             self.init_twin_offset()
             self.type = self._twin_motor.type
@@ -302,14 +305,27 @@
         
         Returns:
             position(rad)
             None if timeout
         """
         return self._pos_feedback * copysign(1, self.reduction)
 
+    def get_abs_pos(self, timeout = 0):
+        """Get motor absolute position.
+        
+        Args:
+            timeout: 0 indicates unlimited timeout(s)
+        
+        Returns:
+            position(rad)
+            None if timeout
+        """
+        return self._pos_feedback * copysign(1, self.reduction)
+
+
     def get_vel(self, timeout = 0):
         """Get motor velocity.
         
         Args:
             timeout: 0 indicates unlimited timeout(s)
         
         Returns:
@@ -485,14 +501,29 @@
         
         Args:
             pos: target position(rad)
             vel_ff: velocity feed forward(rad/s)
             torque_ff:torque feed forward(Nm)
         """
         self._iface._mutex.acquire()
+        pos = pos * copysign(1, self.reduction)
+        self._input_pos = pos
+        self._filter_controller.set_pos(pos)
+        self._track_controller.set_pos(pos, self._pos_feedback, self._vel_feedback)
+        self._iface._mutex.release()
+    
+    def set_abs_pos(self, pos, vel_ff = 0, torque_ff = 0):
+        """Set motor target absolute position.
+        
+        Args:
+            pos: target position(rad)
+            vel_ff: velocity feed forward(rad/s)
+            torque_ff:torque feed forward(Nm)
+        """
+        self._iface._mutex.acquire()
         pos = pos * copysign(1, self.reduction)
         self._input_pos = pos
         self._filter_controller.set_pos(pos)
         self._track_controller.set_pos(pos, self._pos_feedback, self._vel_feedback)
         self._iface._mutex.release()
     
     def set_vel(self, vel, torque_ff = 0):
```

### Comparing `robodyno-1.5.1/robodyno/components/webots/webots_device.py` & `robodyno-1.5.2/robodyno/components/webots/webots_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,18 +21,15 @@
         
         Args:
             iface: webots interface
             id: node id
             type: robodyno device type name
             auto_register: auto register self to webots interface
         """
-        try:
-            self.name = '0x{:02X}'.format(id)
-        except:
-            self.name = id
+        self.id = id
         if not isinstance(iface, Webots):
             raise ValueError('Use a webots interface to init a webots device.')
         self._iface = iface
         if auto_register:
             iface.register(self)
     
     def __del__(self):
```

### Comparing `robodyno-1.5.1/robodyno/interfaces/can_bus.py` & `robodyno-1.5.2/robodyno/interfaces/can_bus.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/interfaces/webots.py` & `robodyno-1.5.2/robodyno/interfaces/webots.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/tools/__init__.py` & `robodyno-1.5.2/robodyno/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/tools/list_devices.py` & `robodyno-1.5.2/robodyno/tools/list_devices.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/tools/monitor.py` & `robodyno-1.5.2/robodyno/tools/monitor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno/tools/utils.py` & `robodyno-1.5.2/robodyno/tools/utils.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno.egg-info/PKG-INFO` & `robodyno-1.5.2/robodyno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodyno
-Version: 1.5.1
+Version: 1.5.2
 Summary: The Robodyno Robot SDK for Python 3
 Home-page: https://github.com/robottime/Robodyno-Python-API
 Author: song
 Author-email: zhaosongy@126.com
 Maintainer: robottime
 Maintainer-email: lab@robottime.cn
 License: MIT License
```

### Comparing `robodyno-1.5.1/robodyno.egg-info/SOURCES.txt` & `robodyno-1.5.2/robodyno.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 robodyno/components/brands/__init__.py
 robodyno/components/brands/robodyno.py
 robodyno/components/brands/uuid.py
 robodyno/components/can_bus/__init__.py
 robodyno/components/can_bus/adaptive_gripper.py
 robodyno/components/can_bus/can_bus_device.py
 robodyno/components/can_bus/motor.py
+robodyno/components/can_bus/pwm_driver.py
 robodyno/components/can_bus/slider_module.py
+robodyno/components/can_bus/stepper_driver.py
 robodyno/components/can_bus/vacuum_gripper.py
 robodyno/components/webots/__init__.py
 robodyno/components/webots/motor.py
+robodyno/components/webots/slider_module.py
 robodyno/components/webots/webots_device.py
 robodyno/interfaces/__init__.py
 robodyno/interfaces/can_bus.py
 robodyno/interfaces/webots.py
 robodyno/tools/__init__.py
 robodyno/tools/list_devices.py
 robodyno/tools/monitor.py
```

### Comparing `robodyno-1.5.1/robodyno.egg-info/entry_points.txt` & `robodyno-1.5.2/robodyno.egg-info/entry_points.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [console_scripts]
 robodyno = robodyno:robodyno
 robodyno-motor = robodyno:robodyno_motor
 
 [robodyno.components.can_bus]
 Motor = robodyno.components.can_bus.motor:Motor
+PwmDriver = robodyno.components.can_bus.pwm_driver:PwmDriver
 SliderModule = robodyno.components.can_bus.slider_module:SliderModule
+StepperDriver = robodyno.components.can_bus.stepper_driver:StepperDriver
 VGripper = robodyno.components.can_bus.vacuum_gripper:VGripper
 
 [robodyno.components.webots]
 Motor = robodyno.components.webots.motor:Motor
+SliderModule = robodyno.components.webots.slider_module:SliderModule
 
 [robodyno.robots]
 FourDoFPallet = robodyno.robots.four_dof_palletizing_robot.four_dof_pallet_robot:FourDoFPallet
 FourDoFScara = robodyno.robots.four_dof_scara_robot.four_dof_scara_robot:FourDoFScara
 SixDoFCollabRobot = robodyno.robots.six_dof_collaborative_robot.six_dof_collab_robot:SixDoFCollabRobot
 ThreeDoFDelta = robodyno.robots.three_dof_delta_robot.three_dof_delta_robot:ThreeDoFDelta
 ThreeDoFPallet = robodyno.robots.three_dof_palletizing_robot.three_dof_pallet_robot:ThreeDoFPallet
```

### Comparing `robodyno-1.5.1/robodyno_robots/four_dof_palletizing_robot/four_dof_pallet_robot.py` & `robodyno-1.5.2/robodyno_robots/four_dof_palletizing_robot/four_dof_pallet_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/four_dof_scara_robot/four_dof_scara_robot.py` & `robodyno-1.5.2/robodyno_robots/four_dof_scara_robot/four_dof_scara_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/six_dof_collaborative_robot/six_dof_collab_robot.py` & `robodyno-1.5.2/robodyno_robots/six_dof_collaborative_robot/six_dof_collab_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/three_dof_delta_robot/three_dof_delta_robot.py` & `robodyno-1.5.2/robodyno_robots/three_dof_delta_robot/three_dof_delta_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/three_dof_palletizing_robot/three_dof_pallet_robot.py` & `robodyno-1.5.2/robodyno_robots/three_dof_palletizing_robot/three_dof_pallet_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/utils/interpolations.py` & `robodyno-1.5.2/robodyno_robots/utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/robodyno_robots/utils/transformations.py` & `robodyno-1.5.2/robodyno_robots/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.5.1/setup.py` & `robodyno-1.5.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 long_description = open('README.md', encoding='utf-8').read()
 
 setup(
     name='robodyno',
-    version='1.5.1',
+    version='1.5.2',
     maintainer='robottime',
     maintainer_email='lab@robottime.cn',
     author='song',
     author_email='zhaosongy@126.com',
     description='The Robodyno Robot SDK for Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -58,19 +58,22 @@
         ':sys_platform == "win32"': [
             'candle-bus'
         ],
     },
     entry_points={
         'robodyno.components.can_bus': [
             'Motor = robodyno.components.can_bus.motor:Motor',
+            'PwmDriver = robodyno.components.can_bus.pwm_driver:PwmDriver',
+            'StepperDriver = robodyno.components.can_bus.stepper_driver:StepperDriver',
             'VGripper = robodyno.components.can_bus.vacuum_gripper:VGripper',
             'SliderModule = robodyno.components.can_bus.slider_module:SliderModule',
         ],
         'robodyno.components.webots': [
             'Motor = robodyno.components.webots.motor:Motor',
+            'SliderModule = robodyno.components.webots.slider_module:SliderModule',
         ],
         'robodyno.robots': [
             'FourDoFPallet = robodyno.robots.four_dof_palletizing_robot.four_dof_pallet_robot:FourDoFPallet',
             'FourDoFScara = robodyno.robots.four_dof_scara_robot.four_dof_scara_robot:FourDoFScara',
             'SixDoFCollabRobot = robodyno.robots.six_dof_collaborative_robot.six_dof_collab_robot:SixDoFCollabRobot',
             'ThreeDoFDelta = robodyno.robots.three_dof_delta_robot.three_dof_delta_robot:ThreeDoFDelta',
             'ThreeDoFPallet = robodyno.robots.three_dof_palletizing_robot.three_dof_pallet_robot:ThreeDoFPallet',
```

