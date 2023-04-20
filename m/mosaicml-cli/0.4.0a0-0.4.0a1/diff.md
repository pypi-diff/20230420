# Comparing `tmp/mosaicml-cli-0.4.0a0.tar.gz` & `tmp/mosaicml-cli-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a0.tar", last modified: Thu Apr 20 19:46:05 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a1.tar", last modified: Thu Apr 20 21:11:00 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a0.tar` & `mosaicml-cli-0.4.0a1.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.410730 mosaicml-cli-0.4.0a0/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 19:46:05.410519 mosaicml-cli-0.4.0a0/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.374460 mosaicml-cli-0.4.0a0/mcli/
--rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.375153 mosaicml-cli-0.4.0a0/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.375745 mosaicml-cli-0.4.0a0/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.376198 mosaicml-cli-0.4.0a0/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.377756 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3292 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.378349 mosaicml-cli-0.4.0a0/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.379230 mosaicml-cli-0.4.0a0/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.381329 mosaicml-cli-0.4.0a0/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)     1102 2023-04-18 18:36:19.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.381752 mosaicml-cli-0.4.0a0/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.382758 mosaicml-cli-0.4.0a0/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.383225 mosaicml-cli-0.4.0a0/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.383609 mosaicml-cli-0.4.0a0/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.384207 mosaicml-cli-0.4.0a0/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.384554 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.385223 mosaicml-cli-0.4.0a0/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.385812 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.386122 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.387457 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     9943 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.389733 mosaicml-cli-0.4.0a0/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.390336 mosaicml-cli-0.4.0a0/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init.py
--rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.391421 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 anna       (501) staff       (20)     9464 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.391803 mosaicml-cli-0.4.0a0/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.392216 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.392797 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.393144 mosaicml-cli-0.4.0a0/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.393457 mosaicml-cli-0.4.0a0/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     7550 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.394765 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.395095 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.395803 mosaicml-cli-0.4.0a0/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.397771 mosaicml-cli-0.4.0a0/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)     8426 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.398121 mosaicml-cli-0.4.0a0/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.400065 mosaicml-cli-0.4.0a0/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.401914 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.402373 mosaicml-cli-0.4.0a0/mcli/proto/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a0/mcli/proto/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-20 00:22:55.000000 mosaicml-cli-0.4.0a0/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.402910 mosaicml-cli-0.4.0a0/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)     1045 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.407472 mosaicml-cli-0.4.0a0/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-20 00:22:47.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.408944 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     4609 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-20 19:46:05.410824 mosaicml-cli-0.4.0a0/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.410108 mosaicml-cli-0.4.0a0/tests/
--rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/tests/test_upgrade.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.250504 mosaicml-cli-0.4.0a1/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 21:11:00.250344 mosaicml-cli-0.4.0a1/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/README.md
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.216455 mosaicml-cli-0.4.0a1/mcli/
+-rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.217087 mosaicml-cli-0.4.0a1/mcli/api/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.217780 mosaicml-cli-0.4.0a1/mcli/api/cluster/
+-rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/cluster/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.218250 mosaicml-cli-0.4.0a1/mcli/api/engine/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/engine/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/engine/engine.py
+-rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/exceptions.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.220217 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/
+-rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     3292 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.221087 mosaicml-cli-0.4.0a1/mcli/api/mint/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/shell.py
+-rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/mint/tty.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.222173 mosaicml-cli-0.4.0a1/mcli/api/model/
+-rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/cluster_details.py
+-rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-20 21:07:59.000000 mosaicml-cli-0.4.0a1/mcli/api/model/run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.224495 mosaicml-cli-0.4.0a1/mcli/api/runs/
+-rw-r--r--   0 anna       (501) staff       (20)     1102 2023-04-18 18:36:19.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.224865 mosaicml-cli-0.4.0a1/mcli/api/schema/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/schema/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.225722 mosaicml-cli-0.4.0a1/mcli/api/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/typing_future.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226128 mosaicml-cli-0.4.0a1/mcli/api/users/
+-rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/users/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226429 mosaicml-cli-0.4.0a1/mcli/cli/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/__init__.py
+-rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/cli.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.226881 mosaicml-cli-0.4.0a1/mcli/cli/common/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.227161 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.227571 mosaicml-cli-0.4.0a1/mcli/cli/m_create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.228254 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.228729 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.229832 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)    10343 2023-04-20 21:08:39.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.231613 mosaicml-cli-0.4.0a1/mcli/cli/m_get/
+-rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/display.py
+-rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_get/users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.232186 mosaicml-cli-0.4.0a1/mcli/cli/m_init/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.233281 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-20 21:09:05.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.233786 mosaicml-cli-0.4.0a1/mcli/cli/m_log/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.234169 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.234709 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.235078 mosaicml-cli-0.4.0a1/mcli/cli/m_root/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.235481 mosaicml-cli-0.4.0a1/mcli/cli/m_run/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     7550 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.236737 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.237046 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.237541 mosaicml-cli-0.4.0a1/mcli/cli/m_util/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/cli/m_util/util.py
+-rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.239123 mosaicml-cli-0.4.0a1/mcli/models/
+-rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/gpu_type.py
+-rw-r--r--   0 anna       (501) staff       (20)     8426 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_cluster.py
+-rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_envvar.py
+-rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/mcli_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/models/run_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.239477 mosaicml-cli-0.4.0a1/mcli/objects/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.241265 mosaicml-cli-0.4.0a1/mcli/objects/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.242677 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.243023 mosaicml-cli-0.4.0a1/mcli/proto/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a1/mcli/proto/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-20 00:22:55.000000 mosaicml-cli-0.4.0a1/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.243365 mosaicml-cli-0.4.0a1/mcli/sdk/
+-rw-r--r--   0 anna       (501) staff       (20)     1045 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/sdk/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.247716 mosaicml-cli-0.4.0a1/mcli/utils/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_cli.py
+-rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_date.py
+-rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-20 00:22:47.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_docker.py
+-rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_epilog.py
+-rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_logging.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_pypi.py
+-rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_rich.py
+-rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_run_status.py
+-rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_spinner.py
+-rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_types.py
+-rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/mcli/utils/utils_yaml.py
+-rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-20 21:10:31.000000 mosaicml-cli-0.4.0a1/mcli/version.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.248966 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     4609 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-20 21:11:00.000000 mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a1/pyproject.toml
+-rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-20 21:11:00.250547 mosaicml-cli-0.4.0a1/setup.cfg
+-rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/setup.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 21:11:00.250029 mosaicml-cli-0.4.0a1/tests/
+-rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-20 21:04:06.000000 mosaicml-cli-0.4.0a1/tests/test_config.py
+-rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/tests/test_simple.py
+-rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a1/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a0/PKG-INFO` & `mosaicml-cli-0.4.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a0
+Version: 0.4.0a1
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a0/README.md` & `mosaicml-cli-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a1/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a1/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a1/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a1/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a1/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a1/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a1/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a1/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a1/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a1/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a1/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a1/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a1/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a1/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a1/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a1/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a1/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/describe_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,57 +26,67 @@
     RUNNING = 'RUNNING'
     COMPLETED = 'COMPLETED'
 
 
 class DescribeRunDetailColumns(Enum):
     NAME = 'name'
     RUN_ID = 'run_uid'
