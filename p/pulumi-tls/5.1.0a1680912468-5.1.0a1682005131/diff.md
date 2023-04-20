# Comparing `tmp/pulumi_tls-5.1.0a1680912468.tar.gz` & `tmp/pulumi_tls-5.1.0a1682005131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1680912468.tar", last modified: Sat Apr  8 00:14:52 2023, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1682005131.tar", last modified: Thu Apr 20 15:43:10 2023, max compression
```

## Comparing `pulumi_tls-5.1.0a1680912468.tar` & `pulumi_tls-5.1.0a1682005131.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54199 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:14:52.717100 pulumi_tls-5.1.0a1680912468/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-08 00:14:52.000000 pulumi_tls-5.1.0a1680912468/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:43:10.233442 pulumi_tls-5.1.0a1682005131/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-20 15:43:10.233442 pulumi_tls-5.1.0a1682005131/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:43:10.229442 pulumi_tls-5.1.0a1682005131/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:43:10.233442 pulumi_tls-5.1.0a1682005131/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54199 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:43:10.229442 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 15:43:10.000000 pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:43:10.233442 pulumi_tls-5.1.0a1682005131/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-20 15:43:09.000000 pulumi_tls-5.1.0a1682005131/setup.py
```

### Comparing `pulumi_tls-5.1.0a1680912468/PKG-INFO` & `pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_tls
-Version: 5.1.0a1680912468
+Name: pulumi-tls
+Version: 5.1.0a1682005131
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1680912468/README.md` & `pulumi_tls-5.1.0a1682005131/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/get_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/locally_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1682005131/pulumi_tls/self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1682005131/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-tls
-Version: 5.1.0a1680912468
+Name: pulumi_tls
+Version: 5.1.0a1682005131
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1680912468/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1682005131/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1680912468/setup.py` & `pulumi_tls-5.1.0a1682005131/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1680912468"
-PLUGIN_VERSION = "5.1.0-alpha.1680912468+26ce95de"
+VERSION = "5.1.0a1682005131"
+PLUGIN_VERSION = "5.1.0-alpha.1682005131+09127122"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'tls', PLUGIN_VERSION])
         except OSError as error:
```

