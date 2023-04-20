# Comparing `tmp/cdk-opinionated-constructs-1.9.1.tar.gz` & `tmp/cdk-opinionated-constructs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-1.9.1.tar", last modified: Wed Nov 23 22:26:05 2022, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.0.0.tar", last modified: Thu Apr 20 10:21:24 2023, max compression
```

## Comparing `cdk-opinionated-constructs-1.9.1.tar` & `cdk-opinionated-constructs-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.260687 cdk-opinionated-constructs-1.9.1/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-1.9.1/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-23 22:26:05.260763 cdk-opinionated-constructs-1.9.1/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    10354 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.240465 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     7612 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5299 2022-11-23 22:24:16.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2607 2022-11-05 20:59:58.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    12206 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.260270 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      970 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       47 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2022-11-23 22:26:05.261502 cdk-opinionated-constructs-1.9.1/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      715 2022-11-23 22:25:39.000000 cdk-opinionated-constructs-1.9.1/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.241167 cdk-opinionated-constructs-1.9.1/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      878 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.247653 cdk-opinionated-constructs-1.9.1/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1591 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.1/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2368 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1513 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2616 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.254670 cdk-opinionated-constructs-1.9.1/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.511159 cdk-opinionated-constructs-2.0.0/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.0.0/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:21:24.511295 cdk-opinionated-constructs-2.0.0/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.0.0/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.497307 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2798 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.510824 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-04-20 10:21:24.000000 cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-04-20 10:21:24.512062 cdk-opinionated-constructs-2.0.0/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-04-20 10:20:36.000000 cdk-opinionated-constructs-2.0.0/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.498141 cdk-opinionated-constructs-2.0.0/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1710 2023-04-05 07:27:40.000000 cdk-opinionated-constructs-2.0.0/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.505181 cdk-opinionated-constructs-2.0.0/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.0/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3177 2023-04-05 07:27:40.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2591 2023-02-20 08:54:39.000000 cdk-opinionated-constructs-2.0.0/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.0/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.0/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.0/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:21:24.508720 cdk-opinionated-constructs-2.0.0/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.0/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-1.9.1/LICENSE` & `cdk-opinionated-constructs-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/alb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,49 @@
 # -*- coding: utf-8 -*-
 """Opinionated CDK construct to create Application load balancer with dedicated
 S3 bucket for storing access logs.
 
 Security parameters are set by default
 """
-from aws_cdk import aws_kms as kms
 from cdk_nag import NagSuppressions
 from cdk_opinionated_constructs.s3 import S3Bucket
 from constructs import Construct
 import aws_cdk as cdk
 import aws_cdk.aws_iam as iam
 import aws_cdk.aws_s3 as s3
 import aws_cdk.aws_elasticloadbalancingv2 as albv2
-import aws_cdk.aws_ec2 as ec2
+import aws_cdk.aws_certificatemanager as certificate_manager
 
 
 class ApplicationLoadBalancer(Construct):
     """Create Application LB."""
 
     # pylint: disable=W0235
     def __init__(self, scope: Construct, construct_id: str):
         """
 
         :param scope:
         :param construct_id:
         """
         super().__init__(scope, construct_id)
 
-    def create_access_logs_bucket(self, bucket_name: str, kms_key: kms.IKey, expiration_days: int) -> s3.Bucket:
+    def create_access_logs_bucket(self, bucket_name: str, expiration_days: int) -> s3.Bucket:
         """Create dedicated access logs bucket using opinionated cdk construct
         from cdk-opinionated-constructs.
 
         :param expiration_days: The number of days after which logs will be deleted
         :param bucket_name: The name of S3 bucket
-        :param kms_key: The kms key
         :return: CDK S3 IBucket object
         """
 
-        alb_access_logs_bucket_construct = S3Bucket(self, id=f"alb_access-logs-{bucket_name}-construct")
+        alb_access_logs_bucket_construct = S3Bucket(self, id=f"alb_access_logs_{bucket_name}_construct")
         alb_access_logs_bucket = alb_access_logs_bucket_construct.create_bucket(
-            bucket_name=bucket_name,
-            kms_key=kms_key,
+            bucket_name=bucket_name, encryption=s3.BucketEncryption.S3_MANAGED
         )
 
