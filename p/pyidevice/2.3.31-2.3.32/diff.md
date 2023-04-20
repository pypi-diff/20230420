# Comparing `tmp/pyidevice-2.3.31.tar.gz` & `tmp/pyidevice-2.3.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyidevice-2.3.31.tar", last modified: Fri Mar 31 09:17:55 2023, max compression
+gzip compressed data, was "pyidevice-2.3.32.tar", last modified: Thu Apr 20 03:34:30 2023, max compression
```

## Comparing `pyidevice-2.3.31.tar` & `pyidevice-2.3.32.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.364703 pyidevice-2.3.31/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 pyidevice-2.3.31/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 pyidevice-2.3.31/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    10613 2023-03-31 09:17:55.364552 pyidevice-2.3.31/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10152 2023-03-21 02:13:30.000000 pyidevice-2.3.31/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.347737 pyidevice-2.3.31/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 pyidevice-2.3.31/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 pyidevice-2.3.31/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 pyidevice-2.3.31/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.352105 pyidevice-2.3.31/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-03-17 09:32:37.000000 pyidevice-2.3.31/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-02-09 09:46:25.000000 pyidevice-2.3.31/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-03-17 09:29:43.000000 pyidevice-2.3.31/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-02-21 09:11:42.000000 pyidevice-2.3.31/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 pyidevice-2.3.31/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      495 2023-03-22 01:55:49.000000 pyidevice-2.3.31/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-03-17 08:58:28.000000 pyidevice-2.3.31/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-03-17 08:58:33.000000 pyidevice-2.3.31/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 pyidevice-2.3.31/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 pyidevice-2.3.31/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 pyidevice-2.3.31/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2022-11-25 10:28:56.000000 pyidevice-2.3.31/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 pyidevice-2.3.31/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 pyidevice-2.3.31/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 pyidevice-2.3.31/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 pyidevice-2.3.31/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.345585 pyidevice-2.3.31/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       23 2023-03-21 02:14:27.000000 pyidevice-2.3.31/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.353472 pyidevice-2.3.31/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    29645 2023-03-17 09:26:47.000000 pyidevice-2.3.31/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1204 2023-03-22 07:43:27.000000 pyidevice-2.3.31/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    17034 2023-02-16 02:38:30.000000 pyidevice-2.3.31/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    10985 2023-01-04 04:18:58.000000 pyidevice-2.3.31/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-03-07 02:40:34.000000 pyidevice-2.3.31/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.357879 pyidevice-2.3.31/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     6867 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1075 2023-03-14 03:42:50.000000 pyidevice-2.3.31/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7843 2023-03-14 03:42:50.000000 pyidevice-2.3.31/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 pyidevice-2.3.31/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 pyidevice-2.3.31/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 pyidevice-2.3.31/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 pyidevice-2.3.31/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 pyidevice-2.3.31/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      907 2023-03-14 03:42:49.000000 pyidevice-2.3.31/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.363422 pyidevice-2.3.31/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 pyidevice-2.3.31/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 pyidevice-2.3.31/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-03-17 09:03:55.000000 pyidevice-2.3.31/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-03-21 02:08:37.000000 pyidevice-2.3.31/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-03-17 09:24:31.000000 pyidevice-2.3.31/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-03-22 02:30:59.000000 pyidevice-2.3.31/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 pyidevice-2.3.31/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2022-09-26 09:47:22.000000 pyidevice-2.3.31/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12590 2023-03-22 02:30:59.000000 pyidevice-2.3.31/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 pyidevice-2.3.31/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 pyidevice-2.3.31/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-03-31 09:17:55.364270 pyidevice-2.3.31/pyidevice.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    10613 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2476 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       10 2023-03-31 09:17:55.000000 pyidevice-2.3.31/pyidevice.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-03-01 11:02:23.000000 pyidevice-2.3.31/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-03-31 09:17:55.364749 pyidevice-2.3.31/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      953 2023-03-31 09:08:36.000000 pyidevice-2.3.31/setup.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.179042 pyidevice-2.3.32/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 pyidevice-2.3.32/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 pyidevice-2.3.32/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10963 2023-04-20 03:34:30.178735 pyidevice-2.3.32/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10544 2023-04-20 03:06:40.000000 pyidevice-2.3.32/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.163995 pyidevice-2.3.32/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 pyidevice-2.3.32/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 pyidevice-2.3.32/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 pyidevice-2.3.32/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.167525 pyidevice-2.3.32/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 pyidevice-2.3.32/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 pyidevice-2.3.32/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-04-07 02:39:15.000000 pyidevice-2.3.32/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-02-21 09:11:42.000000 pyidevice-2.3.32/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 pyidevice-2.3.32/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-04-07 02:35:34.000000 pyidevice-2.3.32/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-03-17 08:58:28.000000 pyidevice-2.3.32/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-03-17 08:58:33.000000 pyidevice-2.3.32/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 pyidevice-2.3.32/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 pyidevice-2.3.32/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 pyidevice-2.3.32/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 pyidevice-2.3.32/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 pyidevice-2.3.32/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 pyidevice-2.3.32/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 pyidevice-2.3.32/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 pyidevice-2.3.32/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.162102 pyidevice-2.3.32/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       23 2023-04-20 03:24:54.000000 pyidevice-2.3.32/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.168689 pyidevice-2.3.32/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    29436 2023-04-20 02:52:36.000000 pyidevice-2.3.32/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 pyidevice-2.3.32/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19123 2023-04-20 03:02:09.000000 pyidevice-2.3.32/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10985 2023-01-04 04:18:58.000000 pyidevice-2.3.32/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 pyidevice-2.3.32/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.172012 pyidevice-2.3.32/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6867 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 pyidevice-2.3.32/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 pyidevice-2.3.32/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 pyidevice-2.3.32/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 pyidevice-2.3.32/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 pyidevice-2.3.32/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 pyidevice-2.3.32/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 pyidevice-2.3.32/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 pyidevice-2.3.32/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 pyidevice-2.3.32/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.177506 pyidevice-2.3.32/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 pyidevice-2.3.32/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 pyidevice-2.3.32/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 pyidevice-2.3.32/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 pyidevice-2.3.32/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 pyidevice-2.3.32/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 pyidevice-2.3.32/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 pyidevice-2.3.32/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2022-09-26 09:47:22.000000 pyidevice-2.3.32/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 pyidevice-2.3.32/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 pyidevice-2.3.32/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 pyidevice-2.3.32/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:34:30.178493 pyidevice-2.3.32/pyidevice.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10963 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2486 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       10 2023-04-20 03:34:30.000000 pyidevice-2.3.32/pyidevice.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 pyidevice-2.3.32/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-04-20 03:34:30.179086 pyidevice-2.3.32/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 pyidevice-2.3.32/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 pyidevice-2.3.32/setup2.py
```

### Comparing `pyidevice-2.3.31/LICENSE` & `pyidevice-2.3.32/LICENSE`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/PKG-INFO` & `pyidevice-2.3.32/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyidevice
-Version: 2.3.31
+Version: 2.3.32
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
-Maintainer: chenpeijie
-Maintainer-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,15 +29,15 @@
 
 ## pip :
     pip install py-ios-device
     
 python version: 3.7 +
 ### Instruments：
 - [x] Get system Memory and CPU data
-- [x] Get processes Memory and CPU data
+- [x] Get application Memory and CPU data
 - [x] Get FPS data
 - [x] Get network data
 - [x] Set the device network status. eg: 2G, 3G ,100% Loss
 - [x] Set the device behaves as though under a high thermal state
 - [x] Monitoring app start、exit、background
 - [x] Launch and Kill app
 - [x] Run xctest. eg: WebDriverAgent
@@ -88,24 +86,29 @@
 Disk    >> {'Data Read': '117.91 GiB', 'Data Read/sec': 0, 'Data Written': '64.28 GiB', 'Data Written/sec': 0, 'Reads in': 9734132, 'Reads in/sec': 9734132, 'Writes Out': 6810640, 'Writes Out/sec': 6810640}
 
 $ pyidevice instruments monitor --filter = memory
 Memory  >> {'App Memory': '699.69 MiB', 'Cached Files': '1.48 GiB', 'Compressed': '155.17 MiB', 'Memory Used': '1.42 GiB', 'Wired Memory': '427.91 MiB', 'Swap Used': '46.25 MiB'}
 
 ```
 
