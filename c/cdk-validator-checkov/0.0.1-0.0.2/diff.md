# Comparing `tmp/cdk-validator-checkov-0.0.1.tar.gz` & `tmp/cdk-validator-checkov-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-validator-checkov-0.0.1.tar", last modified: Wed Apr 19 03:15:51 2023, max compression
+gzip compressed data, was "cdk-validator-checkov-0.0.2.tar", last modified: Thu Apr 20 07:20:21 2023, max compression
```

## Comparing `cdk-validator-checkov-0.0.1.tar` & `cdk-validator-checkov-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/_jsii/cdk-validator-checkov@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:15:40.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:15:51.407322 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-19 03:15:51.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 03:15:51.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:15:51.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 03:15:51.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 03:15:51.000000 cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:20:21.269650 cdk-validator-checkov-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/_jsii/cdk-validator-checkov@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:20:11.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:20:21.273650 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 07:20:21.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 07:20:21.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:20:21.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 07:20:21.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 07:20:21.000000 cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/top_level.txt
```

### Comparing `cdk-validator-checkov-0.0.1/LICENSE` & `cdk-validator-checkov-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-validator-checkov-0.0.1/PKG-INFO` & `cdk-validator-checkov-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-validator-checkov
-Version: 0.0.1
+Version: 0.0.2
 Summary: @bridgecrew/cdk-validator-checkov
 Home-page: https://github.com/bridgecrewio/cdk-validator-checkov.git
 Author: bridgecrew<meet@bridgecrew.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/bridgecrewio/cdk-validator-checkov.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -52,30 +52,62 @@
 pip install cdk-validator-checkov
 ```
 
 ## Usage
 
 To use this plugin in your CDK application add it to the CDK App.
 
+### Python
+
+```python
+from cdk_validator_checkov import CheckovValidator
+
+...
+
+App(
+  policy_validation_beta1=[
+    CheckovValidator()
+  ]
+)
+```
+
+By default, the `CheckovValidator` plugin comes with all `checkov`
+[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
+In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+
+```python
+CheckovValidator(
+  check= ['CKV_AWS_18', 'CKV_AWS_21']
+)
+```
+
+```python
+CheckovValidator(
+  skipCheck= ['CKV_AWS_18', 'CKV_AWS_21']
+}
+```
+
+### TypeScript
+
 ```python
 new App({
   policyValidationBeta1: [
     new CheckovValidator(),
   ],
 });
 ```
 
-By default, the `CheckovValidator` plugin comes with all `checkov`
-[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
-In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+Specify checks:
 
 ```python
 new CheckovValidator({
     check: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
 
+Skip checks:
+
 ```python
 new CheckovValidator({
     skipCheck: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
```

### Comparing `cdk-validator-checkov-0.0.1/README.md` & `cdk-validator-checkov-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -28,30 +28,62 @@
 pip install cdk-validator-checkov
 ```
 
 ## Usage
 
 To use this plugin in your CDK application add it to the CDK App.
 
+### Python
+
+```python
+from cdk_validator_checkov import CheckovValidator
+
+...
+
+App(
+  policy_validation_beta1=[
+    CheckovValidator()
+  ]
+)
+```
+
+By default, the `CheckovValidator` plugin comes with all `checkov`
+[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
+In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+
+```python
+CheckovValidator(
+  check= ['CKV_AWS_18', 'CKV_AWS_21']
+)
+```
+
+```python
+CheckovValidator(
+  skipCheck= ['CKV_AWS_18', 'CKV_AWS_21']
+}
+```
+
+### TypeScript
+
 ```python
 new App({
   policyValidationBeta1: [
     new CheckovValidator(),
   ],
 });
 ```
 
-By default, the `CheckovValidator` plugin comes with all `checkov`
-[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
-In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+Specify checks:
 
 ```python
 new CheckovValidator({
     check: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
 
+Skip checks:
+
 ```python
 new CheckovValidator({
     skipCheck: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
```

### Comparing `cdk-validator-checkov-0.0.1/setup.py` & `cdk-validator-checkov-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-validator-checkov",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "@bridgecrew/cdk-validator-checkov",
     "license": "Apache-2.0",
     "url": "https://github.com/bridgecrewio/cdk-validator-checkov.git",
     "long_description_content_type": "text/markdown",
     "author": "bridgecrew<meet@bridgecrew.io>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_validator_checkov",
         "cdk_validator_checkov._jsii"
     ],
     "package_data": {
         "cdk_validator_checkov._jsii": [
-            "cdk-validator-checkov@0.0.1.jsii.tgz"
+            "cdk-validator-checkov@0.0.2.jsii.tgz"
         ],
         "cdk_validator_checkov": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-validator-checkov-0.0.1/src/cdk_validator_checkov/__init__.py` & `cdk-validator-checkov-0.0.2/src/cdk_validator_checkov/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,32 +29,64 @@
 pip install cdk-validator-checkov
 ```
 
 ## Usage
 
 To use this plugin in your CDK application add it to the CDK App.
 
+### Python
+
+```python
+from cdk_validator_checkov import CheckovValidator
+
+...
+
+App(
+  policy_validation_beta1=[
+    CheckovValidator()
+  ]
+)
+```
+
+By default, the `CheckovValidator` plugin comes with all `checkov`
+[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
+In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+
+```python
+CheckovValidator(
+  check= ['CKV_AWS_18', 'CKV_AWS_21']
+)
+```
+
+```python
+CheckovValidator(
+  skipCheck= ['CKV_AWS_18', 'CKV_AWS_21']
+}
+```
+
+### TypeScript
+
 ```python
 new App({
   policyValidationBeta1: [
     new CheckovValidator(),
   ],
 });
 ```
 
-By default, the `CheckovValidator` plugin comes with all `checkov`
-[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
-In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+Specify checks:
 
 ```python
 new CheckovValidator({
     check: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
 
+Skip checks:
+
 ```python
 new CheckovValidator({
     skipCheck: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
 '''
 import abc
```

### Comparing `cdk-validator-checkov-0.0.1/src/cdk_validator_checkov.egg-info/PKG-INFO` & `cdk-validator-checkov-0.0.2/src/cdk_validator_checkov.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-validator-checkov
-Version: 0.0.1
+Version: 0.0.2
 Summary: @bridgecrew/cdk-validator-checkov
 Home-page: https://github.com/bridgecrewio/cdk-validator-checkov.git
 Author: bridgecrew<meet@bridgecrew.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/bridgecrewio/cdk-validator-checkov.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -52,30 +52,62 @@
 pip install cdk-validator-checkov
 ```
 
 ## Usage
 
 To use this plugin in your CDK application add it to the CDK App.
 
+### Python
+
+```python
+from cdk_validator_checkov import CheckovValidator
+
+...
+
+App(
+  policy_validation_beta1=[
+    CheckovValidator()
+  ]
+)
+```
+
+By default, the `CheckovValidator` plugin comes with all `checkov`
+[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
+In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+
+```python
+CheckovValidator(
+  check= ['CKV_AWS_18', 'CKV_AWS_21']
+)
+```
+
+```python
+CheckovValidator(
+  skipCheck= ['CKV_AWS_18', 'CKV_AWS_21']
+}
+```
+
+### TypeScript
+
 ```python
 new App({
   policyValidationBeta1: [
     new CheckovValidator(),
   ],
 });
 ```
 
-By default, the `CheckovValidator` plugin comes with all `checkov`
-[built-in checks for CloudFormation](https://www.checkov.io/5.Policy%20Index/cloudformation.html).
-In order to disable any of the checks or just run a subset of them you can use the `check` or `skipCheck` property.
+Specify checks:
 
 ```python
 new CheckovValidator({
     check: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
 
+Skip checks:
+
 ```python
 new CheckovValidator({
     skipCheck: ['CKV_AWS_18', 'CKV_AWS_21'],
 });
 ```
```