-    IMAGE = 'image'
     LAST_ATTEMPT_ID = 'last_attempt_id'
+    CLUSTER = 'cluster'
+    GPU_TYPE = 'gpu_type'
+    GPU_NUM = 'gpu_num'
+    CPUS = 'cpus'
+    IMAGE = 'image'
     PRIORITY = 'priority'
 
 
 class DescribeRunLifecycleColumns(Enum):
     STATUS = 'status'
     START_TIME = 'start_time'
     END_TIME = 'end_time'
     DURATION = 'duration'
 
 
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
-RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Image', 'Last Attempt ID', 'Priority']
+RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Attempt ID', 'Cluster', 'Image', 'GPU Type', 'GPU Num']
 
 RUN_LIFECYCLE_DISPLAY_NAMES = [
     'Start Time',
     'End Time',
     'Duration',
 ]
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
 class DescribeRunDetailDisplayItem(MCLIDisplayItem):
     """Tuple that extracts detailed run data for display purposes"""
     name: str
+    run_uid: str
+    last_attempt_id: str
+    cluster: str
     image: str
     last_attempt_id: str
     priority: str
 
     @classmethod
     def from_run(cls, run: Run) -> DescribeRunDetailDisplayItem:
         priority = run.config.scheduling.get('priority', None) or DEFAULT_PRIORITY_NAME
         if priority and priority.lower() == 'default':
             priority = DEFAULT_PRIORITY_NAME
 
         extracted: Dict[str, Any] = {
             DescribeRunDetailColumns.NAME.value: run.config.name,
+            DescribeRunDetailColumns.RUN_ID.value: run.run_uid,
+            DescribeRunDetailColumns.LAST_ATTEMPT_ID.value: run.last_attempt_id,
+            DescribeRunDetailColumns.CLUSTER.value: run.config.cluster,
             DescribeRunDetailColumns.IMAGE.value: run.config.image,
             DescribeRunDetailColumns.LAST_ATTEMPT_ID.value: run.last_attempt_id,
             DescribeRunDetailColumns.PRIORITY.value: priority.lower(),
         }
 
         return DescribeRunDetailDisplayItem(**extracted)