+#### Get application performance data
 
+```bash
+$ pyidevice instruments appmonitor  -b cn.rongcloud.im
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '0 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.28 MiB', 'Threads': 13}
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '3.4 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.30 MiB', 'Threads': 13}
+```
 
-#### Get Processes performance data
-
+#### Get custom application performance data
 ```bash
 $ pyidevice instruments sysmontap --help
-$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter memVirtualSize,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
+$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter physFootprint,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
 
-[('WeChat', {'cpuUsage': 0.03663705586691998, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
-[('WeChat', {'cpuUsage': 0.036558268613227536, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.03663705586691998, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.036558268613227536, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
 
 
 ```
 #### Get FPS data
 
 ```bash
 $ pyidevice instruments fps
```

### Comparing `pyidevice-2.3.31/README.md` & `pyidevice-2.3.32/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## pip :
     pip install py-ios-device
     
 python version: 3.7 +
 ### Instruments：
 - [x] Get system Memory and CPU data
-- [x] Get processes Memory and CPU data
+- [x] Get application Memory and CPU data
 - [x] Get FPS data
 - [x] Get network data
 - [x] Set the device network status. eg: 2G, 3G ,100% Loss
 - [x] Set the device behaves as though under a high thermal state
 - [x] Monitoring app start、exit、background
 - [x] Launch and Kill app
 - [x] Run xctest. eg: WebDriverAgent
