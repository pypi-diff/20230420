# Comparing `tmp/backendpy-0.2.4a4.tar.gz` & `tmp/backendpy-0.2.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backendpy-0.2.4a4.tar", last modified: Sun Apr  2 12:58:53 2023, max compression
+gzip compressed data, was "backendpy-0.2.4a5.tar", last modified: Wed Apr 19 22:57:18 2023, max compression
```

## Comparing `backendpy-0.2.4a4.tar` & `backendpy-0.2.4a5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.547767 backendpy-0.2.4a4/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.4a4/LICENSE
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-02 12:58:53.547767 backendpy-0.2.4a4/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.4a4/README.md
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.379774 backendpy-0.2.4a4/backendpy/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.4a4/backendpy/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.4a4/backendpy/app.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.4a4/backendpy/asgi.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.391774 backendpy-0.2.4a4/backendpy/cli/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.4a4/backendpy/cli/__init__.py
--rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.4a4/backendpy/cli/admin.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.4a4/backendpy/config.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.451771 backendpy-0.2.4a4/backendpy/data_handler/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.4a4/backendpy/data_handler/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.4a4/backendpy/data_handler/data.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.4a4/backendpy/data_handler/fields.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.4a4/backendpy/data_handler/filters.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.4a4/backendpy/data_handler/validators.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.4a4/backendpy/db.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.4a4/backendpy/error.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.4a4/backendpy/exception.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.4a4/backendpy/hook.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.4a4/backendpy/initializer.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.4a4/backendpy/logging.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.463771 backendpy-0.2.4a4/backendpy/middleware/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.4a4/backendpy/middleware/__init__.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.479770 backendpy-0.2.4a4/backendpy/middleware/defaults/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.4a4/backendpy/middleware/defaults/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.4a4/backendpy/middleware/defaults/cors.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.4a4/backendpy/middleware/middleware.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9319 2023-01-04 01:13:10.000000 backendpy-0.2.4a4/backendpy/request.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    14077 2023-01-03 03:01:46.000000 backendpy-0.2.4a4/backendpy/response.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.4a4/backendpy/router.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.4a4/backendpy/templating.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.4a4/backendpy/unittest.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.539768 backendpy-0.2.4a4/backendpy/utils/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.4a4/backendpy/utils/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.4a4/backendpy/utils/bytes.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    11454 2023-03-03 18:05:43.000000 backendpy-0.2.4a4/backendpy/utils/file.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.4a4/backendpy/utils/http.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.4a4/backendpy/utils/json.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-02 12:58:53.391774 backendpy-0.2.4a4/backendpy.egg-info/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/SOURCES.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/dependency_links.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/entry_points.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/requires.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-04-02 12:58:53.000000 backendpy-0.2.4a4/backendpy.egg-info/top_level.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.4a4/pyproject.toml
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-04-02 12:58:53.551767 backendpy-0.2.4a4/setup.cfg
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.722996 backendpy-0.2.4a5/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.4a5/LICENSE
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-19 22:57:18.722996 backendpy-0.2.4a5/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.4a5/README.md
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.507008 backendpy-0.2.4a5/backendpy/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.4a5/backendpy/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.4a5/backendpy/app.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.4a5/backendpy/asgi.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.511008 backendpy-0.2.4a5/backendpy/cli/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.4a5/backendpy/cli/__init__.py
+-rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.4a5/backendpy/cli/admin.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.4a5/backendpy/config.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.603003 backendpy-0.2.4a5/backendpy/data_handler/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.4a5/backendpy/data_handler/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.4a5/backendpy/data_handler/data.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.4a5/backendpy/data_handler/fields.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.4a5/backendpy/data_handler/filters.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.4a5/backendpy/data_handler/validators.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.4a5/backendpy/db.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.4a5/backendpy/error.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.4a5/backendpy/exception.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.4a5/backendpy/hook.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.4a5/backendpy/initializer.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.4a5/backendpy/logging.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.647000 backendpy-0.2.4a5/backendpy/middleware/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.4a5/backendpy/middleware/__init__.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.662999 backendpy-0.2.4a5/backendpy/middleware/defaults/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.4a5/backendpy/middleware/defaults/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.4a5/backendpy/middleware/defaults/cors.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.4a5/backendpy/middleware/middleware.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9319 2023-01-04 01:13:10.000000 backendpy-0.2.4a5/backendpy/request.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    14077 2023-01-03 03:01:46.000000 backendpy-0.2.4a5/backendpy/response.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.4a5/backendpy/router.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.4a5/backendpy/templating.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.4a5/backendpy/unittest.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.710996 backendpy-0.2.4a5/backendpy/utils/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.4a5/backendpy/utils/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.4a5/backendpy/utils/bytes.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    11834 2023-04-19 22:52:27.000000 backendpy-0.2.4a5/backendpy/utils/file.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.4a5/backendpy/utils/http.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.4a5/backendpy/utils/json.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.511008 backendpy-0.2.4a5/backendpy.egg-info/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/entry_points.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/requires.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/top_level.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.4a5/pyproject.toml
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-04-19 22:57:18.726996 backendpy-0.2.4a5/setup.cfg
```

### Comparing `backendpy-0.2.4a4/LICENSE` & `backendpy-0.2.4a5/LICENSE`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/PKG-INFO` & `backendpy-0.2.4a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.4a4
+Version: 0.2.4a5
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.4a4/README.md` & `backendpy-0.2.4a5/README.md`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/app.py` & `backendpy-0.2.4a5/backendpy/app.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/asgi.py` & `backendpy-0.2.4a5/backendpy/asgi.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/cli/admin.py` & `backendpy-0.2.4a5/backendpy/cli/admin.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/config.py` & `backendpy-0.2.4a5/backendpy/config.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/data_handler/data.py` & `backendpy-0.2.4a5/backendpy/data_handler/data.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/data_handler/fields.py` & `backendpy-0.2.4a5/backendpy/data_handler/fields.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/data_handler/filters.py` & `backendpy-0.2.4a5/backendpy/data_handler/filters.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/data_handler/validators.py` & `backendpy-0.2.4a5/backendpy/data_handler/validators.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/db.py` & `backendpy-0.2.4a5/backendpy/db.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/error.py` & `backendpy-0.2.4a5/backendpy/error.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/exception.py` & `backendpy-0.2.4a5/backendpy/exception.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/hook.py` & `backendpy-0.2.4a5/backendpy/hook.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/initializer.py` & `backendpy-0.2.4a5/backendpy/initializer.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/logging.py` & `backendpy-0.2.4a5/backendpy/logging.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/middleware/defaults/cors.py` & `backendpy-0.2.4a5/backendpy/middleware/defaults/cors.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/middleware/middleware.py` & `backendpy-0.2.4a5/backendpy/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/request.py` & `backendpy-0.2.4a5/backendpy/request.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/response.py` & `backendpy-0.2.4a5/backendpy/response.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/router.py` & `backendpy-0.2.4a5/backendpy/router.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/templating.py` & `backendpy-0.2.4a5/backendpy/templating.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/unittest.py` & `backendpy-0.2.4a5/backendpy/unittest.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy/utils/file.py` & `backendpy-0.2.4a5/backendpy/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,24 @@
             await aiofiles.os.remove(path)
         except:
             pass
         return not os.path.exists(path)
     return False
 
 
