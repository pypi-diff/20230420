# Comparing `tmp/ja2mqtt-1.0.1.tar.gz` & `tmp/ja2mqtt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja2mqtt-1.0.1.tar", last modified: Tue Apr 18 11:06:54 2023, max compression
+gzip compressed data, was "ja2mqtt-1.0.2.tar", last modified: Thu Apr 20 20:58:26 2023, max compression
```

## Comparing `ja2mqtt-1.0.1.tar` & `ja2mqtt-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,43 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.697172 ja2mqtt-1.0.1/
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.690805 ja2mqtt-1.0.1/.github/
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.692130 ja2mqtt-1.0.1/.github/workflows/
--rw-r--r--   0 tomas      (501) staff       (20)     1288 2023-04-18 10:58:21.000000 ja2mqtt-1.0.1/.github/workflows/docker-image.yml
--rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/.gitignore
--rw-r--r--   0 tomas      (501) staff       (20)      631 2023-04-18 10:56:21.000000 ja2mqtt-1.0.1/Makefile
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 11:06:54.697040 ja2mqtt-1.0.1/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 10:18:37.000000 ja2mqtt-1.0.1/README-pypi.text
--rw-r--r--   0 tomas      (501) staff       (20)     4113 2023-04-18 09:35:34.000000 ja2mqtt-1.0.1/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.693380 ja2mqtt-1.0.1/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/env.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/ja2mqtt
--rw-r--r--   0 tomas      (501) staff       (20)      178 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/requirements.txt
--rwxr-xr-x   0 tomas      (501) staff       (20)      193 2023-04-14 16:09:33.000000 ja2mqtt-1.0.1/bin/venv-create.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       29 2023-04-14 16:09:33.000000 ja2mqtt-1.0.1/bin/venv-freeze.sh
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.693834 ja2mqtt-1.0.1/config/
--rw-r--r--   0 tomas      (501) staff       (20)     3335 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/config/ja2mqtt.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     1174 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/config/sample-config.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.694098 ja2mqtt-1.0.1/docker/
--rw-r--r--   0 tomas      (501) staff       (20)      935 2023-04-18 08:38:57.000000 ja2mqtt-1.0.1/docker/Dockerfile
--rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 00:34:56.000000 ja2mqtt-1.0.1/docker/docker-compose.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.694460 ja2mqtt-1.0.1/docker/mqtt-config/
--rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/docker/mqtt-config/mosquitto.conf
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.695134 ja2mqtt-1.0.1/ja2mqtt/
--rwxr-xr-x   0 tomas      (501) staff       (20)      218 2023-04-18 11:06:28.000000 ja2mqtt-1.0.1/ja2mqtt/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      788 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/__main__.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.696190 ja2mqtt-1.0.1/ja2mqtt/commands/
--rw-r--r--   0 tomas      (501) staff       (20)     2539 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      875 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/config.py
--rw-r--r--   0 tomas      (501) staff       (20)      869 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/run.py
--rw-r--r--   0 tomas      (501) staff       (20)     1697 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/test.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.696862 ja2mqtt-1.0.1/ja2mqtt/components/
--rw-r--r--   0 tomas      (501) staff       (20)      786 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     8485 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/bridge.py
--rw-r--r--   0 tomas      (501) staff       (20)     5096 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     4879 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/serial.py
--rw-r--r--   0 tomas      (501) staff       (20)     5255 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/simulator.py
--rw-r--r--   0 tomas      (501) staff       (20)    12675 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     7450 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/utils.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.695687 ja2mqtt-1.0.1/ja2mqtt.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      779 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-18 11:06:54.697201 ja2mqtt-1.0.1/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1454 2023-04-18 10:18:52.000000 ja2mqtt-1.0.1/setup.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.125399 ja2mqtt-1.0.2/
+-rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/MANIFEST.in
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-20 20:58:26.125239 ja2mqtt-1.0.2/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/README-pypi.text
+-rw-r--r--   0 tomas      (501) staff       (20)     5471 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/README.md
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.119941 ja2mqtt-1.0.2/bin/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/bin/env.sh
+-rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/bin/ja2mqtt
+-rw-r--r--   0 tomas      (501) staff       (20)      107 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements-dev.txt
+-rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements-setup-py.sh
+-rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/bin/requirements.txt
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.120272 ja2mqtt-1.0.2/config/
+-rw-r--r--   0 tomas      (501) staff       (20)     3676 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/config/ja2mqtt.yaml
+-rw-r--r--   0 tomas      (501) staff       (20)     1852 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/config/sample-config.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.120694 ja2mqtt-1.0.2/docker/
+-rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/docker/Dockerfile
+-rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.2/docker/docker-compose.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.121148 ja2mqtt-1.0.2/docker/mqtt-config/
+-rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/docker/mqtt-config/mosquitto.conf
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.122295 ja2mqtt-1.0.2/ja2mqtt/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      218 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)      831 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/__main__.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.123896 ja2mqtt-1.0.2/ja2mqtt/commands/
+-rw-r--r--   0 tomas      (501) staff       (20)     2642 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1308 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)      883 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/run.py
+-rw-r--r--   0 tomas      (501) staff       (20)     2528 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/commands/test.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.124958 ja2mqtt-1.0.2/ja2mqtt/components/
+-rw-r--r--   0 tomas      (501) staff       (20)      786 2023-04-17 22:42:29.000000 ja2mqtt-1.0.2/ja2mqtt/components/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)    10530 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/components/bridge.py
+-rw-r--r--   0 tomas      (501) staff       (20)     5626 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)     7962 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/components/serial.py
+-rw-r--r--   0 tomas      (501) staff       (20)     6022 2023-04-20 20:26:08.000000 ja2mqtt-1.0.2/ja2mqtt/components/simulator.py
+-rw-r--r--   0 tomas      (501) staff       (20)    13192 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.2/ja2mqtt/utils.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-20 20:58:26.122990 ja2mqtt-1.0.2/ja2mqtt.egg-info/
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)      752 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-20 20:58:26.000000 ja2mqtt-1.0.2/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-20 20:58:26.125443 ja2mqtt-1.0.2/setup.cfg
+-rw-r--r--   0 tomas      (501) staff       (20)     1454 2023-04-18 13:03:48.000000 ja2mqtt-1.0.2/setup.py
```

### Comparing `ja2mqtt-1.0.1/PKG-INFO` & `ja2mqtt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.1/README-pypi.text` & `ja2mqtt-1.0.2/README-pypi.text`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.1/README.md` & `ja2mqtt-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,52 @@
 
 ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
 
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
 
 If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
 
+## Features
+
+* Define Jablotron topology in the YAML configuration file, including sections with their codes, names, and peripherals' positions and names.
+* Implement declarative rules in the ja2mqtt.yaml configuration file to support the serial JA-121T protocol.
+* Read events from Jablotron, such as section arming and disarming, peripheral state changes, and convert them to MQTT events.
+* Use MQTT events to query section states and correlate request and response MQTT events.
+* Implement automated recovery from serial interface failures or MQTT broker connection failures.
+* JA-121T simulator that simulates section state changes, peripheral state changes and heartbeat messages. 
+
 ## Testing using Docker
 
 To test ja2mqtt with the JA-121T simulator, you can utilize the ja2mqtt Docker image that comes with pre-configured settings. The simulator provides a straightforward Jablotron topology with two sections: "House" with code "1" and an initial state of "ARMED", and "Garage" with code "2" and an initial state of "READY". This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
 
-In  order to test ja2mqtt with the simulator, follow the below steps.
+To test ja2mqtt with the simulator, follow the steps below.
 
 1. Run the `docker-compose.yaml` provided in the [docker](https://github.com/tomvit/ja2mqtt/tree/master/docker) directory.
 
    ```
    $ docker-compose up -d
    ```
 
+2. Inspect the logs of ja2mqtt by running the following command:
+
+   ```
+   $ docker logs ja2mqtt
+   ```
+
+3. Publish the MQTT event to retrieve the state of sections as follows:
+
+   ```
+   $ docker exec -it ja2mqtt pub -t ja2mqtt/section/get -d pin=1234
+   <-- send: ja2mqtt/section/get: {"pin": "1234", "corrid": "ca8438b82f16"}
+   --> recv: ja2mqtt/section/house: {"corrid": "ca8438b82f16", "section_code": 1, "section_name": "house", "state": "ARMED"}
+   --> recv: ja2mqtt/section/garage: {"corrid": "ca8438b82f16", "section_code": 2, "section_name": "garage", "state": "READY"}   
+   ```
+
+4. Check the log entries in the ja2mqtt log again to see if the events were generated.
+
 2. Inspect logs of ja2mqtt by running the following command:
 
    ```
    $ docker logs ja2mqtt -f
    ```
 
 3. Publish the mqtt event to retrieve a state of sections as follows:
@@ -34,15 +60,14 @@
 
 4. Check log entries in the ja2mqtt log to see that the following entries are present:
 
    ```
    2023-04-17 21:59:46,203 [mqtt    ] [I] <-- send: ja2mqtt/section/house, data={"section_code": 1, "section_name": "house", "state": "ARMED"}
    2023-04-17 21:59:46,408 [mqtt    ] [I] <-- send: ja2mqtt/section/garage, data={"section_code": 2, "section_name": "garage", "state": "READY"}
    ```
-
 ## Getting Started
 
 To use ja2mqtt, you will need:
 
 * Jablotron alarms with the control unit and the JA-121T serial interface connected to a serial port on your computer. The device uses RS485 interface, which can be connected to your computer using a [USB to RS485 adapter](https://www.aliexpress.com/w/wholesale-ch340-usb-rs485.html).
 
 * A running instance of an MQTT broker. [Mosquitto](https://mosquitto.org/) is the recommended MQTT broker, but others should also work without issues. You can run the MQTT broker on the same machine as ja2mqtt, on a separate machine, or use an existing instance of MQTT broker if you have one.
```