@@ -71,24 +71,29 @@
 Disk    >> {'Data Read': '117.91 GiB', 'Data Read/sec': 0, 'Data Written': '64.28 GiB', 'Data Written/sec': 0, 'Reads in': 9734132, 'Reads in/sec': 9734132, 'Writes Out': 6810640, 'Writes Out/sec': 6810640}
 
 $ pyidevice instruments monitor --filter = memory
 Memory  >> {'App Memory': '699.69 MiB', 'Cached Files': '1.48 GiB', 'Compressed': '155.17 MiB', 'Memory Used': '1.42 GiB', 'Wired Memory': '427.91 MiB', 'Swap Used': '46.25 MiB'}
 
 ```
 
+#### Get application performance data
 
+```bash
+$ pyidevice instruments appmonitor  -b cn.rongcloud.im
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '0 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.28 MiB', 'Threads': 13}
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '3.4 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.30 MiB', 'Threads': 13}
+```
 
-#### Get Processes performance data
-
+#### Get custom application performance data
 ```bash
 $ pyidevice instruments sysmontap --help
-$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter memVirtualSize,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
+$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter physFootprint,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
 
-[('WeChat', {'cpuUsage': 0.03663705586691998, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
-[('WeChat', {'cpuUsage': 0.036558268613227536, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.03663705586691998, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.036558268613227536, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
 
 
 ```
 #### Get FPS data
 
 ```bash
 $ pyidevice instruments fps
```

### Comparing `pyidevice-2.3.31/demo/afc.py` & `pyidevice-2.3.32/demo/afc.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/crash_log.py` & `pyidevice-2.3.32/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/installation_proxy.py` & `pyidevice-2.3.32/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/activity.py` & `pyidevice-2.3.32/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/app_lifecycle.py` & `pyidevice-2.3.32/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/applictionListing.py` & `pyidevice-2.3.32/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/coreprofilesessiontap.py` & `pyidevice-2.3.32/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/coreprofilesessiontap_parse.py` & `pyidevice-2.3.32/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/deviceinfo.py` & `pyidevice-2.3.32/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/gpu.py` & `pyidevice-2.3.32/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/graphics.py` & `pyidevice-2.3.32/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/launchAPP.py` & `pyidevice-2.3.32/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/mobileNotifications.py` & `pyidevice-2.3.32/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/netstatPID.py` & `pyidevice-2.3.32/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/networking.py` & `pyidevice-2.3.32/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/sysmontap.py` & `pyidevice-2.3.32/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/instrument_demo/xcuitest.py` & `pyidevice-2.3.32/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/mobile_config.py` & `pyidevice-2.3.32/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/pcapd.py` & `pyidevice-2.3.32/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/screenshotr.py` & `pyidevice-2.3.32/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/demo/syslog.py` & `pyidevice-2.3.32/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/cli/base.py` & `pyidevice-2.3.32/ios_device/cli/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,42 +232,42 @@
             - installedApplicationsMatching:registerUpdateToken:
             - unregisterUpdateToken:
         :return:
         """
         applist = self.instruments.call(InstrumentsService.ApplicationListing,
                                         "installedApplicationsMatching:registerUpdateToken:",
                                         {}, "").selector
-        # ret = applist
         if bundle_id:
             for app in applist:
                 if app.get('CFBundleIdentifier') == bundle_id:
                     return app
-        # return ret
+        return applist
 
     def sysmontap(self,
                   callback: callable,
                   time: int = 1000,
                   stopSignal: threading.Event = threading.Event()):
         """
         :param time: 获取时间间隔（ms）
         :param stopSignal:
         :param callback:
         :return:
         """
-        self.process_attributes = self.process_attributes or list(self.device_info.sysmonProcessAttributes())
-        self.system_attributes = self.system_attributes or list(self.device_info.sysmonSystemAttributes())
 
         log.info(f'Sysmontap setConfig ...')
-        self.instruments.call(InstrumentsService.Sysmontap, "setConfig:", {
+        config = {
             'ur': time,  # 输出频率 ms
             'bm': 0,
-            'procAttrs': self.process_attributes,  # 输出所有进程信息字段，字段顺序与自定义相同（全量自字段，按需使用）
-            'sysAttrs': self.system_attributes,  # 系统信息字段
             'cpuUsage': True,
-            'sampleInterval': time * 1000000})
+            'sampleInterval': time * 1000000}
+        if self.system_attributes:  # 系统信息字段
+            config['sysAttrs'] = self.system_attributes
+        if self.process_attributes:  # 进程信息字段
+            config['procAttrs'] = self.process_attributes
+        self.instruments.call(InstrumentsService.Sysmontap, "setConfig:", config)
         self.instruments.register_channel_callback(InstrumentsService.Sysmontap, callback)
         self.instruments.call(InstrumentsService.Sysmontap, "start")
         log.info(f'Sysmontap start ...')
         log.info(f'wait for data ...')
         while not stopSignal.wait(1):
             pass
         self.instruments.call(InstrumentsService.Sysmontap, "stop")
```

### Comparing `pyidevice-2.3.31/ios_device/cli/cli.py` & `pyidevice-2.3.32/ios_device/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,19 +23,12 @@
         print(buf)
 
 
 class Command(click.Command):
 
     def __init__(self, *args, **kwargs):
         super(Command, self).__init__(*args, **kwargs)
-        self.params = [
+        self.params[:0] = [
             click.Option(('udid', '--udid'), help='specify unique device identifier'),
             click.Option(('network', '--network'), is_flag=True, help='ios devices on wireless network'),
-            click.Option(('format', '--format'), type=click.Choice(['text', 'json', 'flush']),
-                         help='print format type'),
+            click.Option(('format', '--format'),type=click.Choice(['text','json','flush']), help='print format type'),
         ]
-
-    def invoke(self, ctx):
-        # 获取传入的所有参数和选项的名称和值
-        params = ctx.params
-        # 打印传入的所有参数和选项
-        click.echo(params)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyidevice-2.3.31/ios_device/cli/instruments.py` & `pyidevice-2.3.32/ios_device/cli/instruments.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from ios_device.cli.base import InstrumentsBase
 from ios_device.cli.cli import Command, print_json
 from ios_device.util import Log, api_util
 from ios_device.util.exceptions import InstrumentRPCParseError
 from ios_device.util.gpu_decode import JSEvn, TraceData, GRCDecodeOrder, GRCDisplayOrder
 from ios_device.util.kc_data import kc_data_parse
-from ios_device.util.utils import DumpDisk, DumpNetwork, DumpMemory
+from ios_device.util.utils import DumpDisk, DumpNetwork, DumpMemory, convertBytes
 from ios_device.util.variables import LOG, InstrumentsService
 
 log = Log.getLogger(LOG.Instrument.value)
 
 
 @click.group()
 def cli():
@@ -149,26 +149,66 @@
     def _callback(res):
         api_util.network_caller(res, print_json)
 
     with InstrumentsBase(udid=udid, network=network) as rpc:
         rpc.networking(_callback)
 
 
+@instruments.command('appmonitor', cls=Command)
+@click.option('-t', '--time', type=click.INT, default=1000, help='Output interval time (ms)')
+@click.option('-b', '--bundle_id', required=True, help='Process app bundleId to filter')
+def cmd_appmonitor(udid, network, format, time, bundle_id):
+    """ Get application performance data """
+    proc_filter = ['Pid','Name', 'CPU', 'Memory','DiskReads','DiskWrites','Threads']
+    process_attributes = dataclasses.make_dataclass('SystemProcessAttributes', proc_filter)
+    ios_version = 0
+
+    def on_callback_message(res):
+        if isinstance(res.selector, list):
+            for index, row in enumerate(res.selector):
+                if 'Processes' in row:
+                    for _pid, process in row['Processes'].items():
+                        attrs = process_attributes(*process)
+                        if name and attrs.Name != name:
+                            continue
+                        if not attrs.CPU:
+                            attrs.CPU = 0
+                        if ios_version < LooseVersion('14.0'):
+                            attrs.CPU = attrs.CPU * 40
+                        attrs.CPU = f'{round(attrs.CPU, 2)} %'
+                        attrs.Memory = convertBytes(attrs.Memory)
+                        attrs.DiskReads = convertBytes(attrs.DiskReads)
+                        attrs.DiskWrites = convertBytes(attrs.DiskWrites)
+                        print_json(attrs.__dict__, format)
+
+    with InstrumentsBase(udid=udid, network=network) as rpc:
+        ios_version = rpc.lockdown.ios_version
+        rpc.process_attributes = ['pid','name', 'cpuUsage', 'physFootprint',
+                                  'diskBytesRead','diskBytesWritten','threadCount']
+        if bundle_id:
+            app = rpc.application_listing(bundle_id)
+            if not app:
+                print(f"not find {bundle_id}")
+                return
+            name = app.get('ExecutableName')
+        rpc.sysmontap(on_callback_message, time)
+
+
 @instruments.command('sysmontap', cls=Command)
 @click.option('-t', '--time', type=click.INT, default=1000, help='Output interval time (ms)')
 @click.option('-p', '--pid', type=click.INT, default=None, help='Process ID to filter')
 @click.option('-n', '--name', default=None, help='Process app name to filter')
 @click.option('-b', '--bundle_id', default=None, help='Process app bundleId to filter.Omit show all')
 @click.option('--processes', is_flag=True, help='Only output process information')
 @click.option('--sort', help='Process field sorting')
 @click.option('--proc_filter', help='Process param to filter split by ",". Omit show all')
 @click.option('--sys_filter', help='System param to filter split by ",". Omit show all')
 def cmd_sysmontap(udid, network, format, time, pid, name, bundle_id, processes, sort, proc_filter,
                   sys_filter):
-    """ Get performance data """
+    """ Get more performance data """
 
     def on_callback_message(res):
         if isinstance(res.selector, list):
             data = deepcopy(res.selector)
             processes_data = {}
             for index, row in enumerate(res.selector):
                 if 'Processes' in row:
@@ -263,14 +303,15 @@
                 print("Memory  >>", Memory.decode(data))
                 print("Network >>", Network.decode(data))
                 print("Disk    >>", disk.decode(data))
                 print("CPU     >>", SystemCPUUsage)
 
     with InstrumentsBase(udid=udid, network=network) as rpc:
         rpc.process_attributes = ['name', 'pid']
+        rpc.system_attributes = rpc.device_info.sysmonProcessAttributes()
         rpc.sysmontap(on_callback_message)
 
 
 @instruments.group()
 def condition():
     """
     Set system running condition
@@ -413,8 +454,7 @@
 
 
 @instruments.command('app_lifecycle', cls=Command)
 @click.option('-b', '--bundle_id', default=None, help='Process app bundleId')
 def cmd_app_lifecycle(udid, network, format, bundle_id):
     with InstrumentsBase(udid=udid, network=network) as rpc:
         rpc.app_launch_lifecycle(bundle_id)
-
```

### Comparing `pyidevice-2.3.31/ios_device/cli/mobile.py` & `pyidevice-2.3.32/ios_device/cli/mobile.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/py_ios_device.py` & `pyidevice-2.3.32/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/Installation.py` & `pyidevice-2.3.32/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/Instrument.py` & `pyidevice-2.3.32/ios_device/servers/Instrument.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class InstrumentServer(DTXServer):
     def __init__(self, lockdown=None, udid=None, network=None):
         super().__init__()
         self.lockdown = lockdown or LockdownClient(udid=udid, network=network)
 
     def init(self, cli=None):
-        log.info('InstrumentServer init ...')
         if not cli:
             if self.lockdown.ios_version >= LooseVersion('14.0'):
                 cli = self.lockdown.start_service("com.apple.instruments.remoteserver.DVTSecureSocketProxy")
             else:
                 cli = self.lockdown.start_service("com.apple.instruments.remoteserver")
                 if hasattr(cli.sock, '_sslobj'):
                     cli.sock._sslobj = None  # remoteserver 协议配对成功之后，需要关闭 ssl 协议通道，使用明文传输
```

### Comparing `pyidevice-2.3.31/ios_device/servers/afc.py` & `pyidevice-2.3.32/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/amfi.py` & `pyidevice-2.3.32/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/crash_log.py` & `pyidevice-2.3.32/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/diagnostics_relay.py` & `pyidevice-2.3.32/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/dvt.py` & `pyidevice-2.3.32/ios_device/servers/dvt.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     def register_channel_callback(self, channel: str, callback: typing.Callable):
         """
         Return channel messages
         :param channel:
         :param callback
         """
-        log.info(f'set {channel} callback ...')
+        log.debug(f'set {channel} callback ...')
         channel_id = self.make_channel(channel)
         self._channel_callbacks[channel_id] = callback
 
     def register_undefined_callback(self, callback: typing.Callable):
         """
         Returns all undefined messages
         :param callback
```

### Comparing `pyidevice-2.3.31/ios_device/servers/house_arrest.py` & `pyidevice-2.3.32/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/image_mounter.py` & `pyidevice-2.3.32/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/mc_install.py` & `pyidevice-2.3.32/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/notification_proxy.py` & `pyidevice-2.3.32/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/os_trace.py` & `pyidevice-2.3.32/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/pcapd.py` & `pyidevice-2.3.32/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/screenshotr.py` & `pyidevice-2.3.32/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/simulate_location.py` & `pyidevice-2.3.32/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/spring_board.py` & `pyidevice-2.3.32/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/syslog.py` & `pyidevice-2.3.32/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/servers/testmanagerd.py` & `pyidevice-2.3.32/ios_device/servers/testmanagerd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from distutils.version import LooseVersion
 
 from ..servers.dvt import DTXServer
-from ..util.exceptions import StartServiceError
 from ..util.lockdown import LockdownClient
 
 
 class TestManagerdLockdown(DTXServer):
-    def __init__(self, lockdown=None, udid=None, *args, **kw):
-        super().__init__(*args, **kw)
-        self.lockdown = lockdown or LockdownClient(udid=udid)
+    def __init__(self, lockdown=None, udid=None,network=None):
+        super().__init__()
+        self.lockdown = lockdown or LockdownClient(udid=udid,network=network)
 
     def init(self, cli=None):
         if not cli:
             if self.lockdown.ios_version >= LooseVersion('14.0'):
                 cli = self.lockdown.start_service("com.apple.testmanagerd.lockdown.secure")
             else:
                 cli = self.lockdown.start_service("com.apple.testmanagerd.lockdown")
```

### Comparing `pyidevice-2.3.31/ios_device/util/__init__.py` & `pyidevice-2.3.32/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/api_util.py` & `pyidevice-2.3.32/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/bpylist2.py` & `pyidevice-2.3.32/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/ca.py` & `pyidevice-2.3.32/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/constants.py` & `pyidevice-2.3.32/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/dtx_msg.py` & `pyidevice-2.3.32/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/exceptions.py` & `pyidevice-2.3.32/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/forward.py` & `pyidevice-2.3.32/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/gpu_decode.py` & `pyidevice-2.3.32/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/kc_data.py` & `pyidevice-2.3.32/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/kperf_data.py` & `pyidevice-2.3.32/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/lifecycle.py` & `pyidevice-2.3.32/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/lockdown.py` & `pyidevice-2.3.32/ios_device/util/lockdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         except Exception as E:
             log.debug(f'{E}')
             log.debug(f'No iTunes pairing record found for device {self.identifier}')
             log.debug('Getting pair record from usbmuxd')
         with UsbmuxdClient() as usb:
             return usb.get_pair_record(self.udid)
 
+
     def _validate_pairing(self):
         pair_record = self._get_pair_record() or {}
         self.record = pair_record
         if self.ios_version < LooseVersion('11.0'):  # 11 以下需要双向认证
             resp = self._plist_request('ValidatePair', PairRecord=pair_record)
             if not resp or 'Error' in resp:
                 log.error(f'Failed to ValidatePair: {resp}')
@@ -130,15 +131,15 @@
                     usb.delete_pair_record(self.udid)
                 pair_record = self._get_pair_record() or self.pair_full()
                 if not pair_record:
                     return False
 
         if resp.get('EnableSessionSSL'):
             if not pair_record:
-                self.sslfile = get_home_path(self.cache_dir, f'{self.identifier}.pem')
+                self.sslfile = get_home_path(self.cache_dir,f'{self.identifier}.pem')
 
             else:
                 self.sslfile = write_home_file(
                     self.cache_dir,
                     f'{self.identifier}.pem',
                     pair_record['HostCertificate'] + b'\n' + pair_record['HostPrivateKey']
                 )
```

### Comparing `pyidevice-2.3.31/ios_device/util/plist_service.py` & `pyidevice-2.3.32/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/plistlib.py` & `pyidevice-2.3.32/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/usbmux.py` & `pyidevice-2.3.32/ios_device/util/usbmux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 USBMux client that handles iDevice descovery via USB.
 
 :author: Doug Skrypa (original: Hector Martin "marcan" <hector@marcansoft.com>)
 """
 from .variables import LOG
-from ..util import Log
+from ..util import  Log
 import select
 import socket
 import struct
 import sys
 import plistlib
 from typing import Dict, Union, Optional, Tuple, Any, Mapping, List
 
@@ -165,21 +165,21 @@
             )
         return self.devices
 
     def connect(self, dev, port):
         connector = MuxConnection(self.socketpath, self.protoclass)
         return connector.connect(dev, port)
 
+
     def listen_device(self):
         self.listener.listen()
         while True:
             data = self.listener.proto.getpacket()
             yield data
 
-
 class UsbmuxdClient(MuxConnection):
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
@@ -232,14 +232,15 @@
         self.proto.sendpacket('ReadBUID', tag, payload)
         _, recvtag, data = self.proto.getpacket()
         if recvtag != tag:
             raise MuxError('Reply tag mismatch: expected %d, got %d' % (tag, recvtag))
         return data['BUID']
 
 
+
 class BinaryProtocol:
     TYPE_RESULT = 1
     TYPE_CONNECT = 2
     TYPE_LISTEN = 3
     TYPE_DEVICE_ADD = 4
     TYPE_DEVICE_REMOVE = 5
     TYPE_DEVICE_LIST = 6
```

### Comparing `pyidevice-2.3.31/ios_device/util/utils.py` & `pyidevice-2.3.32/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/ios_device/util/variables.py` & `pyidevice-2.3.32/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.31/pyidevice.egg-info/PKG-INFO` & `pyidevice-2.3.32/pyidevice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyidevice
-Version: 2.3.31
+Version: 2.3.32
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
-Maintainer: chenpeijie
-Maintainer-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,15 +29,15 @@
 
 ## pip :
     pip install py-ios-device
     
 python version: 3.7 +
 ### Instruments：
 - [x] Get system Memory and CPU data
-- [x] Get processes Memory and CPU data
+- [x] Get application Memory and CPU data
 - [x] Get FPS data
 - [x] Get network data
 - [x] Set the device network status. eg: 2G, 3G ,100% Loss
 - [x] Set the device behaves as though under a high thermal state
 - [x] Monitoring app start、exit、background
 - [x] Launch and Kill app
 - [x] Run xctest. eg: WebDriverAgent
@@ -88,24 +86,29 @@
 Disk    >> {'Data Read': '117.91 GiB', 'Data Read/sec': 0, 'Data Written': '64.28 GiB', 'Data Written/sec': 0, 'Reads in': 9734132, 'Reads in/sec': 9734132, 'Writes Out': 6810640, 'Writes Out/sec': 6810640}
 
 $ pyidevice instruments monitor --filter = memory
 Memory  >> {'App Memory': '699.69 MiB', 'Cached Files': '1.48 GiB', 'Compressed': '155.17 MiB', 'Memory Used': '1.42 GiB', 'Wired Memory': '427.91 MiB', 'Swap Used': '46.25 MiB'}
 
 ```
 
+#### Get application performance data
 
+```bash
+$ pyidevice instruments appmonitor  -b cn.rongcloud.im
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '0 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.28 MiB', 'Threads': 13}
+{'Pid': 30897, 'Name': 'SealTalk', 'CPU': '3.4 %', 'Memory': '35.72 MiB', 'DiskReads': '24.12 MiB', 'DiskWrites': '2.30 MiB', 'Threads': 13}
+```
 
-#### Get Processes performance data
-
+#### Get custom application performance data
 ```bash
 $ pyidevice instruments sysmontap --help
-$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter memVirtualSize,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
+$ pyidevice instruments sysmontap  -b com.tencent.xin --proc_filter physFootprint,cpuUsage --processes --sort cpuUsage # 只显示 memVirtualSize,cpuUsage 参数的进程列表，且根据 cpuUsage 字段排序 
 
-[('WeChat', {'cpuUsage': 0.03663705586691998, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
-[('WeChat', {'cpuUsage': 0.036558268613227536, 'memVirtualSize': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.03663705586691998, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
+[('WeChat', {'cpuUsage': 0.036558268613227536, 'physFootprint': 2179284992, 'name': 'WeChat', 'pid': 99269})]
 
 
 ```
 #### Get FPS data
 
 ```bash
 $ pyidevice instruments fps
```

### Comparing `pyidevice-2.3.31/pyidevice.egg-info/SOURCES.txt` & `pyidevice-2.3.32/pyidevice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+setup2.py
 ./ios_device/__init__.py
 ./ios_device/__version__.py
 ./ios_device/main.py
 ./ios_device/py_ios_device.py
 demo/__init__.py
 demo/afc.py
 demo/crash_log.py
```

### Comparing `pyidevice-2.3.31/setup.py` & `pyidevice-2.3.32/setup2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-
-from setuptools import setup
+"""
+@Date    : 2020-12-18
+@Author  : liyachao
+"""
+from setuptools import setup, find_packages
 from ios_device import __version__
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 
 setup(name='pyidevice',
       version=__version__,
       description='Get ios data and operate ios devices',
       author='chenpeijie',
       author_email='cpjsf@163.com',
-      maintainer='chenpeijie',
-      maintainer_email='',
       url='https://github.com/YueChen-C/py-ios-device',
-      packages=["pyidevice"],
+      packages=['pyidevice'],
       package_dir={"pyidevice": "ios_device"},
+      include_package_data=True,
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       install_requires=REQUIREMENTS,
       python_requires=">=3.7",
-      include_package_data=True,
       classifiers=[
           "Programming Language :: Python :: 3",
           "Operating System :: OS Independent",
       ],
       entry_points={
           'console_scripts':{
               'pyidevice=ios_device.main:cli'
```

