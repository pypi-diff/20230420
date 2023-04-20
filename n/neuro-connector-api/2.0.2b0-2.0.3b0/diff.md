# Comparing `tmp/neuro-connector-api-2.0.2b0.tar.gz` & `tmp/neuro-connector-api-2.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-connector-api-2.0.2b0.tar", last modified: Wed Apr 19 13:21:00 2023, max compression
+gzip compressed data, was "neuro-connector-api-2.0.3b0.tar", last modified: Thu Apr 20 08:48:14 2023, max compression
```

## Comparing `neuro-connector-api-2.0.2b0.tar` & `neuro-connector-api-2.0.3b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/neuro-connector-api/
--rw-r--r--   0 runner    (1001) docker     (123)    18438 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/neuro-connector-api/NeuroConnector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:48:14.907092 neuro-connector-api-2.0.3b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 08:48:03.000000 neuro-connector-api-2.0.3b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 08:48:14.907092 neuro-connector-api-2.0.3b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 08:48:03.000000 neuro-connector-api-2.0.3b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:48:14.907092 neuro-connector-api-2.0.3b0/neuro-connector-api/
+-rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-04-20 08:48:03.000000 neuro-connector-api-2.0.3b0/neuro-connector-api/NeuroConnector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:48:14.907092 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 08:48:14.000000 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 08:48:14.000000 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:48:14.000000 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 08:48:14.000000 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 08:48:14.000000 neuro-connector-api-2.0.3b0/neuro_connector_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 08:48:14.907092 neuro-connector-api-2.0.3b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 08:48:03.000000 neuro-connector-api-2.0.3b0/setup.py
```

### Comparing `neuro-connector-api-2.0.2b0/LICENSE` & `neuro-connector-api-2.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-connector-api-2.0.2b0/README.md` & `neuro-connector-api-2.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-connector-api-2.0.2b0/neuro-connector-api/NeuroConnector.py` & `neuro-connector-api-2.0.3b0/neuro-connector-api/NeuroConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         if appToken:
             token = "Bearer " + appToken
         else:
             token = None
 
         self.requestWrapper = RequestWrapper(token=token,
-                                             url=url)
+                                             url=self.url)
 
         assert self.requestWrapper, "couldn't initiate request wrapper"
 
         self.organizationId = organizationId
         assert self.organizationId, "organizationId missing"
 
     def delete_record(self, key):
```

