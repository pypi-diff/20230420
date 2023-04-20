# Comparing `tmp/homeservices-0.2.3.tar.gz` & `tmp/homeservices-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeservices-0.2.3.tar", last modified: Mon Mar 13 13:47:02 2023, max compression
+gzip compressed data, was "homeservices-0.2.5.tar", last modified: Thu Apr 20 15:39:11 2023, max compression
```

## Comparing `homeservices-0.2.3.tar` & `homeservices-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:47:02.901791 homeservices-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-13 13:47:02.901791 homeservices-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-13 13:46:52.000000 homeservices-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:47:02.901791 homeservices-0.2.3/homeservices/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/config-template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:47:02.901791 homeservices-0.2.3/homeservices/webservice/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/webservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/webservice/db_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/webservice/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/webservice/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-13 13:46:52.000000 homeservices-0.2.3/homeservices/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:47:02.901791 homeservices-0.2.3/homeservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-13 13:47:02.000000 homeservices-0.2.3/homeservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-13 13:47:02.000000 homeservices-0.2.3/homeservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 13:47:02.000000 homeservices-0.2.3/homeservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-13 13:47:02.000000 homeservices-0.2.3/homeservices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-13 13:47:02.000000 homeservices-0.2.3/homeservices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 13:47:02.901791 homeservices-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-13 13:46:52.000000 homeservices-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:47:02.901791 homeservices-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:46:52.000000 homeservices-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-13 13:46:52.000000 homeservices-0.2.3/tests/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-13 13:46:52.000000 homeservices-0.2.3/tests/test_000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-20 15:39:11.755286 homeservices-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 15:39:00.000000 homeservices-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/homeservices/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/config-template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/homeservices/webservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/webservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/webservice/db_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/webservice/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/webservice/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-20 15:39:00.000000 homeservices-0.2.5/homeservices/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/homeservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-20 15:39:11.000000 homeservices-0.2.5/homeservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 15:39:11.000000 homeservices-0.2.5/homeservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:39:11.000000 homeservices-0.2.5/homeservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-20 15:39:11.000000 homeservices-0.2.5/homeservices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 15:39:11.000000 homeservices-0.2.5/homeservices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:39:11.755286 homeservices-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-20 15:39:00.000000 homeservices-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:00.000000 homeservices-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:39:11.755286 homeservices-0.2.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-20 15:39:00.000000 homeservices-0.2.5/tests/data/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-20 15:39:00.000000 homeservices-0.2.5/tests/test_000.py
```

### Comparing `homeservices-0.2.3/PKG-INFO` & `homeservices-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeservices
-Version: 0.2.3
+Version: 0.2.5
 Summary: Home webservices for Alexa
 Home-page: https://github.com/Phornee/homeservices
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Home Services
         Tiny webservice to answer Alexa intents
```

### Comparing `homeservices-0.2.3/homeservices/webservice/db_connector.py` & `homeservices-0.2.5/homeservices/webservice/db_connector.py`

 * *Files identical despite different names*

### Comparing `homeservices-0.2.3/homeservices/webservice/webservice.py` & `homeservices-0.2.5/homeservices/webservice/webservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,68 @@
+""" 
+    An entry point for all the services in my home
+"""
 import os
-from flask import Flask, request, make_response, Response
-from flask_compress import Compress
 from urllib import parse
 import json
 from datetime import datetime
 from pathlib import Path
+from flask import Flask, request, make_response, Response
+from flask_compress import Compress
 
-from baseutils_phornee import Config
+from config_yml import Config
+
+from revproxy_auth import RevProxyAuth
 
-from .db_connector import db_factory
 from elecmon import ElectricityMonitor
 
+from .db_connector import db_factory
 
-class HomeServices(object):
 
+class HomeServices():
+    """ Homeservices base class: An entry point for all the services in my home
+    """
     def __init__(self,  template_folder: str, static_folder: str, template_config_path: str = None) -> None:
