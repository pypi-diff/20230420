# Comparing `tmp/moesifwsgi-1.6.0.tar.gz` & `tmp/moesifwsgi-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifwsgi-1.6.0.tar", last modified: Thu Oct 13 04:10:31 2022, max compression
+gzip compressed data, was "dist/moesifwsgi-1.6.1.tar", last modified: Thu Apr 20 01:34:17 2023, max compression
```

## Comparing `moesifwsgi-1.6.0.tar` & `moesifwsgi-1.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:10:31.718540 moesifwsgi-1.6.0/
--rwxr-xr-x   0 praveen    (501) staff       (20)    11911 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/LICENSE
--rw-r--r--   0 praveen    (501) staff       (20)       61 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/MANIFEST.in
--rw-r--r--   0 praveen    (501) staff       (20)    17593 2022-10-13 04:10:31.718652 moesifwsgi-1.6.0/PKG-INFO
--rwxr-xr-x   0 praveen    (501) staff       (20)    16396 2022-09-21 22:56:45.000000 moesifwsgi-1.6.0/README.md
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:10:31.717759 moesifwsgi-1.6.0/moesifwsgi/
--rw-r--r--   0 praveen    (501) staff       (20)       26 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)     4634 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/client_ip.py
--rw-r--r--   0 praveen    (501) staff       (20)     3345 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/event_mapper.py
--rw-r--r--   0 praveen    (501) staff       (20)      810 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/http_response_catcher.py
--rw-r--r--   0 praveen    (501) staff       (20)    10145 2022-09-21 22:56:45.000000 moesifwsgi-1.6.0/moesifwsgi/logger_helper.py
--rw-r--r--   0 praveen    (501) staff       (20)    13030 2022-10-13 04:09:43.000000 moesifwsgi-1.6.0/moesifwsgi/middleware.py
--rw-r--r--   0 praveen    (501) staff       (20)     2834 2022-09-27 01:05:57.000000 moesifwsgi-1.6.0/moesifwsgi/moesif_data_holder.py
--rw-r--r--   0 praveen    (501) staff       (20)     2344 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/parse_body.py
--rw-r--r--   0 praveen    (501) staff       (20)     4018 2022-09-21 22:56:45.000000 moesifwsgi-1.6.0/moesifwsgi/regex_config_helper.py
--rw-r--r--   0 praveen    (501) staff       (20)     2168 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/send_batch_events.py
--rw-r--r--   0 praveen    (501) staff       (20)     6638 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/update_companies.py
--rw-r--r--   0 praveen    (501) staff       (20)     6378 2021-12-24 00:24:54.000000 moesifwsgi-1.6.0/moesifwsgi/update_users.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:10:31.718440 moesifwsgi-1.6.0/moesifwsgi.egg-info/
--rw-r--r--   0 praveen    (501) staff       (20)    17593 2022-10-13 04:10:31.000000 moesifwsgi-1.6.0/moesifwsgi.egg-info/PKG-INFO
--rw-r--r--   0 praveen    (501) staff       (20)      562 2022-10-13 04:10:31.000000 moesifwsgi-1.6.0/moesifwsgi.egg-info/SOURCES.txt
--rw-r--r--   0 praveen    (501) staff       (20)        1 2022-10-13 04:10:31.000000 moesifwsgi-1.6.0/moesifwsgi.egg-info/dependency_links.txt
--rw-r--r--   0 praveen    (501) staff       (20)      104 2022-10-13 04:10:31.000000 moesifwsgi-1.6.0/moesifwsgi.egg-info/requires.txt
--rw-r--r--   0 praveen    (501) staff       (20)       11 2022-10-13 04:10:31.000000 moesifwsgi-1.6.0/moesifwsgi.egg-info/top_level.txt
--rw-r--r--   0 praveen    (501) staff       (20)       67 2022-10-13 04:10:31.718979 moesifwsgi-1.6.0/setup.cfg
--rw-r--r--   0 praveen    (501) staff       (20)     3370 2022-10-13 04:09:43.000000 moesifwsgi-1.6.0/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.931962 moesifwsgi-1.6.1/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11911 2020-06-25 11:08:31.000000 moesifwsgi-1.6.1/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-04-19 17:20:34.000000 moesifwsgi-1.6.1/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    20958 2023-04-20 01:34:17.932272 moesifwsgi-1.6.1/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    16396 2023-04-19 16:52:37.000000 moesifwsgi-1.6.1/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.929460 moesifwsgi-1.6.1/moesifwsgi/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2020-04-19 17:20:34.000000 moesifwsgi-1.6.1/moesifwsgi/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4634 2020-12-29 19:45:45.000000 moesifwsgi-1.6.1/moesifwsgi/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3526 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     1067 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/http_response_catcher.py
+-rw-r--r--   0 keyur      (501) staff       (20)    10434 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)    13821 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3071 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/moesif_data_holder.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2344 2020-12-29 19:47:50.000000 moesifwsgi-1.6.1/moesifwsgi/parse_body.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4018 2022-01-13 23:06:22.000000 moesifwsgi-1.6.1/moesifwsgi/regex_config_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2500 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/send_batch_events.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8531 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/update_companies.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8100 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/moesifwsgi/update_users.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-04-20 01:34:17.931704 moesifwsgi-1.6.1/moesifwsgi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    20958 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      562 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)      104 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       11 2023-04-20 01:34:17.000000 moesifwsgi-1.6.1/moesifwsgi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2023-04-20 01:34:17.933198 moesifwsgi-1.6.1/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3370 2023-04-20 01:32:27.000000 moesifwsgi-1.6.1/setup.py
```

### Comparing `moesifwsgi-1.6.0/LICENSE` & `moesifwsgi-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.0/PKG-INFO` & `moesifwsgi-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: moesifwsgi
-Version: 1.6.0
-Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
-Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
-Author: Moesif, Inc
-Author-email: xing@moesif.com
-License: Apache Software License
-Keywords: log analysis restful api development debug wsgi flask bottle http middleware
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: Log Analysis
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Moesif Middleware for Python WSGI based Frameworks
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
 [![Source Code][ico-source]][link-source]
