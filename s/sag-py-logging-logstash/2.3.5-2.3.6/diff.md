# Comparing `tmp/sag-py-logging-logstash-2.3.5.tar.gz` & `tmp/sag-py-logging-logstash-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-logstash-2.3.5.tar", last modified: Tue Apr  4 07:01:42 2023, max compression
+gzip compressed data, was "sag-py-logging-logstash-2.3.6.tar", last modified: Thu Apr 20 10:03:32 2023, max compression
```

## Comparing `sag-py-logging-logstash-2.3.5.tar` & `sag-py-logging-logstash-2.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:01:42.987369 sag-py-logging-logstash-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-04 07:01:42.987369 sag-py-logging-logstash-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:01:42.983369 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/memory_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:01:42.987369 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-04 07:01:42.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-04 07:01:42.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:01:42.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 07:01:42.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 07:01:42.000000 sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 07:01:42.987369 sag-py-logging-logstash-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-04 07:01:32.000000 sag-py-logging-logstash-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:03:32.191274 sag-py-logging-logstash-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-20 10:03:32.191274 sag-py-logging-logstash-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:03:32.191274 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/memory_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:03:32.191274 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-20 10:03:32.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-20 10:03:32.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:03:32.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 10:03:32.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 10:03:32.000000 sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 10:03:32.195274 sag-py-logging-logstash-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 10:03:23.000000 sag-py-logging-logstash-2.3.6/setup.py
```

### Comparing `sag-py-logging-logstash-2.3.5/LICENSE.txt` & `sag-py-logging-logstash-2.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/PKG-INFO` & `sag-py-logging-logstash-2.3.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: sag-py-logging-logstash
-Version: 2.3.5
-Summary: Python logging logstash handler
-Home-page: https://github.com/SamhammerAG/sag_py_logging_logstash
-Author: Samhammer AG
-Author-email: support@samhammer.de
-License: MIT
-Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging_logstash
-Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging_logstash/issues
-Project-URL: Source, https://github.com/SamhammerAG/sag_py_logging_logstash
-Keywords: logging,logstash
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development
-Classifier: Topic :: System :: Logging
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # sag_py_logging_logstash
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash)
 
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_logging_logstash/badge.svg?branch=master
@@ -44,16 +20,16 @@
 collected events in a separate worker thread to Logstash.
 This way, the main application (or thread) where the log event occurred, doesn't need to
 wait until the submission to the remote Logstash instance succeeded.
 
 This is especially useful for applications like websites or web services or any kind of
 request serving API where response times matter.
 