-        # The ALB access logging function don't work with KMS CMK which is used in the S3 bucket.
-        # To overcome this issue a supported bucket encryption was used - AES256
-        cfn_alb_access_logs_bucket = alb_access_logs_bucket.node.default_child
-        cfn_alb_access_logs_bucket.add_property_override(
-            "BucketEncryption.ServerSideEncryptionConfiguration.0.ServerSideEncryptionByDefault.SSEAlgorithm", "AES256"
-        )
-        cfn_alb_access_logs_bucket.add_property_deletion_override(
-            "BucketEncryption.ServerSideEncryptionConfiguration.0.ServerSideEncryptionByDefault.KMSMasterKeyID"
-        )
         alb_access_logs_bucket.add_to_resource_policy(
             permission=iam.PolicyStatement(
                 effect=iam.Effect.ALLOW,
                 actions=["s3:PutObject"],
                 principals=[iam.ServicePrincipal(service="delivery.logs.amazonaws.com")],
                 resources=[f"{alb_access_logs_bucket.bucket_arn}/*"],
                 conditions={"StringEquals": {"s3:x-amz-acl": "bucket-owner-full-control"}},
@@ -82,111 +70,57 @@
                     "it doesn't require another resource for storing access logs from it",
                 },
             ],
         )
 
         return alb_access_logs_bucket
 
-    def create_alb(
-        self, load_balancer_name: str, vpc: ec2.Vpc, internet_facing: bool = False
-    ) -> albv2.ApplicationLoadBalancer:
-        """Create AWS Application Load Balancer construct.
-
-        :param internet_facing: Set true to create public ALB
-        :param load_balancer_name: The load balancer name
-        :param vpc: CDK construct for VPC
-        :return: CDK construct for Application Load Balancer
-        """
-        return albv2.ApplicationLoadBalancer(
-            self,
-            id=f"{load_balancer_name}-load-balancer",
-            load_balancer_name=load_balancer_name,
-            vpc=vpc,
-            vpc_subnets=ec2.SubnetSelection(subnet_type=ec2.SubnetType.PUBLIC),
-            internet_facing=internet_facing,
-        )
-
     @staticmethod
-    def listeners(alb: albv2.ApplicationLoadBalancer, ports: list[dict]) -> list[dict]:
-        """Create ALB listeners using provided list of dicts.
-
-        Example input:
-        alb_ports = [
-            {
-                "port": "443/tcp",
-                "source": ["0.0.0.0/0"],
-                "protocol": albv2.Protocol.HTTPS,
-                "certificate": imported_acm_certificate,
-                "targets": [ec2_auto_scaling_group],
-            }
-        ]
-
-
-        Example usage:
-        alb_listeners = alb_construct.listeners(alb=alb, ports=alb_ports)
+    def add_connections(
+        alb: albv2.ApplicationLoadBalancer, certificates: list[certificate_manager.ICertificate], ports: list
+    ):
+        """Create ALB listener and target.
 
         :param alb: The CDK construct for Application Load Balancer
+        :param certificates: List of certificates from AWS Certificate Manager
         :param ports: List of dictionaries that contain connection details
-        :return: Updated list of dictionaries to which new key named lister was added
 
