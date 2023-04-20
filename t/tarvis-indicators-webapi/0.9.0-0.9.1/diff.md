# Comparing `tmp/tarvis-indicators-webapi-0.9.0.tar.gz` & `tmp/tarvis-indicators-webapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-indicators-webapi-0.9.0.tar", last modified: Mon Apr 17 17:39:24 2023, max compression
+gzip compressed data, was "tarvis-indicators-webapi-0.9.1.tar", last modified: Thu Apr 20 20:32:04 2023, max compression
```

## Comparing `tarvis-indicators-webapi-0.9.0.tar` & `tarvis-indicators-webapi-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-17 17:39:15.000000 tarvis-indicators-webapi-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-17 17:39:15.000000 tarvis-indicators-webapi-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-17 17:39:15.000000 tarvis-indicators-webapi-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/tarvis/indicators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/tarvis/indicators/webapi/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-04-17 17:39:15.000000 tarvis-indicators-webapi-0.9.0/tarvis/indicators/webapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:39:24.841044 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-17 17:39:24.000000 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-17 17:39:24.000000 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 17:39:24.000000 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 17:39:24.000000 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-17 17:39:24.000000 tarvis-indicators-webapi-0.9.0/tarvis_indicators_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:32:04.905253 tarvis-indicators-webapi-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 20:31:53.000000 tarvis-indicators-webapi-0.9.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-20 20:32:04.905253 tarvis-indicators-webapi-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-20 20:31:53.000000 tarvis-indicators-webapi-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:32:04.905253 tarvis-indicators-webapi-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-20 20:31:53.000000 tarvis-indicators-webapi-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:32:04.901253 tarvis-indicators-webapi-0.9.1/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:32:04.901253 tarvis-indicators-webapi-0.9.1/tarvis/indicators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:32:04.901253 tarvis-indicators-webapi-0.9.1/tarvis/indicators/webapi/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-04-20 20:31:53.000000 tarvis-indicators-webapi-0.9.1/tarvis/indicators/webapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:32:04.905253 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-20 20:32:04.000000 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-20 20:32:04.000000 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:32:04.000000 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:32:04.000000 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 20:32:04.000000 tarvis-indicators-webapi-0.9.1/tarvis_indicators_webapi.egg-info/top_level.txt
```

### Comparing `tarvis-indicators-webapi-0.9.0/LICENSE.txt` & `tarvis-indicators-webapi-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-indicators-webapi-0.9.0/setup.py` & `tarvis-indicators-webapi-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-indicators-webapi",
-    version="0.9.0",
+    version="0.9.1",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Web API Indicators Library",
     long_description=long_description,
     packages=find_namespace_packages(include=["tarvis.*"]),
     python_requires=">=3.10",
```

### Comparing `tarvis-indicators-webapi-0.9.0/tarvis/indicators/webapi/__init__.py` & `tarvis-indicators-webapi-0.9.1/tarvis/indicators/webapi/__init__.py`

 * *Files identical despite different names*

