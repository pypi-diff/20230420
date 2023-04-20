# Comparing `tmp/lnxlink-2023.4.0.tar.gz` & `tmp/lnxlink-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.4.0.tar", last modified: Fri Mar 31 20:02:47 2023, max compression
+gzip compressed data, was "lnxlink-2023.4.1.tar", last modified: Thu Apr 20 18:41:29 2023, max compression
```

## Comparing `lnxlink-2023.4.0.tar` & `lnxlink-2023.4.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12382 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/network_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/network_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/nvidia_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 20:02:47.000000 lnxlink-2023.4.0/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-03-31 20:02:30.000000 lnxlink-2023.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-31 20:02:47.898432 lnxlink-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.613223 lnxlink-2023.4.1/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12635 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/network_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/network_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/nvidia_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:29.613223 lnxlink-2023.4.1/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-20 18:41:28.000000 lnxlink-2023.4.1/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 18:41:29.000000 lnxlink-2023.4.1/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-04-20 18:41:16.000000 lnxlink-2023.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 18:41:29.617223 lnxlink-2023.4.1/setup.cfg
```

### Comparing `lnxlink-2023.4.0/LICENSE.md` & `lnxlink-2023.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/PKG-INFO` & `lnxlink-2023.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
@@ -32,16 +32,16 @@
  * [Installation](#installation)
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
- - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam.
+ - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
@@ -188,7 +188,16 @@
  - xdotool
  - shutdown
  - systemctl
  - xprintidle
  - xdg-open
  - upower
  - xset
+
+## Use Boot Select addon
+This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
+```bash
+# Edit the sudoers file:
+sudo visudo
+# Add this line at the end (replace USER with your username):
+USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
+```
```

### Comparing `lnxlink-2023.4.0/README.md` & `lnxlink-2023.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
  * [Installation](#installation)
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
- - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam.
+ - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
@@ -172,7 +172,16 @@
  - xdotool
  - shutdown
  - systemctl
  - xprintidle
  - xdg-open
  - upower
  - xset
+
+## Use Boot Select addon
+This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
+```bash
+# Edit the sudoers file:
+sudo visudo
+# Add this line at the end (replace USER with your username):
+USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
+```
```

### Comparing `lnxlink-2023.4.0/lnxlink/__main__.py` & `lnxlink-2023.4.1/lnxlink/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,19 @@
         self.client = mqtt.Client()
         self.setup_mqtt()
 
     def publish_monitor_data(self, topic, pub_data):
         # print(topic, pub_data, type(pub_data))
         if pub_data is None:
             return
-        if pub_data == True:
-            pub_data = 'ON'
-        if pub_data == False:
-            pub_data = 'OFF'
+        if isinstance(pub_data, bool):
+            if pub_data is True:
+                pub_data = 'ON'
+            if pub_data is False:
+                pub_data = 'OFF'
         if type(pub_data) in [dict, list]:
             pub_data = json.dumps(pub_data)
         self.client.publish(
             topic,
             payload=pub_data,
             retain=self.config['mqtt']['lwt']['retain']
         )
@@ -151,15 +152,15 @@
                     retain=self.config['mqtt']['lwt']['retain']
                 )
 
     def on_message(self, client, userdata, msg):
         '''MQTT message is received with a module command to excecute'''
         topic = msg.topic.replace(f"{self.pref_topic}/commands/", "")
         message = msg.payload
-        print(f"Message received: {topic}")
+        print(f"Message received {topic}: {message}")
         try:
             message = json.loads(message)
         except Exception as e:
             message = message.decode()
             # print("String could not be converted to JSON")
             # traceback.print_exc()
 
@@ -211,33 +212,36 @@
         '''Send discovery information on Home Assistant for controls'''
         subtopic = addon.name.lower().replace(' ', '/')
         state_topic = f"{self.pref_topic}/monitor_controls/{subtopic}"
         discovery = discovery_template.copy()
         discovery['name'] = f"{self.config['mqtt']['clientId']} {control_name}"
         discovery['unique_id'] = f"{self.config['mqtt']['clientId']}_{control_name.lower().replace(' ', '_')}"
         discovery['enabled_by_default'] = options.get('enabled', True)
-        discovery["command_topic"] = f"{self.pref_topic}/commands/{service}/{control_name.lower().replace(' ', '_')}/"
+        discovery["command_topic"] = f"{self.pref_topic}/commands/{service}/{control_name.replace(' ', '_')}/"
         if 'value_template' in options:
             discovery["value_template"] = options['value_template']
         if 'icon' in options:
             discovery['icon'] = options.get('icon', '')
 
-
         if options['type'] == 'button':
             discovery['state_topic'] = f"{self.pref_topic}/lwt"
         elif options['type'] == 'switch':
             discovery["state_topic"] = state_topic
             discovery["payload_off"] = "OFF"
             discovery["payload_on"] = "ON"
         elif options['type'] == 'text':
             discovery["state_topic"] = state_topic
         elif options['type'] == 'number':
             discovery["state_topic"] = state_topic
             discovery["min"] = options.get('min', 1)
             discovery["max"] = options.get('max', 100)
+            discovery["step"] = options.get('step', 1)
+        elif options['type'] == 'select':
+            discovery["state_topic"] = state_topic
+            discovery["options"] = addon.options
         else:
             return
         self.client.publish(
             f"homeassistant/{options['type']}/lnxlink/{discovery['unique_id']}/config",
             payload=json.dumps(discovery),
             retain=self.config['mqtt']['lwt']['retain'])
```

### Comparing `lnxlink-2023.4.0/lnxlink/config.py` & `lnxlink-2023.4.1/lnxlink/config.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/consts.py` & `lnxlink-2023.4.1/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/__init__.py` & `lnxlink-2023.4.1/lnxlink/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/battery.py` & `lnxlink-2023.4.1/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/camera_used.py` & `lnxlink-2023.4.1/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/disk_usage.py` & `lnxlink-2023.4.1/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/keep_alive.py` & `lnxlink-2023.4.1/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/media.py` & `lnxlink-2023.4.1/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/network_download.py` & `lnxlink-2023.4.1/lnxlink/modules/network_download.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/network_upload.py` & `lnxlink-2023.4.1/lnxlink/modules/network_upload.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/notify.py` & `lnxlink-2023.4.1/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/nvidia_gpu.py` & `lnxlink-2023.4.1/lnxlink/modules/nvidia_gpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.4.1/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/sys_updates.py` & `lnxlink-2023.4.1/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/update.py` & `lnxlink-2023.4.1/lnxlink/modules/update.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/modules/webcam.py` & `lnxlink-2023.4.1/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink/system_monitor.py` & `lnxlink-2023.4.1/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.4.0/lnxlink.egg-info/PKG-INFO` & `lnxlink-2023.4.1/lnxlink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
@@ -32,16 +32,16 @@
  * [Installation](#installation)
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
- - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam.
+ - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
@@ -188,7 +188,16 @@
  - xdotool
  - shutdown
  - systemctl
  - xprintidle
  - xdg-open
  - upower
  - xset
+
+## Use Boot Select addon
+This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
+```bash
+# Edit the sudoers file:
+sudo visudo
+# Add this line at the end (replace USER with your username):
+USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
+```
```

### Comparing `lnxlink-2023.4.0/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.4.1/lnxlink.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 lnxlink.egg-info/dependency_links.txt
 lnxlink.egg-info/entry_points.txt
 lnxlink.egg-info/requires.txt
 lnxlink.egg-info/top_level.txt
 lnxlink/modules/__init__.py
 lnxlink/modules/bash.py
 lnxlink/modules/battery.py
+lnxlink/modules/boot_select.py
+lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
 lnxlink/modules/idle.py
 lnxlink/modules/keep_alive.py
 lnxlink/modules/media.py
 lnxlink/modules/memory.py
@@ -27,14 +29,15 @@
 lnxlink/modules/network_download.py
 lnxlink/modules/network_upload.py
 lnxlink/modules/notify.py
 lnxlink/modules/nvidia_gpu.py
 lnxlink/modules/required_restart.py
 lnxlink/modules/restart.py
 lnxlink/modules/screen_onoff.py
+lnxlink/modules/screenshot.py
 lnxlink/modules/send_keys.py
 lnxlink/modules/shutdown.py
 lnxlink/modules/suspend.py
 lnxlink/modules/sys_updates.py
 lnxlink/modules/update.py
 lnxlink/modules/webcam.py
 lnxlink/modules/xdg_open.py
```

### Comparing `lnxlink-2023.4.0/pyproject.toml` & `lnxlink-2023.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.4.0"
+version           = "2023.4.1"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
```

