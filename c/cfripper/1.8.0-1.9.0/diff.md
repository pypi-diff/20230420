# Comparing `tmp/cfripper-1.8.0.tar.gz` & `tmp/cfripper-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cfripper-1.8.0.tar", last modified: Wed Apr  6 06:28:13 2022, max compression
+gzip compressed data, was "dist/cfripper-1.9.0.tar", last modified: Tue Apr 19 11:05:12 2022, max compression
```

## Comparing `cfripper-1.8.0.tar` & `cfripper-1.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-04-06 06:28:13.000000 cfripper-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-04-06 06:27:57.000000 cfripper-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    19650 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/cloudformation_actions_only_accepts_wildcard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6319 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/config/pluggy/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/pluggy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/pluggy/hookspec.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/pluggy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3035 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/rule_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/config/rule_configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/rule_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/rule_configs/allow_http_ports_open_to_world.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/rule_configs/example_rules_config_for_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/config/rule_configs/firehose_ips.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2696 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/model/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rule_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper/rules/
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/base_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/cloudformation_authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)    15842 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/cross_account_trust.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/ebs_volume_has_sse.py
--rw-r--r--   0 runner    (1001) docker     (121)    16316 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/ec2_security_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/hardcoded_RDS_password.py
--rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/iam_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/kms_key_rotation_enabled.py
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/kms_key_wildcard_principal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/managed_policy_on_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/policy_on_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/privilege_escalation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/s3_lifecycle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/s3_object_versioning.py
--rw-r--r--   0 runner    (1001) docker     (121)     7078 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/s3_public_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/sns_topic_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/sqs_queue_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/wildcard_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    16158 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/wildcard_principals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8500 2022-04-06 06:27:57.000000 cfripper-1.8.0/cfripper/rules/wildcard_resource_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-06 06:28:13.000000 cfripper-1.8.0/cfripper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-04-06 06:27:57.000000 cfripper-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-04-06 06:28:13.000000 cfripper-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-04-06 06:27:57.000000 cfripper-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:12.000000 cfripper-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-04-19 11:05:12.000000 cfripper-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-04-19 11:04:58.000000 cfripper-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19650 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/cloudformation_actions_only_accepts_wildcard.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8463 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6319 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper/config/pluggy/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/pluggy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/pluggy/hookspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/pluggy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/regex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/rule_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper/config/rule_configs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/rule_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/rule_configs/allow_http_ports_open_to_world.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/rule_configs/example_rules_config_for_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/config/rule_configs/firehose_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper/model/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2696 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rule_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:12.000000 cfripper-1.9.0/cfripper/rules/
+-rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/base_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/cloudformation_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15842 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/cross_account_trust.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/ebs_volume_has_sse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16316 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/ec2_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/hardcoded_RDS_password.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/iam_roles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/kms_key_rotation_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/kms_key_wildcard_principal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/managed_policy_on_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/policy_on_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/privilege_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/s3_lifecycle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/s3_object_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7078 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/s3_public_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/sns_topic_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/sqs_queue_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/wildcard_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16158 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/wildcard_principals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8500 2022-04-19 11:04:58.000000 cfripper-1.9.0/cfripper/rules/wildcard_resource_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-19 11:05:11.000000 cfripper-1.9.0/cfripper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-04-19 11:04:58.000000 cfripper-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-04-19 11:05:12.000000 cfripper-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-04-19 11:04:58.000000 cfripper-1.9.0/setup.py
```

### Comparing `cfripper-1.8.0/PKG-INFO` & `cfripper-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfripper
-Version: 1.8.0
+Version: 1.9.0
 Summary: Library and CLI tool for analysing CloudFormation templates and check them for security compliance.
 Home-page: https://github.com/Skyscanner/cfripper
 Author: Skyscanner Product Security
 Author-email: security@skyscanner.net
 License: UNKNOWN
 Description: <p align="center">
         <img src="docs/img/logo.png" width="200">