-        [
-            {
-                'port': '443/tcp',
-                'source': ['0.0.0.0/0'],
-                'protocol': <Protocol.TLS: 'TLS'>,
-                'certificate': <jsii._reference_map.InterfaceDynamicProxy object at 0x12012bfa0>,
-                "targets": [ec2_auto_scaling_group],
-                'listener': <aws_cdk.aws_elasticloadbalancingv2.ApplicationListener object at 0x12018f130>
-            }
-        ]
+        Example usage:
+        add_connections(
+            alb=alb,
+            certificates=[imported_acm_certificate],
+            ports=[
+                {
+                    "back_end_port": 8088,
+                    "front_end_port": 443,
+                    "back_end_protocol": albv2.ApplicationProtocol.HTTPS,
+                    "targets": [service],
+                    "healthy_http_codes": "200,302",
+                    "deregistration_delay": cdk.Duration.minutes(1)
+                }
+            ]
+        )
         """
         for port_definition in ports:
-            port_number = port_definition["port"]
-            port_number = int(port_number.split("/")[0])
-            protocol = port_definition["protocol"]
-            certificate = port_definition["certificate"]
+            front_end_port_number = port_definition["front_end_port"]
+
             listener = alb.add_listener(
-                certificates=[certificate],
-                id=f"{protocol}-{port_number}-listener",
-                port=port_number,
-                protocol=protocol,
+                certificates=certificates,
+                id=f"https_{front_end_port_number}_listener",
+                port=front_end_port_number,
+                protocol=albv2.ApplicationProtocol.HTTPS,
                 ssl_policy=albv2.SslPolicy.FORWARD_SECRECY_TLS12_RES_GCM,
-                open=True,
+                open=False,
             )
-            port_definition["listener"] = listener
-
-        return ports
 
-    @staticmethod
-    def targets(alb_listeners: list[dict]):
-        """
-        Create ALB targets
-        Example input for alb_listeners:
-
-        [
-            {
-                'port': '443/tcp',
-                'source': ['0.0.0.0/0'],
-                'protocol': <Protocol.TLS: 'TLS'>,
-                'certificate': <jsii._reference_map.InterfaceDynamicProxy object at 0x12012bfa0>,
-                "targets": [ec2_auto_scaling_group],
-                "healthy_http_codes": "200,302"
-                'listener': <aws_cdk.aws_elasticloadbalancingv2.ApplicationListener object at 0x12018f130>
-             }
-         ]
-        :param alb_listeners: list of dict that contain port definitions
-        """
-        for port_definition in alb_listeners:
-            port_number = port_definition["port"]
-            port_number = int(port_number.split("/")[0])
-            protocol = port_definition["protocol"]
-            alb_listener = port_definition["listener"]
-            alb_listener.add_targets(
-                id=f"{protocol}-{port_number}-target",
+            back_end_port = port_definition["back_end_port"]
+            listener.add_targets(
+                id=f"{back_end_port}_target",
+                deregistration_delay=port_definition.get("deregistration_delay"),
                 health_check=albv2.HealthCheck(
                     enabled=True,
                     healthy_http_codes=port_definition.get("healthy_http_codes"),
                 ),
-                port=port_number,
-                protocol=protocol,
+                port=back_end_port,
+                protocol=port_definition["back_end_protocol"],
                 targets=port_definition["targets"],
             )
```

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/s3.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Security parameters are set by default
 """
 from constructs import Construct
 import aws_cdk as cdk
 import aws_cdk.aws_s3 as s3
 from aws_cdk import aws_kms as kms
 
-from typing import Union
+from typing import Optional
 
 
 class S3Bucket(Construct):
     """Create opinionated S3 bucket including restricted public access,
     enforced encryption in transit as well as in rest, versioning and lifecycle
     rules."""
 
@@ -25,21 +25,23 @@
         :param id:
         """
         super().__init__(scope, id)
 
     def create_bucket(
         self,
         bucket_name: str,
-        kms_key: kms.IKey,
-        server_access_logs_bucket: Union[None, s3.IBucket] = None,
+        encryption: s3.BucketEncryption,
+        kms_key: Optional[kms.IKey] = None,
+        server_access_logs_bucket: Optional[s3.IBucket] = None,
         enforce_ssl: bool = True,
         **kwargs,
     ) -> s3.Bucket:
         """Create S3 bucket.
 
+        :param encryption: The type of encryption.
         :param kms_key: The kms to be used.
         :param bucket_name: The name of S3 bucket.
         :param enforce_ssl: Bool value if SSL should be enforced.
         :param server_access_logs_bucket: The CDK object for S3 bucket.
         :param kwargs:
          event_bridge_enabled: bool - set to True if s3 events should be sent to event bridge
          server_access_logs_prefix: str - in which prefix logs should be stored
