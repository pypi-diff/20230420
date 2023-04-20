# Comparing `tmp/matomo-0.7.3.tar.gz` & `tmp/matomo-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matomo-0.7.3.tar", last modified: Thu Jan 12 19:46:52 2023, max compression
+gzip compressed data, was "matomo-0.7.4.tar", last modified: Thu Apr 20 17:06:43 2023, max compression
```

## Comparing `matomo-0.7.3.tar` & `matomo-0.7.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-01-12 19:46:52.518751 matomo-0.7.3/
--rw-r--r--   0 markos     (501) staff       (20)     1196 2023-01-12 19:46:52.518307 matomo-0.7.3/PKG-INFO
--rw-r--r--   0 markos     (501) staff       (20)     2191 2023-01-12 19:30:57.000000 matomo-0.7.3/README.md
--rw-r--r--   0 markos     (501) staff       (20)       38 2023-01-12 19:46:52.518914 matomo-0.7.3/setup.cfg
--rw-r--r--   0 markos     (501) staff       (20)     2094 2023-01-12 19:46:35.000000 matomo-0.7.3/setup.py
-drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-01-12 19:46:52.510423 matomo-0.7.3/src/
-drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-01-12 19:46:52.513765 matomo-0.7.3/src/matomo/
--rw-r--r--   0 markos     (501) staff       (20)     5007 2022-12-29 15:08:32.000000 matomo-0.7.3/src/matomo/__init__.py
--rw-r--r--   0 markos     (501) staff       (20)     3331 2022-01-30 10:11:18.000000 matomo-0.7.3/src/matomo/django.py
--rw-r--r--   0 markos     (501) staff       (20)      124 2022-01-30 08:32:52.000000 matomo-0.7.3/src/matomo/request.py
--rw-r--r--   0 markos     (501) staff       (20)    69494 2023-01-12 17:09:16.000000 matomo-0.7.3/src/matomo/tracker.py
-drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-01-12 19:46:52.517592 matomo-0.7.3/src/matomo.egg-info/
--rw-r--r--   0 markos     (501) staff       (20)     1196 2023-01-12 19:46:52.000000 matomo-0.7.3/src/matomo.egg-info/PKG-INFO
--rw-r--r--   0 markos     (501) staff       (20)      308 2023-01-12 19:46:52.000000 matomo-0.7.3/src/matomo.egg-info/SOURCES.txt
--rw-r--r--   0 markos     (501) staff       (20)        1 2023-01-12 19:46:52.000000 matomo-0.7.3/src/matomo.egg-info/dependency_links.txt
--rw-r--r--   0 markos     (501) staff       (20)        1 2021-12-31 09:46:27.000000 matomo-0.7.3/src/matomo.egg-info/not-zip-safe
--rw-r--r--   0 markos     (501) staff       (20)       14 2023-01-12 19:46:52.000000 matomo-0.7.3/src/matomo.egg-info/requires.txt
--rw-r--r--   0 markos     (501) staff       (20)        7 2023-01-12 19:46:52.000000 matomo-0.7.3/src/matomo.egg-info/top_level.txt
+drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-04-20 17:06:43.795655 matomo-0.7.4/
+-rw-r--r--   0 markos     (501) staff       (20)     1196 2023-04-20 17:06:43.795335 matomo-0.7.4/PKG-INFO
+-rw-r--r--   0 markos     (501) staff       (20)     2191 2023-01-12 19:30:57.000000 matomo-0.7.4/README.md
+-rw-r--r--   0 markos     (501) staff       (20)       38 2023-04-20 17:06:43.795765 matomo-0.7.4/setup.cfg
+-rw-r--r--   0 markos     (501) staff       (20)     2094 2023-04-20 17:02:57.000000 matomo-0.7.4/setup.py
+drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-04-20 17:06:43.787349 matomo-0.7.4/src/
+drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-04-20 17:06:43.790854 matomo-0.7.4/src/matomo/
+-rw-r--r--   0 markos     (501) staff       (20)     5007 2022-12-29 15:08:32.000000 matomo-0.7.4/src/matomo/__init__.py
+-rw-r--r--   0 markos     (501) staff       (20)     3331 2022-01-30 10:11:18.000000 matomo-0.7.4/src/matomo/django.py
+-rw-r--r--   0 markos     (501) staff       (20)      124 2022-01-30 08:32:52.000000 matomo-0.7.4/src/matomo/request.py
+-rw-r--r--   0 markos     (501) staff       (20)    69519 2023-04-14 19:08:23.000000 matomo-0.7.4/src/matomo/tracker.py
+drwxr-xr-x   0 markos     (501) staff       (20)        0 2023-04-20 17:06:43.794714 matomo-0.7.4/src/matomo.egg-info/
+-rw-r--r--   0 markos     (501) staff       (20)     1196 2023-04-20 17:06:43.000000 matomo-0.7.4/src/matomo.egg-info/PKG-INFO
+-rw-r--r--   0 markos     (501) staff       (20)      308 2023-04-20 17:06:43.000000 matomo-0.7.4/src/matomo.egg-info/SOURCES.txt
+-rw-r--r--   0 markos     (501) staff       (20)        1 2023-04-20 17:06:43.000000 matomo-0.7.4/src/matomo.egg-info/dependency_links.txt
+-rw-r--r--   0 markos     (501) staff       (20)        1 2021-12-31 09:46:27.000000 matomo-0.7.4/src/matomo.egg-info/not-zip-safe
+-rw-r--r--   0 markos     (501) staff       (20)       14 2023-04-20 17:06:43.000000 matomo-0.7.4/src/matomo.egg-info/requires.txt
+-rw-r--r--   0 markos     (501) staff       (20)        7 2023-04-20 17:06:43.000000 matomo-0.7.4/src/matomo.egg-info/top_level.txt
```

### Comparing `matomo-0.7.3/PKG-INFO` & `matomo-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: matomo
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python Matomo client API
 Home-page: https://github.com/samastur/matomo
 Author: Marko Samastur
 Author-email: matomo@markos.gaivo.net
 Maintainer: Marko Samastur
 Maintainer-email: matomo@markos.gaivo.net
 License: MIT