@@ -445,9 +416,7 @@
 [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
 
 [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
 [link-package]: https://pypi.python.org/pypi/moesifwsgi
 [link-language]: https://pypi.python.org/pypi/moesifwsgi
 [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
 [link-source]: https://github.com/Moesif/moesifwsgi
-
-
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/client_ip.py` & `moesifwsgi-1.6.1/moesifwsgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.0/moesifwsgi/event_mapper.py` & `moesifwsgi-1.6.1/moesifwsgi/event_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from moesifapi.models import *
 from .parse_body import ParseBody
+from .logger_helper import LoggerHelper
 
 
 class EventMapper:
 
     def __init__(self):
         self.parse_body = ParseBody()
+        self.logger_helper = LoggerHelper()
 
     @classmethod
     def to_event(cls, data, event_req, event_rsp):
         # Prepare Event Model
         return EventModel(request=event_req,
                           response=event_rsp,
                           user_id=data.user_id,
@@ -46,25 +48,25 @@
         try:
             response_content = "".join(data.response_chunks)
         except:
             try:
                 response_content = b"".join(data.response_chunks)
             except:
                 if debug:
-                    print('try to join response chunks failed - ')
+                    print('try to join response chunks failed - for pid - ' + self.logger_helper.get_worker_pid())
 
         rsp_headers = None
         if data.response_headers:
             rsp_headers = dict(data.response_headers)
 
         rsp_body = None
         rsp_transfer_encoding = None
         if log_body and response_content:
             if debug:
-                print("about to process response")
+                print("about to process response for pid - " + self.logger_helper.get_worker_pid())
                 print(response_content)
             if isinstance(response_content, str):
                 rsp_body, rsp_transfer_encoding = self.parse_body.parse_string_body(response_content, None,
                                                                                          self.parse_body.transform_headers(
                                                                                              rsp_headers))
             else:
                 rsp_body, rsp_transfer_encoding = self.parse_body.parse_bytes_body(response_content, None,
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/http_response_catcher.py` & `moesifwsgi-1.6.1/moesifwsgi/http_response_catcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """
     moesif.http_response_catcher
 """
 
 from moesifapi.http.http_call_back import *
+from .logger_helper import LoggerHelper
 
 class HttpResponseCatcher(HttpCallBack):
 
     """A class used for catching the HttpResponse object from controllers.
 
     This class inherits HttpCallBack and implements the on_after_response
     method to catch the HttpResponse object as returned by the HttpClient
     after a request is executed.
     """
+
+    def __init__(self):
+        self.logger_helper = LoggerHelper()
+
     def on_before_request(self, request):
         pass
 
     def on_after_response(self, context):
         self.response = context.response
-        print('status from the Moesif API call')
+        print('status from the Moesif API call for pid - ' + self.logger_helper.get_worker_pid())
         print(context.response.status_code)
-        print('headers from moesif response')
+        print('headers from moesif response for pid - ' + self.logger_helper.get_worker_pid())
         print(context.response.headers)
-        print('body from moesif response')
+        print('body from moesif response for pid - ' + self.logger_helper.get_worker_pid())
         print(context.response.raw_body)
         #pass
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/logger_helper.py` & `moesifwsgi-1.6.1/moesifwsgi/logger_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 try:
     from cStringIO import StringIO
 except ImportError:
     from io import StringIO
 from .parse_body import ParseBody
 from io import BytesIO
 import json
@@ -104,15 +106,19 @@
         return None
 
     def get_user_id(self, environ, settings, app, debug, response_headers=dict()):
         username = None
         try:
             identify_user = settings.get("IDENTIFY_USER")
             if identify_user is not None:
-                username = identify_user(app, environ, response_headers)
+                try:
+                    username = identify_user(app, environ, response_headers)
+                except Exception as e:
+                    print("Exception in identify_user function, please check your identify_user method ")
+                    print(e)
             if not username:
                 # Parse request headers
                 request_headers = dict([(k.lower(), v) for k, v in self.parse_request_headers(environ)])
                 # Fetch the auth header name from the config
                 auth_header_names = settings.get('AUTHORIZATION_HEADER_NAME', 'authorization').lower()
                 # Split authorization header name by comma
                 auth_header_names = [x.strip() for x in auth_header_names.split(',')]
@@ -230,7 +236,11 @@
             mask_event_model = settings.get("MASK_EVENT_MODEL")
             if mask_event_model is not None:
                 return mask_event_model(event_model)
         except:
             if debug:
                 print("Can not execute MASK_EVENT_MODEL function. Please check moesif settings.")
         return event_model
+
+    @classmethod
+    def get_worker_pid(cls):
+        return str(os.getpid())
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/middleware.py` & `moesifwsgi-1.6.1/moesifwsgi/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,34 +46,34 @@
         if settings.get('APPLICATION_ID', None):
             self.client = MoesifAPIClient(settings.get('APPLICATION_ID'))
         else:
             raise Exception('Moesif Application ID is required in settings')
 
         if settings.get('DEBUG', False):
             Configuration.BASE_URI = self.get_configuration_uri(settings, 'BASE_URI', 'LOCAL_MOESIF_BASEURL')
-        Configuration.version = 'moesifwsgi-python/1.3.5'
+        Configuration.version = 'moesifwsgi-python/1.6.1'
         self.DEBUG = settings.get('DEBUG', False)
+        self.logger_helper = LoggerHelper()
         if settings.get('CAPTURE_OUTGOING_REQUESTS', False):
             try:
                 if self.DEBUG:
-                    print('Start capturing outgoing requests')
+                    print('Start capturing outgoing requests for pid - ' + self.logger_helper.get_worker_pid())
                 # Start capturing outgoing requests
                 StartCapture().start_capture_outgoing(settings)
             except:
-                print('Error while starting to capture the outgoing events')
+                print('Error while starting to capture the outgoing events for pid - ' + self.logger_helper.get_worker_pid())
         self.api_version = settings.get('API_VERSION')
         self.api_client = self.client.api
         self.LOG_BODY = self.settings.get('LOG_BODY', True)
         if self.DEBUG:
             response_catcher = HttpResponseCatcher()
             self.api_client.http_call_back = response_catcher
         self.client_ip = ClientIp()
         self.app_config = AppConfig()
         self.parse_body = ParseBody()
-        self.logger_helper = LoggerHelper()
         self.event_mapper = EventMapper()
         self.send_async_events = SendEventAsync()
         self.config_etag = None
         self.config = self.app_config.get_config(self.api_client, self.DEBUG)
         self.sampling_percentage = 100
         self.last_updated_time = datetime.utcnow()
         self.moesif_events_queue = queue.Queue()
@@ -83,15 +83,15 @@
         self.is_event_job_scheduled = False
         try:
             if self.config:
                 self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
                     self.config, self.DEBUG)
         except Exception as ex:
             if self.DEBUG:
-                print('Error while parsing application configuration on initialization')
+                print('Error while parsing application configuration on initialization for pid - ' + self.logger_helper.get_worker_pid())
                 print(str(ex))
 
     # Function to get configuration uri
     def get_configuration_uri(self, settings, field, deprecated_field):
         uri = settings.get(field)
         if uri:
             return uri
@@ -113,31 +113,31 @@
                         *self.logger_helper.request_body(environ),
                         request_time
                     )
 
         response_headers_mapping = {}
         def _start_response(status, response_headers, *args):
             # Capture status and response_headers for later processing
-            data_holder.capture_response_status(status, response_headers)
+            data_holder.capture_response_status(status, response_headers, self.DEBUG)
 
             if response_headers:
                 try:
                     for pair in response_headers:
                         response_headers_mapping[pair[0]] = pair[1]
                 except Exception as e:
-                    print('Error while parsing response headers', e)
+                    print('Error while parsing response headers for pid - ' + self.logger_helper.get_worker_pid(), e)
 
             return start_response(status, response_headers, *args)
 
         response_chunks = data_holder.finish_response(self.app(environ, _start_response))
         if self.DEBUG:
             try:
-                print("event response time: ", data_holder.response_time)
+                print("event response time for pid - " + self.logger_helper.get_worker_pid(), data_holder.response_time)
             except Exception as e:
-                print("Error while fetching response time", e)
+                print("Error while fetching response time for pid - " + self.logger_helper.get_worker_pid(), e)
 
         data_holder.set_user_id(self.logger_helper.get_user_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
         data_holder.set_company_id(self.logger_helper.get_company_id(environ, self.settings, self.app, self.DEBUG, response_headers_mapping))
         data_holder.set_metadata(self.logger_helper.get_metadata(environ, self.settings, self.app, self.DEBUG))
         data_holder.set_session_token(self.logger_helper.get_session_token(environ, self.settings, self.app, self.DEBUG))
 
         # return data to WSGI server
@@ -168,33 +168,35 @@
                                 try:
                                     self.schedule_background_job()
                                     self.is_event_job_scheduled = True
                                     self.last_event_job_run_time = datetime.utcnow()
                                 except Exception as ex:
                                     self.is_event_job_scheduled = False
                                     if self.DEBUG:
-                                        print('Error while starting the event scheduler job in background')
+                                        print('Error while starting the event scheduler job in background for pid - '
+                                              + self.logger_helper.get_worker_pid())
                                         print(str(ex))
                             # Add Event to the queue
                             if self.DEBUG:
-                                print('Add Event to the queue')
+                                print('Add Event to the queue for pid - ' + self.logger_helper.get_worker_pid())
                             self.moesif_events_queue.put(event_data)
                         except Exception as ex:
                             if self.DEBUG:
-                                print("Error while adding event to the queue")
+                                print("Error while adding event to the queue for pid - " + self.logger_helper.get_worker_pid())
                                 print(str(ex))
                     else:
                         if self.DEBUG:
-                            print('Skipped Event as the moesif event model is None')
+                            print('Skipped Event as the moesif event model is None for pid - ' + self.logger_helper.get_worker_pid())
                 else:
                     if self.DEBUG:
-                        print("Skipped Event due to sampling percentage: " + str(self.sampling_percentage) + " and random percentage: " + str(random_percentage))
+                        print("Skipped Event due to sampling percentage: " + str(self.sampling_percentage)
+                              + " and random percentage: " + str(random_percentage) + " for pid - " + self.logger_helper.get_worker_pid())
             else:
                 if self.DEBUG:
-                    print('Skipped Event using should_skip configuration option')
+                    print('Skipped Event using should_skip configuration option for pid - ' + self.logger_helper.get_worker_pid())
 
     def process_data(self, data):
 
         # Prepare Event Request Model
         event_req = self.event_mapper.to_request(data, self.LOG_BODY, self.api_version)
 
         # Prepare Event Response Model
@@ -206,29 +208,29 @@
         # Mask Event Model
         return self.logger_helper.mask_event(event_model, self.settings, self.DEBUG)
 
     # Function to listen to the send event job response
     def moesif_event_listener(self, event):
         if event.exception:
             if self.DEBUG:
-                print('Error reading response from the scheduled job')
+                print('Error reading response from the scheduled job for pid - ' + self.logger_helper.get_worker_pid())
         else:
             if event.retval:
                 response_etag, self.last_event_job_run_time = event.retval
                 if response_etag is not None \
                     and self.config_etag is not None \
                     and self.config_etag != response_etag \
                         and datetime.utcnow() > self.last_updated_time + timedelta(minutes=5):
                     try:
                         self.config = self.app_config.get_config(self.api_client, self.DEBUG)
                         self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
                             self.config, self.DEBUG)
                     except Exception as ex:
                         if self.DEBUG:
-                            print('Error while updating the application configuration')
+                            print('Error while updating the application configuration for pid - ' + self.logger_helper.get_worker_pid())
                             print(str(ex))
 
     def schedule_background_job(self):
         try:
             if not self.scheduler:
                 self.scheduler = BackgroundScheduler(daemon=True)
             if not self.scheduler.get_jobs():
@@ -245,17 +247,16 @@
                 # Avoid passing logging message to the ancestor loggers
                 logging.getLogger('apscheduler.executors.default').setLevel(logging.WARNING)
                 logging.getLogger('apscheduler.executors.default').propagate = False
 
                 # Exit handler when exiting the app
                 atexit.register(lambda: self.send_async_events.exit_handler(self.scheduler, self.DEBUG))
         except Exception as ex:
-            if self.DEBUG:
-                print("Error when scheduling the job")
-                print(str(ex))
+            print("Error when scheduling the job for pid - " + self.logger_helper.get_worker_pid())
+            print(str(ex))
 
     def update_user(self, user_profile):
         User().update_user(user_profile, self.api_client, self.DEBUG)
 
     def update_users_batch(self, user_profiles):
         User().update_users_batch(user_profiles, self.api_client, self.DEBUG)
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/moesif_data_holder.py` & `moesifwsgi-1.6.1/moesifwsgi/moesif_data_holder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 import time
 import uuid
+from .logger_helper import LoggerHelper
 
 class DataHolder(object):
     """Capture the data for a request-response."""
     def __init__(self, disable_capture_transaction_id, id, method, url, ip, request_headers, content_length, request_body, transfer_encoding, request_time):
         self.request_id = id
         self.method = method
         self.url = url
@@ -20,14 +21,15 @@
         self.status = -1
         self.response_headers = None
         self.response_chunks = None
         self.response_body_data = None
         self.request_time = request_time
         self.start_at = time.time()
         self.transaction_id = None
+        self.logger_helper = LoggerHelper()
 
         if not disable_capture_transaction_id:
             req_trans_id = [value for key, value in request_headers if key == "X-Moesif-Transaction-Id"]
             if req_trans_id:
                 self.transaction_id = req_trans_id[0]
                 if not self.transaction_id:
                     self.transaction_id = str(uuid.uuid4())
@@ -44,19 +46,22 @@
 
     def set_metadata(self, metadata):
         self.metadata = metadata
 
     def set_session_token(self, session_token):
         self.session_token = session_token
 
-    def capture_response_status(self, status, response_headers):
+    def capture_response_status(self, status, response_headers, debug):
         self.status = status
         # Add transaction id to the response header
         if self.transaction_id:
             response_headers.append(("X-Moesif-Transaction-Id", self.transaction_id))
+        # Add worker process Id
+        if debug:
+            response_headers.append(("X-Moesif-Wsgi-Pid", self.logger_helper.get_worker_pid()))
         self.response_headers = response_headers
 
     def capture_body_data(self, body_data):
         if self.response_body_data is None:
             self.response_body_data = body_data
         else:
             self.response_body_data = self.response_body_data + body_data
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi/parse_body.py` & `moesifwsgi-1.6.1/moesifwsgi/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.0/moesifwsgi/regex_config_helper.py` & `moesifwsgi-1.6.1/moesifwsgi/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.0/moesifwsgi.egg-info/PKG-INFO` & `moesifwsgi-1.6.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,438 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.6.0
+Version: 1.6.1
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
+Description: # Moesif Middleware for Python WSGI based Frameworks
+        
+        [![Built For][ico-built-for]][link-built-for]
+        [![Latest Version][ico-version]][link-package]
+        [![Language Versions][ico-language]][link-language]
+        [![Software License][ico-license]][link-license]
+        [![Source Code][ico-source]][link-source]
+        
+        WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
+        Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
+        
+        [Source Code on GitHub](https://github.com/moesif/moesifwsgi)
+        
+        [WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
+        is a standard (PEP 3333) that describes
+        how a web server communicates with web applications. Many Python Frameworks
+        are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
+        [Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
+        Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
+        easily integrate with [Moesif](https://www.moesif.com).
+        
+        ## How to install
+        
+        ```shell
+        pip install moesifwsgi
+        ```
+        
+        ## How to use
+        
+        ### Flask
+        
+        Wrap your wsgi_app with the Moesif middleware.
+        
+        ```python
+        from moesifwsgi import MoesifMiddleware
+        
+        moesif_settings = {
+            'APPLICATION_ID': 'Your Moesif Application id',
+            'LOG_BODY': True,
+            # ... For other options see below.
+        }
+        
+        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+        
+        ```
+        
+        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+        
+        You can always find your Moesif Application Id at any time by logging 
+        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+        and then clicking _API Keys_.
+        
+        For an example with Flask, see example in the `/examples/flask` folder of this repo.
+        
+        ### Bottle
+        Wrap your bottle app with the Moesif middleware.
+        
+        ```python
+        
+        from moesifwsgi import MoesifMiddleware
+        
+        app = bottle.Bottle()
+        
+        moesif_settings = {
+            'APPLICATION_ID': 'Your Moesif Application Id',
+            'LOG_BODY': True,
+            # ... For other options see below.
+        }
+        
+        bottle.run(app=MoesifMiddleware(app, moesif_settings))
+        
+        ```
+        
+        For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
+        
+        ### Pyramid
+        
+        
+        ```python
+        from pyramid.config import Configurator
+        from moesifwsgi import MoesifMiddleware
+        
+        if __name__ == '__main__':
+            config = Configurator()
+            config.add_route('hello', '/')
+            config.scan()
+            app = config.make_wsgi_app()
+        
+            # configure your moesif settings
+            moesif_settings = {
+                'APPLICATION_ID': 'Your Moesif Application Id',
+                'LOG_BODY': True,
+                # ... For other options see below.
+            }
+            # Put middleware
+            app = MoesifMiddleware(app, moesif_settings)
+        
+            server = make_server('0.0.0.0', 8080, app)
+            server.serve_forever()
+        
+        ```
+        ### Other WSGI frameworks
+        
+        If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
+        Please read the documentation for your specific framework on how to add middleware.
+        
+        ## Configuration options
+        
+        #### __`APPLICATION_ID`__
+        (__required__), _string_, is obtained via your Moesif Account, this is required.
+        
+        #### __`SKIP`__
+        (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
+        and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
+        environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+        
+        #### __`IDENTIFY_USER`__
+        (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+        
+        #### __`IDENTIFY_COMPANY`__
+        (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
+        
+        #### __`GET_METADATA`__
+        (optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
+        returns a dictionary (must be able to be encoded into JSON). This allows your
+        to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
+        
+        #### __`GET_SESSION_TOKEN`__
+        (optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+        
+        #### __`MASK_EVENT_MODEL`__
+        (optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
+        
+        #### __`DEBUG`__
+        (optional) _boolean_, a flag to see debugging messages.
+        
+        #### __`LOG_BODY`__
+        (optional) _boolean_, default True, Set to False to remove logging request and response body.
+        
+        #### __`BATCH_SIZE`__
+        (optional) __int__, default 25, Maximum batch size when sending events to Moesif.
+        
+        #### __`AUTHORIZATION_HEADER_NAME`__
+        (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
+        
+        #### __`AUTHORIZATION_USER_ID_FIELD`__
+        (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
+        
+        #### __`BASE_URI`__
+        (optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
+        
+        ### Options specific to outgoing API calls 
+        
+        The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
+        
+        For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
+        
+        If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
+        
+        #### __`CAPTURE_OUTGOING_REQUESTS`__
+        _boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
+        
+        ##### __`GET_METADATA_OUTGOING`__
+        (optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
+        Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
+        returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
+        
+        ##### __`SKIP_OUTGOING`__
+        (optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
+        and returns true if you want to skip this particular event.
+        
+        ##### __`IDENTIFY_USER_OUTGOING`__
+        (optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+        
+        ##### __`IDENTIFY_COMPANY_OUTGOING`__
+        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
+        
+        ##### __`GET_SESSION_TOKEN_OUTGOING`__
+        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+        
+        ##### __`LOG_BODY_OUTGOING`__
+        (optional) _boolean_, default True, Set to False to remove logging request and response body.
+        
+        ### Example:
+        
+        ```python
+        def identify_user(app, environ, response_headers=dict()):
+            # Your custom code that returns a user id string
+            return "12345"
+        
+        def identify_company(app, environ, response_headers=dict()):
+            # Your custom code that returns a company id string
+            return "67890"
+        
+        def should_skip(app, environ):
+            # Your custom code that returns true to skip logging
+            return "health/probe" in environ.get('PATH_INFO', '')
+        
+        def get_token(app, environ):
+            # If you don't want to use the standard WSGI session token,
+            # add your custom code that returns a string for session/API token
+            return "XXXXXXXXXXXXXX"
+        
+        def mask_event(eventmodel):
+            # Your custom code to change or remove any sensitive fields
+            if 'password' in eventmodel.response.body:
+                eventmodel.response.body['password'] = None
+            return eventmodel
+        
+        def get_metadata(app, environ):
+            return {
+                'datacenter': 'westus',
+                'deployment_version': 'v1.2.3',
+            }
+        
+        moesif_settings = {
+            'APPLICATION_ID': 'Your Moesif Application Id',
+            'DEBUG': False,
+            'LOG_BODY': True,
+            'IDENTIFY_USER': identify_user,
+            'IDENTIFY_COMPANY': identify_company,
+            'GET_SESSION_TOKEN': get_token,
+            'SKIP': should_skip,
+            'MASK_EVENT_MODEL': mask_event,
+            'GET_METADATA': get_metadata,
+            'CAPTURE_OUTGOING_REQUESTS': False
+        }
+        
+        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+        
+        ```
+        
+        ## Update User
+        
+        ### Update A Single User
+        Create or update a user profile in Moesif.
+        The metadata field can be any customer demographic or other info you want to store.
+        Only the `user_id` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+        
+        ```python
+        api_client = MoesifAPIClient("Your Moesif Application Id").api
+        
+        # Only user_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#users for campaign schema
+        # metadata can be any custom object
+        user = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        update_user = api_client.update_user(user)
+        ```
+        
+        ### Update Users in Batch
+        Similar to update_user, but used to update a list of users in one batch. 
+        Only the `user_id` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+        
+        ```python
+        api_client = MoesifAPIClient("Your Moesif Application Id").api
+        
+        userA = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        userB = {
+          'user_id': '54321',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'mary@acmeinc.com',
+            'first_name': 'Mary',
+            'last_name': 'Jane',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 48000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        update_users = api_client.update_users_batch([userA, userB])
+        ```
+        
+        ## Update Company
+        
+        ### Update A Single Company
+        Create or update a company profile in Moesif.
+        The metadata field can be any company demographic or other info you want to store.
+        Only the `company_id` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+        
+        ```python
+        api_client = MoesifAPIClient("Your Moesif Application Id").api
+        
+        # Only company_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
+        # metadata can be any custom object
+        company = {
+          'company_id': '67890',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        }
+        
+        update_company = api_client.update_company(company)
+        ```
+        
+        ### Update Companies in Batch
+        Similar to update_company, but used to update a list of companies in one batch. 
+        Only the `company_id` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+        
+        ```python
+        api_client = MoesifAPIClient("Your Moesif Application Id").api
+        
+        companyA = {
+          'company_id': '67890',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        }
+        
+        companyB = {
+          'company_id': '09876',
+          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'metadata': {
+            'org_name': 'Contoso, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 48000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 53
+            },
+          }
+        }
+        
+        update_companies = api_client.update_companies_batch([companyA, companyB])
+        ```
+        ## Troubleshooting
+        
+        When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
+        In order to resolve that, add the following line to your Dockerfile
+        ```
+        ENV TZ=UTC
+        ```
+        or you could add `RUN apt-get install tzdata` in the Dockerfile.
+        
+        ## Other integrations
+        
+        To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
+        
+        [ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
+        [ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
+        [ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
+        [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+        [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
+        
+        [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
+        [link-package]: https://pypi.python.org/pypi/moesifwsgi
+        [link-language]: https://pypi.python.org/pypi/moesifwsgi
+        [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
+        [link-source]: https://github.com/Moesif/moesifwsgi
+        
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
@@ -21,433 +444,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
-
-# Moesif Middleware for Python WSGI based Frameworks
-
-[![Built For][ico-built-for]][link-built-for]
-[![Latest Version][ico-version]][link-package]
-[![Language Versions][ico-language]][link-language]
-[![Software License][ico-license]][link-license]
-[![Source Code][ico-source]][link-source]
-
-WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
-Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
-
-[Source Code on GitHub](https://github.com/moesif/moesifwsgi)
-
-[WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
-is a standard (PEP 3333) that describes
-how a web server communicates with web applications. Many Python Frameworks
-are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
-[Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
-Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
-easily integrate with [Moesif](https://www.moesif.com).
-
-## How to install
-
-```shell
-pip install moesifwsgi
-```
-
-## How to use
-
-### Flask
-
-Wrap your wsgi_app with the Moesif middleware.
-
-```python
-from moesifwsgi import MoesifMiddleware
-
-moesif_settings = {
-    'APPLICATION_ID': 'Your Moesif Application id',
-    'LOG_BODY': True,
-    # ... For other options see below.
-}
-
-app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-
-```
-
-Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-
-You can always find your Moesif Application Id at any time by logging 
-into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
-and then clicking _API Keys_.
-
-For an example with Flask, see example in the `/examples/flask` folder of this repo.
-
-### Bottle
-Wrap your bottle app with the Moesif middleware.
-
-```python
-
-from moesifwsgi import MoesifMiddleware
-
-app = bottle.Bottle()
-
-moesif_settings = {
-    'APPLICATION_ID': 'Your Moesif Application Id',
-    'LOG_BODY': True,
-    # ... For other options see below.
-}
-
-bottle.run(app=MoesifMiddleware(app, moesif_settings))
-
-```
-
-For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
-
-### Pyramid
-
-
-```python
-from pyramid.config import Configurator
-from moesifwsgi import MoesifMiddleware
-
-if __name__ == '__main__':
-    config = Configurator()
-    config.add_route('hello', '/')
-    config.scan()
-    app = config.make_wsgi_app()
-
-    # configure your moesif settings
-    moesif_settings = {
-        'APPLICATION_ID': 'Your Moesif Application Id',
-        'LOG_BODY': True,
-        # ... For other options see below.
-    }
-    # Put middleware
-    app = MoesifMiddleware(app, moesif_settings)
-
-    server = make_server('0.0.0.0', 8080, app)
-    server.serve_forever()
-
-```
-### Other WSGI frameworks
-
-If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
-Please read the documentation for your specific framework on how to add middleware.
-
-## Configuration options
-
-#### __`APPLICATION_ID`__
-(__required__), _string_, is obtained via your Moesif Account, this is required.
-
-#### __`SKIP`__
-(optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
-
-#### __`IDENTIFY_USER`__
-(optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-
-#### __`IDENTIFY_COMPANY`__
-(optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
-
-#### __`GET_METADATA`__
-(optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
-returns a dictionary (must be able to be encoded into JSON). This allows your
-to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
-
-#### __`GET_SESSION_TOKEN`__
-(optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-
-#### __`MASK_EVENT_MODEL`__
-(optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
-
-#### __`DEBUG`__
-(optional) _boolean_, a flag to see debugging messages.
-
-#### __`LOG_BODY`__
-(optional) _boolean_, default True, Set to False to remove logging request and response body.
-
-#### __`BATCH_SIZE`__
-(optional) __int__, default 25, Maximum batch size when sending events to Moesif.
-
-#### __`AUTHORIZATION_HEADER_NAME`__
-(optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
-
-#### __`AUTHORIZATION_USER_ID_FIELD`__
-(optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
-
-#### __`BASE_URI`__
-(optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
-
-### Options specific to outgoing API calls 
-
-The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
-
-For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
-
-If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
-
-#### __`CAPTURE_OUTGOING_REQUESTS`__
-_boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
-
-##### __`GET_METADATA_OUTGOING`__
-(optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
-Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
-returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
-
-##### __`SKIP_OUTGOING`__
-(optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
-and returns true if you want to skip this particular event.
-
-##### __`IDENTIFY_USER_OUTGOING`__
-(optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-
-##### __`IDENTIFY_COMPANY_OUTGOING`__
-(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
-
-##### __`GET_SESSION_TOKEN_OUTGOING`__
-(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-
-##### __`LOG_BODY_OUTGOING`__
-(optional) _boolean_, default True, Set to False to remove logging request and response body.
-
-### Example:
-
-```python
-def identify_user(app, environ, response_headers=dict()):
-    # Your custom code that returns a user id string
-    return "12345"
-
-def identify_company(app, environ, response_headers=dict()):
-    # Your custom code that returns a company id string
-    return "67890"
-
-def should_skip(app, environ):
-    # Your custom code that returns true to skip logging
-    return "health/probe" in environ.get('PATH_INFO', '')
-
-def get_token(app, environ):
-    # If you don't want to use the standard WSGI session token,
-    # add your custom code that returns a string for session/API token
-    return "XXXXXXXXXXXXXX"
-
-def mask_event(eventmodel):
-    # Your custom code to change or remove any sensitive fields
-    if 'password' in eventmodel.response.body:
-        eventmodel.response.body['password'] = None
-    return eventmodel
-
-def get_metadata(app, environ):
-    return {
-        'datacenter': 'westus',
-        'deployment_version': 'v1.2.3',
-    }
-
-moesif_settings = {
-    'APPLICATION_ID': 'Your Moesif Application Id',
-    'DEBUG': False,
-    'LOG_BODY': True,
-    'IDENTIFY_USER': identify_user,
-    'IDENTIFY_COMPANY': identify_company,
-    'GET_SESSION_TOKEN': get_token,
-    'SKIP': should_skip,
-    'MASK_EVENT_MODEL': mask_event,
-    'GET_METADATA': get_metadata,
-    'CAPTURE_OUTGOING_REQUESTS': False
-}
-
-app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-
-```
-
-## Update User
-
-### Update A Single User
-Create or update a user profile in Moesif.
-The metadata field can be any customer demographic or other info you want to store.
-Only the `user_id` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-
-```python
-api_client = MoesifAPIClient("Your Moesif Application Id").api
-
-# Only user_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#users for campaign schema
-# metadata can be any custom object
-user = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-update_user = api_client.update_user(user)
-```
-
-### Update Users in Batch
-Similar to update_user, but used to update a list of users in one batch. 
-Only the `user_id` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-
-```python
-api_client = MoesifAPIClient("Your Moesif Application Id").api
-
-userA = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-userB = {
-  'user_id': '54321',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'mary@acmeinc.com',
-    'first_name': 'Mary',
-    'last_name': 'Jane',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 48000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-update_users = api_client.update_users_batch([userA, userB])
-```
-
-## Update Company
-
-### Update A Single Company
-Create or update a company profile in Moesif.
-The metadata field can be any company demographic or other info you want to store.
-Only the `company_id` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-
-```python
-api_client = MoesifAPIClient("Your Moesif Application Id").api
-
-# Only company_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#update-a-company for campaign schema
-# metadata can be any custom object
-company = {
-  'company_id': '67890',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-}
-
-update_company = api_client.update_company(company)
-```
-
-### Update Companies in Batch
-Similar to update_company, but used to update a list of companies in one batch. 
-Only the `company_id` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-
-```python
-api_client = MoesifAPIClient("Your Moesif Application Id").api
-
-companyA = {
-  'company_id': '67890',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-}
-
-companyB = {
-  'company_id': '09876',
-  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'metadata': {
-    'org_name': 'Contoso, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 48000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 53
-    },
-  }
-}
-
-update_companies = api_client.update_companies_batch([companyA, companyB])
-```
-## Troubleshooting
-
-When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
-In order to resolve that, add the following line to your Dockerfile
-```
-ENV TZ=UTC
-```
-or you could add `RUN apt-get install tzdata` in the Dockerfile.
-
-## Other integrations
-
-To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
-
-[ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
-[ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
-[ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
-[ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-[ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
-
-[link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
-[link-package]: https://pypi.python.org/pypi/moesifwsgi
-[link-language]: https://pypi.python.org/pypi/moesifwsgi
-[link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
-[link-source]: https://github.com/Moesif/moesifwsgi
-
-
```

### Comparing `moesifwsgi-1.6.0/moesifwsgi.egg-info/SOURCES.txt` & `moesifwsgi-1.6.1/moesifwsgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.6.0/setup.py` & `moesifwsgi-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifwsgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.6.0',
+    version='1.6.1',
 
     description='Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-wsgi/',
```