@@ -47,23 +49,29 @@
         """
 
         return s3.Bucket(
             self,
             id=bucket_name,
             auto_delete_objects=True,
             block_public_access=s3.BlockPublicAccess(
-                block_public_acls=True, block_public_policy=True, ignore_public_acls=True, restrict_public_buckets=True
+                block_public_acls=True,
+                block_public_policy=True,
+                ignore_public_acls=True,
+                restrict_public_buckets=True,
             ),
             bucket_name=bucket_name,
-            encryption=s3.BucketEncryption.KMS,
+            encryption=encryption,
             encryption_key=kms_key,
             enforce_ssl=enforce_ssl,
-            event_bridge_enabled=True if kwargs.get("event_bridge_enabled") else False,
+            event_bridge_enabled=bool(kwargs.get("event_bridge_enabled")),
             lifecycle_rules=[
-                s3.LifecycleRule(enabled=True, noncurrent_version_expiration=cdk.Duration.days(amount=1)),
+                s3.LifecycleRule(
+                    enabled=True,
+                    noncurrent_version_expiration=cdk.Duration.days(amount=1),
+                ),
                 s3.LifecycleRule(
                     enabled=True,
                     expired_object_delete_marker=True,
                     abort_incomplete_multipart_upload_after=cdk.Duration.days(7),
                 ),
             ],
             public_read_access=False,
```

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs/wafv2.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,35 +228,30 @@
 
         :param resource_arn: The ARN of resource that will be protected by WAF
         :param web_acl_arn: The WEB Application Access Control List ARN
         :return: wafv2.CfnWebACLAssociation
         """
         return wafv2.CfnWebACLAssociation(self, "ACLAssociation", resource_arn=resource_arn, web_acl_arn=web_acl_arn)
 
-    def web_acl_log(self, log_group_name: str) -> logs.LogGroup:
-        """Create CloudWatch log group and associate it with WAF.
+    def web_acl_log(self, web_acl_arn: str, log_group_name: str) -> wafv2.CfnLoggingConfiguration:
+        """Configure provided log group as a target for WAF log destination.
 
+        :param web_acl_arn: The WEB Application Access Control List ARN
         :param log_group_name: The name of log group
