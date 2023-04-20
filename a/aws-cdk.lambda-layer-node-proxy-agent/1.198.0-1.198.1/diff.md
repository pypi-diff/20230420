# Comparing `tmp/aws-cdk.lambda-layer-node-proxy-agent-1.198.0.tar.gz` & `tmp/aws-cdk.lambda-layer-node-proxy-agent-1.198.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src061017101/src/packages/@aws-cdk/lambda-layer-node-proxy-agent/dist/python/aws-cdk.lambda-layer-node-proxy-", last modified: Wed Mar 22 19:40:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src451122087/src/packages/@aws-cdk/lambda-layer-node-proxy-agent/dist/python/aws-cdk.lambda-layer-node-proxy-", last modified: Tue Mar 28 21:38:39 2023, max compression
```

## Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0.tar` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/README.md
--rw-r--r--   0 root         (0) root         (0)      236 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1960 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/
--rw-r--r--   0 root         (0) root         (0)      488 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1321680 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/lambda-layer-node-proxy-agent@1.198.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 19:40:01.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-22 19:40:06.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-03-28 21:38:33.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-03-28 21:38:33.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      776 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      488 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1320770 2023-03-28 21:38:33.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/lambda-layer-node-proxy-agent@1.198.1.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 21:38:34.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-03-28 21:38:38.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      644 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 21:38:38.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-03-28 21:38:39.000000 aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/top_level.txt
```

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/LICENSE` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/PKG-INFO` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.lambda-layer-node-proxy-agent
-Version: 1.198.0
+Version: 1.198.1
 Summary: An AWS Lambda layer that contains the `proxy-agent` NPM dependency
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/README.md` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/setup.py` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.lambda-layer-node-proxy-agent",
-    "version": "1.198.0",
+    "version": "1.198.1",
     "description": "An AWS Lambda layer that contains the `proxy-agent` NPM dependency",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.lambda_layer_node_proxy_agent",
         "aws_cdk.lambda_layer_node_proxy_agent._jsii"
     ],
     "package_data": {
         "aws_cdk.lambda_layer_node_proxy_agent._jsii": [
-            "lambda-layer-node-proxy-agent@1.198.0.jsii.tgz"
+            "lambda-layer-node-proxy-agent@1.198.1.jsii.tgz"
         ],
         "aws_cdk.lambda_layer_node_proxy_agent": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk.aws-lambda==1.198.0",
-        "aws-cdk.core==1.198.0",
+        "aws-cdk.aws-lambda==1.198.1",
+        "aws-cdk.core==1.198.1",
         "constructs>=3.3.69, <4.0.0",
         "jsii>=1.74.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk/lambda_layer_node_proxy_agent/__init__.py` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk/lambda_layer_node_proxy_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/PKG-INFO` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.lambda-layer-node-proxy-agent
-Version: 1.198.0
+Version: 1.198.1
 Summary: An AWS Lambda layer that contains the `proxy-agent` NPM dependency
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws-cdk.lambda-layer-node-proxy-agent-1.198.0/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/SOURCES.txt` & `aws-cdk.lambda-layer-node-proxy-agent-1.198.1/src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/SOURCES.txt
 src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/dependency_links.txt
 src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/requires.txt
 src/aws_cdk.lambda_layer_node_proxy_agent.egg-info/top_level.txt
 src/aws_cdk/lambda_layer_node_proxy_agent/__init__.py
 src/aws_cdk/lambda_layer_node_proxy_agent/py.typed
 src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/__init__.py
-src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/lambda-layer-node-proxy-agent@1.198.0.jsii.tgz
+src/aws_cdk/lambda_layer_node_proxy_agent/_jsii/lambda-layer-node-proxy-agent@1.198.1.jsii.tgz
```

