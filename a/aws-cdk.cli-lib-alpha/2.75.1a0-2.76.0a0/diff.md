# Comparing `tmp/aws-cdk.cli-lib-alpha-2.75.1a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.76.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src905434118/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.75.1a0.tar", last modified: Tue Apr 18 23:36:02 2023, max compression
+gzip compressed data, was "/codebuild/output/src551313152/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.76.0a0.tar", last modified: Thu Apr 20 00:54:45 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.75.1a0.tar` & `aws-cdk.cli-lib-alpha-2.76.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-04-18 23:35:42.000000 aws-cdk.cli-lib-alpha-2.75.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-18 23:35:44.000000 aws-cdk.cli-lib-alpha-2.75.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4179 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3192 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   189502 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  3641727 2023-04-18 23:35:42.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.75.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4179 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-04-20 00:54:35.000000 aws-cdk.cli-lib-alpha-2.76.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-20 00:54:36.000000 aws-cdk.cli-lib-alpha-2.76.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   194202 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  3571729 2023-04-20 00:54:35.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.76.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:54:38.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-04-20 00:54:44.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 00:54:45.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:54:44.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-20 00:54:44.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 00:54:44.000000 aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.76.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.76.0a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.76.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.75.1a0
+Version: 2.76.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/README.md` & `aws-cdk.cli-lib-alpha-2.76.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/setup.py` & `aws-cdk.cli-lib-alpha-2.76.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.75.1.a0",
+    "version": "2.76.0.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.75.1-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.76.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,16 +209,19 @@
     :stability: experimental
     '''
 
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
+        asset_parallelism: typing.Optional[builtins.bool] = None,
+        asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
         ci: typing.Optional[builtins.bool] = None,
+        concurrency: typing.Optional[jsii.Number] = None,
         exclusively: typing.Optional[builtins.bool] = None,
         execute: typing.Optional[builtins.bool] = None,
         force: typing.Optional[builtins.bool] = None,
         notification_arns: typing.Optional[typing.Sequence[builtins.str]] = None,
         outputs_file: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         progress: typing.Optional["StackActivityProgress"] = None,
@@ -246,16 +249,19 @@
         strict: typing.Optional[builtins.bool] = None,
         trace: typing.Optional[builtins.bool] = None,
         verbose: typing.Optional[builtins.bool] = None,
         version_reporting: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) cdk deploy.
 
+        :param asset_parallelism: (experimental) Whether to build/publish assets in parallel. Default: false
+        :param asset_prebuild: (experimental) Whether to build all assets before deploying the first stack (useful for failing Docker builds). Default: true
         :param change_set_name: (experimental) Optional name to use for the CloudFormation change set. If not provided, a name will be generated automatically. Default: - auto generate a name
         :param ci: (experimental) Whether we are on a CI system. Default: - ``false`` unless the environment variable ``CI`` is set
+        :param concurrency: (experimental) Maximum number of simultaneous deployments (dependency permitting) to execute. Default: 1
         :param exclusively: (experimental) Only perform action on the given stack. Default: false
         :param execute: (experimental) Whether to execute the ChangeSet Not providing ``execute`` parameter will result in execution of ChangeSet. Default: true
         :param force: (experimental) Always deploy, even if templates are identical. Default: false
         :param notification_arns: (experimental) ARNs of SNS topics that CloudFormation will notify with stack related events. Default: - no notifications
         :param outputs_file: (experimental) Path to file where stack outputs will be written after a successful deploy as JSON. Default: - Outputs are not written to any file
         :param parameters: (experimental) Additional parameters for CloudFormation at deploy time. Default: {}
         :param progress: (experimental) Display mode for stack activity events. The default in the CLI is StackActivityProgress.BAR. But since this is an API it makes more sense to set the default to StackActivityProgress.EVENTS Default: StackActivityProgress.EVENTS
@@ -466,16 +472,19 @@
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/cli-lib-alpha.IAwsCdkCli"
 
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
+        asset_parallelism: typing.Optional[builtins.bool] = None,
+        asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
         ci: typing.Optional[builtins.bool] = None,
+        concurrency: typing.Optional[jsii.Number] = None,
         exclusively: typing.Optional[builtins.bool] = None,
         execute: typing.Optional[builtins.bool] = None,
         force: typing.Optional[builtins.bool] = None,
         notification_arns: typing.Optional[typing.Sequence[builtins.str]] = None,
         outputs_file: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         progress: typing.Optional["StackActivityProgress"] = None,
@@ -503,16 +512,19 @@
         strict: typing.Optional[builtins.bool] = None,
         trace: typing.Optional[builtins.bool] = None,
         verbose: typing.Optional[builtins.bool] = None,
         version_reporting: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) cdk deploy.
 
+        :param asset_parallelism: (experimental) Whether to build/publish assets in parallel. Default: false
+        :param asset_prebuild: (experimental) Whether to build all assets before deploying the first stack (useful for failing Docker builds). Default: true
         :param change_set_name: (experimental) Optional name to use for the CloudFormation change set. If not provided, a name will be generated automatically. Default: - auto generate a name
         :param ci: (experimental) Whether we are on a CI system. Default: - ``false`` unless the environment variable ``CI`` is set
+        :param concurrency: (experimental) Maximum number of simultaneous deployments (dependency permitting) to execute. Default: 1
         :param exclusively: (experimental) Only perform action on the given stack. Default: false
         :param execute: (experimental) Whether to execute the ChangeSet Not providing ``execute`` parameter will result in execution of ChangeSet. Default: true
         :param force: (experimental) Always deploy, even if templates are identical. Default: false
         :param notification_arns: (experimental) ARNs of SNS topics that CloudFormation will notify with stack related events. Default: - no notifications
         :param outputs_file: (experimental) Path to file where stack outputs will be written after a successful deploy as JSON. Default: - Outputs are not written to any file
         :param parameters: (experimental) Additional parameters for CloudFormation at deploy time. Default: {}
         :param progress: (experimental) Display mode for stack activity events. The default in the CLI is StackActivityProgress.BAR. But since this is an API it makes more sense to set the default to StackActivityProgress.EVENTS Default: StackActivityProgress.EVENTS
@@ -541,16 +553,19 @@
         :param trace: (experimental) Print trace for stack warnings. Default: false
         :param verbose: (experimental) show debug logs. Default: false
         :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
 
         :stability: experimental
         '''
         options = DeployOptions(
+            asset_parallelism=asset_parallelism,
+            asset_prebuild=asset_prebuild,
             change_set_name=change_set_name,
             ci=ci,
+            concurrency=concurrency,
             exclusively=exclusively,
             execute=execute,
             force=force,
             notification_arns=notification_arns,
             outputs_file=outputs_file,
             parameters=parameters,
             progress=progress,
@@ -1891,16 +1906,19 @@
             check_type(argname="argument producer", value=producer, expected_type=type_hints["producer"])
         return typing.cast("AwsCdkCli", jsii.sinvoke(cls, "fromCloudAssemblyDirectoryProducer", [producer]))
 
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
+        asset_parallelism: typing.Optional[builtins.bool] = None,
+        asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
         ci: typing.Optional[builtins.bool] = None,
+        concurrency: typing.Optional[jsii.Number] = None,
         exclusively: typing.Optional[builtins.bool] = None,
         execute: typing.Optional[builtins.bool] = None,
         force: typing.Optional[builtins.bool] = None,
         notification_arns: typing.Optional[typing.Sequence[builtins.str]] = None,
         outputs_file: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         progress: typing.Optional[StackActivityProgress] = None,
@@ -1928,16 +1946,19 @@
         strict: typing.Optional[builtins.bool] = None,
         trace: typing.Optional[builtins.bool] = None,
         verbose: typing.Optional[builtins.bool] = None,
         version_reporting: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) cdk deploy.
 
