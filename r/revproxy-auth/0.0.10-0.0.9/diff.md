# Comparing `tmp/revproxy_auth-0.0.10.tar.gz` & `tmp/revproxy_auth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.0.10.tar", last modified: Thu Apr 20 15:35:53 2023, max compression
+gzip compressed data, was "revproxy_auth-0.0.9.tar", last modified: Fri Apr 14 07:04:15 2023, max compression
```

## Comparing `revproxy_auth-0.0.10.tar` & `revproxy_auth-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/config-template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-20 15:35:53.000000 revproxy_auth-0.0.10/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 15:35:53.000000 revproxy_auth-0.0.10/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:35:53.000000 revproxy_auth-0.0.10/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 15:35:53.000000 revproxy_auth-0.0.10/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 15:35:53.000000 revproxy_auth-0.0.10/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:35:53.778741 revproxy_auth-0.0.10/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/tests/data/test_result
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-20 15:35:40.000000 revproxy_auth-0.0.10/tests/test_000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/config-template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.663046 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/data/test_result
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/test_000.py
```

### Comparing `revproxy_auth-0.0.10/PKG-INFO` & `revproxy_auth-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.0.10
+Version: 0.0.9
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Authproxy
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.0.10/README.md` & `revproxy_auth-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.10/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.0.9/revproxy_auth/revproxy_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,14 @@
 
             return flask_response
         else:
             return resp
 
     def _build_cookie(self, req_dict: dict) -> tuple:
         mapping_info = self._config['mapping'].get(req_dict['host'])
-        if not mapping_info:
-            return None, None
-
         host = mapping_info.get('host')
         endpoint = mapping_info.get('endpoint')
         method = mapping_info.get('method')
         params = req_dict['params']
 
         ser_head = {}
         for head in req_dict['headers']:
@@ -169,16 +166,14 @@
                              data = data,
                              headers = headers,
                              timeout=10)
         return ApiRestResponse(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
     def _reask_credentials(self, request_dict: dict, old_cookie_name: str = None) -> ApiRestResponse:
         new_cookie, new_cookie_name = self._build_cookie(request_dict)
-        if not new_cookie: # Unable to build cookie for requested path: host unknown
-            return ApiRestResponse(request_dict['host'], status=501)
         self._clear_expired_cookies() # Housekeeping
         print(f'Creating new cookie {new_cookie_name}')
         self._write_cookie(new_cookie, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
         response.created_local_cookies[new_cookie_name] = new_cookie
         if old_cookie_name:
             response.delete_cookies['token'] = request_dict['host']
```

### Comparing `revproxy_auth-0.0.10/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.10/revproxy_auth/templates/form.html` & `revproxy_auth-0.0.9/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.10/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.0.9/revproxy_auth.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.0.10
+Version: 0.0.9
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Authproxy
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.0.10/setup.py` & `revproxy_auth-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.0.10",
+    version="0.0.9",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
```

### Comparing `revproxy_auth-0.0.10/tests/data/test_result` & `revproxy_auth-0.0.9/tests/data/test_result`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.10/tests/test_000.py` & `revproxy_auth-0.0.9/tests/test_000.py`

 * *Files identical despite different names*