```

### Comparing `matomo-0.7.3/README.md` & `matomo-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `matomo-0.7.3/setup.py` & `matomo-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "requests>=2.*"
 ]
 
 ###############################################################################
 
 AUTHOR = "Marko Samastur"
 AUTHOR_EMAIL = "matomo@markos.gaivo.net"
-VERSION = "0.7.3"
+VERSION = "0.7.4"
 LICENSE = "MIT"
 URL = "https://github.com/samastur/matomo"
 DESCRIPTION = "Python Matomo client API"
 LONG = (
     "This is a Python implementation of the Matomo tracking and analytics APIs "
     "based on PHP version with an almost 100% compatible API."
 )
```

### Comparing `matomo-0.7.3/src/matomo/__init__.py` & `matomo-0.7.4/src/matomo/__init__.py`

 * *Files identical despite different names*

### Comparing `matomo-0.7.3/src/matomo/django.py` & `matomo-0.7.4/src/matomo/django.py`

 * *Files identical despite different names*

### Comparing `matomo-0.7.3/src/matomo/tracker.py` & `matomo-0.7.4/src/matomo/tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 
 def urlencode_plus(s):
     if type(s) == str:
         return quote(s)
     elif type(s) == dict:
         return urlencode(s)
+    elif type(s) == int:
+        return str(s)
     else:
-        raise TypeError("urlencode_plus works only on strings and dicts.", s)
+        raise TypeError("urlencode_plus works only on strings, integers and dicts.", s)
 
 
 #
 # This module is hand-corrected version of an automated translation of PHP MatomoTracker
 #
 
 is_int = lambda x: isinstance(x, int)
@@ -117,15 +119,15 @@
         * @param str api_url "http://example.org/matomo/" or "http://matomo.example.org/"
                                 If set, will overwrite MatomoTracker.URL
         """
         self.request = request
         self.request_method = "GET"
         self.response = None
         self.ecommerceItems = []
-        self.attributionInfo = []
+        self.attributionInfo = None
         self.eventCustomVar = {}
         self.forcedDatetime = ""
         self.forcedNewVisit = False
         self.networkTime = 0
         self.serverTime = 0
         self.transferTime = 0
         self.domProcessingTime = 0
@@ -438,15 +440,15 @@
         tracking request.
 
         * @param str tracking_api_parameter The name of the tracking API parameter, eg 'bw_bytes'
         * @param str value Tracking parameter value that shall be sent for this tracking parameter.
         * @return self
         * @throws Exception
         """
