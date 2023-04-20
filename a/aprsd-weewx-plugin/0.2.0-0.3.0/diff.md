# Comparing `tmp/aprsd_weewx_plugin-0.2.0.tar.gz` & `tmp/aprsd_weewx_plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd_weewx_plugin-0.2.0.tar", last modified: Tue Jan 10 01:42:54 2023, max compression
+gzip compressed data, was "aprsd_weewx_plugin-0.3.0.tar", last modified: Thu Apr 20 19:49:58 2023, max compression
```

## Comparing `aprsd_weewx_plugin-0.2.0.tar` & `aprsd_weewx_plugin-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.988559 aprsd_weewx_plugin-0.2.0/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.968357 aprsd_weewx_plugin-0.2.0/.github/
--rw-r--r--   0 i530566    (501) staff       (20)      677 2022-12-20 17:23:30.000000 aprsd_weewx_plugin-0.2.0/.github/FUNDING.yml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 i530566    (501) staff       (20)       68 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/AUTHORS
--rw-r--r--   0 i530566    (501) staff       (20)      373 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/ChangeLog
--rw-r--r--   0 i530566    (501) staff       (20)    35148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/LICENSE
--rw-r--r--   0 i530566    (501) staff       (20)     1970 2022-12-20 17:23:31.000000 aprsd_weewx_plugin-0.2.0/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-01-10 01:42:54.988789 aprsd_weewx_plugin-0.2.0/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)     2784 2021-09-14 18:50:36.000000 aprsd_weewx_plugin-0.2.0/README.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.969934 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/
--rw-r--r--   0 i530566    (501) staff       (20)      644 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.979909 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/
--rw-r--r--   0 i530566    (501) staff       (20)      115 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2727 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/opts.py
--rw-r--r--   0 i530566    (501) staff       (20)     1168 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/weewx.py
--rw-r--r--   0 i530566    (501) staff       (20)    12484 2023-01-10 01:42:42.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/weewx.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.976985 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/
--rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)      836 2023-01-10 01:42:54.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 i530566    (501) staff       (20)       84 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/entry_points.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2022-12-02 21:36:09.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/not-zip-safe
--rw-r--r--   0 i530566    (501) staff       (20)       46 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/pbr.json
--rw-r--r--   0 i530566    (501) staff       (20)       39 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/requires.txt
--rw-r--r--   0 i530566    (501) staff       (20)       19 2023-01-10 01:42:47.000000 aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.986454 aprsd_weewx_plugin-0.2.0/docs/
--rw-r--r--   0 i530566    (501) staff       (20)      619 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/authors.rst
--rw-r--r--   0 i530566    (501) staff       (20)      520 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.2.0/docs/clean_docs.py
--rwxr-xr-x   0 i530566    (501) staff       (20)     5019 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.2.0/docs/conf.py
--rw-r--r--   0 i530566    (501) staff       (20)       33 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/contributing.rst
--rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/history.rst
--rw-r--r--   0 i530566    (501) staff       (20)      323 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/index.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/docs/installation.rst
--rw-r--r--   0 i530566    (501) staff       (20)       94 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/requirements-dev.txt
--rw-r--r--   0 i530566    (501) staff       (20)       39 2022-12-29 16:28:41.000000 aprsd_weewx_plugin-0.2.0/requirements.txt
--rw-r--r--   0 i530566    (501) staff       (20)     1057 2023-01-10 01:42:54.991369 aprsd_weewx_plugin-0.2.0/setup.cfg
--rw-r--r--   0 i530566    (501) staff       (20)      952 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.2.0/setup.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-10 01:42:54.988015 aprsd_weewx_plugin-0.2.0/tests/
--rw-r--r--   0 i530566    (501) staff       (20)       48 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/tests/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)      534 2023-01-10 01:42:41.000000 aprsd_weewx_plugin-0.2.0/tests/test_aprsd_weewx_plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)     1994 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.2.0/tox.ini
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.268166 aprsd_weewx_plugin-0.3.0/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.246635 aprsd_weewx_plugin-0.3.0/.github/
+-rw-r--r--   0 i530566    (501) staff       (20)      677 2022-12-20 17:23:30.000000 aprsd_weewx_plugin-0.3.0/.github/FUNDING.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)       68 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/AUTHORS
+-rw-r--r--   0 i530566    (501) staff       (20)      448 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/ChangeLog
+-rw-r--r--   0 i530566    (501) staff       (20)    35148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/LICENSE
+-rw-r--r--   0 i530566    (501) staff       (20)     1970 2022-12-20 17:23:31.000000 aprsd_weewx_plugin-0.3.0/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 19:49:58.268509 aprsd_weewx_plugin-0.3.0/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)     2784 2021-09-14 18:50:36.000000 aprsd_weewx_plugin-0.3.0/README.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.248175 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/
+-rw-r--r--   0 i530566    (501) staff       (20)      644 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.257023 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/
+-rw-r--r--   0 i530566    (501) staff       (20)      115 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2727 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/opts.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1168 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/weewx.py
+-rw-r--r--   0 i530566    (501) staff       (20)    12549 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/weewx.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.254565 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/
+-rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)      836 2023-04-20 19:49:58.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       84 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2022-12-02 21:36:09.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 i530566    (501) staff       (20)       46 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/pbr.json
+-rw-r--r--   0 i530566    (501) staff       (20)       39 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/requires.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       19 2023-04-20 19:49:44.000000 aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.264427 aprsd_weewx_plugin-0.3.0/docs/
+-rw-r--r--   0 i530566    (501) staff       (20)      619 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/authors.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      520 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.0/docs/clean_docs.py
+-rwxr-xr-x   0 i530566    (501) staff       (20)     5019 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.0/docs/conf.py
+-rw-r--r--   0 i530566    (501) staff       (20)       33 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/contributing.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/history.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      323 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/index.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/docs/installation.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       94 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/requirements-dev.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       39 2022-12-29 16:28:41.000000 aprsd_weewx_plugin-0.3.0/requirements.txt
+-rw-r--r--   0 i530566    (501) staff       (20)     1057 2023-04-20 19:49:58.274684 aprsd_weewx_plugin-0.3.0/setup.cfg
+-rw-r--r--   0 i530566    (501) staff       (20)      952 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.0/setup.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 19:49:58.267202 aprsd_weewx_plugin-0.3.0/tests/
+-rw-r--r--   0 i530566    (501) staff       (20)       48 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/tests/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)      534 2023-04-20 19:48:44.000000 aprsd_weewx_plugin-0.3.0/tests/test_aprsd_weewx_plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1994 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.0/tox.ini
```

### Comparing `aprsd_weewx_plugin-0.2.0/.github/FUNDING.yml` & `aprsd_weewx_plugin-0.3.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/.pre-commit-config.yaml` & `aprsd_weewx_plugin-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/LICENSE` & `aprsd_weewx_plugin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/Makefile` & `aprsd_weewx_plugin-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/PKG-INFO` & `aprsd_weewx_plugin-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd_weewx_plugin
-Version: 0.2.0
+Version: 0.3.0
 Summary: HAM Radio APRSD that reports weather from a weewx weather station.
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: GPL-3.0
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `aprsd_weewx_plugin-0.2.0/README.rst` & `aprsd_weewx_plugin-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/__init__.py` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/opts.py` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/conf/weewx.py` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/conf/weewx.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin/weewx.py` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin/weewx.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     def on_connect(self, client, userdata, flags, rc):
         LOG.info(f"Connected to MQTT {self._mqtt_host} ({rc})")
         client.subscribe("weather/loop")
 
     def on_message(self, client, userdata, msg):
         wx_data = json.loads(msg.payload)
         LOG.debug("Got WX data")
+        LOG.debug(wx_data)
         # Make sure we have only 1 item in the queue
         if self.msg_queue.qsize() >= 1:
             self.msg_queue.clear()
         self.msg_queue.put(wx_data)
         self.wx_queue.clear()
         self.wx_queue.put(wx_data)
 
@@ -313,15 +314,16 @@
         wind_gust = float(wx_data.get("windGust_mph", 0.00))
         temperature = float(wx_data.get("outTemp_F", 0.00))
         rain_last_hr = float(wx_data.get("hourRain_in", 0.00))
         rain_last_24_hrs = float(wx_data.get("rain24_in", 0.00))
         rain_since_midnight = float(wx_data.get("day_Rain_in", 0.00))
         humidity = float(wx_data.get("outHumidity", 0.00))
         # * 330.863886667
-        pressure = float(wx_data.get("relbarometer", 0.00)) * 10
+        # inHg * 33.8639 = mBar
+        pressure = float(wx_data.get("pressure_inHg", 0.00)) * 33.8639
         return aprsd.packets.WeatherPacket(
             from_call=self.callsign,
             to_call="APRS",
             latitude=self.convert_latitude(float(self.latitude)),
             longitude=self.convert_longitude(float(self.longitude)),
             course=int(wind_dir),
             speed=wind_speed,
```

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/PKG-INFO` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd-weewx-plugin
-Version: 0.2.0
+Version: 0.3.0
 Summary: HAM Radio APRSD that reports weather from a weewx weather station.
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: GPL-3.0
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `aprsd_weewx_plugin-0.2.0/aprsd_weewx_plugin.egg-info/SOURCES.txt` & `aprsd_weewx_plugin-0.3.0/aprsd_weewx_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/docs/Makefile` & `aprsd_weewx_plugin-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/docs/clean_docs.py` & `aprsd_weewx_plugin-0.3.0/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/docs/conf.py` & `aprsd_weewx_plugin-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/docs/installation.rst` & `aprsd_weewx_plugin-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/setup.cfg` & `aprsd_weewx_plugin-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/setup.py` & `aprsd_weewx_plugin-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/tests/test_aprsd_weewx_plugin.py` & `aprsd_weewx_plugin-0.3.0/tests/test_aprsd_weewx_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.2.0/tox.ini` & `aprsd_weewx_plugin-0.3.0/tox.ini`

 * *Files identical despite different names*