-        :return: CDK CloudWatch logs.LogGroup
+        :return: AWS CDK wafv2.CfnLoggingConfiguration
         """
-        return logs.LogGroup(
+
+        log_group = logs.LogGroup(
             self,
             id="web_acl_log_group",
             log_group_name=log_group_name,
             retention=logs.RetentionDays.ONE_WEEK,
             removal_policy=cdk.RemovalPolicy.DESTROY,
         )
 
-    def web_acl_log_config(self, web_acl_arn: str, log_group: logs.LogGroup) -> wafv2.CfnLoggingConfiguration:
-        """Configure provided log group as a target for WAF log destination.
-
-        :param web_acl_arn: The WEB Application Access Control List ARN
-        :param log_group: The CDK construct of a CloudWatch log group
-        :return: AWS CDK wafv2.CfnLoggingConfiguration
-        """
         return wafv2.CfnLoggingConfiguration(
             self,
             id="web_acl_cfn_log_configuration",
             log_destination_configs=[
                 cdk.Stack.of(self).format_arn(
                     arn_format=cdk.ArnFormat.COLON_RESOURCE_NAME,
                     service="logs",
```

### Comparing `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.0.0/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 README.md
 setup.cfg
 setup.py
 ./cdk_opinionated_constructs/__init__.py
 ./cdk_opinionated_constructs/alb.py
 ./cdk_opinionated_constructs/ecr.py
 ./cdk_opinionated_constructs/lmb.py
+./cdk_opinionated_constructs/nlb.py
+./cdk_opinionated_constructs/rds_instance.py
 ./cdk_opinionated_constructs/s3.py
 ./cdk_opinionated_constructs/sns.py
 ./cdk_opinionated_constructs/wafv2.py
 ./test/__init__.py
 ./test/app.py
 ./test/stacks/__init__.py
 ./test/stacks/alb_stack.py
 ./test/stacks/ecr_stack.py
+./test/stacks/lmb_docker_stack.py
+./test/stacks/lmb_monitoring_stack.py
 ./test/stacks/lmb_stack.py
+./test/stacks/nlb_stack.py
+./test/stacks/rds_mysql_stack.py
+./test/stacks/rds_postgresql_stack.py
 ./test/stacks/s3_stack.py
 ./test/stacks/sns_stack.py
 ./test/stacks/wafv2_stack.py
 ./test/unit/__init__.py
 ./test/unit/test_alb_stack.py
 ./test/unit/test_ecr_stack.py
 ./test/unit/test_lmb_stack.py
```

### Comparing `cdk-opinionated-constructs-1.9.1/setup.cfg` & `cdk-opinionated-constructs-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/setup.py` & `cdk-opinionated-constructs-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="1.9.1",
+    version="2.0.0",
     description="AWS CDK constructs come without added security configurations.",
-    long_description="Very rarely this is validated during the CI pipeline via tools like CDK-NAG. The idea behind this project is to create secured constructs from the start.",
+    long_description="The idea behind this project is to create secured constructs from the start. \n"
+    "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
-        "aws-cdk-lib>=2.51.1",
-        "constructs>=10.0.0,<11.0.0",
+        "aws-cdk-lib>=2.69.0",
+        "constructs>=10.1.232,<11.0.0",
+        "cdk-monitoring-constructs>=3.0.0,<5.0.0",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/app.py` & `cdk-opinionated-constructs-2.0.0/test/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,46 @@
 """Main app."""
 
 import aws_cdk as cdk
 import os
 from stacks.s3_stack import TestS3Stack
 from stacks.sns_stack import TestSNSStack
 from stacks.lmb_stack import TestAWSPythonLambdaFunctionStack
+from stacks.lmb_monitoring_stack import TestAWSPythonLambdaFunctionStackMonitoring
 from stacks.wafv2_stack import TestWAFv2Stack
 from stacks.alb_stack import TestALBStack
 from stacks.ecr_stack import TestECRStack
-
+from stacks.nlb_stack import TestNLBStack
+from stacks.rds_postgresql_stack import TestRDSPostgreSQLStack
+from stacks.rds_mysql_stack import TestRDSMySQLStack
 
 CDK_ENV = cdk.Environment(account=os.environ["CDK_DEFAULT_ACCOUNT"], region=os.environ["CDK_DEFAULT_REGION"])
 
 app = cdk.App()
 TestS3Stack(app, "TestS3Stack")
 TestSNSStack(app, "TestSNSStack")
-TestAWSPythonLambdaFunctionStack(
+TestLambdaStack = TestAWSPythonLambdaFunctionStack(
     app,
     "TestAWSLambdaFunctionStack",
     env=CDK_ENV,
     props={"project": "test_project", "service_name": "example_lambda_function"},
 )
+TestLambdaMonitoringStack = TestAWSPythonLambdaFunctionStackMonitoring(
+    app,
+    "TestAWSLambdaFunctionMonitoringStack",
+    env=CDK_ENV,
+    props=TestLambdaStack.output_props,
+)
+TestAWSPythonLambdaFunctionStack = TestAWSPythonLambdaFunctionStack(
+    app,
+    "TestAWSLambdaDockerFunctionStack",
+    env=CDK_ENV,
+    props={"project": "test_project", "service_name": "example_lambda_function"},
+)
 TestWAFv2Stack(app, "TestWAFv2Stack", env=CDK_ENV)
 TestALBStack(app, "TestALBStack", env=CDK_ENV)
 TestECRStack(app, "TestECRStack", env=CDK_ENV)
+TestNLBStack(app, "TestNLBStack", env=CDK_ENV)
+TestRDSPostgreSQLStack(app, "TestRDSPostgreSQLStack", env=CDK_ENV)
+TestRDSMySQLStack(app, "TestRDSMySQLStack", env=CDK_ENV)
 
 app.synth()
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/alb_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 # -*- coding: utf-8 -*-
 """Example code for Application Load Balancer cdk stack."""
-from aws_cdk import Stack
+from aws_cdk import Stack, Duration
 from constructs import Construct
 
-from aws_cdk import aws_kms as kms
 import aws_cdk.aws_ec2 as ec2
+import aws_cdk.aws_certificatemanager as certificate_manager
+import aws_cdk.aws_elasticloadbalancingv2 as albv2
 from cdk_opinionated_constructs.alb import ApplicationLoadBalancer
 
 from cdk_nag import NagSuppressions
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks
 
 
 class TestALBStack(Stack):
     """Test generated EC2 ALB against AWS recommendations."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         vpc = ec2.Vpc(self, id="vpc")
-        shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
+        certificate = certificate_manager.Certificate(self, "certificate", domain_name="example.com")
 
         NagSuppressions.add_resource_suppressions(
             vpc,
             suppressions=[
                 {
                     "id": "AwsSolutions-VPC7",
                     "reason": "Test VPC, flow logs logs aren't required here.",
                 },
             ],
         )
 
         alb_construct = ApplicationLoadBalancer(self, construct_id="alb_construct")
 
