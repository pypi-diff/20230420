# Comparing `tmp/browserstack_sdk-1.7.1.tar.gz` & `tmp/browserstack_sdk-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserstack_sdk-1.7.1.tar", last modified: Tue Apr 18 13:36:57 2023, max compression
+gzip compressed data, was "browserstack_sdk-1.7.2.tar", last modified: Thu Apr 20 11:37:53 2023, max compression
```

## Comparing `browserstack_sdk-1.7.1.tar` & `browserstack_sdk-1.7.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-18 13:36:57.176038 browserstack_sdk-1.7.1/
--rw-r--r--   0 francis    (503) wheel        (0)     4335 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/LICENSE.txt
--rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-04-18 13:36:57.175857 browserstack_sdk-1.7.1/PKG-INFO
--rw-r--r--   0 francis    (503) wheel        (0)      815 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/README.md
-drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-18 13:36:57.174743 browserstack_sdk-1.7.1/browserstack_sdk/
--rw-r--r--   0 francis    (503) wheel        (0)   178916 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/browserstack_sdk/__init__.py
--rw-r--r--   0 francis    (503) wheel        (0)       22 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/browserstack_sdk/_version.py
--rw-r--r--   0 francis    (503) wheel        (0)     3891 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/browserstack_sdk/browserstack.framework.yml.sample
--rw-r--r--   0 francis    (503) wheel        (0)     3125 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/browserstack_sdk/browserstack.generic.yml.sample
-drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-18 13:36:57.175545 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/
--rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/PKG-INFO
--rw-r--r--   0 francis    (503) wheel        (0)      466 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 francis    (503) wheel        (0)        1 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 francis    (503) wheel        (0)      139 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/entry_points.txt
--rw-r--r--   0 francis    (503) wheel        (0)       70 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/requires.txt
--rw-r--r--   0 francis    (503) wheel        (0)       43 2023-04-18 13:36:57.000000 browserstack_sdk-1.7.1/browserstack_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-18 13:36:57.175664 browserstack_sdk-1.7.1/pytest_browserstackplugin/
--rw-r--r--   0 francis    (503) wheel        (0)    11051 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/pytest_browserstackplugin/plugin.py
--rw-r--r--   0 francis    (503) wheel        (0)       38 2023-04-18 13:36:57.176092 browserstack_sdk-1.7.1/setup.cfg
--rw-r--r--   0 francis    (503) wheel        (0)     1343 2023-04-18 13:36:41.000000 browserstack_sdk-1.7.1/setup.py
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-20 11:37:53.333213 browserstack_sdk-1.7.2/
+-rw-r--r--   0 francis    (503) wheel        (0)     4335 2023-04-20 11:36:25.000000 browserstack_sdk-1.7.2/LICENSE.txt
+-rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-04-20 11:37:53.333097 browserstack_sdk-1.7.2/PKG-INFO
+-rw-r--r--   0 francis    (503) wheel        (0)     1834 2023-04-20 11:36:25.000000 browserstack_sdk-1.7.2/README.md
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-20 11:37:53.332218 browserstack_sdk-1.7.2/browserstack_sdk/
+-rw-r--r--   0 francis    (503) wheel        (0)    75696 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/browserstack_sdk/__init__.py
+-rw-r--r--   0 francis    (503) wheel        (0)       22 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/browserstack_sdk/_version.py
+-rw-r--r--   0 francis    (503) wheel        (0)    11390 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/browserstack_sdk/constants.py
+-rw-r--r--   0 francis    (503) wheel        (0)     4971 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/browserstack_sdk/messages.py
+-rw-r--r--   0 francis    (503) wheel        (0)     6440 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/browserstack_sdk/playwright.py
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-20 11:37:53.332816 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/
+-rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 francis    (503) wheel        (0)      456 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 francis    (503) wheel        (0)        1 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 francis    (503) wheel        (0)      139 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 francis    (503) wheel        (0)       70 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/requires.txt
+-rw-r--r--   0 francis    (503) wheel        (0)       43 2023-04-20 11:37:53.000000 browserstack_sdk-1.7.2/browserstack_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-04-20 11:37:53.332921 browserstack_sdk-1.7.2/pytest_browserstackplugin/
+-rw-r--r--   0 francis    (503) wheel        (0)     5593 2023-04-20 11:37:28.000000 browserstack_sdk-1.7.2/pytest_browserstackplugin/plugin.py
+-rw-r--r--   0 francis    (503) wheel        (0)       38 2023-04-20 11:37:53.333245 browserstack_sdk-1.7.2/setup.cfg
+-rw-r--r--   0 francis    (503) wheel        (0)     1343 2023-04-20 11:36:25.000000 browserstack_sdk-1.7.2/setup.py
```

### Comparing `browserstack_sdk-1.7.1/LICENSE.txt` & `browserstack_sdk-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browserstack_sdk-1.7.1/PKG-INFO` & `browserstack_sdk-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserstack_sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK for browserstack selenium-webdriver tests
 Author: BrowserStack
 Author-email: support@browserstack.com
 License: BrowserStack Software License Agreement
         The “Licensed Software” under this BrowserStack Software License Agreement (“Agreement”) shall be used by
         you only if You agree to the following terms and conditions. Downloading the Licensed Software and indicating
         your consent to the terms of this license constitutes a binding Agreement between BrowserStack and You. If
```

### Comparing `browserstack_sdk-1.7.1/browserstack_sdk.egg-info/PKG-INFO` & `browserstack_sdk-1.7.2/browserstack_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserstack-sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK for browserstack selenium-webdriver tests
 Author: BrowserStack
 Author-email: support@browserstack.com
 License: BrowserStack Software License Agreement
         The “Licensed Software” under this BrowserStack Software License Agreement (“Agreement”) shall be used by
         you only if You agree to the following terms and conditions. Downloading the Licensed Software and indicating
         your consent to the terms of this license constitutes a binding Agreement between BrowserStack and You. If
```

### Comparing `browserstack_sdk-1.7.1/setup.py` & `browserstack_sdk-1.7.2/setup.py`

 * *Files identical despite different names*