-        """_summary_
-
+        """
         Args:
             template_folder (string): Path for the Flask templates
             static_folder (string): Path for the Flask static info
         """
+
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
-        self.app.add_url_rule('/', 'index', self.index, methods=['GET'])
+
+        self.revproxy_auth = RevProxyAuth()
+
+        self.app.add_url_rule('/', 'auth', self.auth, methods=['GET', 'POST'])
+        self.app.add_url_rule('/<path:path>', 'path_redirect', self.revproxy_auth.path_redirect,
+                              methods=['GET', 'POST'])
         self.app.add_url_rule('/alexaintent', 'alexaintent', self.alexa_intent, methods=['GET'])
         self.app.add_url_rule('/customsensor', 'customsensor', self.custom_sensor, methods=['GET'])
         self.app.add_url_rule('/besthour', 'besthour', self.best_hour, methods=['GET'])
+
         Compress(self.app)
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
-        self.config = Config(self.getClassName(), template_config_path, 'config.yml')
+        self.config = Config(self.get_class_name(), template_config_path, 'config.yml')
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = db_factory(influx_conn_type)
         self.conn.openConn(self.config['influxdbconn'])
 
     @classmethod
-    def getClassName(cls) -> str:
+    def get_class_name(cls) -> str:
         """
         Returns:
            string: class name
         """
         return "homeservices"
 
-    def getApp(self) -> Flask:
+    def get_app(self) -> Flask:
         """
         Returns:
             Flask app: The flask app
         """
         return self.app
 
     def run(self) -> None:
@@ -62,21 +75,31 @@
         """Main entry point
 
         Returns:
             http_response: response string
         """
         return 'This is the Pi server.'
 
+    def auth(self) -> Response:
+        """Main entry point
+        Returns:
+            http_response: response string
+        """
+        resp = self.revproxy_auth.path_redirect("/")
+        return resp
+
+ 
     def _read_last_measures(self, number_of_measures: int, sensor_name: str) -> list:
         sensor_table = {'jardín': '2', 'cocina': '1', 'buhardilla': '3'}
 
         points = None
 
         if sensor_name in sensor_table:
-            points = self.conn.read_last_measures(number_of_measures=number_of_measures, sensor_id=sensor_table[sensor_name])
+            points = self.conn.read_last_measures(number_of_measures=number_of_measures, 
+                                                  sensor_id=sensor_table[sensor_name])
 
         return points
 
     def best_hour(self) -> Response:
         """Answer to sensor requests. It returns
 
         Returns:
@@ -99,17 +122,17 @@
                 elec_mon = ElectricityMonitor()
                 best_hour, price = elec_mon.get_better_timeslice(time, datetime.now())
 
                 if best_hour.day == datetime.now().day:
                     if best_hour.hour == datetime.now().hour:
                         response_phrase = "Ya mismo, cuanto antes mejor."
                     else:
-                        response_phrase = "A las {}.".format(best_hour.hour)
+                        response_phrase = f"A las {best_hour.hour}."
                 else:
-                    response_phrase = "A las {} de mañana.".format(best_hour.hour)
+                    response_phrase = f"A las {best_hour.hour} de mañana."
 
                 response = make_response(response_phrase.encode('UTF-8'))
                 response.mimetype = "text/plain"
                 response.headers['Pragma'] = 'no-cache'
                 response.headers["Expires"] = 0
                 response.headers['Cache-Control'] = 'no-cache, no-store, must-revalidate'
             else:
@@ -129,16 +152,15 @@
                 sensor = params['sensor'][0]
 
                 points = self._read_last_measures(1, sensor)
 
                 if points:
                     point = points[0]
 
-                    response = make_response(json.dumps('{{"temp" : {}, "hum" : {} }}'.format(point['temp'],
-                                                                                              point['humidity'])))
+                    response = make_response(json.dumps(f'{{"temp" : {point["temp"]}, "hum" : {point["humidity"]} }}'))
                     response.mimetype = "application/json"
                     response.headers['Pragma'] = 'no-cache'
                     response.headers["Expires"] = 0
                     response.headers['Cache-Control'] = 'no-cache, no-store, must-revalidate'
                 else:
                     response = make_response("Sensor not found", 404)
             else:
@@ -171,18 +193,17 @@
                     elif delta < -0.6:
                         trend = ' y bajando a saco'
                     elif delta < -0.3:
                         trend = ' y bajando'
                     elif delta < -0.1:
                         trend = ' y bajando ligeramente'
 