```

### Comparing `cfripper-1.8.0/README.md` & `cfripper-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/boto3_client.py` & `cfripper-1.9.0/cfripper/boto3_client.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/cli.py` & `cfripper-1.9.0/cfripper/cli.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/cloudformation_actions_only_accepts_wildcard.py` & `cfripper-1.9.0/cfripper/cloudformation_actions_only_accepts_wildcard.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/constants.py` & `cfripper-1.9.0/cfripper/config/constants.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/filter.py` & `cfripper-1.9.0/cfripper/config/filter.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/pluggy/utils.py` & `cfripper-1.9.0/cfripper/config/pluggy/utils.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/regex.py` & `cfripper-1.9.0/cfripper/config/regex.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,100 @@
 import re
 
 """
 Check for Principals where root is being used.
 Valid:
-- arn:aws:iam::437628376:root
-- arn:aws:iam::344345345:root
+- arn:aws:iam::123456789012:root
 - arn:aws:iam:::root
 Invalid:
-- arn:aws:iam::437628376:not-root
+- arn:aws:iam::123456789012:not-root
 - potato
 """
 REGEX_CROSS_ACCOUNT_ROOT = re.compile(r"arn:aws:iam::\d*:root")
 
 """
 Check for use of wildcard in two bad cases: full wildcard, or wildcard in account ID.
 Valid:
 - *
+- ?*
+- **
 - arn:aws:iam::*:12345
 Invalid:
-- arn:aws:iam::444455556666:root
+- arn:aws:iam::123456789012:root
 - potato
-- arn:aws:iam::12345:*
+- arn:aws:iam::123456789012:*
 """
-REGEX_FULL_WILDCARD_PRINCIPAL = re.compile(r"^((\w*:){0,1}\*|arn:aws:iam::\*:.*)$")
+REGEX_FULL_WILDCARD_PRINCIPAL = re.compile(r"^((\w*:)?[*?]+|arn:aws:iam::[*?]+:.*)$")
 
 """
 Check for use of wildcard or account-wide principals.
 Valid:
 - arn:aws:iam::123456789012:*
 - arn:aws:iam::123456789012:service-*
 - arn:aws:iam::123456789012:root
+- arn:aws:iam::123456789012:*-role
 - 123456789012
 Invalid:
 - *
 - potato
-- arn:aws:iam::123456789012:*not-root
+- arn:aws:iam::123456789012:not-root
 """
-REGEX_PARTIAL_WILDCARD_PRINCIPAL = re.compile(r"^\d{12}|arn:aws:iam::.*:(.*\*|root)$")
+REGEX_PARTIAL_WILDCARD_PRINCIPAL = re.compile(r"^(\d+)|(arn:aws:iam::(\d+):(.*[*?]+|[*?]+.*|root))$")
 
 """
 Check for use of wildcard, when applied to the specific elements of an Action.
 For example, sts:AssumeRole* or sts:*. This regex is not checking for use of `*` on its own.
 Valid:
 - sts:AssumeRole*
 - sts:*
+- sts:Assume????
+- sts:??????Role
+- sts:*Role*
 Invalid:
 - sts:AssumeRole
 - sts:AssumeRole-Thing-This
 - *
 """
-REGEX_WILDCARD_POLICY_ACTION = re.compile(r"^(\w*:)(\w*)\*(\w*)$")
+REGEX_WILDCARD_POLICY_ACTION = re.compile(r"^(\w*:)(.*)[*?]+(.*)$")
 
 """
-Check for Principals where root is being used.
+Check for Principals where a star is being used.
 Valid:
 - *
 - abc*def
 - abcdef*
 - *abcdef
 Invalid:
-- arn:aws:iam::437628376:not-root
+- arn:aws:iam::123456789012:not-root
 - potato
 """
 REGEX_CONTAINS_STAR = re.compile(r"^.*[*].*$")
 
 
 """
 Check for root wildcard
 Valid:
 - *
 Invalid:
 - abc*def
 - abcdef*
 - *abcdef
-- arn:aws:iam::437628376:not-root
+- arn:aws:iam::123456789012:not-root
 - potato
 """
 REGEX_IS_STAR = re.compile(r"^\*$")
 
 
 """
 Check for arns
 It has 4 groups. The first one for service name, the second one for region, the third, for account id, the last one
 for resource id
 Valid:
-- arn:aws:iam::437628376:not-root
-- arn:aws:iam::437628376:root
+- arn:aws:iam::123456789012:not-root
+- arn:aws:iam::123456789012:root
 - arn:aws:s3:::my_corporate_bucket
 Invalid:
 - potato
 """
 REGEX_ARN = re.compile(r"^arn:aws:(\w+):(\w*):(\d*):(.+)$")
 
 
