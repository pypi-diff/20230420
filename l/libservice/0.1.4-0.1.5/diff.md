# Comparing `tmp/libservice-0.1.4.tar.gz` & `tmp/libservice-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libservice-0.1.4.tar", last modified: Mon Feb 20 13:22:36 2023, max compression
+gzip compressed data, was "libservice-0.1.5.tar", last modified: Thu Apr 20 08:55:27 2023, max compression
```

## Comparing `libservice-0.1.4.tar` & `libservice-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.756478 libservice-0.1.4/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.4/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.4/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.4/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     4357 2023-02-20 13:22:36.756478 libservice-0.1.4/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     3460 2023-02-20 09:52:23.000000 libservice-0.1.4/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/libservice/
--rw-rw-r--   0 joente    (1000) joente    (1000)      134 2023-02-20 10:29:20.000000 libservice-0.1.4/libservice/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      228 2023-02-17 12:33:12.000000 libservice-0.1.4/libservice/asset.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-02-17 14:23:33.000000 libservice-0.1.4/libservice/check.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      451 2023-02-17 12:38:35.000000 libservice-0.1.4/libservice/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/libservice/hub/
--rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.4/libservice/hub/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.4/libservice/hub/client.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.756478 libservice-0.1.4/libservice/hub/net/
--rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.4/libservice/hub/net/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.4/libservice/hub/net/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.4/libservice/hub/net/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.4/libservice/hub/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.4/libservice/logger.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     7459 2023-02-20 10:18:27.000000 libservice-0.1.4/libservice/serviceroom.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.4/libservice/severity.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.4/libservice/start.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.756478 libservice-0.1.4/libservice/ticonn/
--rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.4/libservice/ticonn/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.4/libservice/ticonn/ticonn.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-20 13:22:36.752478 libservice-0.1.4/libservice.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     4357 2023-02-20 13:22:36.000000 libservice-0.1.4/libservice.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-02-20 13:22:36.000000 libservice-0.1.4/libservice.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-02-20 13:22:36.000000 libservice-0.1.4/libservice.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-02-20 13:22:36.000000 libservice-0.1.4/libservice.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-02-20 13:22:36.000000 libservice-0.1.4/libservice.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-02-17 12:12:03.000000 libservice-0.1.4/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-02-20 13:22:36.756478 libservice-0.1.4/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.4/setup.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-02-20 13:20:40.000000 libservice-0.1.4/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.741952 libservice-0.1.5/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.5/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.5/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.5/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-20 08:55:27.749952 libservice-0.1.5/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3543 2023-04-20 08:27:55.000000 libservice-0.1.5/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/libservice/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      134 2023-02-20 10:29:20.000000 libservice-0.1.5/libservice/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      489 2023-04-20 08:02:15.000000 libservice-0.1.5/libservice/asset.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-02-17 14:23:33.000000 libservice-0.1.5/libservice/check.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      451 2023-02-17 12:38:35.000000 libservice-0.1.5/libservice/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/libservice/hub/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.5/libservice/hub/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.5/libservice/hub/client.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/libservice/hub/net/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.5/libservice/hub/net/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.5/libservice/hub/net/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.5/libservice/hub/net/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.5/libservice/hub/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.5/libservice/logger.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     7459 2023-02-20 10:18:27.000000 libservice-0.1.5/libservice/serviceroom.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.5/libservice/severity.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.5/libservice/start.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/libservice/ticonn/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.5/libservice/ticonn/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.5/libservice/ticonn/ticonn.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 08:55:27.749952 libservice-0.1.5/libservice.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-20 08:55:27.000000 libservice-0.1.5/libservice.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-04-20 08:55:27.000000 libservice-0.1.5/libservice.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-04-20 08:55:27.000000 libservice-0.1.5/libservice.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-04-20 08:55:27.000000 libservice-0.1.5/libservice.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-04-20 08:55:27.000000 libservice-0.1.5/libservice.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-04-20 08:15:18.000000 libservice-0.1.5/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-04-20 08:55:27.753952 libservice-0.1.5/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.5/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-04-20 08:27:18.000000 libservice-0.1.5/version.py
```

### Comparing `libservice-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `libservice-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `libservice-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/.github/workflows/ci.yml` & `libservice-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/.gitignore` & `libservice-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/LICENSE` & `libservice-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/PKG-INFO` & `libservice-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.4
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.5
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -86,15 +86,16 @@
 
 if __name__ == '__main__':
     start(
       collector_key='my_server',
       version='0.1.0',
       checks=(MyCheck, ),
       start_func=start_func,
-      close_func=close_func)
+      close_func=close_func,
+      no_count=False)  # When True, the check(s) do not count (counter + lastseen)
 
 ```
 
 ## ASCII item names
 
 InfraSonar requires each item to have a unique _name_ property. The value for _name_ must be a _string_ with ASCII compatible character.
 When your _name_ is not guaranteed to be ASCII compatible, the following code replaces the incompatible characters with question marks (`?`):
```

### Comparing `libservice-0.1.4/README.md` & `libservice-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
 if __name__ == '__main__':
     start(
       collector_key='my_server',
       version='0.1.0',
       checks=(MyCheck, ),
       start_func=start_func,
-      close_func=close_func)
+      close_func=close_func,
+      no_count=False)  # When True, the check(s) do not count (counter + lastseen)
 
 ```
 
 ## ASCII item names
 
 InfraSonar requires each item to have a unique _name_ property. The value for _name_ must be a _string_ with ASCII compatible character.
 When your _name_ is not guaranteed to be ASCII compatible, the following code replaces the incompatible characters with question marks (`?`):
```

### Comparing `libservice-0.1.4/libservice/check.py` & `libservice-0.1.5/libservice/check.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/hub/client.py` & `libservice-0.1.5/libservice/hub/client.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/hub/net/package.py` & `libservice-0.1.5/libservice/hub/net/package.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/hub/net/protocol.py` & `libservice-0.1.5/libservice/hub/net/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/hub/protocol.py` & `libservice-0.1.5/libservice/hub/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/logger.py` & `libservice-0.1.5/libservice/logger.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/serviceroom.py` & `libservice-0.1.5/libservice/serviceroom.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice/start.py` & `libservice-0.1.5/libservice/start.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/libservice.egg-info/PKG-INFO` & `libservice-0.1.5/libservice.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.4
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.5
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -86,15 +86,16 @@
 
 if __name__ == '__main__':
     start(
       collector_key='my_server',
       version='0.1.0',
       checks=(MyCheck, ),
       start_func=start_func,
-      close_func=close_func)
+      close_func=close_func,
+      no_count=False)  # When True, the check(s) do not count (counter + lastseen)
 
 ```
 
 ## ASCII item names
 
 InfraSonar requires each item to have a unique _name_ property. The value for _name_ must be a _string_ with ASCII compatible character.
 When your _name_ is not guaranteed to be ASCII compatible, the following code replaces the incompatible characters with question marks (`?`):
```

### Comparing `libservice-0.1.4/libservice.egg-info/SOURCES.txt` & `libservice-0.1.5/libservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libservice-0.1.4/setup.py` & `libservice-0.1.5/setup.py`

 * *Files identical despite different names*

