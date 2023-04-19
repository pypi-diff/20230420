# Comparing `tmp/glapi-0.7.2.tar.gz` & `tmp/glapi-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glapi-0.7.2.tar", last modified: Sat May 21 17:03:50 2022, max compression
+gzip compressed data, was "glapi-0.7.3.tar", last modified: Wed Apr 19 23:28:32 2023, max compression
```

## Comparing `glapi-0.7.2.tar` & `glapi-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 17:03:50.664444 glapi-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-21 17:03:41.000000 glapi-0.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      343 2022-05-21 17:03:50.664444 glapi-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-05-21 17:03:41.000000 glapi-0.7.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-21 17:03:41.000000 glapi-0.7.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 17:03:50.662444 glapi-0.7.2/glapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3655 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     5925 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/epic.py
--rw-rw-rw-   0 root         (0) root         (0)     4800 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/issue.py
--rw-rw-rw-   0 root         (0) root         (0)     4459 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6861 2022-05-21 17:03:41.000000 glapi-0.7.2/glapi/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 17:03:50.664444 glapi-0.7.2/glapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2022-05-21 17:03:50.000000 glapi-0.7.2/glapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2022-05-21 17:03:50.000000 glapi-0.7.2/glapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-21 17:03:50.000000 glapi-0.7.2/glapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2022-05-21 17:03:50.000000 glapi-0.7.2/glapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-05-21 17:03:50.000000 glapi-0.7.2/glapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-05-21 17:03:41.000000 glapi-0.7.2/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-05-21 17:03:41.000000 glapi-0.7.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-21 17:03:50.664444 glapi-0.7.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      698 2022-05-21 17:03:41.000000 glapi-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.398032 glapi-0.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-19 23:28:22.000000 glapi-0.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-19 23:28:32.397032 glapi-0.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-04-19 23:28:22.000000 glapi-0.7.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-19 23:28:22.000000 glapi-0.7.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.396031 glapi-0.7.3/glapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     5925 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/epic.py
+-rw-rw-rw-   0 root         (0) root         (0)     4800 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/issue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4459 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.397032 glapi-0.7.3/glapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-19 23:28:22.000000 glapi-0.7.3/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-19 23:28:22.000000 glapi-0.7.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 23:28:32.398032 glapi-0.7.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      698 2023-04-19 23:28:22.000000 glapi-0.7.3/setup.py
```

### Comparing `glapi-0.7.2/glapi/configuration.py` & `glapi-0.7.3/glapi/configuration.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/connection.py` & `glapi-0.7.3/glapi/connection.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/epic.py` & `glapi-0.7.3/glapi/epic.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/group.py` & `glapi-0.7.3/glapi/group.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/issue.py` & `glapi-0.7.3/glapi/issue.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/project.py` & `glapi-0.7.3/glapi/project.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.2/glapi/user.py` & `glapi-0.7.3/glapi/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         result = list()
         params = dict()
 
         # check for connection ready
         if self.id and self.connection.token and self.connection.version:
 
             # check params
-            if date_end: params["created_before"] = date_end
-            if date_start: params["created_after"] = date_start
+            if date_end: params["before"] = date_end
+            if date_start: params["after"] = date_start
 
             # if actions are provided
             if actions:
 
                 # loop through actions
                 for action in actions:
```

### Comparing `glapi-0.7.2/setup.py` & `glapi-0.7.3/setup.py`

 * *Files identical despite different names*