@@ -98,50 +103,52 @@
 Valid:
 - arn:aws:s3:::*
 - arn:aws:iam:*:*:*
 - arn:aws:*:::*
 Invalid:
 - potato
 - arn:aws:s3:::my_corporate_bucket
-- arn:aws:iam::437628376:root
+- arn:aws:iam::123456789012:root
 """
-REGEX_WILDCARD_ARN = re.compile(r"^arn:aws:([*\w]+):(\*)?:(\*)?:([*?]+)$")
+REGEX_WILDCARD_ARN = re.compile(r"^arn:aws:([*\w]+):([*?]*):([*?]*):([*?]+)$")
 
 
 """
 Check for iam arns
 It has 2 groups. The first one for account id, the last one for resource id
 Valid:
-- arn:aws:iam::437628376:not-root
+- arn:aws:iam::123456789012:not-root
 Invalid:
 - arn:aws:s3:::my_corporate_bucket
 - potato
 """
-REGEX_IAM_ARN = re.compile(r"^arn:aws:iam::(\d*):(.*)$")
+REGEX_IAM_ARN = re.compile(r"^arn:aws:iam::(\d+):(.*)$")
 
 
 """
 Check for sts arns
 It has 2 groups. The first one for account id, the last one for resource id
 Valid:
-- arn:aws:sts::437628376:not-root
+- arn:aws:sts::123456789012:not-root
 Invalid:
 - arn:aws:s3:::my_corporate_bucket
 - potato
 """
-REGEX_STS_ARN = re.compile(r"^arn:aws:sts::(\d*):(.*)$")
+REGEX_STS_ARN = re.compile(r"^arn:aws:sts::(\d+):(.*)$")
 
 
 """
-Check for wildcards after colons
+Check for a wildcard star or wildcards immediately after the last colon
 Valid:
 - *