-        alb = alb_construct.create_alb(
-            load_balancer_name="alb",
+        alb_name = "alb"
+        alb = albv2.ApplicationLoadBalancer(
+            self,
+            id=f"{alb_name}_load_balancer",
             internet_facing=True,
+            load_balancer_name=alb_name,
             vpc=vpc,
+            vpc_subnets=ec2.SubnetSelection(subnet_type=ec2.SubnetType.PUBLIC),
         )
 
-        alb_access_logs_bucket = alb_construct.create_access_logs_bucket(
-            bucket_name="bucket-name", kms_key=shared_kms_key, expiration_days=7
-        )
+        alb_access_logs_bucket = alb_construct.create_access_logs_bucket(bucket_name="bucket-name", expiration_days=7)
 
         alb.log_access_logs(bucket=alb_access_logs_bucket)
 
+        alb_construct.add_connections(
+            alb=alb,
+            certificates=[certificate],
+            ports=[
+                {
+                    "back_end_port": 8088,
+                    "front_end_port": 443,
+                    "back_end_protocol": albv2.ApplicationProtocol.HTTP,
+                    "targets": [],
+                    "healthy_http_codes": "200,302",
+                    "deregistration_delay": Duration.minutes(1),
+                }
+            ],
+        )
+
         # Validate stack against AWS Solutions checklist
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/lmb_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Test AWS Lambda function construct against cdk-nag."""
+"""Test AWS Lambda function construct."""
 from aws_cdk import Stack
 from constructs import Construct
 from cdk_opinionated_constructs.lmb import AWSPythonLambdaFunction
 import aws_cdk.aws_lambda as lmb
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
@@ -12,34 +12,38 @@
 class TestAWSPythonLambdaFunctionStack(Stack):
     """Test generated sns topic against AWS solutions  checks."""
 
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
 
         lmb_construct = AWSPythonLambdaFunction(self, id="lmb_construct")
-        lmb_signing_profile = lmb_construct.signing_profile(signing_profile_name="signing_profile_name")
-        lmb_signing = lmb_construct.signing_config(lmb_signing_profile)
-        lmb_construct.create_lambda_function(
+        lmb_signing = lmb_construct.signing_config(signing_profile_name="signing_profile_name")
+        lmb_function = lmb_construct.create_lambda_function(
             code_path=f'{props["service_name"]}',
             env=env,
             function_name=props["service_name"],
-            timeout=6,
-            layer=lmb.LayerVersion.from_layer_version_arn(
-                self,
-                id="aws_lambda_powertools_layer",
-                layer_version_arn="arn:aws:lambda:eu-west-1:123456789012:layer:aws-lambda-powertools-python-layer:1",
-            ),
+            timeout=10,
+            layers=[
+                lmb.LayerVersion.from_layer_version_arn(
+                    self,
+                    id="aws_lambda_powertools_layer",
+                    layer_version_arn="arn:aws:lambda:eu-west-1:123456789012:layer:aws-lambda-powertools-python-layer:1",
+                )
+            ],
             env_variables={
                 "POWERTOOLS_SERVICE_NAME": props["service_name"],
                 "LOG_LEVEL": "DEBUG",
             },
             reserved_concurrent_executions=1,
             signing_config=lmb_signing,
         )
 
+        self.output_props = props.copy()
+        self.output_props["lmb_function"] = lmb_function
+
         # Validate stack against AWS Solutions checklist
         nag_suppression_rule_list = self.nag_suppression()
         NagSuppressions.add_stack_suppressions(self, nag_suppression_rule_list)
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
 
     @staticmethod
     def nag_suppression() -> list:
@@ -54,7 +58,15 @@
             },
             {
                 "id": "AwsSolutions-IAM5",
                 "reason": "There isn't a way to tailor IAM policy using more restrictive permissions for "
                 "used API calls logs:CreateLogGroup, xray:PutTelemetryRecords, xray:PutTraceSegments",
             },
         ]
+
+    @property
+    def outputs(self):
+        """Update props dictionary.
+
+        :return: Updated props dict
+        """
+        return self.output_props
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/s3_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 """Test S3 construct against cdk-nag."""
 from aws_cdk import Stack
 from constructs import Construct
 from cdk_opinionated_constructs.s3 import S3Bucket
 import aws_cdk.aws_kms as kms
+import aws_cdk.aws_s3 as s3
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestS3Stack(Stack):
     """Test generated s3 bucket against AWS solutions  checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
 
         s3_bucket_construct = S3Bucket(self, id="bucket")
-        access_logs_bucket = s3_bucket_construct.create_bucket(bucket_name="access-logs-bucket", kms_key=shared_kms_key)
+        access_logs_bucket = s3_bucket_construct.create_bucket(
+            bucket_name="access-logs-bucket", encryption=s3.BucketEncryption.S3_MANAGED
+        )
 
         NagSuppressions.add_resource_suppressions(
             access_logs_bucket,
             [
                 {
                     "id": "AwsSolutions-S1",
                     "reason": "This is the access logs bucket, "
@@ -29,13 +32,14 @@
                 },
             ],
         )
 
         s3_bucket_construct.create_bucket(
             bucket_name="test-s3-bucket",
             kms_key=shared_kms_key,
+            encryption=s3.BucketEncryption.KMS,
             server_access_logs_bucket=access_logs_bucket,
             server_access_logs_prefix="test-s3-bucket",
         )
 
         # Validate stack against AWS Solutions checklist
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.0.0/test/stacks/wafv2_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # -*- coding: utf-8 -*-
 """Test AWS WAFv2 construct against cdk-nag."""
 from aws_cdk import Stack
 from constructs import Construct
 import aws_cdk.aws_ec2 as ec2
-from aws_cdk import aws_kms as kms
+import aws_cdk.aws_elasticloadbalancingv2 as albv2
 from cdk_opinionated_constructs.alb import ApplicationLoadBalancer
 from cdk_opinionated_constructs.wafv2 import WAFv2
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestWAFv2Stack(Stack):
     """Test generated sns topic against AWS solutions  checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         vpc = ec2.Vpc(self, id="vpc")
-        shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
 
         NagSuppressions.add_resource_suppressions(
             vpc,
             suppressions=[
                 {
                     "id": "AwsSolutions-VPC7",
                     "reason": "Test VPC, flow logs logs aren't required here.",
                 },
             ],
         )
 
         alb_construct = ApplicationLoadBalancer(self, construct_id="alb_construct")
 
-        alb = alb_construct.create_alb(
-            load_balancer_name="alb",
+        alb_name = "alb"
+        alb = albv2.ApplicationLoadBalancer(
+            self,
+            id=f"{alb_name}_load_balancer",
             internet_facing=True,
+            load_balancer_name=alb_name,
             vpc=vpc,
+            vpc_subnets=ec2.SubnetSelection(subnet_type=ec2.SubnetType.PUBLIC),
         )
 
-        alb_access_logs_bucket = alb_construct.create_access_logs_bucket(
-            bucket_name="bucket-name", kms_key=shared_kms_key, expiration_days=7
-        )
+        alb_access_logs_bucket = alb_construct.create_access_logs_bucket(bucket_name="bucket-name", expiration_days=7)
 
         alb.log_access_logs(bucket=alb_access_logs_bucket)
 
         wafv2_construct = WAFv2(self, construct_id="wafv2_construct")
 
         wafv2_acl = wafv2_construct.web_acl(
             name="wafv2",
@@ -58,14 +59,14 @@
             aws_account_takeover_prevention={
                 "login_path": "/portal/login",
                 "payload_type": "FORM_ENCODED",
                 "password_field": "data[AuthUser][password]",
                 "username_field": "data[AuthUser][userId]",
             },
         )
-        wafv2_construct.web_acl_association(resource_arn=alb.load_balancer_arn, web_acl_arn=wafv2_acl.attr_arn)
-        wafv2_log_group = wafv2_construct.web_acl_log(log_group_name="aws-waf-logs-wafv2")
 
-        wafv2_construct.web_acl_log_config(log_group=wafv2_log_group, web_acl_arn=wafv2_acl.attr_arn)
+        wafv2_construct.web_acl_log(log_group_name="aws-waf-logs-wafv2", web_acl_arn=wafv2_acl.attr_arn)
+
+        wafv2_construct.web_acl_association(resource_arn=alb.load_balancer_arn, web_acl_arn=wafv2_acl.attr_arn)
 
         # Validate stack against AWS Solutions checklist
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.1/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.0.0/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