+async def remove_file(path):
+    if os.path.isfile(path):
+        try:
+            await aiofiles.os.remove(path)
+        except:
+            pass
+        return not os.path.exists(path)
+    return False
+
+
 async def get_checksum(data=b'', path=None, chunk_size=32768):
     h = hashlib.blake2b()
     if path:
         async with aiofiles.open(path, 'rb') as f:
             while chunk := await f.read(chunk_size):
                 h.update(chunk)
     elif isinstance(data, types.AsyncGeneratorType):
@@ -132,14 +142,18 @@
             await f.write(data)
             h.update(data)
     if os.path.isfile(path):
         return h.hexdigest()
     return None
 
 
+async def get_file_size(path):
+    return await aiofiles.os.path.getsize(path)
+
+
 def get_human_readable_size(size, precision=1):
     for suffix in ['B', 'KB', 'MB', 'GB']:
         if size < 1024.0:
             return '%.*f%s' % (precision, size, suffix)
         size /= 1024.0
     return '%.*f%s' % (precision, size, 'TB')
 
@@ -150,14 +164,18 @@
 
 
 def get_suffix_mimetype(filename):
     type, encoding = mimetypes.guess_type(filename)
     return type
 
 
+def get_extension_mimetype(extension):
+    return mimetypes.types_map.get(f'.{extension}')
+
+
 def get_type(value) -> list[str] | None:
     if not value:
         raise Exception('file text content error')
     # Binery files signatures list
     type_signs = [
         # image
         (['jpeg', 'jpg'],
```

### Comparing `backendpy-0.2.4a4/backendpy/utils/http.py` & `backendpy-0.2.4a5/backendpy/utils/http.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/backendpy.egg-info/PKG-INFO` & `backendpy-0.2.4a5/backendpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.4a4
+Version: 0.2.4a5
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.4a4/backendpy.egg-info/SOURCES.txt` & `backendpy-0.2.4a5/backendpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a4/setup.cfg` & `backendpy-0.2.4a5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = backendpy
-version = v0.2.4-alpha.4
+version = v0.2.4-alpha.5
 author = Savang Co.
 author_email = backendpy@savang.com
 description = Async (ASGI) Python web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Backendpy, Web, Framework, Python, Async, ASGI
 license = BSD 3-Clause License
```

