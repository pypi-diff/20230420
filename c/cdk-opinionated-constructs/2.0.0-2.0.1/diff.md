# Comparing `tmp/cdk-opinionated-constructs-2.0.0.tar.gz` & `tmp/cdk-opinionated-constructs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-2.0.0.tar", last modified: Thu Apr 20 10:21:24 2023, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.0.1.tar", last modified: Thu Apr 20 10:39:09 2023, max compression
```

## Comparing `cdk-opinionated-constructs-2.0.0.tar` & `cdk-opinionated-constructs-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.511159 cdk-opinionated-constructs-2.0.0/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.0.0/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:21:24.511295 cdk-opinionated-constructs-2.0.0/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.0.0/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.497307 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2798 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.510824 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-04-20 10:21:24.512062 cdk-opinionated-constructs-2.0.0/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-04-20 10:20:36.000000 cdk-opinionated-constructs-2.0.0/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.498141 cdk-opinionated-constructs-2.0.0/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1710 2023-04-05 07:27:40.000000 cdk-opinionated-constructs-2.0.0/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.505181 cdk-opinionated-constructs-2.0.0/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.0/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3177 2023-04-05 07:27:40.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2591 2023-02-20 08:54:39.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.0/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.508720 cdk-opinionated-constructs-2.0.0/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.302361 cdk-opinionated-constructs-2.0.1/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.0.1/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:39:09.303619 cdk-opinionated-constructs-2.0.1/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.0.1/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.127497 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2798 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.298337 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-04-20 10:39:09.309152 cdk-opinionated-constructs-2.0.1/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-04-20 10:38:52.000000 cdk-opinionated-constructs-2.0.1/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.135496 cdk-opinionated-constructs-2.0.1/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.0.1/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.243334 cdk-opinionated-constructs-2.0.1/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.1/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.1/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.273664 cdk-opinionated-constructs-2.0.1/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-2.0.0/LICENSE` & `cdk-opinionated-constructs-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/README.md` & `cdk-opinionated-constructs-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/setup.cfg` & `cdk-opinionated-constructs-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/setup.py` & `cdk-opinionated-constructs-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="2.0.0",
+    version="2.0.1",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk-opinionated-constructs-2.0.0/test/app.py` & `cdk-opinionated-constructs-2.0.1/test/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 """Main app."""
 
-import aws_cdk as cdk
 import os
-from stacks.s3_stack import TestS3Stack
-from stacks.sns_stack import TestSNSStack
-from stacks.lmb_stack import TestAWSPythonLambdaFunctionStack
-from stacks.lmb_monitoring_stack import TestAWSPythonLambdaFunctionStackMonitoring
-from stacks.wafv2_stack import TestWAFv2Stack
+
+import aws_cdk as cdk
+
 from stacks.alb_stack import TestALBStack
 from stacks.ecr_stack import TestECRStack
+from stacks.lmb_docker_stack import TestAWSLambdaDockerFunctionStack
+from stacks.lmb_monitoring_stack import TestAWSPythonLambdaFunctionStackMonitoring
+from stacks.lmb_stack import TestAWSPythonLambdaFunctionStack
 from stacks.nlb_stack import TestNLBStack
-from stacks.rds_postgresql_stack import TestRDSPostgreSQLStack
 from stacks.rds_mysql_stack import TestRDSMySQLStack
+from stacks.rds_postgresql_stack import TestRDSPostgreSQLStack
+from stacks.s3_stack import TestS3Stack
+from stacks.sns_stack import TestSNSStack
+from stacks.wafv2_stack import TestWAFv2Stack
 
 CDK_ENV = cdk.Environment(account=os.environ["CDK_DEFAULT_ACCOUNT"], region=os.environ["CDK_DEFAULT_REGION"])
 
 app = cdk.App()
 TestS3Stack(app, "TestS3Stack")
 TestSNSStack(app, "TestSNSStack")
 TestLambdaStack = TestAWSPythonLambdaFunctionStack(
@@ -27,15 +30,15 @@
 )
 TestLambdaMonitoringStack = TestAWSPythonLambdaFunctionStackMonitoring(
     app,
     "TestAWSLambdaFunctionMonitoringStack",
     env=CDK_ENV,
     props=TestLambdaStack.output_props,
 )
-TestAWSPythonLambdaFunctionStack = TestAWSPythonLambdaFunctionStack(
+TestAWSPythonLambdaFunctionStack = TestAWSLambdaDockerFunctionStack(
     app,
     "TestAWSLambdaDockerFunctionStack",
     env=CDK_ENV,
     props={"project": "test_project", "service_name": "example_lambda_function"},
 )
 TestWAFv2Stack(app, "TestWAFv2Stack", env=CDK_ENV)
 TestALBStack(app, "TestALBStack", env=CDK_ENV)
```

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_docker_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import aws_cdk.aws_ec2 as ec2
 import aws_cdk as cdk
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
-class TestAWSPythonLambdaFunctionStack(Stack):
+class TestAWSLambdaDockerFunctionStack(Stack):
     """Test generated sns topic against AWS solutions  checks."""
 
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
 
         vpc = ec2.Vpc(self, id="vpc")
         NagSuppressions.add_resource_suppressions(
@@ -33,21 +33,22 @@
             self,
             id="ecr_repository",
             auto_delete_images=True,
             encryption=ecr.RepositoryEncryption.AES_256,
             image_scan_on_push=True,
             image_tag_mutability=ecr.TagMutability.IMMUTABLE,
             repository_name="test_ecr_repository",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
         )
 
         lmb_construct = AWSDockerLambdaFunction(self, id="lmb_construct")
         lmb_function = lmb_construct.create_lambda_function(
             code=lmb.DockerImageCode.from_ecr(
                 repository=ecr_repository,
-                tag="0",
+                tag_or_digest="0",
             ),
             env=env,
             ephemeral_storage_size=cdk.Size.gibibytes(amount=10),
             function_name=props["service_name"],
             timeout=60,
             memory_size=512,
             env_variables={
```

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,19 @@
     def nag_suppression() -> list:
         """Create CFN-NAG suppression.
 
         :return:
         """
         return [
             {
+                "id": "AwsSolutions-L1",
+                "reason": "Supressing false positive, lambda is using latest runtime available at the moment which"
+                "is python3.10",
+            },
+            {
                 "id": "AwsSolutions-IAM4",
                 "reason": "Using managed policies is allowed",
             },
             {
                 "id": "AwsSolutions-IAM5",
                 "reason": "There isn't a way to tailor IAM policy using more restrictive permissions for "
                 "used API calls logs:CreateLogGroup, xray:PutTelemetryRecords, xray:PutTraceSegments",
```

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.0.1/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.0/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.0.1/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