### Comparing `ja2mqtt-1.0.1/config/ja2mqtt.yaml` & `ja2mqtt-1.0.2/config/ja2mqtt.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,27 @@
   - read: !py pattern('STATE {{ v }} (READY|ARMED_PART|ARMED|SERVICE|BLOCKED|OFF)')
     write:
       section_code: {{ v }}
       section_name: {{ k }}
       state: !py data.match.group(1)
 {% endfor %}
 
+{% for v in topology.peripheral if v.type == 'motion-sensor' %}
+- name: ja2mqtt/motion/{{ v.name }}
+  rules:
+  - read: !py prf_state({'{{ v['pos'] }}':'ON'})
+    write:
+      name: {{ v.name }}
+      type: {{ v.type }}
+      pos: {{ v.pos }}
+
+    # allow to process next rule when this rule matches
+    process_next_rule: True
+{% endfor %}
+
 # generic error
 - name: ja2mqtt/error
   rules:
   - read: !py pattern('ERROR. ([0-9]+) (.+)')
     write:
       error_number: !py data.match.group(1)
       error_message: !py data.match.group(2)
```

### Comparing `ja2mqtt-1.0.1/docker/Dockerfile` & `ja2mqtt-1.0.2/docker/Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,21 @@
 RUN cd /opt/ja2mqtt && \
   mkdir config && \
   mkdir logs && \
   pip install install/ja2mqtt-*.tar.gz && \
   rm -fr /opt/ja2mqtt/install
 
 # copy default ja2mqtt configuration
