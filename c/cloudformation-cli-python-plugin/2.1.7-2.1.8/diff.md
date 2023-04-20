# Comparing `tmp/cloudformation-cli-python-plugin-2.1.7.tar.gz` & `tmp/cloudformation-cli-python-plugin-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudformation-cli-python-plugin-2.1.7.tar", last modified: Fri Jan 13 22:35:12 2023, max compression
+gzip compressed data, was "dist/cloudformation-cli-python-plugin-2.1.8.tar", last modified: Thu Apr 20 17:22:48 2023, max compression
```

## Comparing `cloudformation-cli-python-plugin-2.1.7.tar` & `cloudformation-cli-python-plugin-2.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.244383 cloudformation-cli-python-plugin-2.1.7/
--rw-r--r--   0 himanshs   (504) staff       (20)    10142 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/LICENSE
--rw-r--r--   0 himanshs   (504) staff       (20)      143 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/MANIFEST.in
--rw-r--r--   0 himanshs   (504) staff       (20)     4116 2023-01-13 22:35:12.244559 cloudformation-cli-python-plugin-2.1.7/PKG-INFO
--rw-r--r--   0 himanshs   (504) staff       (20)     3075 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/README.md
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.227847 cloudformation-cli-python-plugin-2.1.7/python/
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.234595 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/
--rw-r--r--   0 himanshs   (504) staff       (20)     4116 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO
--rw-r--r--   0 himanshs   (504) staff       (20)      984 2023-01-13 22:35:12.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 himanshs   (504) staff       (20)        1 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 himanshs   (504) staff       (20)      475 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/entry_points.txt
--rw-r--r--   0 himanshs   (504) staff       (20)       52 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/requires.txt
--rw-r--r--   0 himanshs   (504) staff       (20)        5 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/top_level.txt
--rw-r--r--   0 himanshs   (504) staff       (20)        1 2023-01-13 22:35:11.000000 cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/zip-safe
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.228005 cloudformation-cli-python-plugin-2.1.7/python/rpdk/
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.237239 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/
--rw-r--r--   0 himanshs   (504) staff       (20)      101 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/__init__.py
--rw-r--r--   0 himanshs   (504) staff       (20)    14824 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/codegen.py
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.238944 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/data/
--rw-r--r--   0 himanshs   (504) staff       (20)     1759 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/data/Python.gitignore
--rw-r--r--   0 himanshs   (504) staff       (20)        0 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/data/__init__.py
--rw-r--r--   0 himanshs   (504) staff       (20)     1417 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/parser.py
--rw-r--r--   0 himanshs   (504) staff       (20)     1681 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/resolver.py
-drwxr-xr-x   0 himanshs   (504) staff       (20)        0 2023-01-13 22:35:12.243805 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/
--rw-r--r--   0 himanshs   (504) staff       (20)     1806 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/README.md
--rw-r--r--   0 himanshs   (504) staff       (20)     3618 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/handlers.py
--rw-r--r--   0 himanshs   (504) staff       (20)     3384 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/hook_handlers.py
--rw-r--r--   0 himanshs   (504) staff       (20)     2337 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/hook_models.py
--rw-r--r--   0 himanshs   (504) staff       (20)     2544 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/models.py
--rw-r--r--   0 himanshs   (504) staff       (20)       30 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/requirements.txt
--rw-r--r--   0 himanshs   (504) staff       (20)     2364 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/target_model.py
--rw-r--r--   0 himanshs   (504) staff       (20)      738 2023-01-13 22:35:12.245423 cloudformation-cli-python-plugin-2.1.7/setup.cfg
--rw-r--r--   0 himanshs   (504) staff       (20)     2750 2023-01-13 20:56:53.000000 cloudformation-cli-python-plugin-2.1.7/setup.py
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/
+-rw-r--r--   0 izoran   (22393816) amazon     (100)    10142 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/LICENSE
+-rw-r--r--   0 izoran   (22393816) amazon     (100)      143 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/MANIFEST.in
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     4925 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/PKG-INFO
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     3075 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/README.md
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     4925 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 izoran   (22393816) amazon     (100)      984 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)        1 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)      476 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)       52 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/requires.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)        5 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/top_level.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)        1 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/zip-safe
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/
+-rw-r--r--   0 izoran   (22393816) amazon     (100)      101 2023-04-20 16:20:40.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/__init__.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)    16576 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/codegen.py
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     1759 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/Python.gitignore
+-rw-r--r--   0 izoran   (22393816) amazon     (100)        0 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/__init__.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     1417 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/parser.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     1681 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/resolver.py
+drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     1806 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/README.md
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     3618 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/handlers.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     3384 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_handlers.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     2337 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_models.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     2544 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/models.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)       30 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/requirements.txt
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     2232 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/target_model.py
+-rw-r--r--   0 izoran   (22393816) amazon     (100)      738 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/setup.cfg
+-rw-r--r--   0 izoran   (22393816) amazon     (100)     2750 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cloudformation-cli-python-plugin-2.1.7/LICENSE` & `cloudformation-cli-python-plugin-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/PKG-INFO` & `cloudformation-cli-python-plugin-2.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-python-plugin
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python 3.6 and 3.7 language support for the CloudFormation CLI
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
+Description: # AWS CloudFormation Resource Provider Python Plugin
+        
+        The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
+        
+        This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
+        
+        ## AWS CloudFormation Resource Provider Python Plugin
+        
+        The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
+        
+        This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
+        
+        [![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
+        
+        ## Community
+        
+        Join us on Discord! Connect & interact with CloudFormation developers &
+        experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
+        Guard and more:
+        
+        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+        
+        Installation
+        ------------
+        
+        ```bash
+        pip install cloudformation-cli-python-plugin
+        ```
+        
+        Howto
+        -----
+        
+        ```
+        $ cfn init
+        Initializing new project
+        What's the name of your resource type?
+        (Organization::Service::Resource)
+        >> Foo::Bar::Baz
+        Select a language for code generation:
+        [1] java
+        [2] csharp
+        [3] python36
+        [4] python37
+        (enter an integer):
+        >> 4
+        Use docker for platform-independent packaging (Y/n)?
+        This is highly recommended unless you are experienced
+        with cross-platform Python packaging.
+        >> y
+        Initialized a new project in <>
+        $ cfn submit --dry-run
+        $ cat <<EOT > test.json
+        {
+          "credentials": {
+            "accessKeyId": "",
+            "secretAccessKey": "",
+            "sessionToken": ""
+          },
+          "action": "CREATE",
+          "request": {
+            "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
+            "desiredResourceState": {
+              "Title": "This_Is_The_Title_For_My_Example",
+              "TestCode": "NOT_STARTED"
+            },
+            "previousResourceState": null,
+            "logicalResourceIdentifier": null
+          },
+          "callbackContext": null
+        }
+        EOT
+        $ sam local invoke TestEntrypoint --event test.json
+        ```
+        
+        Development
+        -----------
+        
+        For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
+        
+        ```
+        python3 -m venv env
+        source env/bin/activate
+        pip install -e . -e src/ \
+          -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
+        pre-commit install
+        ```
+        
+        Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
+        
+        ```
+        # run all hooks on all files, mirrors what the CI runs
+        pre-commit run --all-files
+        # run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
+        pre-commit run pytest-local
+        ```
+        
+        License
+        -------
+        
+        This library is licensed under the Apache 2.0 License.
+        
 Keywords: Amazon Web Services AWS CloudFormation
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AWS CloudFormation Resource Provider Python Plugin
-
-The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
-
-This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
-
-## AWS CloudFormation Resource Provider Python Plugin
-
-The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
-
-This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
-
-[![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
-
-## Community
-
-Join us on Discord! Connect & interact with CloudFormation developers &
-experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
-Guard and more:
-
-[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
-
-Installation
-------------
-
-```bash
-pip install cloudformation-cli-python-plugin
-```
-
-Howto
------
-
-```
-$ cfn init
-Initializing new project
-What's the name of your resource type?
-(Organization::Service::Resource)
->> Foo::Bar::Baz
-Select a language for code generation:
-[1] java
-[2] csharp
-[3] python36
-[4] python37
-(enter an integer):
->> 4
-Use docker for platform-independent packaging (Y/n)?
-This is highly recommended unless you are experienced
-with cross-platform Python packaging.
->> y
-Initialized a new project in <>
-$ cfn submit --dry-run
-$ cat <<EOT > test.json
-{
-  "credentials": {
-    "accessKeyId": "",
-    "secretAccessKey": "",
-    "sessionToken": ""
-  },
-  "action": "CREATE",
-  "request": {
-    "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
-    "desiredResourceState": {
-      "Title": "This_Is_The_Title_For_My_Example",
-      "TestCode": "NOT_STARTED"
-    },
-    "previousResourceState": null,
-    "logicalResourceIdentifier": null
-  },
-  "callbackContext": null
-}
-EOT
-$ sam local invoke TestEntrypoint --event test.json
-```
-
-Development
------------
-
-For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
-
-```
-python3 -m venv env
-source env/bin/activate
-pip install -e . -e src/ \
-  -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
-pre-commit install
-```
-
-Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
-
-```
-# run all hooks on all files, mirrors what the CI runs
-pre-commit run --all-files
-# run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
-pre-commit run pytest-local
-```
-
-License
--------
-
-This library is licensed under the Apache 2.0 License.
```

### Comparing `cloudformation-cli-python-plugin-2.1.7/README.md` & `cloudformation-cli-python-plugin-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO` & `cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-python-plugin
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python 3.6 and 3.7 language support for the CloudFormation CLI
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
+Description: # AWS CloudFormation Resource Provider Python Plugin
+        
+        The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
+        
+        This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
+        
+        ## AWS CloudFormation Resource Provider Python Plugin
+        
+        The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
+        
+        This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
+        
+        [![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
+        
+        ## Community
+        
+        Join us on Discord! Connect & interact with CloudFormation developers &
+        experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
+        Guard and more:
+        
+        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+        
+        Installation
+        ------------
+        
+        ```bash
+        pip install cloudformation-cli-python-plugin
+        ```
+        
+        Howto
+        -----
+        
+        ```
+        $ cfn init
+        Initializing new project
+        What's the name of your resource type?
+        (Organization::Service::Resource)
+        >> Foo::Bar::Baz
+        Select a language for code generation:
+        [1] java
+        [2] csharp
+        [3] python36
+        [4] python37
+        (enter an integer):
+        >> 4
+        Use docker for platform-independent packaging (Y/n)?
+        This is highly recommended unless you are experienced
+        with cross-platform Python packaging.
+        >> y
+        Initialized a new project in <>
+        $ cfn submit --dry-run
+        $ cat <<EOT > test.json
+        {
+          "credentials": {
+            "accessKeyId": "",
+            "secretAccessKey": "",
+            "sessionToken": ""
+          },
+          "action": "CREATE",
+          "request": {
+            "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
+            "desiredResourceState": {
+              "Title": "This_Is_The_Title_For_My_Example",
+              "TestCode": "NOT_STARTED"
+            },
+            "previousResourceState": null,
+            "logicalResourceIdentifier": null
+          },
+          "callbackContext": null
+        }
+        EOT
+        $ sam local invoke TestEntrypoint --event test.json
+        ```
+        
+        Development
+        -----------
+        
+        For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
+        
+        ```
+        python3 -m venv env
+        source env/bin/activate
+        pip install -e . -e src/ \
+          -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
+        pre-commit install
+        ```
+        
+        Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
+        
+        ```
+        # run all hooks on all files, mirrors what the CI runs
+        pre-commit run --all-files
+        # run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
+        pre-commit run pytest-local
+        ```
+        
+        License
+        -------
+        
+        This library is licensed under the Apache 2.0 License.
+        
 Keywords: Amazon Web Services AWS CloudFormation
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AWS CloudFormation Resource Provider Python Plugin
-
-The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
-
-This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
-
-## AWS CloudFormation Resource Provider Python Plugin
-
-The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
-
-This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
-
-[![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
-
-## Community
-
-Join us on Discord! Connect & interact with CloudFormation developers &
-experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
-Guard and more:
-
-[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
-
-Installation
-------------
-
-```bash
-pip install cloudformation-cli-python-plugin
-```
-
-Howto
------
-
-```
-$ cfn init
-Initializing new project
-What's the name of your resource type?
-(Organization::Service::Resource)
->> Foo::Bar::Baz
-Select a language for code generation:
-[1] java
-[2] csharp
-[3] python36
-[4] python37
-(enter an integer):
->> 4
-Use docker for platform-independent packaging (Y/n)?
-This is highly recommended unless you are experienced
-with cross-platform Python packaging.
->> y
-Initialized a new project in <>
-$ cfn submit --dry-run
-$ cat <<EOT > test.json
-{
-  "credentials": {
-    "accessKeyId": "",
-    "secretAccessKey": "",
-    "sessionToken": ""
-  },
-  "action": "CREATE",
-  "request": {
-    "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
-    "desiredResourceState": {
-      "Title": "This_Is_The_Title_For_My_Example",
-      "TestCode": "NOT_STARTED"
-    },
-    "previousResourceState": null,
-    "logicalResourceIdentifier": null
-  },
-  "callbackContext": null
-}
-EOT
-$ sam local invoke TestEntrypoint --event test.json
-```
-
-Development
------------
-
-For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
-
-```
-python3 -m venv env
-source env/bin/activate
-pip install -e . -e src/ \
-  -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
-pre-commit install
-```
-
-Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
-
-```
-# run all hooks on all files, mirrors what the CI runs
-pre-commit run --all-files
-# run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
-pre-commit run pytest-local
-```
-
-License
--------
-
-This library is licensed under the Apache 2.0 License.
```

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt` & `cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/codegen.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/codegen.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import zipfile
 from docker.errors import APIError, ContainerError, ImageLoadError
 from pathlib import PurePosixPath
 from requests.exceptions import ConnectionError as RequestsConnectionError
 from rpdk.core.data_loaders import resource_stream
 from rpdk.core.exceptions import DownstreamError, SysExitRecommendedError
 from rpdk.core.init import input_with_validation
-from rpdk.core.jsonutils.resolver import ContainerType, resolve_models
+from rpdk.core.jsonutils.resolver import (
+    UNDEFINED,
+    ContainerType,
+    ResolvedType,
+    resolve_models,
+)
 from rpdk.core.plugin_base import LanguagePlugin
 from rpdk.core.project import ARTIFACT_TYPE_HOOK
 from subprocess import PIPE, CalledProcessError, run as subprocess_run  # nosec
 from tempfile import TemporaryFile
 from typing import Dict
 
 from . import __version__
@@ -206,16 +211,56 @@
             template = self.env.get_template("hook_models.py")
         else:
             template = self.env.get_template("models.py")
 
         contents = template.render(support_lib_pkg=SUPPORT_LIB_PKG, models=models)
         project.overwrite(path, contents)
 
+        if project.artifact_type == ARTIFACT_TYPE_HOOK:
+            self._generate_target_models(project)
+
         LOG.debug("Generate complete")
 
+    def _generate_target_models(self, project):
+        target_model_dir = self.package_root / self.package_name / "target_models"
+
+        LOG.debug("Removing generated models: %s", target_model_dir)
+        shutil.rmtree(target_model_dir, ignore_errors=True)
+
+        target_model_dir.mkdir(parents=True, exist_ok=True)
+        template = self.env.get_template("target_model.py")
+
+        for target_type_name, target_info in project.target_info.items():
+            target_schema = target_info["Schema"]
+            target_namespace = [
+                s.lower() for s in target_type_name.split("::")
+            ]  # AWS::SQS::Queue -> awssqsqueue
+            target_name = "".join(
+                [s.capitalize() for s in target_namespace]
+            )  # awssqsqueue -> AwsSqsQueue
+            target_model_file = "{}.py".format(
+                "_".join(target_namespace)
+            )  # awssqsqueue -> aws_sqs_queue.py
+
+            models = resolve_models(target_schema, target_name)
+
+            # TODO: Remove once tagging is fully supported
+            if models.get(target_name, {}).get("Tags"):  # pragma: no cover
+                models[target_name]["Tags"] = ResolvedType(
+                    ContainerType.PRIMITIVE, UNDEFINED
+                )
+
+            path = target_model_dir / target_model_file
+            LOG.debug("Writing file: %s", path)
+
+            contents = template.render(
+                support_lib_pkg=SUPPORT_LIB_PKG, models=models, target_name=target_name
+            )
+            project.overwrite(path, contents)
+
     # pylint: disable=unused-argument
     # the argument "project" is not used here but is used in codegen.py of other plugins
     # this method is called in cloudformation-cli/src/rpdk/core/project.py
     def get_plugin_information(self, project) -> Dict:
         return self._get_plugin_information()
 
     def _pre_package(self, build_path):
@@ -326,14 +371,15 @@
                 image=image,
                 command=command,
                 auto_remove=True,
                 volumes=volumes,
                 stream=True,
                 entrypoint="",
                 user=localuser,
+                platform="linux/amd64",
             )
         except RequestsConnectionError as e:
             # it seems quite hard to reliably extract the cause from
             # ConnectionError. we replace it with a friendlier error message
             # and preserve the cause for debug traceback
             cause = RequestsConnectionError(
                 "Could not connect to docker - is it running?"
```

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/data/Python.gitignore` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/Python.gitignore`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/parser.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/parser.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/resolver.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/resolver.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/README.md` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/README.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/handlers.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/handlers.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/hook_handlers.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/hook_models.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_models.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/models.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/models.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/python/rpdk/python/templates/target_model.py` & `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/target_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,20 +39,16 @@
     def _deserialize(
         cls: Type["_{{ model }}"],
         json_data: Optional[Mapping[str, Any]],
     ) -> Optional["_{{ model }}"]:
         if not json_data:
             return None
         {% if model == (target_name) %}
-        data = dict(filter(lambda e: e[0] in cls.__dataclass_fields__, json_data.items()))
-        if not data:
-            return None
-
         dataclasses = {n: o for n, o in getmembers(sys.modules[__name__]) if isclass(o)}
-        recast_object(cls, data, dataclasses)
+        recast_object(cls, json_data, dataclasses)
         {% endif %}
         return cls(
             {% for name, type in properties.items() %}
             {% set container = type.container %}
             {% set resolved_type = type.type %}
             {% if container == ContainerType.MODEL %}
             {{ name }}={{ resolved_type }}._deserialize(json_data.get("{{ name }}")),
```

### Comparing `cloudformation-cli-python-plugin-2.1.7/setup.cfg` & `cloudformation-cli-python-plugin-2.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.7/setup.py` & `cloudformation-cli-python-plugin-2.1.8/setup.py`

 * *Files identical despite different names*