-Usage
------
+## Usage
+
 Example::
 
     from logstash_async.handler import AsynchronousLogstashHandler
     from logstash_async.formatter import LogstashFormatter
     import logging
 
     logstash_handler = AsynchronousLogstashHandler(
@@ -72,17 +48,35 @@
     logging.basicConfig(
     level="INFO",
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     handlers=logging_handlers)
 
     logging.getLogger().info("Logging Message", extra = {'new_field':"value"})
 
-Local Installation
-------------------
 
-pip install sag_py_logging_logstash
+### Installation
+pip install sag-py-logging-logstash
+
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
+
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
 
-How to publish
---------------
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/cache.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/cache.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/constants.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/constants.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/formatter.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from datetime import date, datetime
 
 from sag_py_logging_logstash.constants import constants
 
 try:
     import json
 except ImportError:
-    import simplejson as json
+    import simplejson as json  # type: ignore
 
 
 class LogstashFormatter(logging.Formatter):
     # ----------------------------------------------------------------------
     # pylint: disable=too-many-arguments
     def __init__(
         self,
```

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/handler.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # This software may be modified and distributed under the terms
 # of the MIT license.  See the LICENSE file for details.
 
 from logging import Handler
+from typing import Union
 
 from sag_py_logging_logstash.constants import constants
 from sag_py_logging_logstash.formatter import LogstashFormatter
 from sag_py_logging_logstash.utils import safe_log_via_print
 from sag_py_logging_logstash.worker import LogProcessingWorker
 
 from .transport import HttpTransport
@@ -89,17 +90,17 @@
     # ----------------------------------------------------------------------
     def _worker_thread_is_running(self):
         return self._worker_thread is not None and self._worker_thread.is_alive()
 
     # ----------------------------------------------------------------------
     def _format_record(self, record):
         self._create_formatter_if_necessary()
-        formatted = self.formatter.format(record)
+        formatted: Union[str, bytes] = self.formatter.format(record)
         if isinstance(formatted, str):
-            formatted = formatted.encode(self._encoding)  # pylint: disable=redefined-variable-type
+            formatted = formatted.encode(self._encoding)
         return formatted + b"\n"
 
     # ----------------------------------------------------------------------
     def _create_formatter_if_necessary(self):
         if self.formatter is None:
             self.formatter = LogstashFormatter()
```

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/memory_cache.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/memory_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             # there is really nothing for us to do. Right now
             # this use-case does not raise an error. Instead, we
             # just log the message.
             if event_to_queue:
                 event_to_queue["pending_delete"] = False
             else:
                 self.logger.warning(
-                    "Could not requeue event with id {}. " "It does not appear to be in the cache.".format(event["id"])
+                    "Could not requeue event with id {}. It does not appear to be in the cache.".format(event["id"])
                 )
 
     # ----------------------------------------------------------------------
     def delete_queued_events(self):
         ids_to_delete = [event["id"] for event in self._cache.values() if event["pending_delete"]]
         self._delete_events(ids_to_delete)
 
@@ -84,9 +84,9 @@
     def _delete_events(self, ids_to_delete):
         for event_id in ids_to_delete:
             # If the event is not in the cache, is there anything
             # that we can do. This currently doesn't throw an error.
             event = self._cache.pop(event_id, None)
             if not event:
                 self.logger.warning(
-                    "Could not delete event with id {}. " "It does not appear to be in the cache.".format(event_id)
+                    "Could not delete event with id {}. It does not appear to be in the cache.".format(event_id)
                 )
```

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/transport.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         port: int,
         timeout: Union[None, float],
         ssl_enable: bool,
         use_logging: bool,
     ):
         self._host = host
         self._port = port
-        self._timeout = None if timeout is TimeoutNotSet else timeout
+        self._timeout = None if timeout is TimeoutNotSet else timeout  # type: ignore
         self._ssl_enable = ssl_enable
         self._use_logging = use_logging
         super().__init__()
 
     @abstractmethod
     def send(self, events: list, **kwargs):
         pass
@@ -86,15 +86,15 @@
     :type max_content_length: int
     """
 
     def __init__(
         self,
         host: str,
         port: int,
-        timeout: Union[None, float] = TimeoutNotSet,
+        timeout: Union[None, float] = TimeoutNotSet,  # type: ignore
         ssl_enable: bool = True,
         use_logging: bool = False,
         **kwargs,
     ):
         super().__init__(host, port, timeout, ssl_enable, use_logging)
         self._username = kwargs.get("username", None)
         self._password = kwargs.get("password", None)
@@ -135,16 +135,15 @@
                 current_event = None
                 if not current_batch:
                     return
                 yield current_batch
             if current_event is None:
                 return
             if len(current_event) > self._max_content_length:
-                msg = "The event size <%s> is greater than the max content length <%s>."
-                msg += "Skipping event."
+                msg = "The event size <%s> is greater than the max content length <%s>. Skipping event."
                 if self._use_logging:
                     logger.warning(msg, len(current_event), self._max_content_length)
                 continue
             obj = json.loads(current_event)
             content_length = len(json.dumps(current_batch + [obj]).encode("utf8"))
             if content_length > self._max_content_length:
                 batch = current_batch
```

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/utils.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/utils.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash/worker.py` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash/worker.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/sag_py_logging_logstash.egg-info/SOURCES.txt` & `sag-py-logging-logstash-2.3.6/sag_py_logging_logstash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.5/setup.py` & `sag-py-logging-logstash-2.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 with open("requirements.txt", "r") as fin:
     REQS = fin.read().splitlines()
 
+with open("requirements-dev.txt", "r") as fin:
+    REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
+
 setuptools.setup(
     name="sag-py-logging-logstash",
-    version="2.3.5",
+    version="2.3.6",
     description="Python logging logstash handler",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging_logstash",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +28,14 @@
         "Topic :: Software Development",
         "Topic :: System :: Logging",
     ],
     keywords="logging, logstash",
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"]},
+    extras_require={"dev": REQS_DEV},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_logging_logstash",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_logging_logstash/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_logging_logstash",
     },
 )
```

