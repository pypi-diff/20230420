# Comparing `tmp/aprsd_weewx_plugin-0.3.1.tar.gz` & `tmp/aprsd_weewx_plugin-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd_weewx_plugin-0.3.1.tar", last modified: Thu Apr 20 20:00:33 2023, max compression
+gzip compressed data, was "aprsd_weewx_plugin-0.3.2.tar", last modified: Thu Apr 20 20:16:09 2023, max compression
```

## Comparing `aprsd_weewx_plugin-0.3.1.tar` & `aprsd_weewx_plugin-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.797811 aprsd_weewx_plugin-0.3.1/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.752976 aprsd_weewx_plugin-0.3.1/.github/
--rw-r--r--   0 i530566    (501) staff       (20)      677 2022-12-20 17:23:30.000000 aprsd_weewx_plugin-0.3.1/.github/FUNDING.yml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 i530566    (501) staff       (20)       68 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/AUTHORS
--rw-r--r--   0 i530566    (501) staff       (20)      489 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/ChangeLog
--rw-r--r--   0 i530566    (501) staff       (20)    35148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/LICENSE
--rw-r--r--   0 i530566    (501) staff       (20)     1970 2022-12-20 17:23:31.000000 aprsd_weewx_plugin-0.3.1/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 20:00:33.798040 aprsd_weewx_plugin-0.3.1/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)     2784 2021-09-14 18:50:36.000000 aprsd_weewx_plugin-0.3.1/README.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.755476 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/
--rw-r--r--   0 i530566    (501) staff       (20)      644 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.785340 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/
--rw-r--r--   0 i530566    (501) staff       (20)      115 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2727 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/opts.py
--rw-r--r--   0 i530566    (501) staff       (20)     1168 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/weewx.py
--rw-r--r--   0 i530566    (501) staff       (20)    12535 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/weewx.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.765494 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/
--rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)      836 2023-04-20 20:00:33.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 i530566    (501) staff       (20)       84 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/entry_points.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2022-12-02 21:36:09.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/not-zip-safe
--rw-r--r--   0 i530566    (501) staff       (20)       47 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/pbr.json
--rw-r--r--   0 i530566    (501) staff       (20)       39 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/requires.txt
--rw-r--r--   0 i530566    (501) staff       (20)       19 2023-04-20 20:00:19.000000 aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.795272 aprsd_weewx_plugin-0.3.1/docs/
--rw-r--r--   0 i530566    (501) staff       (20)      619 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/authors.rst
--rw-r--r--   0 i530566    (501) staff       (20)      520 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.1/docs/clean_docs.py
--rwxr-xr-x   0 i530566    (501) staff       (20)     5019 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.1/docs/conf.py
--rw-r--r--   0 i530566    (501) staff       (20)       33 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/contributing.rst
--rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/history.rst
--rw-r--r--   0 i530566    (501) staff       (20)      323 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/index.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/docs/installation.rst
--rw-r--r--   0 i530566    (501) staff       (20)       94 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/requirements-dev.txt
--rw-r--r--   0 i530566    (501) staff       (20)       39 2022-12-29 16:28:41.000000 aprsd_weewx_plugin-0.3.1/requirements.txt
--rw-r--r--   0 i530566    (501) staff       (20)     1057 2023-04-20 20:00:33.800341 aprsd_weewx_plugin-0.3.1/setup.cfg
--rw-r--r--   0 i530566    (501) staff       (20)      952 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.1/setup.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:00:33.797165 aprsd_weewx_plugin-0.3.1/tests/
--rw-r--r--   0 i530566    (501) staff       (20)       48 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/tests/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)      534 2023-04-20 19:59:44.000000 aprsd_weewx_plugin-0.3.1/tests/test_aprsd_weewx_plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)     1994 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.1/tox.ini
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.277728 aprsd_weewx_plugin-0.3.2/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.233554 aprsd_weewx_plugin-0.3.2/.github/
+-rw-r--r--   0 i530566    (501) staff       (20)      677 2022-12-20 17:23:30.000000 aprsd_weewx_plugin-0.3.2/.github/FUNDING.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)       68 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/AUTHORS
+-rw-r--r--   0 i530566    (501) staff       (20)      519 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/ChangeLog
+-rw-r--r--   0 i530566    (501) staff       (20)    35148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/LICENSE
+-rw-r--r--   0 i530566    (501) staff       (20)     1970 2022-12-20 17:23:31.000000 aprsd_weewx_plugin-0.3.2/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 20:16:09.278015 aprsd_weewx_plugin-0.3.2/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)     2784 2021-09-14 18:50:36.000000 aprsd_weewx_plugin-0.3.2/README.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.235357 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/
+-rw-r--r--   0 i530566    (501) staff       (20)      644 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.245315 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/
+-rw-r--r--   0 i530566    (501) staff       (20)      115 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2727 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/opts.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1168 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/weewx.py
+-rw-r--r--   0 i530566    (501) staff       (20)    12554 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/weewx.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.242269 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/
+-rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)      836 2023-04-20 20:16:09.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       84 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2022-12-02 21:36:09.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 i530566    (501) staff       (20)       47 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/pbr.json
+-rw-r--r--   0 i530566    (501) staff       (20)       39 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/requires.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       19 2023-04-20 20:15:56.000000 aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.274462 aprsd_weewx_plugin-0.3.2/docs/
+-rw-r--r--   0 i530566    (501) staff       (20)      619 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/authors.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      520 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.2/docs/clean_docs.py
+-rwxr-xr-x   0 i530566    (501) staff       (20)     5019 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.2/docs/conf.py
+-rw-r--r--   0 i530566    (501) staff       (20)       33 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/contributing.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       28 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/history.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      323 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/index.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1148 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/docs/installation.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       94 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/requirements-dev.txt
+-rw-r--r--   0 i530566    (501) staff       (20)       39 2022-12-29 16:28:41.000000 aprsd_weewx_plugin-0.3.2/requirements.txt
+-rw-r--r--   0 i530566    (501) staff       (20)     1057 2023-04-20 20:16:09.280665 aprsd_weewx_plugin-0.3.2/setup.cfg
+-rw-r--r--   0 i530566    (501) staff       (20)      952 2021-09-12 16:04:55.000000 aprsd_weewx_plugin-0.3.2/setup.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-20 20:16:09.276912 aprsd_weewx_plugin-0.3.2/tests/
+-rw-r--r--   0 i530566    (501) staff       (20)       48 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/tests/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)      534 2023-04-20 20:15:22.000000 aprsd_weewx_plugin-0.3.2/tests/test_aprsd_weewx_plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1994 2021-09-12 16:04:08.000000 aprsd_weewx_plugin-0.3.2/tox.ini
```

### Comparing `aprsd_weewx_plugin-0.3.1/.github/FUNDING.yml` & `aprsd_weewx_plugin-0.3.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/.pre-commit-config.yaml` & `aprsd_weewx_plugin-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/LICENSE` & `aprsd_weewx_plugin-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/Makefile` & `aprsd_weewx_plugin-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/PKG-INFO` & `aprsd_weewx_plugin-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd_weewx_plugin
-Version: 0.3.1
+Version: 0.3.2
 Summary: HAM Radio APRSD that reports weather from a weewx weather station.
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: GPL-3.0
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `aprsd_weewx_plugin-0.3.1/README.rst` & `aprsd_weewx_plugin-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/__init__.py` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/opts.py` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/conf/weewx.py` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/conf/weewx.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin/weewx.py` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin/weewx.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,16 +313,17 @@
         wind_speed = float(wx_data.get("windSpeed_mph", 0.00))
         wind_gust = float(wx_data.get("windGust_mph", 0.00))
         temperature = float(wx_data.get("outTemp_F", 0.00))
         rain_last_hr = float(wx_data.get("hourRain_in", 0.00))
         rain_last_24_hrs = float(wx_data.get("rain24_in", 0.00))
         rain_since_midnight = float(wx_data.get("day_Rain_in", 0.00))
         humidity = float(wx_data.get("outHumidity", 0.00))
-        # inHg * 330.863886667 = mBar
-        pressure = float(wx_data.get("pressure_inHg", 0.00)) * 330.863886667
+        # * 330.863886667
+        # inHg * 33.8639 = mBar
+        pressure = float(wx_data.get("pressure_inHg", 0.00)) * 33.8639 * 10
         return aprsd.packets.WeatherPacket(
             from_call=self.callsign,
             to_call="APRS",
             latitude=self.convert_latitude(float(self.latitude)),
             longitude=self.convert_longitude(float(self.longitude)),
             course=int(wind_dir),
             speed=wind_speed,
```

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/PKG-INFO` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd-weewx-plugin
-Version: 0.3.1
+Version: 0.3.2
 Summary: HAM Radio APRSD that reports weather from a weewx weather station.
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: GPL-3.0
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `aprsd_weewx_plugin-0.3.1/aprsd_weewx_plugin.egg-info/SOURCES.txt` & `aprsd_weewx_plugin-0.3.2/aprsd_weewx_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/docs/Makefile` & `aprsd_weewx_plugin-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/docs/clean_docs.py` & `aprsd_weewx_plugin-0.3.2/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/docs/conf.py` & `aprsd_weewx_plugin-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/docs/installation.rst` & `aprsd_weewx_plugin-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/setup.cfg` & `aprsd_weewx_plugin-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/setup.py` & `aprsd_weewx_plugin-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/tests/test_aprsd_weewx_plugin.py` & `aprsd_weewx_plugin-0.3.2/tests/test_aprsd_weewx_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd_weewx_plugin-0.3.1/tox.ini` & `aprsd_weewx_plugin-0.3.2/tox.ini`

 * *Files identical despite different names*