+        :param asset_parallelism: (experimental) Whether to build/publish assets in parallel. Default: false
+        :param asset_prebuild: (experimental) Whether to build all assets before deploying the first stack (useful for failing Docker builds). Default: true
         :param change_set_name: (experimental) Optional name to use for the CloudFormation change set. If not provided, a name will be generated automatically. Default: - auto generate a name
         :param ci: (experimental) Whether we are on a CI system. Default: - ``false`` unless the environment variable ``CI`` is set
+        :param concurrency: (experimental) Maximum number of simultaneous deployments (dependency permitting) to execute. Default: 1
         :param exclusively: (experimental) Only perform action on the given stack. Default: false
         :param execute: (experimental) Whether to execute the ChangeSet Not providing ``execute`` parameter will result in execution of ChangeSet. Default: true
         :param force: (experimental) Always deploy, even if templates are identical. Default: false
         :param notification_arns: (experimental) ARNs of SNS topics that CloudFormation will notify with stack related events. Default: - no notifications
         :param outputs_file: (experimental) Path to file where stack outputs will be written after a successful deploy as JSON. Default: - Outputs are not written to any file
         :param parameters: (experimental) Additional parameters for CloudFormation at deploy time. Default: {}
         :param progress: (experimental) Display mode for stack activity events. The default in the CLI is StackActivityProgress.BAR. But since this is an API it makes more sense to set the default to StackActivityProgress.EVENTS Default: StackActivityProgress.EVENTS