-COPY files/sample-config.yaml /opt/ja2mqtt/config
+COPY files/sample-config.yaml /opt/ja2mqtt/config/config.yaml
 COPY files/ja2mqtt.yaml /opt/ja2mqtt/config
 
 # create helper scripts
-RUN echo -e "#!/bin/sh\n/usr/bin/ja2mqtt pub -c /opt/ja2mqtt/config/sample-config.yaml \$*">/usr/bin/pub && \
+RUN echo -e "#!/bin/sh\n/usr/bin/ja2mqtt pub \$*">/usr/bin/pub && \
   chmod +x /usr/bin/pub
 
+ENV JA2MQTT_CONFIG=config/config.yaml
+ENV JA2MQTT_NO_ANSI=True
+ENV JA2MQTT_DEBUG=False
+
 # start the command on running the container
 WORKDIR /opt/ja2mqtt
-CMD [ "/usr/bin/ja2mqtt", "--debug", "run", "-c", "config/sample-config.yaml" ]
+CMD [ "/usr/bin/ja2mqtt", "run", "-c", "config/config.yaml" ]
```

### Comparing `ja2mqtt-1.0.1/docker/mqtt-config/mosquitto.conf` & `ja2mqtt-1.0.2/docker/mqtt-config/mosquitto.conf`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.1/ja2mqtt/__main__.py` & `ja2mqtt-1.0.2/ja2mqtt/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import traceback
 
 import click
 
 import ja2mqtt.config as ja2mqtt_config
 
 from .commands import ja2mqtt
-from .utils import Map
+from .utils import Map, bcolors, format_str_color
 
 
 def signal_quit(signal, frame):
     """
     Function called when process ends when any signal is received. The function
     sets the `exit_event` so that all worker threads using the event can gracefully end.
     """
@@ -23,12 +23,13 @@
 # register `signal_quit` function for all signals.
 for sig in ("TERM", "HUP", "INT"):
     signal.signal(getattr(signal, "SIG" + sig), signal_quit)
 
 try:
     ja2mqtt(prog_name="ja2mqtt")
 except Exception as e:
-    sys.stderr.write(f"ERROR: {str(e)}\n")
-    if ja2mqtt_config.DEBUG:
-        print("---")
-        traceback.print_exc()
-        print("---")
+    sys.stderr.write(
+        format_str_color(
+            f"ERROR: {str(e)}\n", bcolors.ERROR, not ja2mqtt_config.ANSI_COLORS
+        )
+    )
+    sys.exit(1)
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.2/ja2mqtt/commands/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,23 +19,25 @@
         self.params.insert(
             0,
             Option(
                 ("-c", "--config"),
                 metavar="<file>",
                 required=True,
                 help="Configuration file",
+                default=ja2mqtt_config.CONFIG_FILE,
             ),
         )
         self.params.insert(
             0,
             Option(
                 ("-e", "--env"),
                 metavar="<file>",
                 required=False,
                 help="Environment variable file",
+                default=ja2mqtt_config.CONFIG_ENV,
             ),
         )
 
     def init_logging(self, config):
         init_logging(
             config.get_dir_path(config.root("logs")),
             "run",
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.2/ja2mqtt/commands/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     serial = Serial(config)
     mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config)
     bridge = SerialMQTTBridge(config)
 
     bridge.set_mqtt(mqtt)
     bridge.set_serial(serial)
 
-    mqtt.start(ja2mqtt_config.exit_event)
-    serial.start(ja2mqtt_config.exit_event)
+    for x in (mqtt, serial, bridge):
+        x.start(ja2mqtt_config.exit_event)
 
-    mqtt.join()
-    serial.join()
+    for x in (mqtt, serial, bridge):
+        x.join()
 
     log.info("Done.")
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/commands/test.py` & `ja2mqtt-1.0.2/ja2mqtt/commands/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # @author: Tomas Vitvar, https://vitvar.com, tomas@vitvar.com
 
 from __future__ import absolute_import, unicode_literals
 
 import json
 import logging
 import time
+import sys
 
 import click
 
 import ja2mqtt.config as ja2mqtt_config
 from ja2mqtt import __version__ as version
 from ja2mqtt.components import MQTT
-from ja2mqtt.config import Config, init_logging, ja2mqtt_def
+from ja2mqtt.config import Config, init_logging, ja2mqtt_def, correlation_id
 from ja2mqtt.utils import Map, dict_from_string, randomString
 
 from . import BaseCommandLogOnly
 
 
 @click.command("pub", help="Publish a ja2mqtt topic in MQTT.", cls=BaseCommandLogOnly)
 @click.option(
@@ -33,30 +34,55 @@
     "--data",
     "data",
     multiple=True,
     metavar="<d1 d2 ...>",
     required=False,
     help="Data as a key=value pair",
 )
-def command_publish(config, topic, data, log):
+@click.option(
+    "--timeout",
+    "timeout",
+    metavar="<timeout>",
+    required=False,
+    type=float,
+    help="Timeout to wait for responses. The default is correlation timeout from the ja2mqtt configuration.",
+)
+def command_publish(config, topic, data, log, timeout):
     ja2mqtt = ja2mqtt_def(config)
     _topic = next(filter(lambda x: x["name"] == topic, ja2mqtt("mqtt2serial")), None)
     if _topic is None:
         raise Exception(
             f"The topic with name '{topic}' does not exist in the ja2mqtt definition file!"
         )
 
     _data = {}
     for d in data:
         _data = dict_from_string(d, _data)
 
-    cor_id = ja2mqtt("options.correlation_id", None)
-    if cor_id is not None:
-        _data[cor_id] = randomString(12, letters="abcdef0123456789")
+    field, id = correlation_id(ja2mqtt.root)
+    if field is not None:
+        _data[field] = id
+
+    def _wait_for_response(topic, payload):
+        data = Map(json.loads(payload))
+        if field is None or data.get(field) == id:
+            print(f"--> recv: {topic}: {payload}")
+
+    def _on_connect(client, userdata, flags, rc):
+        for topic in ja2mqtt.root("serial2mqtt"):
+            client.subscribe(topic["name"])
 
     mqtt = MQTT(f"ja2mqtt-test-{randomString(5)}", config)
+    mqtt.on_message_ext = _wait_for_response
+    mqtt.on_connect_ext = _on_connect
     mqtt.start(ja2mqtt_config.exit_event)
     try:
         mqtt.wait_is_connected(ja2mqtt_config.exit_event)
+        print(f"<-- send: {_topic['name']}: {json.dumps(_data)}")
         mqtt.publish(_topic["name"], json.dumps(_data))
+        time.sleep(
+            ja2mqtt.root("system.correlation_timeout", 1.5)
+            if timeout is None
+            else timeout
+        )
     finally:
         ja2mqtt_config.exit_event.set()
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.2/ja2mqtt/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.1/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.2/ja2mqtt/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,222 +1,290 @@
 # -*- coding: utf-8 -*-
 # @author: Tomas Vitvar, https://vitvar.com, tomas@vitvar.com
 
 from __future__ import absolute_import, unicode_literals
 
-import json
-import logging
+import random
 import re
+import string
 import threading
 import time
-from queue import Queue
+from functools import reduce
 
-import paho.mqtt.client as mqtt
 
-from ja2mqtt.config import Config
-from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
+class bcolors:
+    HEADER = "\033[95m"
+    OKBLUE = "\033[94m"
+    OKGREEN = "\033[32m"
+    WARNING = "\033[33m"
+    ERROR = "\033[91m"
+    ENDC = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+    LIGHTGRAY = "\033[90m"
+    MAGENTA = "\033[35m"
+
+
+def format_str_color(str, color, disable=False):
+    color = None if disable else color
+    return (
+        (color if color is not None else "")
+        + str
+        + (bcolors.ENDC if color is not None else "")
+    )
+
+
+class PythonExpression:
+    def __init__(self, expr):
+        self.expr_str = expr
+        self.expr = self.compile()
+
+    def compile(self):
+        return compile(self.expr_str, "<string>", "eval")
+
+    def eval(self, scope):
+        return eval(self.expr, {}, scope)
+
+    def __getstate__(self):
+        return (self.expr_str, None)
+
+    def __setstate__(self, state):
+        self.expr_str, _ = state
+        self.expr = self.compile()
 
-from . import Component
-from .simulator import Simulator
+    def __str__(self):
+        return "!py %s" % self.expr_str
 
 
-class Pattern:
-    def __init__(self, pattern):
-        self.match = None
-        self.pattern = pattern
-        self.re = re.compile(self.pattern)
+MAP_IGNORE_KEY_ERROR = True
 
-    def __str__(self):
-        return f"r'{self.pattern}'" if self.match is None else self.match.group(0)
 
-    def __eq__(self, other):
-        self.match = self.re.match(other)
-        return self.match is not None
-
-
-class Topic:
-    def __init__(self, topic):
-        self.name = topic["name"]
-        self.disabled = topic.get("disabled", False)
-        self.rules = []
-        for rule_def in topic["rules"]:
-            self.rules.append(Map(rule_def))
-
-    def check_rule_data(self, read, data, scope, path=None):
-        if path is None:
-            path = []
-        try:
-            for k, v in read.items():
-                path += [k]
-                if k not in data.keys():
-                    raise Exception(f"Missing property {k}.")
-                else:
-                    if not isinstance(v, PythonExpression) and type(v) != type(data[k]):
-                        raise Exception(
-                            f"Invalid type of property {'.'.join(path)}, found: {type(data[k]).__name__}, expected: {type(v).__name__}"
-                        )
-                    if type(v) == dict:
-                        self.check_rule_data(v, data[k], scope, path)
+# *** helper Map object
+class Map(dict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__set_data__(*args, **kwargs)
+
+    def __set_data__(self, *args, **kwargs):
+        for arg in args:
+            if isinstance(arg, dict):
+                for k, v in arg.items():
+                    if isinstance(v, dict):
+                        self[k] = Map(v)
                     else:
-                        if isinstance(v, PythonExpression):
-                            v = v.eval(scope)
-                        if v != data[k]:
-                            raise Exception(
-                                f"Invalid value of property {'.'.join(path)}, found: {data[k]}, exepcted: {v}"
-                            )
+                        self[k] = v
+
+        if kwargs:
+            for k, v in kwargs.items():
+                if isinstance(v, dict):
+                    self[k] = Map(v)
+                else:
+                    self[k] = v
+
+    def __getattr__(self, attr):
+        a = self.get(attr)
+        if a is None and not MAP_IGNORE_KEY_ERROR:
+            raise KeyError(f'The key "{attr}" is undefined!')
+        return a
+
+    def __setattr__(self, key, value):
+        self.__setitem__(key, value)
+
+    def __delattr__(self, item):
+        self.__delitem__(item)
+
+    def __setitem__(self, key, value):
+        super(Map, self).__setitem__(key, value)
+        self.__dict__.update({key: value})
+
+    def __delitem__(self, key):
+        super(Map, self).__delitem__(key)
+        del self.__dict__[key]
+
+    def to_json(self, encoder=None, exclude=[]):
+        d = {k: v for k, v in self.__dict__.items() if k not in exclude}
+        return json.dumps(d, skipkeys=True, cls=encoder)
+
+    def update(self, map):
+        if isinstance(map, Map):
+            self.__dict__.update(map.__dict__)
+        if isinstance(map, dict):
+            self.__dict__.update(map)
+
+    def search(self, callback, item=None, expand=None, data=None):
+        if item == None:
+            item = self
+        if isinstance(item, dict):
+            for k, v in item.items():
+                if not expand or expand(k):
+                    data = self.search(callback, v, expand, callback(k, v, data))
+        if isinstance(item, list):
+            for v in item:
+                data = self.search(callback, v, expand, data)
+        return data
+
+
+def deep_eval(data, scope, raise_ex=False):
+    if isinstance(data, dict):
+        for key, value in data.items():
+            data[key] = deep_eval(value, scope, raise_ex)
+    elif isinstance(data, list):
+        for inx, x in enumerate(data):
+            data[inx] = deep_eval(x, scope, raise_ex)
+    elif callable(getattr(data, "eval", None)):
+        try:
+            data = data.eval(scope)
         except Exception as e:
-            raise Exception(f"Topic data validation failed. {str(e)}")
+            if raise_ex:
+                raise Exception(
+                    f"The Python expression '{data.expr_str}' failed. %s." % (str(e))
+                )
+            else:
+                data = None
+    return data
 
 
-class SerialMQTTBridge(Component):
-    def __init__(self, config):
-        super().__init__(config, "bridge")
-        self.mqtt = None
-        self.serial = None
-        self.topics_serial2mqtt = []
-        self.topics_mqtt2serial = []
-        self._scope = None
-        self.request_queue = Queue()
-
-        ja2mqtt_file = self.config.get_dir_path(config.root("ja2mqtt"))
-        ja2mqtt = Config(ja2mqtt_file, scope=self.scope(), use_template=True)
-        for topic_def in ja2mqtt("serial2mqtt"):
-            self.topics_serial2mqtt.append(Topic(topic_def))
-        for topic_def in ja2mqtt("mqtt2serial"):
-            self.topics_mqtt2serial.append(Topic(topic_def))
-        self.correlation_id = ja2mqtt("system.correlation_id", None)
-        self.correlation_timeout = ja2mqtt("system.correlation_timeout", 0)
-        self.topic_sys_error = ja2mqtt("system.topic_sys_error", None)
-        self.request = None
-
-        self.log.info(f"The ja2mqtt definition file is {ja2mqtt_file}")
-        self.log.info(
-            f"There are {len(self.topics_serial2mqtt)} serial2mqtt and {len(self.topics_mqtt2serial)} mqtt2serial topics."
-        )
-        self.log.debug(
-            f"The serial2mqtt topics are: {', '.join([x.name + ('' if not x.disabled else ' (disabled)') for x in self.topics_serial2mqtt])}"
-        )
-        self.log.debug(
-            f"The mqtt2serial topics are: {', '.join([x.name + ('' if not x.disabled else ' (disabled)') for x in self.topics_mqtt2serial])}"
-        )
-
-    def update_correlation(self, data):
-        if self.request_queue.qsize() > 0:
-            self.request = self.request_queue.get()
-        if self.request is not None:
+def deep_find(dic, keys, default=None, type=None, delim="."):
+    val = reduce(
+        lambda di, key: di.get(key, default) if isinstance(di, dict) else default,
+        keys.split(delim),
+        dic,
+    )
+    if val == default:
+        return default
+    return type(val) if type != None else val
+
+
+def import_class(name):
+    components = name.split(".")
+    mod = __import__(components[0])
+    for comp in components[1:]:
+        mod = getattr(mod, comp)
+    return mod
+
+
+def randomString(stringLength=10, letters=None):
+    """Generate a random string of fixed length"""
+    if letters is None:
+        letters = string.ascii_lowercase
+    return "".join(random.choice(letters) for i in range(stringLength))
+
+
+def is_number(s):
+    s = str(s)
+    p = re.compile(r"^[\+\-]?[0-9]*(\.[0-9]+)?$")
+    return s != "" and p.match(s)
+
+
+def perf_counter(counter=None):
+    if counter is None:
+        return time.perf_counter()
+    else:
+        return time.perf_counter() - counter
+
+
+def deep_merge(source, destination):
+    for key, value in source.items():
+        if isinstance(value, dict):
+            node = destination.setdefault(key, {})
+            deep_merge(value, node)
+        else:
             if (
-                time.time() - self.request.created_time < self.correlation_timeout
-                and self.request.ttl > 0
+                key in destination
+                and isinstance(destination[key], list)
+                and isinstance(value, list)
             ):
-                if self.request.cor_id is not None:
-                    data[self.correlation_id] = self.request.cor_id
-                self.request.ttl -= 1
+                for x in value:
+                    destination[key].append(x)
+            else:
+                if key not in destination:
+                    destination[key] = value
+    return destination
+
+
+def merge_dicts(*dicts):
+    result = {}
+    for d in dicts:
+        if d is not None:
+            result.update(d)
+    return result
+
+
+class PathDef:
+    def __init__(self, path_def):
+        self.path_def = path_def
+
+    def params(self, path):
+        path_re = self.path_def
+
+        # find all params in path_def
+        params_def = re.findall("(\{[a-zA-Z0-9_\.]+\})", self.path_def)
+
+        # create re pattern by replacing parameters in path_def with pattern to match parameter values
+        for p_def in params_def:
+            path_re = path_re.replace(p_def, "([a-zA-Z\-0-9\._]+)")
+
+        # get params values
+        res = re.findall("^" + path_re + "$", path)
+        values = []
+        for x in res:
+            if type(x) is tuple:
+                values.extend(list(x))
+            else:
+                values.append(x)
+
+        params = Map()
+        params.params = Map()
+        params.__path_def__ = self.path_def
+        params.__path__ = path
+        params.replace = self.replace
+        for x in range(0, len(params_def)):
+            if x < len(values):
+                params.params[params_def[x][1:-1]] = str(values[x])
+            else:
+                # Msg.warn_msg("The path '%s' does not match definition '%s'"%(path, self.path_def))
+                return None
+
+        return params
+
+    def replace(self, params, paramsMap):
+        new_path = params.__path__
+        for k, v in paramsMap.items():
+            if params.params.get(k):
+                new_path = new_path.replace("%s" % params.params.get(k), v, 1)
             else:
-                self.log.debug(
-                    "Discarding the request for correlation. The correlation timeout or TTL expired."
+                raise Exception(
+                    "The param '%s' has not been found in path definition '%s'."
+                    % (k, self.path_def)
                 )
-                self.request = None
-        return data
 
-    def scope(self):
-        if self._scope is None:
-            self._scope = Map(
-                topology=self.config.root("topology"),
-                pattern=lambda x: Pattern(x),
-                format=lambda x, **kwa: x.format(**kwa),
-            )
-        return self._scope
-
-    def update_scope(self, key, value=None, remove=False):
-        if self._scope is None:
-            self.scope()
-        if not remove:
-            self._scope[key] = value
-        else:
-            if key in self._scope:
-                del self._scope[key]
+        return new_path
 
-    def on_mqtt_connect(self, client, userdata, flags, rc):
-        for topic in self.topics_mqtt2serial:
-            self.mqtt.subscribe(topic.name)
-
-    def on_mqtt_message(self, topic_name, payload):
-        if not self.serial.is_ready():
-            self.log.warn(
-                "No messages will be processed. The serial interface is not available."
-            )
-            return
-        try:
-            data = Map(json.loads(payload))
-        except Exception as e:
-            raise Exception(f"Cannot parse the event data. {str(e)}")
 
-        self.log.debug(f"The event data parsed as JSON object: {data}")
-        for topic in self.topics_mqtt2serial:
-            if topic.name == topic_name:
-                if topic.disabled:
-                    continue
-                for rule in topic.rules:
-                    topic.check_rule_data(rule.read, data, self.scope())
-                    self.log.debug(
-                        "The event data is valid according to the defined rules."
-                    )
-                    _data = Map(data)
-                    self.update_scope("data", _data)
-                    try:
-                        s = deep_eval(rule.write, self._scope)
-                        self.request_queue.put(
-                            Map(
-                                cor_id=_data.get(self.correlation_id),
-                                created_time=time.time(),
-                                ttl=rule.get("request_ttl", 1),
-                            )
-                        )
-                        self.serial.writeline(s)
-                    finally:
-                        self.update_scope("data", remove=True)
-
-    def on_serial_data(self, data):
-        if not self.mqtt.connected:
-            self.log.warn(
-                "No events will be published. The client is not connected to the MQTT broker."
-            )
-            return
-
-        _rule = None
-        current_time = time.time()
-        for topic in self.topics_serial2mqtt:
-            for rule in topic.rules:
-                if isinstance(rule.read, PythonExpression):
-                    _data = rule.read.eval(self.scope())
+def remove_ansi_escape(text):
+    ansi_escape = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
+    return ansi_escape.sub("", text)
+
+
+def dict_from_string(s, d={}):
+    result = d
+    parts = s.split("=")
+    if len(parts) == 2:
+        key = parts[0]
+        value = parts[1]
+        keys = key.split(".")
+        current_dict = result
+        for i, k in enumerate(keys):
+            if k not in current_dict:
+                if i == len(keys) - 1:
+                    current_dict[k] = value
                 else:
-                    _data = rule.read
-                if _data == data:
-                    _rule = rule
-                    if not topic.disabled:
-                        self.update_scope("data", _data)
-                        try:
-                            d0 = self.update_correlation(Map())
-                            if not rule.require_request or self.request is not None:
-                                if rule.no_correlation:
-                                    d0 = {}
-                                d1 = deep_merge(rule.write, d0)
-                                d2 = deep_eval(d1, self._scope)
-                                write_data = json.dumps(d2)
-                                self.mqtt.publish(topic.name, write_data)
-                                break
-                        finally:
-                            self.update_scope("data", remove=True)
-            if _rule is not None:
-                break
-
-        if _rule is None:
-            self.log.debug(f"No rule found for the data: {data}")
-
-    def set_mqtt(self, mqtt):
-        self.mqtt = mqtt
-        self.mqtt.on_connect_ext = self.on_mqtt_connect
-        self.mqtt.on_message_ext = self.on_mqtt_message
-
-    def set_serial(self, serial):
-        self.serial = serial
-        serial.on_data_ext = self.on_serial_data
+                    current_dict[k] = {}
+            current_dict = current_dict[k]
+    return result
+
+
+def str2bool(s):
+    if type(s) == str:
+        return s.lower() in ["True", "true"]
+    else:
+        raise Exception(f"Invalid type: {type(s)}")
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.2/ja2mqtt/components/mqtt.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,45 +33,58 @@
         self.keepalive = self.config.value_int("keepalive", default=60)
         self.reconnect_after = self.config.value_int("reconnect_after", default=30)
         self.loop_timeout = self.config.value_int("loop_timeout", default=1)
         self.client = None
         self.connected = False
         self.on_connect_ext = None
         self.on_message_ext = None
+        self.on_error_ext = None
         self.log.info(f"The MQTT client configured for {self.address}.")
         self.log.debug(f"The MQTT object is {self}.")
 
     def __str__(self):
         return (
             f"{self.__class__}: name={self.name}, address={self.address}, port={self.port}, keepalive={self.keepalive}, "
             + f"reconnect_after={self.reconnect_after}, loop_timeout={self.loop_timeout}, connected={self.connected}"
         )
 
+    def on_error(self, exception):
+        print(str(exception))
+        self.log.error(str(exception))
+        if self.on_error_ext is not None:
+            self.on_error_ext(exception)
+
     def on_message(self, client, userdata, message):
         topic_name = message._topic.decode("utf-8")
         payload = str(message.payload.decode("utf-8"))
         self.log.info(f"--> recv: {topic_name}, payload={payload}")
         if self.on_message_ext is not None:
             try:
                 self.on_message_ext(topic_name, payload)
             except Exception as e:
-                self.log.error(str(e))
+                self.on_error(e)
 
     def on_connect(self, client, userdata, flags, rc):
         self.connected = True
         self.client.on_message = self.on_message
         self.log.info(f"Connected to the MQTT broker at {self.address}:{self.port}")
         if self.on_connect_ext is not None:
-            self.on_connect_ext(client, userdata, flags, rc)
+            try:
+                self.on_connect_ext(client, userdata, flags, rc)
+            except Exception as e:
+                self.on_error(e)
 
     def on_disconnect(self, client, userdata, rc):
-        self.log.info(f"Disconnected from the MQTT broker.")
-        if rc != 0:
-            self.log.error("The client was disconnected unexpectedly.")
-        self.connected = False
+        try:
+            self.log.info(f"Disconnected from the MQTT broker.")
+            self.connected = False
+            if rc != 0:
+                raise Exception("The client was disconnected unexpectedly.")
+        except Exception as e:
+            self.on_error(e)
 
     def init_client(self):
         self.client = mqtt.Client(self.client_name)
         self.client.on_connect = self.on_connect
         self.client.on_disconnect = self.on_disconnect
 
     def subscribe(self, topic):
@@ -91,17 +104,19 @@
             while not exit_event.is_set():
                 try:
                     self.client.connect(
                         self.address, port=self.port, keepalive=self.keepalive
                     )
                     break
                 except Exception as e:
-                    self.log.error(
-                        f"Cannot connect to the MQTT broker at {self.address}:{self.port}. {str(e)}. "
-                        + f"Will attemmpt to reconnect after {self.reconnect_after} seconds."
+                    self.on_error(
+                        Exception(
+                            f"Cannot connect to the MQTT broker at {self.address}:{self.port}. {str(e)}. "
+                            + f"Will attemmpt to reconnect after {self.reconnect_after} seconds."
+                        )
                     )
                     exit_event.wait(self.reconnect_after)
 
     def wait_is_connected(self, exit_event, timeout=0):
         start_time = time.time()
         while (
             not exit_event.is_set()
@@ -116,17 +131,19 @@
         try:
             while not exit_event.is_set():
                 try:
                     self.client.loop(timeout=self.loop_timeout, max_packets=1)
                     if not self.connected:
                         raise Exception("Not connected to MQTT broker.")
                 except Exception as e:
-                    self.log.error(
-                        f"Error occurred in the MQTT loop. {str(e)}"
-                        + f"Will attemmpt to reconnect after {self.reconnect_after} seconds."
+                    self.on_error(
+                        Exception(
+                            f"Error occurred in the MQTT loop. {str(e)}"
+                            + f"Will attemmpt to reconnect after {self.reconnect_after} seconds."
+                        )
                     )
                     exit_event.wait(self.reconnect_after)
                     self.__wait_for_connection(exit_event, reconnect=True)
         finally:
             if self.connected:
                 self.client.disconnect()
             self.log.info("MQTT worker ended.")
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.2/ja2mqtt/components/simulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import absolute_import, unicode_literals
 
 import json
 import logging
 import re
 import threading
 import time
+import random
 from queue import Empty, Queue
 
 import paho.mqtt.client as mqtt
 import serial as py_serial
 
 from ja2mqtt.config import Config
 from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
@@ -55,27 +56,28 @@
 
 
 class Simulator:
     def __init__(self, config, encoding):
         self.log = logging.getLogger("simulator")
         self.config = config
         self.response_delay = config.value_int("response_delay", default=0.5)
+        self.prf_state_bits = config.value_int("prf_state_bits", default=24)
         self.rules = [Map(x) for x in config.value("rules")]
         self.sections = {
             str(x["code"]): Section(Map(x)) for x in config.value("sections")
         }
         self.pin = config.value("pin")
         self.timeout = 1
         self.buffer = Queue()
         self.encoding = encoding
 
     def __str__(self):
         return (
             f"{self.__class__}: pin={self.pin}, timeout={self.timeout}, response_delay={self.response_delay}, "
-            + f"sections={[str(x) for x in self.sections.values()]}, rules={self.rules}"
+            + f"prf_state_bits={self.prf_state_bits}, sections={[str(x) for x in self.sections.values()]}, rules={self.rules}"
         )
 
     def open(self, exit_event):
         pass
 
     def close(self):
         pass
@@ -138,24 +140,46 @@
 
     def readline(self):
         try:
             return bytes(self.buffer.get(timeout=self.timeout), self.encoding)
         except Empty:
             return b""
 
+    def scope(self):
+
+        from .serial import encode_prfstate
+
+        def _prf_random_states(*pos, on_prob=0.5):
+            prf = { str(p):("ON" if random.random() < on_prob else "OFF") for p in pos }
+            return "PRFSTATE " + encode_prfstate(prf, self.prf_state_bits)
+
+        return Map(
+            random = lambda a,b: a+round(random.random()*b),
+            prf_randon_states = _prf_random_states,
+        )
+
     def worker(self, exit_event):
+
+        _scope = self.scope()
+
+        def _value(v):
+            if isinstance(v, PythonExpression):
+                return v.eval(_scope)
+            else:
+                return v
+
         try:
             while not exit_event.is_set():
                 current_time = time.time()
                 for rule in self.rules:
-                    if rule.get("time"):
+                    if rule.get("time_next"):
                         if rule.__last_write is None:
                             rule.__last_write = current_time
-                        if current_time - rule.__last_write > rule.time:
-                            self.buffer.put(rule.write)
+                        if current_time - rule.__last_write > _value(rule.time_next):
+                            self.buffer.put(_value(rule.write))
                             rule.__last_write = current_time
                 exit_event.wait(0.5)
         finally:
             self.log.info("Simulator worker ended.")
 
     def start(self, exit_event):
         self.thread = threading.Thread(
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt/config.py` & `ja2mqtt-1.0.2/ja2mqtt/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,25 +25,31 @@
 from .utils import (
     Map,
     PythonExpression,
     deep_find,
     deep_merge,
     import_class,
     merge_dicts,
+    randomString,
+    str2bool,
 )
 
 # they must be in a form ${VARIABLE_NAME}
 ENVNAME_PATTERN = "[A-Z0-9_]+"
 ENVPARAM_PATTERN = "\$\{%s\}" % ENVNAME_PATTERN
 
 # consolidated variables supplied via env file and environment variables
 ENV = {}
 
-DEBUG = False
-ANSI_COLORS = True
+DEBUG = str2bool(os.getenv("JA2MQTT_DEBUG", "False"))
+ANSI_COLORS = not str2bool(os.getenv("JA2MQTT_NO_ANSI", "False"))
+CONFIG_FILE = os.getenv("JA2MQTT_CONFIG", None)
+CONFIG_ENV = os.getenv("JA2MQTT_ENV", None)
+
+env_variables = ["JA2MQTT_DEBUG", "JA2MQTT_NO_ANSI", "JA2MQTT_CONFIG", "JA2MQTT_ENV"]
 
 # global exit event
 exit_event = Event()
 
 
 class Jinja2TemplateLoader(jinja2.BaseLoader):
     def get_source(self, environment, template):
@@ -383,7 +389,13 @@
 
 def ja2mqtt_def(config):
     return Config(
         config.get_dir_path(config.root("ja2mqtt")),
         scope=Map(topology=config.root("topology")),
         use_template=True,
     )
+
+
+def correlation_id(ja2mqtt):
+    corrid_field = ja2mqtt("system.correlation_id", None)
+    corr_id = randomString(12, letters="abcdef0123456789")
+    return corrid_field, corr_id if corrid_field is not None else None
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.2/ja2mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.1/ja2mqtt.egg-info/SOURCES.txt` & `ja2mqtt-1.0.2/ja2mqtt.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-.gitignore
-Makefile
+MANIFEST.in
 README-pypi.text
 README.md
 setup.py
-.github/workflows/docker-image.yml
 bin/env.sh
 bin/ja2mqtt
+bin/requirements-dev.txt
+bin/requirements-setup-py.sh
 bin/requirements.txt
-bin/venv-create.sh
-bin/venv-freeze.sh
 config/ja2mqtt.yaml
 config/sample-config.yaml
 docker/Dockerfile
 docker/docker-compose.yaml
 docker/mqtt-config/mosquitto.conf
 ja2mqtt/__init__.py
 ja2mqtt/__main__.py
```

### Comparing `ja2mqtt-1.0.1/setup.py` & `ja2mqtt-1.0.2/setup.py`

 * *Files identical despite different names*