-        regex = re.compile("/^dimension([0-9]+)$/")
+        regex = re.compile("^dimension([0-9]+)$")
         matches = re.findall(regex, tracking_api_parameter)
         if len(matches):
             # Unlike PHP preg_match it returns captured subpattern as first element
             self.set_custom_dimension(matches[0], value)
             return self
 
         self.customParameters[tracking_api_parameter] = value
@@ -1447,15 +1449,15 @@
     def set_request_method_non_bulk(self, method):
         """
         Sets the request method to POST, which is recommended when using set_token_auth()
         to prevent the token from being recorded in server logs. Avoid using redirects
         when using POST to prevent the loss of POST values. When using Log Analytics,
         be aware that POST requests are not parseable/replayable.
 
-        * @param str method. Either 'POST' or 'get'
+        * @param str method. Either 'POST' or 'GET'
         * @return self
         """
         self.request_method = "POST" if method.upper() == "POST" else "GET"
         return self
 
     def set_proxy(self, proxy, proxy_port=80, proxy_type="https"):
         """
@@ -1793,33 +1795,24 @@
 
         * @param cookie_name
         * @param cookie_value
         * @param cookie_ttl
         * @return string
         """
         cookie_expire = self.currentTs + cookie_ttl
-        cookie_header = (
-            f"Set-Cookie: {urlencode_plus(cookie_name)}={urlencode_plus(cookie_value)}"(
-                f"; expires='{time.strftime('%a, %d-%m-%Y %H:%M:%S', cookie_expire)} GMT"
-                if cookie_expire
-                else ""
-            )(f"; path='{self.configCookiePath}" if self.configCookiePath else "")(
-                f"; domain='{self.configCookieDomain}"
-                if self.configCookieDomain
-                else ""
-            )(
-                f"; secure" if self.configCookieSecure else ""
-            )(
-                f"; HttpOnly" if self.configCookieHTTPOnly else ""
-            )(
-                f"; SameSite={urlencode_plus(self.configCookieSameSite)}"
-                if self.configCookieSameSite
-                else ""
-            )
-        )
+        cookie_name = urlencode_plus(cookie_name)
+        cookie_value = urlencode_plus(cookie_value)
+        expires = f"; expires='{time.strftime('%a, %d-%m-%Y %H:%M:%S', time.gmtime(cookie_expire))} GMT" if cookie_expire else ""
+        path = f"; path={self.configCookiePath}" if self.configCookiePath else ""
+        domain = f"; domain={self.configCookieDomain}" if self.configCookieDomain else ""
+        secure = "; secure" if self.configCookieSecure else ""
+        http_only = "; HttpOnly" if self.configCookieHTTPOnly else ""
+        same_site = f"; SameSite={urlencode_plus(self.configCookieSameSite)}" if self.configCookieSameSite else ""
+
+        cookie_header = f"Set-Cookie: {cookie_name}={cookie_value}{expires}{path}{domain}{secure}{http_only}{same_site}"
         return cookie_header
 
     def set_cookie(self, cookie_name, cookie_value, cookie_ttl):
         """
         Sets a first party cookie to the client to improve dual JS-Python tracking.
 
         This replicates the matomo.js tracker algorithms for consistency and better accuracy.
@@ -1913,14 +1906,14 @@
         self.incomingTrackerCookies = {}
 
         if headers:
             header_name = "set-cookie:"
             header_name_length = len(header_name)
 
             for header in headers:
-                if strpos(header.lower(), header_name) != 0:
+                if strpos(header.lower(), header_name) is False:
                     continue
                 cookies = header[header_name_length:].strip()
                 pos_end = strpos(cookies, ";")
                 if pos_end is not False:  # 0 != False
                     cookies = cookies[:pos_end]
                 self.incomingTrackerCookies = parse_qs(cookies)
```

### Comparing `matomo-0.7.3/src/matomo.egg-info/PKG-INFO` & `matomo-0.7.4/src/matomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: matomo
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python Matomo client API
 Home-page: https://github.com/samastur/matomo
 Author: Marko Samastur
 Author-email: matomo@markos.gaivo.net
 Maintainer: Marko Samastur
 Maintainer-email: matomo@markos.gaivo.net
 License: MIT
```