-                    response_phrase = """Hace {} grados{},
-                                         y la humedad es del {:.0f} por ciento.""".format(points[0]['temp'],
-                                                                                          trend,
-                                                                                          points[0]['humidity'])
+                    response_phrase = (f"Hace {points[0]['temp']} grados{trend},"
+                                       f"y la humedad es del {points[0]['humidity']:.0f} por ciento.")
+
                     if points[0]['humidity'] > 98:
                         response_phrase += " Es muy posible que esté lloviendo."
 
                     if points[0]['temp'] < 5:
                         response_phrase += " ¡Joder, que frio hace!."
                     elif points[0]['temp'] < 10:
                         response_phrase += " Hace bastante fresquete."
```

### Comparing `homeservices-0.2.3/homeservices.egg-info/PKG-INFO` & `homeservices-0.2.5/homeservices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeservices
-Version: 0.2.3
+Version: 0.2.5
 Summary: Home webservices for Alexa
 Home-page: https://github.com/Phornee/homeservices
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Home Services
         Tiny webservice to answer Alexa intents
```

### Comparing `homeservices-0.2.3/setup.py` & `homeservices-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="homeservices",
-    version="0.2.3",
+    version="0.2.5",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Home webservices for Alexa",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/homeservices",
     packages=setuptools.find_packages(),
     package_data={
         '': ['*.yml'],
+        'tests': ['data/*.yml']
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation"
     ],
@@ -26,11 +27,13 @@
         'Flask>=1.1.2',
         'gunicorn>=20.1.0',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'tzlocal>=4.1',
         'influxdb_wrapper>=0.0.3',
         'baseutils_phornee>=0.1.1',
+        'config_yml>=0.2.0',
+        'revproxy_auth>=0.0.10',
         'elecmon>=0.0.2'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `homeservices-0.2.3/tests/test_000.py` & `homeservices-0.2.5/tests/test_000.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+""" Unit tests """
 import unittest
 from pathlib import Path
 
 from homeservices import HomeServices
 
 
 class Testing(unittest.TestCase):
-    templates_path = "{}/templates".format(Path().absolute())
-    static_path = "{}/static".format(Path().absolute())
+    """Unittesting
+    """
+    templates_path = f'{Path().absolute()}/templates'
+    static_path = f'{Path().absolute()}/static'
 
-    template_config_path = '{}/data/config-template.yml'.format(Path(__file__).parent)
+    template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
     service = HomeServices(template_folder=templates_path,
                            static_folder=static_path,
                            template_config_path=template_config_path)
-    client = service.getApp().test_client()
+    client = service.get_app().test_client()
 
     points = [{'time': '2022-12-19T13:32:02.501231Z', 'tags': {'sensorid': '1'},
                                                       'fields': {'humidity': 53.3, 'temp': 20.3}},
               {'time': '2022-12-19T13:30:02.442527Z', 'tags': {'sensorid': '1'},
                                                       'fields': {'humidity': 53.3, 'temp': 20.3}},
               {'time': '2022-12-19T13:28:03.145696Z', 'tags': {'sensorid': '1'},
                                                       'fields': {'humidity': 53.3, 'temp': 20.3}},
@@ -37,26 +40,32 @@
               {'time': '2022-12-19T13:28:03.145696Z', 'tags': {'sensorid': '3'},
                                                       'fields': {'humidity': 53.3, 'temp': 20.3}},
               {'time': '2022-12-19T13:26:02.852427Z', 'tags': {'sensorid': '3'},
                                                       'fields': {'humidity': 53.4, 'temp': 20.2}}]
     service.conn.insert('DHT22', points)
 
     def test_index(self):
+        """ Test for the main entry point
+        """
         response = self.client.get('/')
-        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.status_code, 501)
 
     def test_alexaintent(self):
+        """Test for alexa intent
+        """
         response = self.client.get('/alexaintent')
         self.assertEqual(response.status_code, 404)
         response = self.client.get('/alexaintent?sensor=buhardilla')
         self.assertEqual(response.status_code, 200)
         response = self.client.get('/alexaintent?sensor=unexisting')
         self.assertEqual(response.status_code, 404)
 
     def test_customsensor(self):
+        """Custom sensor test
+        """
         response = self.client.get('/customsensor')
         self.assertEqual(response.status_code, 404)
         response = self.client.get('/customsensor?sensor=buhardilla')
         self.assertEqual(response.status_code, 200)
         response = self.client.get('/customsensor?sensor=unexisting')
         self.assertEqual(response.status_code, 404)
```

