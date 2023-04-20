# Comparing `tmp/carly-0.9.0.tar.gz` & `tmp/carly-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carly-0.9.0.tar", last modified: Tue Nov 27 09:54:40 2018, max compression
+gzip compressed data, was "carly-0.9.1.tar", last modified: Tue Jan 29 17:11:42 2019, max compression
```

## Comparing `carly-0.9.0.tar` & `carly-0.9.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      206 2018-11-26 18:27:00.850000 carly-0.9.0/carly/__init__.py
--rw-r--r--   0        0        0     1524 2018-11-27 09:24:24.110000 carly-0.9.0/carly/clock.py
--rw-r--r--   0        0        0     1596 2018-11-27 09:52:24.510000 carly-0.9.0/carly/context.py
--rw-r--r--   0        0        0     5879 2018-11-27 09:52:24.510000 carly-0.9.0/carly/hook.py
--rw-r--r--   0        0        0     2065 2018-11-27 09:52:24.510000 carly-0.9.0/carly/tcp.py
--rw-r--r--   0        0        0      449 2018-11-26 18:27:00.850000 carly-0.9.0/carly/threads.py
--rw-r--r--   0        0        0      824 2018-11-27 09:52:24.510000 carly-0.9.0/carly/udp.py
--rw-r--r--   0        0        0      837 2018-11-27 09:52:24.510000 carly-0.9.0/carly/websocket.py
--rw-r--r--   0        0        0      393 2018-11-27 09:52:44.500000 carly-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 carly-0.9.0/setup.py
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 carly-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      206 2018-11-26 18:27:00.850000 carly-0.9.1/carly/__init__.py
+-rw-r--r--   0        0        0     1609 2019-01-29 17:05:10.680000 carly-0.9.1/carly/clock.py
+-rw-r--r--   0        0        0     1596 2018-11-27 09:52:24.510000 carly-0.9.1/carly/context.py
+-rw-r--r--   0        0        0     5879 2018-11-27 09:52:24.510000 carly-0.9.1/carly/hook.py
+-rw-r--r--   0        0        0     2065 2018-11-27 09:52:24.510000 carly-0.9.1/carly/tcp.py
+-rw-r--r--   0        0        0      449 2018-11-26 18:27:00.850000 carly-0.9.1/carly/threads.py
+-rw-r--r--   0        0        0      824 2018-11-27 09:52:24.510000 carly-0.9.1/carly/udp.py
+-rw-r--r--   0        0        0      837 2018-11-27 09:52:24.510000 carly-0.9.1/carly/websocket.py
+-rw-r--r--   0        0        0      474 2019-01-29 17:07:53.430000 carly-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 carly-0.9.1/setup.py
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 carly-0.9.1/PKG-INFO
```

### Comparing `carly-0.9.0/carly/clock.py` & `carly-0.9.1/carly/clock.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
 
 from twisted.internet import reactor
-from twisted.internet.defer import Deferred
+from twisted.internet.defer import Deferred, inlineCallbacks
 
 DEFAULT_TIMEOUT = 0.2
 
 
 def withTimeout(deferred, timeout=None):
     if timeout is None:
         timeout = DEFAULT_TIMEOUT
@@ -30,21 +30,27 @@
     if len(calls) != expected:
         raise AssertionError(
             '\n\nExpected {} delayed calls, found {}: {}'.format(
                 expected, len(calls), strings
         ))
 
 
+def _pump():
+    d = Deferred()
+    reactor.callLater(0, lambda: d.callback(None))
+    return d
+
+
+@inlineCallbacks
 def advanceTime(seconds):
     """
     Advance the reactor time by the number of seconds or partial seconds
     specified.
     """
+    yield _pump()
     now = reactor.seconds()
     for call in reactor.getDelayedCalls():
         currentSecondsFromNow = call.getTime() - now
         newSecondsFromNow = max(0, currentSecondsFromNow - seconds)
         call.reset(newSecondsFromNow)
     # give the reactor a chance to run calls we're brought forward:
-    d = Deferred()
-    reactor.callLater(0, lambda: d.callback(None))
-    return d
+    yield _pump()
```

### Comparing `carly-0.9.0/carly/context.py` & `carly-0.9.1/carly/context.py`

 * *Files identical despite different names*

### Comparing `carly-0.9.0/carly/hook.py` & `carly-0.9.1/carly/hook.py`

 * *Files identical despite different names*

### Comparing `carly-0.9.0/carly/tcp.py` & `carly-0.9.1/carly/tcp.py`

 * *Files identical despite different names*

### Comparing `carly-0.9.0/carly/udp.py` & `carly-0.9.1/carly/udp.py`

 * *Files identical despite different names*

### Comparing `carly-0.9.0/carly/websocket.py` & `carly-0.9.1/carly/websocket.py`

 * *Files identical despite different names*

### Comparing `carly-0.9.0/setup.py` & `carly-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Twisted>=18.9,<19.0', 'attrs>=18.2,<19.0']
 
 setup_kwargs = {
     'name': 'carly',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A tool for putting messages into and collecting responses from Twisted servers using real networking',
     'long_description': None,
     'author': 'Chris Withers',
     'author_email': 'chris@withers.org',
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `carly-0.9.0/PKG-INFO` & `carly-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carly
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool for putting messages into and collecting responses from Twisted servers using real networking
 Home-page: None
 Author: Chris Withers
 Author-email: chris@withers.org
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