-- arn:aws:iam::437628376:*
+- arn:aws:iam::123456789012:*
+- arn:aws:iam::123456789012:??????
+- arn:aws:iam::123456789012:?*
 - sns:*
 Invalid:
 - arn:aws:s3:::my_corporate_bucket
 - arn:aws:s3:::my_corporate_bucket*
 - arn:aws:s3:::*my_corporate_bucket
 - potato
 - sns:Get*
 """
-REGEX_HAS_STAR_OR_STAR_AFTER_COLON = re.compile(r"^(\w*:)*\*$")
+REGEX_HAS_STAR_OR_STAR_AFTER_COLON = re.compile(r"^(\w*:)*[*?]+$")
```

### Comparing `cfripper-1.8.0/cfripper/config/rule_config.py` & `cfripper-1.9.0/cfripper/config/rule_config.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/rule_configs/allow_http_ports_open_to_world.py` & `cfripper-1.9.0/cfripper/config/rule_configs/allow_http_ports_open_to_world.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/rule_configs/example_rules_config_for_cli.py` & `cfripper-1.9.0/cfripper/config/rule_configs/example_rules_config_for_cli.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/config/rule_configs/firehose_ips.py` & `cfripper-1.9.0/cfripper/config/rule_configs/firehose_ips.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/model/result.py` & `cfripper-1.9.0/cfripper/model/result.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/model/utils.py` & `cfripper-1.9.0/cfripper/model/utils.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rule_processor.py` & `cfripper-1.9.0/cfripper/rule_processor.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/__init__.py` & `cfripper-1.9.0/cfripper/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/base_rules.py` & `cfripper-1.9.0/cfripper/rules/base_rules.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/cloudformation_authentication.py` & `cfripper-1.9.0/cfripper/rules/cloudformation_authentication.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/cross_account_trust.py` & `cfripper-1.9.0/cfripper/rules/cross_account_trust.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/ebs_volume_has_sse.py` & `cfripper-1.9.0/cfripper/rules/ebs_volume_has_sse.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/ec2_security_group.py` & `cfripper-1.9.0/cfripper/rules/ec2_security_group.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/hardcoded_RDS_password.py` & `cfripper-1.9.0/cfripper/rules/hardcoded_RDS_password.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/iam_roles.py` & `cfripper-1.9.0/cfripper/rules/iam_roles.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/kms_key_rotation_enabled.py` & `cfripper-1.9.0/cfripper/rules/kms_key_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/kms_key_wildcard_principal.py` & `cfripper-1.9.0/cfripper/rules/kms_key_wildcard_principal.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/managed_policy_on_user.py` & `cfripper-1.9.0/cfripper/rules/managed_policy_on_user.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/policy_on_user.py` & `cfripper-1.9.0/cfripper/rules/policy_on_user.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/privilege_escalation.py` & `cfripper-1.9.0/cfripper/rules/privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/s3_bucket_policy.py` & `cfripper-1.9.0/cfripper/rules/s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/s3_lifecycle_configuration.py` & `cfripper-1.9.0/cfripper/rules/s3_lifecycle_configuration.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/s3_object_versioning.py` & `cfripper-1.9.0/cfripper/rules/s3_object_versioning.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/s3_public_access.py` & `cfripper-1.9.0/cfripper/rules/s3_public_access.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/sns_topic_policy.py` & `cfripper-1.9.0/cfripper/rules/sns_topic_policy.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/sqs_queue_policy.py` & `cfripper-1.9.0/cfripper/rules/sqs_queue_policy.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/wildcard_policies.py` & `cfripper-1.9.0/cfripper/rules/wildcard_policies.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/wildcard_principals.py` & `cfripper-1.9.0/cfripper/rules/wildcard_principals.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper/rules/wildcard_resource_rule.py` & `cfripper-1.9.0/cfripper/rules/wildcard_resource_rule.py`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/cfripper.egg-info/PKG-INFO` & `cfripper-1.9.0/cfripper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfripper
-Version: 1.8.0
+Version: 1.9.0
 Summary: Library and CLI tool for analysing CloudFormation templates and check them for security compliance.
 Home-page: https://github.com/Skyscanner/cfripper
 Author: Skyscanner Product Security
 Author-email: security@skyscanner.net
 License: UNKNOWN
 Description: <p align="center">
         <img src="docs/img/logo.png" width="200">
```

### Comparing `cfripper-1.8.0/cfripper.egg-info/SOURCES.txt` & `cfripper-1.9.0/cfripper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfripper-1.8.0/setup.py` & `cfripper-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,45 @@
 dev_requires = [
     "black==22.3.0",
     "flake8>=3.3.0",
     "isort==4.3.21",
     "pytest>=3.6",
     "pytest-cov>=2.5.1",
     "pip-tools>=5.3.1",
-    "moto==1.3.14",
+    "moto[cloudformation,s3]>=3.0.0",
 ]
 
 docs_requires = [
-    "ansi2html==1.5.2",
-    "Markdown==3.2.2",
-    "markdown-include==0.5.1",
+    "click==8.1.2",
+    "csscompressor==0.9.5",
+    "ghp-import==2.0.2",
+    "htmlmin==0.1.12",
+    "importlib-metadata==4.11.3",
+    "Jinja2==3.1.1",
+    "jsmin==3.0.1",
+    "Markdown==3.3.6",
+    "MarkupSafe==2.1.1",
+    "mergedeep==1.3.4",
+    "mkdocs==1.3.0",
     "mkdocs-exclude==1.0.2",
-    "mkdocs-macros-plugin==0.4.9",
-    "mkdocs-material==5.5.12",
-    "mkdocs-material-extensions==1.0",
-    "mkdocs-minify-plugin==0.3.0",
-    "mkdocs==1.1.2",
-    "pygments==2.5.2",
+    "mkdocs-macros-plugin==0.7.0",
+    "mkdocs-material==8.2.8",
+    "mkdocs-material-extensions==1.0.3",
+    "mkdocs-minify-plugin==0.5.0",
+    "packaging==21.3",
+    "Pygments==2.11.2",
+    "pymdown-extensions==9.3",
+    "pyparsing==3.0.7",
+    "python-dateutil==2.8.2",
+    "PyYAML==6.0",
+    "pyyaml_env_tag==0.1",
+    "six==1.16.0",
+    "termcolor==1.1.0",
+    "watchdog==2.1.7",
+    "zipp==3.8.0",
 ]
 
 setup(
     name="cfripper",
     version=__version__,
     author="Skyscanner Product Security",
     author_email="security@skyscanner.net",
```

