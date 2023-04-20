# Comparing `tmp/cli-aws-mfa-0.0.7.tar.gz` & `tmp/cli-aws-mfa-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-aws-mfa-0.0.7.tar", last modified: Wed Apr 19 11:36:11 2023, max compression
+gzip compressed data, was "cli-aws-mfa-0.0.8.tar", last modified: Thu Apr 20 05:52:07 2023, max compression
```

## Comparing `cli-aws-mfa-0.0.7.tar` & `cli-aws-mfa-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:36:11.337499 cli-aws-mfa-0.0.7/
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:36:11.336274 cli-aws-mfa-0.0.7/MFA/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.7/MFA/__init__.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     4341 2023-04-19 11:26:05.000000 cli-aws-mfa-0.0.7/MFA/mfa.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1374 2023-04-19 11:36:11.337296 cli-aws-mfa-0.0.7/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1122 2023-04-19 11:32:09.000000 cli-aws-mfa-0.0.7/README.md
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1658 2023-04-19 11:27:22.000000 cli-aws-mfa-0.0.7/cli.py
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:36:11.337124 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1374 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      264 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       40 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/entry_points.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/requires.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        8 2023-04-19 11:36:11.000000 cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/top_level.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-19 11:36:11.337535 cli-aws-mfa-0.0.7/setup.cfg
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      953 2023-04-19 11:36:06.000000 cli-aws-mfa-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/MFA/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/MFA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/MFA/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 05:52:07.000000 cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 05:52:07.269818 cli-aws-mfa-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 05:51:56.000000 cli-aws-mfa-0.0.8/setup.py
```

### Comparing `cli-aws-mfa-0.0.7/MFA/mfa.py` & `cli-aws-mfa-0.0.8/MFA/mfa.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.7/PKG-INFO` & `cli-aws-mfa-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.7
+Version: 0.0.8
 Summary: AWS CLI MFA - Easily Manage Session Token
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # AWS CLI MFA
 
 Developed by Ajeet Yadav
 
 ## Example of How To Use
```

### Comparing `cli-aws-mfa-0.0.7/README.md` & `cli-aws-mfa-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.7/cli.py` & `cli-aws-mfa-0.0.8/cli.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.7/cli_aws_mfa.egg-info/PKG-INFO` & `cli-aws-mfa-0.0.8/cli_aws_mfa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.7
+Version: 0.0.8
 Summary: AWS CLI MFA - Easily Manage Session Token
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # AWS CLI MFA
 
 Developed by Ajeet Yadav
 
 ## Example of How To Use
```

### Comparing `cli-aws-mfa-0.0.7/setup.py` & `cli-aws-mfa-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "AWS CLI MFA - Easily Manage Session Token"
 LONG_DESCRIPTION = "Use MFA to increase the security of your AWS environment. Signing in with MFA requires an authentication code from an MFA device."
 
 # Setting up
 setup(
     name="cli-aws-mfa",
     version=VERSION,
```

