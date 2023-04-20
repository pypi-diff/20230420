# Comparing `tmp/deterrers-api-0.3.tar.gz` & `tmp/deterrers-api-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-api-0.3.tar", last modified: Mon Apr 17 13:17:50 2023, max compression
+gzip compressed data, was "deterrers-api-0.4.tar", last modified: Thu Apr 20 13:51:05 2023, max compression
```

## Comparing `deterrers-api-0.3.tar` & `deterrers-api-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:17:50.803898 deterrers-api-0.3/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrers-api-0.3/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrers-api-0.3/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-17 13:17:50.803898 deterrers-api-0.3/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-04-13 20:00:47.000000 deterrers-api-0.3/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:17:50.803898 deterrers-api-0.3/deterrers_api.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-17 13:17:50.000000 deterrers-api-0.3/deterrers_api.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-04-17 13:17:50.000000 deterrers-api-0.3/deterrers_api.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-17 13:17:50.000000 deterrers-api-0.3/deterrers_api.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-17 13:17:50.000000 deterrers-api-0.3/deterrers_api.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-17 13:17:50.000000 deterrers-api-0.3/deterrers_api.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:17:50.803898 deterrers-api-0.3/deterrersapi/
--rw-r--r--   0 lars      (1000) lars      (1000)     5808 2023-04-17 13:09:49.000000 deterrers-api-0.3/deterrersapi/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrers-api-0.3/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-17 13:17:50.803898 deterrers-api-0.3/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      688 2023-04-17 13:16:08.000000 deterrers-api-0.3/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.634222 deterrers-api-0.4/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrers-api-0.4/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrers-api-0.4/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-20 13:51:05.634222 deterrers-api-0.4/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-04-13 20:00:47.000000 deterrers-api-0.4/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.633222 deterrers-api-0.4/deterrers_api.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.634222 deterrers-api-0.4/deterrersapi/
+-rw-r--r--   0 lars      (1000) lars      (1000)     6156 2023-04-20 13:47:06.000000 deterrers-api-0.4/deterrersapi/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrers-api-0.4/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-20 13:51:05.634222 deterrers-api-0.4/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      688 2023-04-20 13:47:40.000000 deterrers-api-0.4/setup.py
```

### Comparing `deterrers-api-0.3/LICENSE` & `deterrers-api-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.3/PKG-INFO` & `deterrers-api-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.3
+Version: 0.4
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-api-0.3/README.md` & `deterrers-api-0.4/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.3/deterrers_api.egg-info/PKG-INFO` & `deterrers-api-0.4/deterrers_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.3
+Version: 0.4
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-api-0.3/deterrersapi/__init__.py` & `deterrers-api-0.4/deterrersapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,29 +137,38 @@
         '''Delete IP from DETERRERS.
 
         :param ipv4: IPv4 address to delete
         :type ipv4: str
         '''
         return self.__delete('host/', {'ipv4_addr': ipv4})
 
-    def update(self, ipv4: str, profile: str, firewall: str) -> None:
+    def update(self, ipv4: str,
+               profile: None | str = None,
+               firewall: None | str = None,
+               admins: None | list[str] = None) -> None:
         '''Update IP address information in DETERRERS.
 
         :param ipv4: IPv4 address to update
         :type ipv4: str
         :param profile: Firewall profile to use.
                         Must be a valid profile or an empty string string.
-        :type profile: str
+        :type profile: str | None
         :param firewall: Host firewall. Must be one of the UI options
                          or an empty string.
-        :type firewall: str
+        :type firewall: str | None
+        :param admins: List of admins for address
+        :type admins: list[str] | None
         '''
-        data = {'ipv4_addr': ipv4,
-                'service_profile': profile,
-                'fw': firewall}
+        data = {'ipv4_addr': ipv4}
+        if profile is not None:
+            data['service_profile'] = profile
+        if firewall is not None:
+            data['fw'] = firewall
+        if admins is not None:
+            data['admin_ids'] = admins
         return self.__patch('host/', data)
 
     def action(self, ipv4: str, action: str) -> None:
         '''Activate firewall profile or block IP address in perimeter firewall.
 
         :param ipv4: IPv4 address to update
         :type ipv4: str
```

### Comparing `deterrers-api-0.3/setup.py` & `deterrers-api-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-api',
-    version='0.3',
+    version='0.4',
     description='Python API client for DETERRERS',
     url='https://github.com/virtUOS/deterrers-api',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrersapi'],
     license_files=('LICENSE'),
```