@@ -1966,16 +1987,19 @@
         :param trace: (experimental) Print trace for stack warnings. Default: false
         :param verbose: (experimental) show debug logs. Default: false
         :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
 
         :stability: experimental
         '''
         options = DeployOptions(
+            asset_parallelism=asset_parallelism,
+            asset_prebuild=asset_prebuild,
             change_set_name=change_set_name,
             ci=ci,
+            concurrency=concurrency,
             exclusively=exclusively,
             execute=execute,
             force=force,
             notification_arns=notification_arns,
             outputs_file=outputs_file,
             parameters=parameters,
             progress=progress,
@@ -2272,16 +2296,19 @@
         "role_arn": "roleArn",
         "stacks": "stacks",
         "staging": "staging",
         "strict": "strict",
         "trace": "trace",
         "verbose": "verbose",
         "version_reporting": "versionReporting",
+        "asset_parallelism": "assetParallelism",
+        "asset_prebuild": "assetPrebuild",
         "change_set_name": "changeSetName",
         "ci": "ci",
+        "concurrency": "concurrency",
         "exclusively": "exclusively",
         "execute": "execute",
         "force": "force",
         "notification_arns": "notificationArns",
         "outputs_file": "outputsFile",
         "parameters": "parameters",
         "progress": "progress",
@@ -2312,16 +2339,19 @@
         role_arn: typing.Optional[builtins.str] = None,
         stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
         staging: typing.Optional[builtins.bool] = None,
         strict: typing.Optional[builtins.bool] = None,
         trace: typing.Optional[builtins.bool] = None,
         verbose: typing.Optional[builtins.bool] = None,
         version_reporting: typing.Optional[builtins.bool] = None,
+        asset_parallelism: typing.Optional[builtins.bool] = None,
+        asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
         ci: typing.Optional[builtins.bool] = None,
+        concurrency: typing.Optional[jsii.Number] = None,
         exclusively: typing.Optional[builtins.bool] = None,
         execute: typing.Optional[builtins.bool] = None,
         force: typing.Optional[builtins.bool] = None,
         notification_arns: typing.Optional[typing.Sequence[builtins.str]] = None,
         outputs_file: typing.Optional[builtins.str] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         progress: typing.Optional[StackActivityProgress] = None,
@@ -2349,16 +2379,19 @@
         :param role_arn: (experimental) Role to pass to CloudFormation for deployment. Default: - use the bootstrap cfn-exec role
         :param stacks: (experimental) List of stacks to deploy. Default: - all stacks
         :param staging: (experimental) Copy assets to the output directory. Needed for local debugging the source files with SAM CLI Default: false
         :param strict: (experimental) Do not construct stacks with warnings. Default: false
         :param trace: (experimental) Print trace for stack warnings. Default: false
         :param verbose: (experimental) show debug logs. Default: false
         :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
+        :param asset_parallelism: (experimental) Whether to build/publish assets in parallel. Default: false
+        :param asset_prebuild: (experimental) Whether to build all assets before deploying the first stack (useful for failing Docker builds). Default: true
         :param change_set_name: (experimental) Optional name to use for the CloudFormation change set. If not provided, a name will be generated automatically. Default: - auto generate a name
         :param ci: (experimental) Whether we are on a CI system. Default: - ``false`` unless the environment variable ``CI`` is set
+        :param concurrency: (experimental) Maximum number of simultaneous deployments (dependency permitting) to execute. Default: 1
         :param exclusively: (experimental) Only perform action on the given stack. Default: false
         :param execute: (experimental) Whether to execute the ChangeSet Not providing ``execute`` parameter will result in execution of ChangeSet. Default: true
         :param force: (experimental) Always deploy, even if templates are identical. Default: false
         :param notification_arns: (experimental) ARNs of SNS topics that CloudFormation will notify with stack related events. Default: - no notifications
         :param outputs_file: (experimental) Path to file where stack outputs will be written after a successful deploy as JSON. Default: - Outputs are not written to any file
         :param parameters: (experimental) Additional parameters for CloudFormation at deploy time. Default: {}
         :param progress: (experimental) Display mode for stack activity events. The default in the CLI is StackActivityProgress.BAR. But since this is an API it makes more sense to set the default to StackActivityProgress.EVENTS Default: StackActivityProgress.EVENTS
@@ -2396,16 +2429,19 @@
             check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
             check_type(argname="argument stacks", value=stacks, expected_type=type_hints["stacks"])
             check_type(argname="argument staging", value=staging, expected_type=type_hints["staging"])
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
             check_type(argname="argument trace", value=trace, expected_type=type_hints["trace"])
             check_type(argname="argument verbose", value=verbose, expected_type=type_hints["verbose"])
             check_type(argname="argument version_reporting", value=version_reporting, expected_type=type_hints["version_reporting"])
+            check_type(argname="argument asset_parallelism", value=asset_parallelism, expected_type=type_hints["asset_parallelism"])
+            check_type(argname="argument asset_prebuild", value=asset_prebuild, expected_type=type_hints["asset_prebuild"])
             check_type(argname="argument change_set_name", value=change_set_name, expected_type=type_hints["change_set_name"])
             check_type(argname="argument ci", value=ci, expected_type=type_hints["ci"])
+            check_type(argname="argument concurrency", value=concurrency, expected_type=type_hints["concurrency"])
             check_type(argname="argument exclusively", value=exclusively, expected_type=type_hints["exclusively"])
             check_type(argname="argument execute", value=execute, expected_type=type_hints["execute"])
             check_type(argname="argument force", value=force, expected_type=type_hints["force"])
             check_type(argname="argument notification_arns", value=notification_arns, expected_type=type_hints["notification_arns"])
             check_type(argname="argument outputs_file", value=outputs_file, expected_type=type_hints["outputs_file"])
             check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
             check_type(argname="argument progress", value=progress, expected_type=type_hints["progress"])
@@ -2451,18 +2487,24 @@
             self._values["strict"] = strict
         if trace is not None:
             self._values["trace"] = trace
         if verbose is not None:
             self._values["verbose"] = verbose
         if version_reporting is not None:
             self._values["version_reporting"] = version_reporting
+        if asset_parallelism is not None:
+            self._values["asset_parallelism"] = asset_parallelism
+        if asset_prebuild is not None:
+            self._values["asset_prebuild"] = asset_prebuild
         if change_set_name is not None:
             self._values["change_set_name"] = change_set_name
         if ci is not None:
             self._values["ci"] = ci
+        if concurrency is not None:
+            self._values["concurrency"] = concurrency
         if exclusively is not None:
             self._values["exclusively"] = exclusively
         if execute is not None:
             self._values["execute"] = execute
         if force is not None:
             self._values["force"] = force
         if notification_arns is not None:
@@ -2709,14 +2751,36 @@
 
         :stability: experimental
         '''
         result = self._values.get("version_reporting")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def asset_parallelism(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Whether to build/publish assets in parallel.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("asset_parallelism")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def asset_prebuild(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Whether to build all assets before deploying the first stack (useful for failing Docker builds).
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("asset_prebuild")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def change_set_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) Optional name to use for the CloudFormation change set.
 
         If not provided, a name will be generated automatically.
 
         :default: - auto generate a name
 
@@ -2733,14 +2797,25 @@
 
         :stability: experimental
         '''
         result = self._values.get("ci")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def concurrency(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) Maximum number of simultaneous deployments (dependency permitting) to execute.
+
+        :default: 1
+
+        :stability: experimental
+        '''
+        result = self._values.get("concurrency")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def exclusively(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Only perform action on the given stack.
 
         :default: false
 
         :stability: experimental
         '''
@@ -3861,16 +3936,19 @@
     role_arn: typing.Optional[builtins.str] = None,
     stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
     staging: typing.Optional[builtins.bool] = None,
     strict: typing.Optional[builtins.bool] = None,
     trace: typing.Optional[builtins.bool] = None,
     verbose: typing.Optional[builtins.bool] = None,
     version_reporting: typing.Optional[builtins.bool] = None,
+    asset_parallelism: typing.Optional[builtins.bool] = None,
+    asset_prebuild: typing.Optional[builtins.bool] = None,
     change_set_name: typing.Optional[builtins.str] = None,
     ci: typing.Optional[builtins.bool] = None,
+    concurrency: typing.Optional[jsii.Number] = None,
     exclusively: typing.Optional[builtins.bool] = None,
     execute: typing.Optional[builtins.bool] = None,
     force: typing.Optional[builtins.bool] = None,
     notification_arns: typing.Optional[typing.Sequence[builtins.str]] = None,
     outputs_file: typing.Optional[builtins.str] = None,
     parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     progress: typing.Optional[StackActivityProgress] = None,
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.76.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.75.1a0
+Version: 2.76.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

