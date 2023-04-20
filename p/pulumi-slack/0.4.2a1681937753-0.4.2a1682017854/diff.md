# Comparing `tmp/pulumi_slack-0.4.2a1681937753.tar.gz` & `tmp/pulumi_slack-0.4.2a1682017854.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.2a1681937753.tar", last modified: Wed Apr 19 21:06:21 2023, max compression
+gzip compressed data, was "pulumi_slack-0.4.2a1682017854.tar", last modified: Thu Apr 20 19:15:34 2023, max compression
```

## Comparing `pulumi_slack-0.4.2a1681937753.tar` & `pulumi_slack-0.4.2a1682017854.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:06:21.368453 pulumi_slack-0.4.2a1681937753/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 21:06:21.368453 pulumi_slack-0.4.2a1681937753/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:06:21.364453 pulumi_slack-0.4.2a1681937753/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:06:21.364453 pulumi_slack-0.4.2a1681937753/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:06:21.364453 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:06:21.368453 pulumi_slack-0.4.2a1681937753/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-19 21:06:21.000000 pulumi_slack-0.4.2a1681937753/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.530107 pulumi_slack-0.4.2a1682017854/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/setup.py
```

### Comparing `pulumi_slack-0.4.2a1681937753/PKG-INFO` & `pulumi_slack-0.4.2a1682017854/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.2a1681937753
+Version: 0.4.2a1682017854
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Slack Resource Provider
 
 The Slack Provider enables you to manage Slack resources via Pulumi.
 
 ## Installing
```

### Comparing `pulumi_slack-0.4.2a1681937753/README.md` & `pulumi_slack-0.4.2a1682017854/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/__init__.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/conversation.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/get_user.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/provider.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.2a1682017854/pulumi_slack/usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-slack
-Version: 0.4.2a1681937753
+Version: 0.4.2a1682017854
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Slack Resource Provider
 
 The Slack Provider enables you to manage Slack resources via Pulumi.
 
 ## Installing
```

### Comparing `pulumi_slack-0.4.2a1681937753/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1681937753/setup.py` & `pulumi_slack-0.4.2a1682017854/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.2a1681937753"
-PLUGIN_VERSION = "0.4.2-alpha.1681937753+4dddcbf8"
+VERSION = "0.4.2a1682017854"
+PLUGIN_VERSION = "0.4.2-alpha.1682017854+5c7b6a6e"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'slack', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "slack Pulumi Package - Development Version"
 
 
 setup(name='pulumi_slack',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for managing Slack workspaces.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

