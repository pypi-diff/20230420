# Comparing `tmp/alibabacloud_maxcompute20220104-1.0.0.tar.gz` & `tmp/alibabacloud_maxcompute20220104-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_maxcompute20220104-1.0.0.tar", last modified: Tue May 10 03:46:24 2022, max compression
+gzip compressed data, was "dist/alibabacloud_maxcompute20220104-1.1.0.tar", last modified: Thu Apr 20 08:22:00 2023, max compression
```

## Comparing `alibabacloud_maxcompute20220104-1.0.0.tar` & `alibabacloud_maxcompute20220104-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25477 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104/client.py
--rw-r--r--   0 root         (0) root         (0)    42569 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2645 2022-05-10 03:46:24.000000 alibabacloud_maxcompute20220104-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100353 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104/client.py
+-rw-r--r--   0 root         (0) root         (0)   300057 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-04-20 08:22:00.000000 alibabacloud_maxcompute20220104-1.1.0/setup.py
```

### Comparing `alibabacloud_maxcompute20220104-1.0.0/LICENSE` & `alibabacloud_maxcompute20220104-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-1.0.0/PKG-INFO` & `alibabacloud_maxcompute20220104-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_maxcompute20220104
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud MaxCompute (20220104) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_maxcompute20220104-1.0.0/README-CN.md` & `alibabacloud_maxcompute20220104-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-1.0.0/README.md` & `alibabacloud_maxcompute20220104-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_maxcompute20220104-1.0.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO` & `alibabacloud_maxcompute20220104-1.1.0/alibabacloud_maxcompute20220104.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-maxcompute20220104
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud MaxCompute (20220104) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_maxcompute20220104-1.0.0/setup.py` & `alibabacloud_maxcompute20220104-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_maxcompute20220104.
 
-Created on 10/05/2022
+Created on 20/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_maxcompute20220104"
 NAME = "alibabacloud_maxcompute20220104" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MaxCompute (20220104) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