```

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_interactive/m_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shlex
 import subprocess
 from typing import Optional
 
 from mcli.api.exceptions import cli_error_handler
 from mcli.cli.m_interactive import kube_config
 from mcli.config import MCLIConfig
-from mcli.sdk import RunConfig, RunStatus, create_run, get_clusters, get_runs, wait_for_run_status
+from mcli.sdk import RunConfig, RunStatus, create_run, get_clusters, get_run, wait_for_run_status
 from mcli.utils.utils_interactive import simple_prompt
 from mcli.utils.utils_logging import FAIL, INFO, OK, WARN
 from mcli.utils.utils_types import get_hours_type
 
 logger = logging.getLogger(__name__)
 
 
@@ -70,18 +70,15 @@
         elif len(clusters) == 1:
             cluster = clusters[0].name
         else:
             raise RuntimeError('Multiple clusters available. Please use the --cluster argument to set the '
                                'cluster to use for interactive')
 
     if reconnect:
-        all_runs = get_runs([reconnect])
-        if not all_runs:
-            raise RuntimeError(f'Could not find an interactive session named {reconnect}')
-        run = all_runs[0]
+        run = get_run(reconnect)
         logger.info(f'{INFO} Attempting to reconnect to session: [cyan]{run.name}[/]')
     else:
         if cpus and cpus != 1:
             logger.info(f'{WARN} Specifying cpus not currently supported. Submitting interactive run with {gpus} gpus')
 
         config = RunConfig(
             name=name or f'interactive-{(gpu_type or "none").replace("_", "-")}-{gpus or 0}'.lower(),
@@ -116,15 +113,15 @@
 
         namespace = simple_prompt(
             f'Which kube namespace should be used to connect to the interactive run? [{default_namespace}]',
             default=default_namespace,
             mandatory=False,
         )
 
-        pod_id = f"{run.run_uid}-{rank}"
+        pod_id = f"{run.last_attempt_id}-{rank}"
         logger.info(f'{INFO} Waiting for session to start with pod [blue]{pod_id}[/]...')
         logger.info(f'{INFO} Press Ctrl+C to quit and interact with your session manually.')
         run = wait_for_run_status(run, status=RunStatus.RUNNING, timeout=300)
 
         rank_str = f"node rank [cyan]{rank}[/] of " if rank > 0 else ""
         logger.info(f'{OK} Connecting to {rank_str}interactive session [cyan]{run.name}[/]')
```

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a1/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/config.py` & `mosaicml-cli-0.4.0a1/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a1/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a1/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a1/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a1/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a1/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a1/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a1/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a1/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a1/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mcli/version.py` & `mosaicml-cli-0.4.0a1/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a0"
+__version__ = "0.4.0a1"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a0
+Version: 0.4.0a1
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a1/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 
 [all]
-sphinx-markdown-tables>=0.0.15
-sphinx-argparse>=0.3.1
+pytest-mock>=3.7.0
+pyright>=1.1.256
+sphinxcontrib-serializinghtml>=1.1.5
+yapf>=0.33.0
+pytest-cov>=4.0.0
+sphinx-panels>=0.6.0
+furo>=2022.3.4
+pylint>=2.12.2
+sphinxcontrib-devhelp>=1.0.2
+sphinxcontrib-katex>=0.8.6
+sphinx-copybutton>=0.5.0
+sphinx-design
 sphinx_external_toc>=0.3.0
-sphinxcontrib-qthelp>=1.0.3
+pytest>=6.2.5
+sphinx>=4.4.0
+sphinx-rtd-theme>=1.0.0
+myst-parser>=0.16.1
+sphinxext-opengraph>=0.6.1
+sphinx-argparse>=0.3.1
+isort>=5.9.3
+radon>=5.1.0
+pre-commit>=2.17.0
 sphinxcontrib-htmlhelp>=2.0.0
-pylint>=2.12.2
+sphinxcontrib-jsmath>=1.0.1
 sphinxcontrib-images>=0.9.4
-sphinx-copybutton>=0.5.0
 sphinxcontrib-applehelp>=1.0.2
-sphinx>=4.4.0
+sphinxcontrib-qthelp>=1.0.3
+sphinx-markdown-tables>=0.0.15
 sphinxemoji>=0.2.0
-sphinxext-opengraph>=0.6.1
-sphinxcontrib-devhelp>=1.0.2
 toml>=0.10.2
-sphinx-panels>=0.6.0
-pytest-cov>=4.0.0
-sphinxcontrib-jsmath>=1.0.1
-pytest-mock>=3.7.0
-sphinxcontrib-serializinghtml>=1.1.5
-myst-parser>=0.16.1
-sphinx-design
-furo>=2022.3.4
-sphinx-rtd-theme>=1.0.0
-pre-commit>=2.17.0
-radon>=5.1.0
-yapf>=0.33.0
-pyright>=1.1.256
-pytest>=6.2.5
-sphinxcontrib-katex>=0.8.6
-isort>=5.9.3
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest-cov>=4.0.0
```

### Comparing `mosaicml-cli-0.4.0a0/pyproject.toml` & `mosaicml-cli-0.4.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/setup.py` & `mosaicml-cli-0.4.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/tests/test_config.py` & `mosaicml-cli-0.4.0a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a0/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a1/tests/test_upgrade.py`

 * *Files identical despite different names*

