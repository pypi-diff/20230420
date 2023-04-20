# Comparing `tmp/mosaicml-cli-0.3.9.tar.gz` & `tmp/mosaicml-cli-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.3.9.tar", last modified: Thu Apr 20 19:06:23 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a0.tar", last modified: Thu Apr 20 19:46:05 2023, max compression
```

## Comparing `mosaicml-cli-0.3.9.tar` & `mosaicml-cli-0.4.0a0.tar`

### file list

```diff
@@ -1,273 +1,191 @@
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.957165 mosaicml-cli-0.3.9/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-20 19:06:23.956825 mosaicml-cli-0.3.9/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     7799 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/README.md
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.824750 mosaicml-cli-0.3.9/mcli/
--rw-r--r--   0 wai        (502) staff       (20)       54 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.826116 mosaicml-cli-0.3.9/mcli/api/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.826844 mosaicml-cli-0.3.9/mcli/api/cluster/
--rw-r--r--   0 wai        (502) staff       (20)      134 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/cluster/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4141 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.827918 mosaicml-cli-0.3.9/mcli/api/engine/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/engine/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    26222 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/engine/engine.py
--rw-r--r--   0 wai        (502) staff       (20)      787 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/engine/utils.py
--rw-r--r--   0 wai        (502) staff       (20)    11677 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/exceptions.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.856766 mosaicml-cli-0.3.9/mcli/api/inference_deployments/
--rw-r--r--   0 wai        (502) staff       (20)      879 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3421 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     3292 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     6124 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     1044 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     1126 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.857132 mosaicml-cli-0.3.9/mcli/api/kube/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.858600 mosaicml-cli-0.3.9/mcli/api/kube/runs/
--rw-r--r--   0 wai        (502) staff       (20)      856 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4900 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_create_run.py
--rw-r--r--   0 wai        (502) staff       (20)     5042 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_delete_runs.py
--rw-r--r--   0 wai        (502) staff       (20)    14458 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_run_logs.py
--rw-r--r--   0 wai        (502) staff       (20)    16261 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     5981 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_stop_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     6210 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_watch_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.859645 mosaicml-cli-0.3.9/mcli/api/mint/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/api/mint/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6870 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/mint/shell.py
--rw-r--r--   0 wai        (502) staff       (20)     2216 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.9/mcli/api/mint/tty.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.860595 mosaicml-cli-0.3.9/mcli/api/model/
--rw-r--r--   0 wai        (502) staff       (20)      209 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6186 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/cluster_details.py
--rw-r--r--   0 wai        (502) staff       (20)     2987 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/model/inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     8057 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.862591 mosaicml-cli-0.3.9/mcli/api/runs/
--rw-r--r--   0 wai        (502) staff       (20)     1102 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/runs/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2750 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_create_run.py
--rw-r--r--   0 wai        (502) staff       (20)     3926 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     7971 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 wai        (502) staff       (20)    10440 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     5099 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     3937 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 wai        (502) staff       (20)    10619 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.863066 mosaicml-cli-0.3.9/mcli/api/schema/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/schema/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      636 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.864260 mosaicml-cli-0.3.9/mcli/api/secrets/
--rw-r--r--   0 wai        (502) staff       (20)      309 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/secrets/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2365 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     3697 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)      508 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/types.py
--rw-r--r--   0 wai        (502) staff       (20)     2354 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/typing_future.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.864854 mosaicml-cli-0.3.9/mcli/api/users/
--rw-r--r--   0 wai        (502) staff       (20)      139 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/users/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2694 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.865288 mosaicml-cli-0.3.9/mcli/cli/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/__init__.py
--rwxr-xr-x   0 wai        (502) staff       (20)     7182 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/cli.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.867688 mosaicml-cli-0.3.9/mcli/cli/common/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/common/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2670 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 wai        (502) staff       (20)     7238 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.868707 mosaicml-cli-0.3.9/mcli/cli/m_clean/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_clean/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      950 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_clean/m_clean.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.869362 mosaicml-cli-0.3.9/mcli/cli/m_connect/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1541 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.871643 mosaicml-cli-0.3.9/mcli/cli/m_create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    11513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/cluster.py
--rw-r--r--   0 wai        (502) staff       (20)     7167 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/env_var.py
--rw-r--r--   0 wai        (502) staff       (20)     4217 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/m_create.py
--rw-r--r--   0 wai        (502) staff       (20)    24927 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.872616 mosaicml-cli-0.3.9/mcli/cli/m_delete/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    14072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/delete.py
--rw-r--r--   0 wai        (502) staff       (20)     8562 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.873226 mosaicml-cli-0.3.9/mcli/cli/m_deploy/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3896 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.874786 mosaicml-cli-0.3.9/mcli/cli/m_describe/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4409 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     9943 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     1860 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.879197 mosaicml-cli-0.3.9/mcli/cli/m_get/
--rw-r--r--   0 wai        (502) staff       (20)      549 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/clusters.py
--rw-r--r--   0 wai        (502) staff       (20)     6452 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/display.py
--rw-r--r--   0 wai        (502) staff       (20)     1315 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/envvars.py
--rw-r--r--   0 wai        (502) staff       (20)     5467 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     4866 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/m_get.py
--rw-r--r--   0 wai        (502) staff       (20)     9517 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/runs.py
--rw-r--r--   0 wai        (502) staff       (20)     3567 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     1580 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.879935 mosaicml-cli-0.3.9/mcli/cli/m_init/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4113 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/m_init.py
--rw-r--r--   0 wai        (502) staff       (20)     9374 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.880843 mosaicml-cli-0.3.9/mcli/cli/m_interactive/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     9005 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 wai        (502) staff       (20)    16203 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/m_interactive.py
--rw-r--r--   0 wai        (502) staff       (20)     4601 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/temp_mcloud_interactive.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881147 mosaicml-cli-0.3.9/mcli/cli/m_log/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_log/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8633 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881472 mosaicml-cli-0.3.9/mcli/cli/m_ping/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1742 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881785 mosaicml-cli-0.3.9/mcli/cli/m_predict/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.882103 mosaicml-cli-0.3.9/mcli/cli/m_root/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_root/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.882417 mosaicml-cli-0.3.9/mcli/cli/m_run/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_run/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    10034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.883410 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2973 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 wai        (502) staff       (20)     1927 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 wai        (502) staff       (20)     1408 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 wai        (502) staff       (20)      881 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.883783 mosaicml-cli-0.3.9/mcli/cli/m_stop/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3847 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.884231 mosaicml-cli-0.3.9/mcli/cli/m_use/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_use/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_use/m_use.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.885029 mosaicml-cli-0.3.9/mcli/cli/m_util/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     9853 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/kube_util.py
--rw-r--r--   0 wai        (502) staff       (20)     1147 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/m_util.py
--rw-r--r--   0 wai        (502) staff       (20)     6515 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/util.py
--rw-r--r--   0 wai        (502) staff       (20)    16462 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.886444 mosaicml-cli-0.3.9/mcli/models/
--rw-r--r--   0 wai        (502) staff       (20)     1199 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8555 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/inference_deployment_config.py
--rw-r--r--   0 wai        (502) staff       (20)     3693 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_cluster.py
--rw-r--r--   0 wai        (502) staff       (20)      563 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/models/mcli_envvar.py
--rw-r--r--   0 wai        (502) staff       (20)     3386 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_integration.py
--rw-r--r--   0 wai        (502) staff       (20)     9400 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_secret.py
--rw-r--r--   0 wai        (502) staff       (20)    17234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/run_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.886888 mosaicml-cli-0.3.9/mcli/objects/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.888435 mosaicml-cli-0.3.9/mcli/objects/integrations/
--rw-r--r--   0 wai        (502) staff       (20)      660 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      671 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/apt_packages.py
--rw-r--r--   0 wai        (502) staff       (20)     1287 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/comet.py
--rw-r--r--   0 wai        (502) staff       (20)     2597 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/git_repo.py
--rw-r--r--   0 wai        (502) staff       (20)     3491 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/local.py
--rw-r--r--   0 wai        (502) staff       (20)     2126 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/mosaicml_agent.py
--rw-r--r--   0 wai        (502) staff       (20)      810 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/pip_packages.py
--rw-r--r--   0 wai        (502) staff       (20)     2742 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/wandb.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.890277 mosaicml-cli-0.3.9/mcli/objects/secrets/
--rw-r--r--   0 wai        (502) staff       (20)     1090 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4913 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/cluster_secret.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.895446 mosaicml-cli-0.3.9/mcli/objects/secrets/create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3953 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/base.py
--rw-r--r--   0 wai        (502) staff       (20)     3461 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     2406 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     7554 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 wai        (502) staff       (20)     3855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     6701 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 wai        (502) staff       (20)     3782 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     1634 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/env_var.py
--rw-r--r--   0 wai        (502) staff       (20)     1122 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     2893 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/mounted.py
--rw-r--r--   0 wai        (502) staff       (20)     2855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/oci.py
--rw-r--r--   0 wai        (502) staff       (20)     2577 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     3952 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.896776 mosaicml-cli-0.3.9/mcli/proto/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/proto/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.897426 mosaicml-cli-0.3.9/mcli/sdk/
--rw-r--r--   0 wai        (502) staff       (20)     1298 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/sdk/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.898437 mosaicml-cli-0.3.9/mcli/serverside/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.903585 mosaicml-cli-0.3.9/mcli/serverside/clusters/
--rw-r--r--   0 wai        (502) staff       (20)      381 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    11245 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster.py
--rw-r--r--   0 wai        (502) staff       (20)    23072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_instances.py
--rw-r--r--   0 wai        (502) staff       (20)     4005 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_pv_setup.py
--rw-r--r--   0 wai        (502) staff       (20)     2793 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/gpu_type.py
--rw-r--r--   0 wai        (502) staff       (20)     2824 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/instance_type.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.921675 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/
--rw-r--r--   0 wai        (502) staff       (20)     1603 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      548 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/microk8s.py
--rw-r--r--   0 wai        (502) staff       (20)     2219 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r10z1.py
--rw-r--r--   0 wai        (502) staff       (20)     2822 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z1.py
--rw-r--r--   0 wai        (502) staff       (20)     2495 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z4.py
--rw-r--r--   0 wai        (502) staff       (20)     2759 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r3z1.py
--rw-r--r--   0 wai        (502) staff       (20)     5355 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r4z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1049 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1161 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z10.py
--rw-r--r--   0 wai        (502) staff       (20)     2497 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z2.py
--rw-r--r--   0 wai        (502) staff       (20)     1062 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z3.py
--rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z4.py
--rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z5.py
--rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z6.py
--rw-r--r--   0 wai        (502) staff       (20)     1214 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z7.py
--rw-r--r--   0 wai        (502) staff       (20)     1242 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z9.py
--rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1071 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z2.py
--rw-r--r--   0 wai        (502) staff       (20)     1054 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z3.py
--rw-r--r--   0 wai        (502) staff       (20)     1061 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r99z1.py
--rw-r--r--   0 wai        (502) staff       (20)      310 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/volumekind.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.926609 mosaicml-cli-0.3.9/mcli/serverside/job/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    15654 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_job.py
--rw-r--r--   0 wai        (502) staff       (20)      465 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_config_map_typing.py
--rw-r--r--   0 wai        (502) staff       (20)     6471 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job.py
--rw-r--r--   0 wai        (502) staff       (20)     8090 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job_typing.py
--rw-r--r--   0 wai        (502) staff       (20)     7524 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
--rw-r--r--   0 wai        (502) staff       (20)      459 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_service_typing.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.927972 mosaicml-cli-0.3.9/mcli/serverside/runners/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/runners/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5770 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/runners/runner.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.948090 mosaicml-cli-0.3.9/mcli/utils/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5306 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_cli.py
--rw-r--r--   0 wai        (502) staff       (20)     6073 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/utils/utils_config.py
--rw-r--r--   0 wai        (502) staff       (20)      740 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_date.py
--rw-r--r--   0 wai        (502) staff       (20)    10453 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_docker.py
--rw-r--r--   0 wai        (502) staff       (20)    12947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_epilog.py
--rw-r--r--   0 wai        (502) staff       (20)      751 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_file.py
--rw-r--r--   0 wai        (502) staff       (20)    11769 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_interactive.py
--rw-r--r--   0 wai        (502) staff       (20)    49322 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_kube.py
--rw-r--r--   0 wai        (502) staff       (20)     6980 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_kube_labels.py
--rw-r--r--   0 wai        (502) staff       (20)     4832 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_logging.py
--rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 wai        (502) staff       (20)      359 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_modules.py
--rw-r--r--   0 wai        (502) staff       (20)     6614 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_pypi.py
--rw-r--r--   0 wai        (502) staff       (20)     6513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_rancher.py
--rw-r--r--   0 wai        (502) staff       (20)     3115 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_rich.py
--rw-r--r--   0 wai        (502) staff       (20)     8533 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_run_status.py
--rw-r--r--   0 wai        (502) staff       (20)     4350 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 wai        (502) staff       (20)     1103 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_spinner.py
--rw-r--r--   0 wai        (502) staff       (20)    11437 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_string_functions.py
--rw-r--r--   0 wai        (502) staff       (20)     3954 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_types.py
--rw-r--r--   0 wai        (502) staff       (20)     1001 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_yaml.py
--rw-r--r--   0 wai        (502) staff       (20)     3885 2023-04-20 18:58:54.000000 mosaicml-cli-0.3.9/mcli/version.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.951930 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     7263 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wai        (502) staff       (20)        1 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wai        (502) staff       (20)       75 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 wai        (502) staff       (20)     1552 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 wai        (502) staff       (20)       11 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 wai        (502) staff       (20)    31087 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/pyproject.toml
--rw-r--r--   0 wai        (502) staff       (20)       38 2023-04-20 19:06:23.957367 mosaicml-cli-0.3.9/setup.cfg
--rw-r--r--   0 wai        (502) staff       (20)     2991 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/setup.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.954109 mosaicml-cli-0.3.9/tests/
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.955987 mosaicml-cli-0.3.9/tests/submit/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6393 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/test_cluster.py
--rw-r--r--   0 wai        (502) staff       (20)     9266 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/test_cluster_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     7973 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/test_config.py
--rw-r--r--   0 wai        (502) staff       (20)       62 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/tests/test_simple.py
--rw-r--r--   0 wai        (502) staff       (20)     6116 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/tests/test_upgrade.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.410730 mosaicml-cli-0.4.0a0/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 19:46:05.410519 mosaicml-cli-0.4.0a0/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/README.md
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.374460 mosaicml-cli-0.4.0a0/mcli/
+-rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.375153 mosaicml-cli-0.4.0a0/mcli/api/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.375745 mosaicml-cli-0.4.0a0/mcli/api/cluster/
+-rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/cluster/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.376198 mosaicml-cli-0.4.0a0/mcli/api/engine/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/engine/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/engine/engine.py
+-rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/exceptions.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.377756 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/
+-rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     3292 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.378349 mosaicml-cli-0.4.0a0/mcli/api/mint/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/shell.py
+-rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/mint/tty.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.379230 mosaicml-cli-0.4.0a0/mcli/api/model/
+-rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/cluster_details.py
+-rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/model/run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.381329 mosaicml-cli-0.4.0a0/mcli/api/runs/
+-rw-r--r--   0 anna       (501) staff       (20)     1102 2023-04-18 18:36:19.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.381752 mosaicml-cli-0.4.0a0/mcli/api/schema/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/schema/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.382758 mosaicml-cli-0.4.0a0/mcli/api/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/typing_future.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.383225 mosaicml-cli-0.4.0a0/mcli/api/users/
+-rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/users/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.383609 mosaicml-cli-0.4.0a0/mcli/cli/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/__init__.py
+-rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/cli.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.384207 mosaicml-cli-0.4.0a0/mcli/cli/common/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.384554 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.385223 mosaicml-cli-0.4.0a0/mcli/cli/m_create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.385812 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.386122 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.387457 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     9943 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.389733 mosaicml-cli-0.4.0a0/mcli/cli/m_get/
+-rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/display.py
+-rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-20 17:34:06.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_get/users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.390336 mosaicml-cli-0.4.0a0/mcli/cli/m_init/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.391421 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 anna       (501) staff       (20)     9464 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.391803 mosaicml-cli-0.4.0a0/mcli/cli/m_log/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.392216 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.392797 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.393144 mosaicml-cli-0.4.0a0/mcli/cli/m_root/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.393457 mosaicml-cli-0.4.0a0/mcli/cli/m_run/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     7550 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.394765 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.395095 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.395803 mosaicml-cli-0.4.0a0/mcli/cli/m_util/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/cli/m_util/util.py
+-rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.397771 mosaicml-cli-0.4.0a0/mcli/models/
+-rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/gpu_type.py
+-rw-r--r--   0 anna       (501) staff       (20)     8426 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_cluster.py
+-rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_envvar.py
+-rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/mcli_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/models/run_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.398121 mosaicml-cli-0.4.0a0/mcli/objects/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.400065 mosaicml-cli-0.4.0a0/mcli/objects/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.401914 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.402373 mosaicml-cli-0.4.0a0/mcli/proto/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 22:34:58.000000 mosaicml-cli-0.4.0a0/mcli/proto/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-20 00:22:55.000000 mosaicml-cli-0.4.0a0/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.402910 mosaicml-cli-0.4.0a0/mcli/sdk/
+-rw-r--r--   0 anna       (501) staff       (20)     1045 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/sdk/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.407472 mosaicml-cli-0.4.0a0/mcli/utils/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_cli.py
+-rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_date.py
+-rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-20 00:22:47.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_docker.py
+-rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_epilog.py
+-rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_logging.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_pypi.py
+-rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_rich.py
+-rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_run_status.py
+-rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_spinner.py
+-rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_types.py
+-rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/mcli/utils/utils_yaml.py
+-rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/mcli/version.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.408944 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     4609 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-20 19:46:05.000000 mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-20 17:48:17.000000 mosaicml-cli-0.4.0a0/pyproject.toml
+-rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-20 19:46:05.410824 mosaicml-cli-0.4.0a0/setup.cfg
+-rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/setup.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-20 19:46:05.410108 mosaicml-cli-0.4.0a0/tests/
+-rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-20 19:43:30.000000 mosaicml-cli-0.4.0a0/tests/test_config.py
+-rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/tests/test_simple.py
+-rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a0/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.3.9/PKG-INFO` & `mosaicml-cli-0.4.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.9
+Version: 0.4.0a0
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.9/README.md` & `mosaicml-cli-0.4.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -127,28 +127,21 @@
 **And… you are done!**
 
 A few notes for later on:
 
 - To exit the virtual environment later on: `$ deactivate`
 - To get back into your virtual environment: `$ source venv/bin/activate`
 
-## MCloud vs Legacy `mcli`
-
-`mcli` is now intended to primarily work indirectly with compute clusters through MCLoud, which is done through the MAPI endpoint.
-However, `mcli` can still talk directly to select Kubernetes clusters in what we call "Legacy" mode.
-This is maintained currently for internal users and customers that rely on "interactive" sessions (ie `mcli interactive`), as this feature is not yet supported in MCloud.
-
 ## Running against mcloud as a developer
 
 There are currently 6 MCLI Modes. To use a mode other than the default `PROD`, set your local environment variable `MCLI_MODE` or specify the mode when you run MCLI commands (e.g. `MCLI_MODE=DEV mcli get runs`)
 
 | Mode       | Used By         | MAPI Endpoint                            | Use cases                                              | API Key                                                    |
 | ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------- |
 | `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://cloud.mosaicml.com/account#)     |
-| `LEGACY`   | Any             | N/A                                      | Customers who haven't moved over to mcloud yet         | N/A                                                        |
 | `INTERNAL` | Internal users  | https://api.mosaicml.com/graphql         | Internal/alpha features in a prod environment          | Create one [here](https://cloud.mosaicml.com/account#)     |
 | `STAGING`  | Developers only | https://staging.api.mosaicml.com/graphql | Test changes queued for prod release                   | Testing api key                                            |
 | `DEV`      | Developers only | https://dev.api.mosaicml.com/graphql     | Test against dev branch of mcloud                      | Create one [here](https://dev.cloud.mosaicml.com/account#) |
 | `LOCAL`    | Developers only | http://localhost:3001/graphql            | Test local mcloud changes                              | Testing api key                                            |
 
 Note for almost all of these modes, you need to set an api key to talk to MAPI:
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a0/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a0/mcli/api/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from gql.client import Client, ReconnectingAsyncClientSession
 from gql.transport import AsyncTransport
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from graphql import DocumentNode
 from websockets.exceptions import ConnectionClosed, PayloadTooBig, WebSocketException
 
-from mcli.api.exceptions import KubernetesException, MAPIException, MCLIConfigError, MultiMAPIException
+from mcli.api.exceptions import MAPIException, MCLIConfigError, MultiMAPIException
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.config import MESSAGE, get_timeout
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable-next=invalid-name
 THREADPOOL_WORKERS = 10
@@ -365,34 +365,14 @@
         A Future for the return value of ``f``
     """
     if not connection:
         connection = MAPIConnection.get_current_connection()
     return connection.pool.submit(f, *args, **kwargs)
 
 
-def run_kube_in_threadpool(
-    f: Callable[..., ThreadedOutput],
-    *args: Any,
-    connection: Optional[MAPIConnection] = None,
-    **kwargs: Any,
-) -> Future[ThreadedOutput]:
-    """Wrap a function that calls Kubernetes and returns a :type DeserializableModel: in
-    a Future
-
-    Args:
-        f: Function that calls Kubernetes
-        *args, **kwargs: Arbitrary arguments with which to call ``f``
-        connection: Optional :type MAPIConnection: whose threadpool will be used
-
-    Returns:
-        A Future for the return value of ``f``
-    """
-    return run_in_threadpool(KubernetesException.wrap(f), *args, connection=connection, **kwargs)
-
-
 ModelT = TypeVar('ModelT', bound=DeserializableModel)
 
 
 def run_plural_mapi_request(
     query: str,
     query_function: str,
     return_model_type: Optional[Type[ModelT]] = None,
@@ -589,51 +569,14 @@
     if len(items) == 1:
         return items[0]
     else:
         raise MAPIException(status=HTTPStatus.INTERNAL_SERVER_ERROR,
                             message='Request returned no items, but expected 1')
 
 
-def run_empty_mapi_request(
-    query: str,
-    query_function: str,
-    variables: Optional[Dict[str, Any]] = None,
-    connection: Optional[MAPIConnection] = None,
-) -> Future[None]:
-    """Run a GraphQL query against MAPI a future for the response
-
-    If the result succeeds, ``future.result()`` will return ``None``, otherwise it will
-    error with a ``MAPIException``.
-
-    Args:
-        query: Query to run
-        query_function: GraphQL endpoint for the query (e.g. 'createRun')
-        variables: Variables to be passed to the GraphQL endpoint. Defaults to None.
-        connection: The MAPI connection that should be used. Defaults to the connection
-            returned by `MAPIConnection.get_current_connection()`.
-
-    Returns:
-        A `concurrent.futures.Future` for the request. You can retrieve the data using
-        `future.result()` with an optional `timeout` argument.
-    """
-    if not connection:
-        connection = MAPIConnection.get_current_connection()
-
-    future = connection.pool.submit(
-        _threaded_empty_mapi_request,
-        api_key=connection.api_key,
-        endpoint=connection.endpoint,
-        query=query,
-        variables=variables,
-        query_function=query_function,
-    )
-
-    return future
-
-
 def _threaded_empty_mapi_request(
     api_key: str,
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]],
     query_function: str,
 ) -> None:
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a0/mcli/api/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import functools
 import logging
 import re
 import textwrap
 from concurrent.futures import TimeoutError as FuturesTimeoutError
 from enum import Enum
 from http import HTTPStatus
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional
 
 import requests
-from kubernetes.client.exceptions import ApiException
 
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MESSAGE = 'Unknown Error'
 
@@ -199,93 +198,24 @@
 
 
 class MAPIErrorMessages(Enum):
 
     NOT_FOUND_CLUSTER = 'No clusters found. Please contact your organization administrator to set one up'
 
 
-class KubernetesErrorDesc(Enum):
-    """Provides descriptions for common Kubernetes errors that we might encounter
-    """
-
-    UNAUTHORIZED = ('Invalid cluster credentials: Please contact your cluster administrator by sending a '
-                    'message to your MosaicML customer support slack channel')
-    FORBIDDEN = ('Invalid permissions: The requested action is not allowed. Please contact your cluster administrator '
-                 'by sending a message to your MosaicML customer support slack channel')
-    NOT_FOUND = 'Object not found: Could not find the requested object'
-    CONFLICT = 'Object already exists: Please ensure you are using unique names'
-    UNPROCESSABLE_ENTITY = ('Submitted object misconfigured: This usually occurs when secrets and other objects '
-                            'are duplicated. Please double-check and try again.')
-    INTERNAL_SERVER_ERROR = ('Cluster error: The cluster seems to be struggling with something. '
-                             'Please report this issue to your cluster administrator by sending a message to your '
-                             'MosaicML customer support slack channel')
-
-
-# pylint: disable-next=invalid-name
-TFunc = TypeVar('TFunc', bound=Callable[..., Any])
-
-
+# TODO: deprecate
 class KubernetesException(MAPIException):
-    """Exceptions raised when a Kubernetes request fails
+    """Deprecated exception, use MAPIException instead
 
     Args:
         status: The status code for the exception
         message: A brief description of the error
         description: An optional longer description of the error
-
-    Details:
-    Kubernetes will respond with a variety of status codes when a request fails. Below are some of the common ones:
-    - 401: User credentials were invalid. Check with your cluster administrator on how to get new ones
-    - 403: User credentials were valid, but the requested action is not allowed
-    - 409: Attempted to create an object with a name that already exists. Change the name and try again.
-    - 422: Submitted object misconfigured: This usually occurs when secrets and other objects
-           are duplicated. Please double-check and try again.
-    - 500: Internal cluster error. Please report the issue
     """
 
-    @classmethod
-    def transform_api_exception(
-        cls: Type[KubernetesException],
-        e: ApiException,
-    ) -> Union[KubernetesException, ApiException]:
-
-        try:
-            status = HTTPStatus(e.status)
-            message = KubernetesErrorDesc[status.name].value  # pylint: disable=no-member
-        except (KeyError, TypeError):
-            return e
-
-        logger.debug(f'Transformed Kubernetes exception: {e}')
-        return cls(status=status, message=message)
-
-    @classmethod
-    def wrap(cls, f: TFunc) -> TFunc:
-        """Wrap the provided callable to catch any Kubernetes ApiException and
-        throw a transformed KubernetesException
-
-        Args:
-            f: Callable that might raise an ApiException
-
-        Raises:
-            KubernetesException: Raised if an ApiException was hit that we know how to message to the user
-            ApiException: Raised if an unfamiliar ApiException is hit
-
-        Returns:
-            A wrapped callable
-        """
-
-        @functools.wraps(f)
-        def wrapped(*args: Any, **kwargs: Any):
-            try:
-                return f(*args, **kwargs)
-            except ApiException as e:
-                raise cls.transform_api_exception(e) from e
-
-        return wrapped  # type: ignore
-
 
 def cli_error_handler(command: Optional[str] = None):
 
     def decorator(func):
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import List, Optional, Union, overload
 
 from typing_extensions import Literal
 
 from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.config import MCLIConfig
+from mcli.models.gpu_type import GPUType
 from mcli.models.mcli_cluster import Cluster
-from mcli.serverside.clusters.gpu_type import GPUType
 
 __all__ = ['get_inference_deployments']
 
 QUERY_FUNCTION = 'getInferenceDeployments'
 VARIABLE_DATA_NAME = 'getInferenceDeploymentsData'
 QUERY = f"""
 query GetInferenceDeployments(${VARIABLE_DATA_NAME}: GetInferenceDeploymentsInput!) {{
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a0/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_stop_runs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,79 @@
-"""Implements the stop_runs API for Kubernetes"""
+""" Stop a run. """
 from __future__ import annotations
 
-from concurrent.futures import Future, as_completed
-from http import HTTPStatus
-from typing import Dict, List, Optional, Union, cast, overload
+from concurrent.futures import Future
+from typing import List, Optional, Union, overload
 
-from kubernetes.client.exceptions import ApiException
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import run_kube_in_threadpool
-from mcli.api.exceptions import KubernetesException
-from mcli.api.kube.runs.api_delete_runs import _get_cluster_runs
-from mcli.api.model import Run
-from mcli.utils.utils_kube import ClusterRun, delete_pod_tombstone, get_rank0_pod, use_context
-from mcli.utils.utils_run_status import RunStatus
+from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
+from mcli.api.model.run import Run
+from mcli.config import MCLIConfig
+
+__all__ = ['stop_runs']
+
+QUERY_FUNCTION = 'stopRuns'
+VARIABLE_DATA_NAME = 'getRunsData'
+QUERY = f"""
+mutation StopRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
+  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+    id
+    name
+    runInput
+    createdByEmail
+    status
+    createdAt
+    startedAt
+    completedAt
+    updatedAt
+    reason
+  }}
+}}"""
 
 
-def _threaded_stop_runs(runs: Union[List[str], List[Run]]):
-    """Threaded function for stopping a list of runs
+@overload
+def stop_run(run: Union[str, Run], timeout: Optional[float] = 10, future: Literal[False] = False) -> Run:
+    ...
 
-    Args:
-        runs: List of runs to stop
 
-    Returns:
-        A list of :type Run: that were stopped
+@overload
+def stop_run(run: Union[str, Run], timeout: Optional[float] = None, future: Literal[True] = True) -> Future[Run]:
+    ...
 
-    Raises:
-        KubernetesException: Raised if stopping any of the requested runs failed.
-    """
-    if not runs:
-        return []
 
-    if not all(isinstance(r, Run) for r in runs):
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.kube.runs import get_runs
-        runs = get_runs(runs=[r.name if isinstance(r, Run) else r for r in runs])
-    runs = cast(List[Run], runs)
-
-    run_dict: Dict[str, Run] = {r.name: r for r in runs}
-    cluster_runs = _get_cluster_runs(runs)
-    futures: Dict[Future[bool], str] = {
-        run_kube_in_threadpool(_get_and_stop_pods, pr): pr.name for pr in cluster_runs
-    }  # type: ignore
-    failed_runs: List[str] = []
-    failed_status: Optional[HTTPStatus] = None
-    for fs in as_completed(futures):
-        run_name = futures[fs]
-        run = run_dict[run_name]
-        try:
-            _ = fs.result()  # Succeeded if it didn't error
-            run.status = RunStatus.STOPPED
-        except (KubernetesException, ApiException) as e:
-            failed_runs.append(run_name)
-            # Keep the last failure status for the error raised below
-            failed_status = e.status if isinstance(e, KubernetesException) else HTTPStatus(e.status)
-    if failed_runs:
-        raise KubernetesException(status=failed_status or HTTPStatus.INTERNAL_SERVER_ERROR,
-                                  message=f'Failed to stop {len(failed_runs)} runs. Please try again. '
-                                  f'The runs that failed to stop were:\n{failed_runs}')
-
-    return list(run_dict.values())
-
-
-def _get_and_stop_pods(cluster_run: ClusterRun) -> bool:
-    """Stop a single run by first getting the rank 0 pod and then deleting its tombstone
-    file
+def stop_run(run: Union[str, Run], timeout: Optional[float] = 10, future: bool = False):
+    """Stop a run
 
-    NOTE: Since the run will error if the rank 0 pod goes down, we only need to stop it
-    explicitly.
-    """
+    Stop a run currently running in the MosaicML platform.
 
-    namespace = cluster_run.context.namespace
-    assert namespace is not None, 'Invalid cluster: namespace should never be None'
+    Args:
+        run (``Optional[str | ``:class:`~mcli.api.model.run.Run` ``]``):
+            A run or run name to stop. Using :class:`~mcli.api.model.run.Run` objects is most
+            efficient. See the note below.
+        timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
+            If the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
+            will be raised. If ``future`` is ``True``, this value will be ignored.
+        future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
+            call to :func:`stop_run` will return immediately and the request will be
+            processed in the background. This takes precedence over the ``timeout``
+            argument. To get the list of :class:`~mcli.api.model.run.Run` output,
+            use ``return_value.result()`` with an optional ``timeout`` argument.
 
-    with use_context(cluster_run.context.name):
-        try:
-            # Get the rank 0 pod. If it doesn't exist, then return True since the run has likely failed
-            rank0_pod = get_rank0_pod(cluster_run.name, namespace)
-        except RuntimeError:
-            return True
-        return delete_pod_tombstone(rank0_pod, namespace)
+    Raises:
+        MapiException: Raised if stopping the requested runs failed
+            A successfully stopped run will have the status ```RunStatus.STOPPED```
+
+    Returns:
+        If future is False:
+            Stopped :class:`~mcli.api.model.run.Run` object
+        Otherwise:
+            A :class:`~concurrent.futures.Future` for the object
+    """
+    return stop_runs([run], timeout, future)[0]  # type: ignore
 
 
 @overload
 def stop_runs(runs: Union[List[str], List[Run]],
               timeout: Optional[float] = 10,
               future: Literal[False] = False) -> List[Run]:
     ...
@@ -92,17 +82,15 @@
 @overload
 def stop_runs(runs: Union[List[str], List[Run]],
               timeout: Optional[float] = None,
               future: Literal[True] = True) -> Future[List[Run]]:
     ...
 
 
-def stop_runs(runs: Union[List[str], List[Run]],
-              timeout: Optional[float] = 10,
-              future: bool = False) -> Union[List[Run], Future[List[Run]]]:
+def stop_runs(runs: Union[List[str], List[Run]], timeout: Optional[float] = 10, future: bool = False):
     """Stop a list of runs
 
     Stop a list of runs currently running in the MosaicML platform.
 
     Args:
         runs (``Optional[List[str] | List[``:class:`~mcli.api.model.run.Run` ``]]``):
             A list of runs or run names to stop. Using :class:`~mcli.api.model.run.Run`
@@ -113,36 +101,40 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`stop_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        KubernetesException: Raised if stopping any of the requested runs failed. All
+        MapiException: Raised if stopping any of the requested runs failed. All
             successfully stopped runs will have the status ```RunStatus.STOPPED```. You can
             freely retry any stopped and unstopped runs if this error is raised due to a
             connection issue.
 
     Returns:
         If future is False:
             A list of stopped :class:`~mcli.api.model.run.Run` objects
         Otherwise:
             A :class:`~concurrent.futures.Future` for the list
-
-    Note:
-        The Kubernetes API requires the cluster for each run. If you provide ``runs`` as a
-        list of names, we will get this by calling :func:`~mcli.sdk.get_runs`. Since
-        a common way to get the list of runs is to have already called
-        :func:`~mcli.sdk.get_runs`, you can avoid a second call by passing
-        the output of that call in directly.
-
-    Warning:
-        Stopping runs does not occur immediately. You may see up to a 40 second delay
-        between your request and the run actually stopping.
     """
+    # Extract run names
+    run_names = [r.name if isinstance(r, Run) else r for r in runs]
 
-    response = run_kube_in_threadpool(_threaded_stop_runs, runs)
-
-    if not future:
-        return response.result(timeout=timeout)
-    else:
-        return response
+    filters = {}
+    if run_names:
+        filters['name'] = {'in': run_names}
+
+    variables = {VARIABLE_DATA_NAME: {'filters': filters}}
+
+    cfg = MCLIConfig.load_config(safe=True)
+    if cfg.user_id:
+        variables[VARIABLE_DATA_NAME]['entity'] = {
+            'userIds': [cfg.user_id],
+        }
+
+    response = run_plural_mapi_request(
+        query=QUERY,
+        query_function=QUERY_FUNCTION,
+        return_model_type=Run,
+        variables=variables,
+    )
+    return get_return_response(response, future=future, timeout=timeout)
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a0/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a0/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a0/mcli/api/model/cluster_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Set
 
 from dateutil import parser
 
 from mcli.api.exceptions import MAPI_DESERIALIZATION_ERROR
 from mcli.api.schema.generic_model import DeserializableModel
-from mcli.models.mcli_cluster import Cluster
 from mcli.models.run_config import SchedulingConfig, SchedulingTranslation
-from mcli.serverside.clusters.gpu_type import GPUType
 from mcli.utils.utils_serializable_dataclass import SerializableDataclass
 
 logger = logging.getLogger(__name__)
 
 
 def check_response(response: Dict[str, Any], expected: Set[str]) -> None:
     missing = expected - set(response)
@@ -111,18 +109,14 @@
         check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'gpuNums'})
         return cls(name=response['name'],
                    gpu_type=response['gpuType'],
                    gpus=response['gpusPerNode'],
                    nodes=response['numNodes'],
                    gpu_nums=response['gpuNums'])
 
-    @classmethod
-    def from_available_instances(cls, available_instances: Dict[GPUType, List[int]]) -> List[Instance]:
-        return [Instance('', gpu_type.value, 0, 0, gpu_nums) for gpu_type, gpu_nums in available_instances.items()]
-
     def __lt__(self, other: Instance):
         if self.gpu_type.lower() == 'none':
             return True
         return self.gpu_type < other.gpu_type
 
 
 def get_provider_name(raw_provider: str):
@@ -166,10 +160,7 @@
                    allow_multinode=response.get('allowMultinode', False),
                    cluster_instances=[Instance.from_mapi_response(i) for i in response.get('allowedInstances', [])],
                    utilization=utilization,
                    id=response.get('id'))
 
     def __lt__(self, other: ClusterDetails):
         return self.name < other.name
-
-    def to_cluster(self) -> Cluster:
-        return Cluster(name=self.name, kubernetes_context='', namespace='')
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a0/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a0/mcli/api/model/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from datetime import datetime
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
 from mcli.models.run_config import FinalRunConfig, RunConfig
-from mcli.serverside.job.mcli_job import MCLIJobType
 from mcli.utils.utils_run_status import RunStatus
 
 
 @dataclass
 class Node(DeserializableModel):
     """Node linked to a run
     """
@@ -70,18 +69,14 @@
         'status',
         'createdAt',
         'updatedAt',
         'runInput',
         'createdByEmail',
     ])
 
-    # This "job type" field is used only by interactive sessions in kube mcli
-    # Let's add it as an optional only to be used by api.kube.get_runs
-    _type: Optional[MCLIJobType] = None
-
     def clone(
         self,
         name: Optional[str] = None,
         image: Optional[str] = None,
         cluster: Optional[str] = None,
         instance: Optional[str] = None,
         nodes: Optional[int] = None,
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_get_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from typing_extensions import Literal
 
 from mcli.api.engine.engine import get_return_response, run_paginated_mapi_request, run_plural_mapi_request
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
+from mcli.models.gpu_type import GPUType
 from mcli.models.mcli_cluster import Cluster
-from mcli.serverside.clusters.gpu_type import GPUType
 from mcli.utils.utils_run_status import RunStatus
 
 __all__ = ['get_runs', 'get_run']
 
 QUERY_FUNCTION = 'getRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
 QUERY = f"""
```

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a0/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a0/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a0/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a0/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a0/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a0/mcli/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import sys
 from string import ascii_lowercase
 from typing import Tuple
 
 import argcomplete
 
 from mcli import config
-from mcli.api.exceptions import MCLIConfigError
-from mcli.cli.m_clean.m_clean import clean_mcli
 from mcli.cli.m_connect.m_connect import add_connect_argparser
 from mcli.cli.m_create.m_create import add_create_argparser
 from mcli.cli.m_delete.m_delete import add_delete_argparser
 from mcli.cli.m_deploy.m_deploy import add_deploy_argparser
 from mcli.cli.m_describe.m_describe import add_describe_parser
 from mcli.cli.m_get.m_get import add_get_argparser
 from mcli.cli.m_init.m_init import initialize_mcli
@@ -28,32 +26,26 @@
 from mcli.cli.m_ping.m_ping import add_ping_parser
 from mcli.cli.m_predict.m_predict import add_predict_parser
 from mcli.cli.m_root.m_config import m_get_config
 from mcli.cli.m_run.m_run import add_run_argparser
 from mcli.cli.m_set_unset.m_set import add_set_argparser
 from mcli.cli.m_set_unset.m_unset import add_unset_argparser
 from mcli.cli.m_stop.m_stop import add_stop_parser
-from mcli.cli.m_use.m_use import add_use_argparser
 from mcli.cli.m_util.m_util import add_util_argparser
 from mcli.config import FeatureFlag, MCLIConfig
 from mcli.utils.utils_cli import MCLIArgumentParser
 from mcli.utils.utils_logging import console_handler
 from mcli.utils.utils_pypi import NeedsUpdateError, check_new_update_available
 from mcli.version import get_formatted_version, print_version
 
 logger = logging.getLogger('mcli')
 logger.setLevel(logging.INFO)
 logger.addHandler(console_handler)
 
 
-def add_clean_argparser(subparser: argparse._SubParsersAction) -> None:
-    clean_parser: argparse.ArgumentParser = subparser.add_parser('clean', aliases=['cl'], help='Clean MCLI')
-    clean_parser.set_defaults(func=clean_mcli)
-
-
 def add_root_commands(subparser: argparse._SubParsersAction) -> None:
     """Adds root level commands to the CLI
 
     Args:
         subparser: The subparser to add commands to
     """
     config_parser: argparse.ArgumentParser = subparser.add_parser(
@@ -100,35 +92,25 @@
 
     add_root_commands(subparser=subparser)
     return parser, subparser
 
 
 def get_parser(is_admin: bool = False) -> argparse.ArgumentParser:
     parser, subparser = get_mcli_root('mcli' if not is_admin else 'mcli-admin')
-    try:
-        conf = MCLIConfig.load_config(safe=True)
-    except MCLIConfigError:
-        # If MCLIConfig has not been initialized, we skip
-        # adding any subcommands that are gated behind
-        # setup or feature flags
-        pass
-    else:
-        use_mcloud = conf.feature_enabled(FeatureFlag.USE_MCLOUD)
-        if not use_mcloud:
-            add_init_kube_parser(subparser=subparser)
-
-        if conf.internal:
-            add_use_argparser(subparser=subparser)
-            add_clean_argparser(subparser=subparser)
-
-        if conf.feature_enabled(FeatureFlag.MCLOUD_INTERACTIVE):
-            add_connect_argparser(subparser=subparser)
-            add_interactive_argparser(subparser=subparser)
-        elif conf.allow_interactive:
-            kube_interactive_argparser(subparser=subparser)
+
+    conf = MCLIConfig.load_config(safe=True)
+
+    if conf.mcli_mode.is_legacy():
+        add_init_kube_parser(subparser=subparser)
+
+    if conf.feature_enabled(FeatureFlag.MCLOUD_INTERACTIVE):
+        add_connect_argparser(subparser=subparser)
+        add_interactive_argparser(subparser=subparser)
+    elif conf.allow_interactive:
+        kube_interactive_argparser(subparser=subparser)
 
     add_create_argparser(subparser=subparser)
     add_delete_argparser(subparser=subparser)
     add_deploy_argparser(subparser=subparser)
     add_describe_parser(subparser=subparser)
     add_get_argparser(subparser=subparser, is_admin=is_admin)
     add_log_parser(subparser=subparser)
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a0/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a0/mcli/cli/common/run_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import argparse
 import fnmatch
 import functools
 import logging
 from typing import Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MCLIException
-from mcli.config import FeatureFlag, MCLIConfig
 from mcli.sdk import Run, get_runs
 from mcli.utils.utils_cli import SubmissionType, comma_separated, date_time_parse
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 from mcli.utils.utils_string_functions import is_glob
 
 logger = logging.getLogger(__name__)
@@ -166,20 +165,16 @@
         if action_all is False:
             raise MCLIException('Must specify at least one filter or --all')
 
     if not name_filter:
         # Accept all that pass other filters
         name_filter = []
 
-    conf = MCLIConfig.load_config(safe=True)
-
     # Use get_runs only for the non-glob names provided
     glob_filters, run_names = _split_glob_filters(name_filter)
-    if not conf.feature_enabled(FeatureFlag.USE_MCLOUD) and not conf.clusters:
-        raise MCLIException('No clusters found. You must have at least 1 cluster added before working with runs.')
 
     with console_status('Retrieving requested runs...'):
         runs = get_runs(
             runs=(run_names or None) if not glob_filters else None,
             cluster_names=cluster_filter,
             user_emails=user_filter,
             before=before_filter,
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_get/m_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,114 @@
-""" mcli create Commands """
+""" CLI Get options"""
 import argparse
-import logging
-import textwrap
+from typing import List, Optional
 
-from mcli.cli.m_create.cluster import CLUSTER_EXAMPLES, configure_cluster_argparser, create_new_cluster
-from mcli.cli.m_create.env_var import configure_env_var_argparser, create_new_env_var
-from mcli.cli.m_create.secret import configure_secret_argparser, create_new_secret
-from mcli.config import FeatureFlag, MCLIConfig
+from mcli import config
+from mcli.cli.m_get import cli_get_secrets, get_clusters, get_users
+from mcli.cli.m_get.display import OutputDisplay
+from mcli.cli.m_get.inference_deployments import get_deployments_argparser
+from mcli.cli.m_get.runs import get_runs_argparser
+from mcli.models.mcli_secret import SecretType
 
-logger = logging.getLogger(__name__)
 
-
-def create(**kwargs) -> int:
+def get_entrypoint(parser, **kwargs) -> int:
     del kwargs
-    mock_parser = configure_argparser(parser=argparse.ArgumentParser())
-    mock_parser.print_help()
+    parser.print_help()
     return 0
 
 
 def add_common_arguments(parser: argparse.ArgumentParser):
-    parser.add_argument('--no-input', action='store_true', help='Do not query for user input')
-
+    parser.add_argument('-o',
+                        '--output',
+                        type=OutputDisplay,
+                        choices=list(OutputDisplay),
+                        default=OutputDisplay.TABLE,
+                        metavar='FORMAT',
+                        help=f'Output display format. Should be one of {list(OutputDisplay)}')
 
-def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    conf = MCLIConfig.load_config(safe=True)
 
+def configure_argparser(parser: argparse.ArgumentParser, is_admin: bool = False) -> argparse.ArgumentParser:
     subparsers = parser.add_subparsers(title='MCLI Objects',
-                                       description='The table below shows the objects that you can create',
+                                       description='The table below shows the objects that you can get information on',
                                        help='DESCRIPTION',
                                        metavar='OBJECT')
-    parser.set_defaults(func=create)
+    parser.set_defaults(func=get_entrypoint, parser=parser)
 
-    if not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-        # pylint: disable=invalid-name
-        CLUSTER_DESC = textwrap.dedent("""
-                                        Add a new cluster in which you can launch runs. If you do not know the appropriate
-                                        context, running `mcli create cluster` alone will give you a list of options to
-                                        choose from.""")
-
-        cluster_parser = subparsers.add_parser('cluster',
-                                               aliases=['clusters', 'platforms', "platform"],
-                                               help='Add a cluster to launch runs in',
-                                               description=CLUSTER_DESC,
-                                               epilog=CLUSTER_EXAMPLES,
-                                               formatter_class=argparse.RawDescriptionHelpFormatter)
-        configure_cluster_argparser(cluster_parser)
-        add_common_arguments(cluster_parser)
-        cluster_parser.set_defaults(func=create_new_cluster)
-
-        environment_parser = subparsers.add_parser(
-            'env',
-            aliases=['envs'],
-            help='Create environment variables to use across your runs',
-            description='Setup environment variables that will be used in all of your subsequent workloads',
-        )
-        configure_env_var_argparser(environment_parser)
-        add_common_arguments(environment_parser)
-        environment_parser.set_defaults(func=create_new_env_var)
+    cluster_parser = subparsers.add_parser('clusters',
+                                           aliases=['cluster', 'platforms', 'platform'],
+                                           help='List registered clusters')
+    cluster_parser.add_argument('--ids',
+                                action='store_true',
+                                dest='include_ids',
+                                default=config.ADMIN_MODE,
+                                help='Include the cluster ids in the output')
+    add_common_arguments(cluster_parser)
+    cluster_parser.set_defaults(func=get_clusters)
+
+    if is_admin:
+        user_parser = subparsers.add_parser('user', aliases=['users'], help='List users')
+        add_common_arguments(user_parser)
+        user_parser.set_defaults(func=get_users)
 
     # pylint: disable-next=invalid-name
-    SECRET_EXAMPLES = textwrap.dedent("""
+    SECRET_EXAMPLES = """
 
-    Examples:
+Examples:
 
-    # Create an "env" (environment variable) secret
-    mcli create secret env FOO=super-secret-api-key-1234
-    """)
+> mcli get secrets
+NAME         TYPE
+foo          environment
+docker-cred  docker_registry
+file         mounted
+
+> mcli get secrets --type environment
+NAME         TYPE
+foo          environment
+    """
     secrets_parser = subparsers.add_parser(
-        'secret',
-        aliases=['secrets'],
-        help='Create secrets and credentials to add to your runs',
-        description='Add secrets and credentials that will be added to all of your '
-        'subsequent runs. For details on exactly how each type of secret is added to '
-        'your run, look to the individual secret type docs.',
+        'secrets',
+        aliases=['secret'],
+        help='List registered secrets and credentials',
+        description='List all of your registered secrets and credentials. Each '
+        'listed secret will be added to your run automatically. For details on '
+        'exactly how each type of secret is added to your run, look to the '
+        'individual secret type docs.',
         epilog=SECRET_EXAMPLES,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    configure_secret_argparser(secrets_parser, secret_handler=create_new_secret)
-    # Secret creation only happens through subparsers, so just print help if a subparser isn't specified
-    secrets_parser.set_defaults(func=lambda **kwargs: secrets_parser.print_help())
+    add_common_arguments(secrets_parser)
+    secrets_parser.set_defaults(func=cli_get_secrets)
+    secrets_parser.add_argument('--type',
+                                choices=["all"] + [i.name for i in SecretType if i != SecretType.generic],
+                                default="all",
+                                dest='secret_type',
+                                help='Filter and show only secrets of this type')
+    secrets_parser.add_argument('--ids',
+                                action='store_true',
+                                dest='include_ids',
+                                default=config.ADMIN_MODE,
+                                help='Include the secret ids in the output')
+    runs_parser = get_runs_argparser(subparsers)
+    add_common_arguments(runs_parser)
+    deployments_parser = get_deployments_argparser(subparsers)
+    add_common_arguments(deployments_parser)
 
     return parser
 
 
-def add_create_argparser(subparser: argparse._SubParsersAction,) -> argparse.ArgumentParser:
-    create_parser: argparse.ArgumentParser = subparser.add_parser(
-        'create',
-        help='Create an MCLI object. See `mcli create -h` for available objects',
-        description='Create an MCLI object. These objects assist in running your workloads in various ways.',
+def add_get_argparser(subparser: argparse._SubParsersAction,
+                      is_admin: bool = False,
+                      parents: Optional[List[argparse.ArgumentParser]] = None) -> argparse.ArgumentParser:
+    """Adds the get parser to a subparser
+
+    Args:
+        subparser: the Subparser to add the Get parser to
+    """
+    del parents
+
+    get_parser: argparse.ArgumentParser = subparser.add_parser(
+        'get',
+        aliases=['g'],
+        help='Get info about objects created with mcli',
     )
-    create_parser = configure_argparser(parser=create_parser)
-    return create_parser
+    get_parser = configure_argparser(parser=get_parser, is_admin=is_admin)
+    return get_parser
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_delete/m_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,26 @@
 """ m delete Entrypoint """
 import argparse
 from typing import List, Optional
 
 from mcli.cli.common.run_filters import configure_submission_filter_argparser
-from mcli.cli.m_delete.delete import (delete_cluster, delete_deployment, delete_environment_variable, delete_run,
-                                      delete_secret)
-from mcli.config import FeatureFlag, MCLIConfig
+from mcli.cli.m_delete.delete import delete_deployment, delete_run, delete_secret
 from mcli.utils.utils_cli import CLIExample, Description, SubmissionType, get_example_text
 
 # pylint: disable-next=invalid-name
 _description = Description("""
 The table below shows the objects that you can delete. For each object below, you can
 delete or more of them by name. Each object also supports glob-style selection and --all
 to delete all.
 
 To view object-specific additional help, run:
 
 mcli delete <object> --help
 """)
 
-_cluster_description = Description("""
-Remove cluster(s) from your setup. This prevents you from launching runs on any of their
-instances.
-""")
-_cluster_example_all = CLIExample(example='mcli delete clusters rXzX rXzY', description='Delete multiple clusters')
-_CLUSTER_EXAMPLES = [
-    _cluster_example_all,
-    CLIExample(example='mcli delete clusters rXz*', description='Delete clusters that match a pattern'),
-    CLIExample(example='mcli delete clusters --all', description='Delete all clusters'),
-]
-
-_env_description = Description("""
-Delete one or more environment variables from your standard workload setup.
-""")
-_env_example_all = CLIExample(example='mcli delete env FOO', description='Delete an environment variable FOO')
-_env_examples = [
-    _env_example_all,
-    CLIExample(example='mcli delete envs FOO BAR', description='Delete multiple environment variables'),
-    CLIExample(example='mcli delete envs --all', description='Delete all environment variables'),
-]
-
 _secret_description = Description("""
 Delete one or more secrets from your standard workload setup. These secrets will be
 removed completely from the secrets database and no longer added to any subsequent runs.
 """)
 _secret_example_all = CLIExample(example='mcli delete secrets foo bar', description='Delete secrets foo and bar')
 _secret_examples = [
     CLIExample(example='mcli delete secret foo', description='Delete a secret named foo'),
@@ -72,18 +49,15 @@
 _deployments_example_simple = CLIExample(example='mcli delete deployment deployment-name',
                                          description='Delete a specific deployment')
 _deployments_example_all = CLIExample(example='mcli delete deployment --all',
                                       description='Delete all deployments (Please be careful!)')
 
 _deployments_examples = [_deployments_example_all, _deployments_example_simple]
 
-_all_examples = [
-    _cluster_example_all, _env_example_all, _secret_example_all, _run_example_simple, _run_example_status,
-    _deployments_example_all
-]
+_all_examples = [_secret_example_all, _run_example_simple, _run_example_status, _deployments_example_all]
 
 
 def delete(parser, **kwargs) -> int:
     del kwargs
     parser.print_help()
     return 0
 
@@ -93,61 +67,21 @@
                         '--force',
                         dest='force',
                         action='store_true',
                         help='Skip confirmation dialog before deleting. Please be careful!')
 
 
 def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    conf = MCLIConfig.load_config(safe=True)
     subparsers = parser.add_subparsers(
         title='MCLI Objects',
         help='DESCRIPTION',
         metavar='OBJECT',
     )
     parser.set_defaults(func=delete, parser=parser)
 
-    if not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-        cluster_parser = subparsers.add_parser(
-            'cluster',
-            aliases=['clusters', 'platform', 'platforms'],
-            help='Delete one or more clusters',
-            description=_cluster_description,
-            epilog=get_example_text(*_CLUSTER_EXAMPLES),
-            formatter_class=argparse.RawDescriptionHelpFormatter,
-        )
-        cluster_parser.add_argument(
-            'cluster_names',
-            nargs='*',
-            metavar='CLUSTER',
-            help='The name of the cluster(s) to delete. Also supports glob-style pattern matching')
-        cluster_parser.add_argument('-a', '--all', dest='delete_all', action='store_true', help='Delete all clusters')
-        cluster_parser.set_defaults(func=delete_cluster)
-        add_common_args(cluster_parser)
-
-    environment_parser = subparsers.add_parser(
-        'env',
-        aliases=['envs'],
-        help='Delete one or more environment variables',
-        description=_env_description,
-        epilog=get_example_text(*_env_examples),
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    environment_parser.add_argument(
-        'variable_names',
-        nargs='*',
-        metavar='ENV',
-        help='The name(s) of the environment variable(s) to delete. Also supports glob-style pattern matching')
-    environment_parser.add_argument('-a',
-                                    '--all',
-                                    dest='delete_all',
-                                    action='store_true',
-                                    help='Delete all environment variables')
-    environment_parser.set_defaults(func=delete_environment_variable)
-    add_common_args(environment_parser)
-
     secrets_parser = subparsers.add_parser(
         'secret',
         aliases=['secrets'],
         help='Delete one or more secrets',
         description=_secret_description,
         epilog=get_example_text(*_secret_examples),
         formatter_class=argparse.RawDescriptionHelpFormatter,
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 from rich.table import Table
 
-from mcli.api.exceptions import KubernetesException, MAPIException, MCLIConfigError
+from mcli.api.exceptions import MAPIException, MCLIConfigError
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table
 from mcli.config import MESSAGE
 from mcli.sdk import InferenceDeployment
 from mcli.utils.utils_logging import FAIL, FormatString, format_string
 
 logger = logging.getLogger(__name__)
@@ -93,15 +93,15 @@
     """
     del kwargs
 
     deployments: List[InferenceDeployment] = []
     try:
         name_filter = [deployment_name] if deployment_name else None
         deployments = get_deployments_with_filters(name_filter=name_filter, latest=True)
-    except (KubernetesException, MAPIException, RuntimeError) as e:
+    except (MAPIException, RuntimeError) as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MCLIConfigError:
         logger.error(MESSAGE.MCLI_NOT_INITIALIZED)
 
     if len(deployments) == 0:
         logger.error(f'No inference deployments found for name: {deployment_name}')
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_log/m_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,129 +4,98 @@
 import argparse
 import logging
 import os
 import sys
 from http import HTTPStatus
 from typing import Optional
 
-from kubernetes.client.exceptions import ApiException
-
-from mcli.api.exceptions import KubernetesException, MAPIException
+from mcli.api.exceptions import MAPIException
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
-from mcli.config import MESSAGE, FeatureFlag, MCLIConfig, MCLIConfigError
-from mcli.models.mcli_cluster import Cluster
-from mcli.sdk import Run, delete_runs, follow_run_logs, get_run_logs, get_runs
-from mcli.utils.utils_epilog import CommonLog, EpilogSpinner, RunEpilog
-from mcli.utils.utils_logging import FAIL, INFO, console, err_console
-from mcli.utils.utils_run_status import PodStatus, RunStatus
+from mcli.config import MESSAGE, MCLIConfigError
+from mcli.sdk import Run, follow_run_logs, get_run_logs, get_runs
+from mcli.utils.utils_epilog import CommonLog
+from mcli.utils.utils_logging import FAIL, INFO, err_console
+from mcli.utils.utils_run_status import RunStatus
 
 logger = logging.getLogger(__name__)
 
 
 def get_latest_run() -> Run:
     """Retrieve the latest run for the user
     """
     runs = get_runs(future=False)
     if not runs:
-        raise KubernetesException(status=HTTPStatus.NOT_FOUND, message='No runs found')
+        raise MAPIException(status=HTTPStatus.NOT_FOUND, message='No runs found')
     return sorted(runs, key=lambda x: x.created_at, reverse=True)[0]
 
 
 # pylint: disable-next=too-many-statements
 def get_logs(
     run_name: Optional[str] = None,
     rank: Optional[int] = None,
     follow: bool = False,
     failed: bool = False,
     **kwargs,
 ) -> int:
     del kwargs
 
     try:
-        # Verify that the user has initialized their config
-        conf: MCLIConfig = MCLIConfig.load_config(safe=True)
-
         run: Optional[Run] = None
         with err_console.status('Getting run details...') as spinner:
             if run_name is None:
                 spinner.update('No run name provided. Finding latest run...')
                 run = get_latest_run()
                 logger.info(f'{INFO} No run name provided. Displaying log of latest run: [cyan]{run.name}[/]')
             else:
                 runs = get_runs(runs=[run_name])
                 if not runs:
-                    raise KubernetesException(status=HTTPStatus.NOT_FOUND,
-                                              message=f'Could not find run: [red]{run_name}[/]')
+                    raise MAPIException(status=HTTPStatus.NOT_FOUND, message=f'Could not find run: [red]{run_name}[/]')
                 run = runs[0]
 
         if follow and run.status.before(RunStatus.RUNNING):
-            timeout = 300
-            if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-                with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
-                    run = watcher.follow()
-            else:
-                with Cluster.use(run.config.cluster) as cluster:
-                    # Pod is creating, so let's use an epilog
-                    logger.info(f'{INFO} Waiting for run to start, press Ctrl+C to quit')
-                    epilog = RunEpilog(run.name, cluster.namespace)
-                    status: Optional[PodStatus] = None
-                    with EpilogSpinner() as spinner:
-                        status = epilog.wait_until(callback=spinner, timeout=timeout)
-                    if status is None:
-                        # Pod epilog timed out
-                        logger.info(f'{INFO} Run {run.name} did not start within {timeout} seconds. Try again later.')
-                        return 1
-                    run.status = status.state
+            with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
+                run = watcher.follow()
+
         if run.status == RunStatus.FAILED_PULL:
             CommonLog(logger).log_pod_failed_pull(run.name, run.config.image)
-            if not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-                with console.status('Deleting failed run...'):
-                    delete_runs([run])
             return 1
         elif run.status.before(RunStatus.QUEUED, inclusive=True):
             # Pod still waiting to be scheduled. Return
             logger.error(f'{FAIL} Run {run.name} has not been scheduled')
             return 1
         elif run.status.before(RunStatus.RUNNING):
             # Pod still not running, probably because follow==False
             logger.error(f'{FAIL} Run has not yet started. You can check the status with `mcli get runs` '
                          'and try again later.')
             return 1
 
         last_line: Optional[str] = None
-        end: str = '' if conf.feature_enabled(FeatureFlag.USE_MCLOUD) else '\n'
+        end: str = ''
         if follow:
             for line in follow_run_logs(run, rank=rank, timeout=300):
                 print(line, end=end)
                 if line:
                     last_line = line
         else:
-            if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-                log_lines = get_run_logs(run, rank=rank, timeout=300, failed=failed)
-            else:
-                log_lines = get_run_logs(run, rank=rank, timeout=300, failed=failed).split('\n')
+            log_lines = get_run_logs(run, rank=rank, timeout=300, failed=failed)
 
             for line in log_lines:
                 # When using progress bars we randomly get newlines added. By default,
                 # kubernetes does not return empty lines when streaming, which is
                 # replicated in `follow_run_logs`. We'll do that here for parity
                 if line:
                     last_line = line
                     print(line, end=end)
 
         # Progress bars are weird. Let's add a final newline so that if the printing
         # ends on an incompleted progress bar, it isn't erased
         if last_line and (last_line.endswith('\x1B[A') or end == ''):
             print('', file=sys.stderr)
 
-    except (KubernetesException, MAPIException) as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except ApiException as e:
-        e = KubernetesException.transform_api_exception(e)
+    except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except RuntimeError as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MCLIConfigError:
         logger.error(MESSAGE.MCLI_NOT_INITIALIZED)
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_run/m_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """ mcli run Entrypoint """
 import argparse
 import logging
 import textwrap
 from http import HTTPStatus
 from typing import Optional
 
-from mcli.api.exceptions import KubernetesException, MAPIException, MCLIConfigError, MCLIRunConfigValidationError
-from mcli.api.kube.runs import create_run as kube_create_run
-from mcli.api.kube.runs import delete_runs
-from mcli.api.runs import create_run
+from mcli.api.exceptions import MAPIException, cli_error_handler
+from mcli.api.runs import create_run, delete_runs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
-from mcli.config import FeatureFlag, MCLIConfig
-from mcli.models.mcli_cluster import Cluster
+from mcli.config import MCLIConfig
 from mcli.models.run_config import VALID_OPTIMIZATION_LEVELS
 from mcli.sdk import Run, RunConfig, follow_run_logs, get_run, wait_for_run_status
-from mcli.serverside.clusters.cluster import InvalidPriorityError
-from mcli.serverside.clusters.cluster_instances import InstanceTypeUnavailable
-from mcli.utils.utils_epilog import CommonLog, EpilogSpinner, RunEpilog
-from mcli.utils.utils_logging import FAIL, INFO, OK
+from mcli.utils.utils_epilog import CommonLog
+from mcli.utils.utils_logging import INFO, OK
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
 
 
 def print_help(**kwargs) -> int:
@@ -30,63 +25,54 @@
     _configure_parser(mock_parser)
     mock_parser.print_help()
     return 1
 
 
 def follow_run(run: Run) -> int:
     final_config = run.config
-    conf = MCLIConfig.load_config(safe=True)
     last_status: Optional[RunStatus] = None
-    if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-        with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
-            run = watcher.follow()
-            last_status = run.status
-    else:
-        with Cluster.use(final_config.cluster) as cluster:
-            logger.info(f'{INFO} Run [cyan]{run.name}[/] submitted. Waiting for it to start...')
-            logger.info(f'{INFO} You can press Ctrl+C to quit and follow your run manually.')
-            epilog = RunEpilog(run.name, cluster.namespace)
-            with EpilogSpinner() as spinner:
-                state = epilog.wait_until(callback=spinner, timeout=300)
-                last_status = state.state if state else None
+
+    with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
+        run = watcher.follow()
+        last_status = run.status
 
     # Wait timed out
     common_log = CommonLog(logger)
     if last_status is None:
         common_log.log_timeout()
         return 0
     elif last_status == RunStatus.FAILED_PULL:
         common_log.log_pod_failed_pull(run.name, final_config.image)
-        if not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-            with console_status('Deleting failed run...'):
-                delete_runs([run])
+        with console_status('Deleting failed run...'):
+            delete_runs([run])
         return 1
     elif last_status == RunStatus.FAILED:
         common_log.log_pod_failed(run.name)
         return 1
     elif last_status.before(RunStatus.RUNNING):
         common_log.log_unknown_did_not_start()
         logger.debug(last_status)
         return 1
 
     logger.info(f'{OK} Run [cyan]{run.name}[/] started')
     logger.info(f'{INFO} Following run logs. Press Ctrl+C to quit.\n')
 
-    end = '' if conf.feature_enabled(FeatureFlag.USE_MCLOUD) else '\n'
+    end = ''
     for line in follow_run_logs(run, rank=0):
         print(line, end=end)
     if not end:
         print('')
 
     wait_for_run_status(run, status=RunStatus.COMPLETED, timeout=10)
 
     return 0
 
 
 # pylint: disable-next=too-many-statements
+@cli_error_handler('mcli run')
 def run_entrypoint(
     file: Optional[str] = None,
     clone: Optional[str] = None,
     follow: bool = True,
     override_cluster: Optional[str] = None,
     override_gpu_type: Optional[str] = None,
     override_gpu_num: Optional[int] = None,
@@ -96,108 +82,73 @@
     override_priority: Optional[str] = None,
     override_nodes: Optional[int] = None,
     override_instance: Optional[str] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
-    cluster_name: Optional[str] = None
-    try:
-        if file:
-            run_config = RunConfig.from_file(path=file)
-        elif clone:
-            found_run = get_run(clone)
-            if found_run.submitted_config is None:
-                raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {clone}")
-            run_config = found_run.submitted_config
-        else:
-            return print_help()
-
-        # command line overrides
-        # only supports basic format for now and not structured params
-        if override_cluster is not None:
-            run_config.compute['cluster'] = override_cluster
-
-        if override_gpu_type is not None:
-            run_config.compute['gpu_type'] = override_gpu_type
-
-        if override_gpu_num is not None:
-            run_config.compute['gpus'] = override_gpu_num
-
-        if override_image is not None:
-            run_config.image = override_image
-
-        if override_name is not None:
-            run_config.name = override_name
-
-        if override_optimization_level is not None:
-            run_config.optimization_level = override_optimization_level
-
-        if override_priority is not None:
-            run_config.scheduling['priority'] = override_priority
-
-        if override_instance is not None:
-            run_config.compute['instance'] = override_instance
-
-        if override_nodes is not None:
-            run_config.compute['nodes'] = override_nodes
-
-        conf = MCLIConfig.load_config(safe=True)
-
-        with console_status('Submitting run...'):
-            if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-                # TODO: Move this out when legacy priority is removed
-
-                run = create_run(run=run_config, timeout=None)
-            else:
-                run = kube_create_run(run=run_config,
-                                      _priority=run_config.scheduling.get('priority', None),
-                                      timeout=None)
-        cluster_name = run.config.cluster
-
-        if not follow:
-            log_cmd = f'mcli logs {run.name}'
-            message = f"""
-            {OK} Run [cyan]{run.name}[/] submitted.
-
-            To see the run\'s status, use:
-
-            [bold]mcli get runs[/]
-
-            To see the run\'s logs, use:
-
-            [bold]{log_cmd}[/]
-            """
-            logger.info(textwrap.dedent(message).strip())
-            return 0
-        else:
-            return follow_run(run)
+    if file:
+        run_config = RunConfig.from_file(path=file)
+    elif clone:
+        run = get_run(clone)
+        if run.submitted_config is None:
+            raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {clone}")
+        run_config = run.submitted_config
+    else:
+        return print_help()
 
-    except (MAPIException, KubernetesException) as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except (InstanceTypeUnavailable) as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except (MCLIRunConfigValidationError) as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except (MCLIConfigError) as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except InvalidPriorityError as e:
-        e.cluster = cluster_name
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except RuntimeError as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except FileNotFoundError as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
+    # command line overrides
+    # only supports basic format for now and not structured params
+    if override_cluster is not None:
+        run_config.cluster = override_cluster
+
+    if override_gpu_type is not None:
+        run_config.gpu_type = override_gpu_type
+
+    if override_gpu_num is not None:
+        run_config.gpu_num = override_gpu_num
+
+    if override_image is not None:
+        run_config.image = override_image
+
+    if override_name is not None:
+        run_config.name = override_name
+
+    if override_optimization_level is not None:
+        run_config.optimization_level = override_optimization_level
+
+    if override_priority is not None:
+        run_config.scheduling['priority'] = override_priority
+
+    if override_instance is not None:
+        run_config.compute['instance'] = override_instance
+
+    if override_nodes is not None:
+        run_config.compute['nodes'] = override_nodes
+
+    with console_status('Submitting run...'):
+        run = create_run(run=run_config, timeout=None)
+
+    if not follow:
+        log_cmd = f'mcli logs {run.name}'
+        message = f"""
+        {OK} Run [cyan]{run.name}[/] submitted.
+
+        To see the run\'s status, use:
+
+        [bold]mcli get runs[/]
+
+        To see the run\'s logs, use:
+
+        [bold]{log_cmd}[/]
+        """
+        logger.info(textwrap.dedent(message).strip())
+        return 0
+    else:
+        return follow_run(run)
 
 
 def add_run_argparser(subparser: argparse._SubParsersAction) -> None:
     run_parser: argparse.ArgumentParser = subparser.add_parser(
         'run',
         aliases=['r'],
         help='Launch a run in the MosaicML platform',
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ mcli set Entrypoint """
 import argparse
 
 from mcli.cli.m_set_unset.api_key import configure_api_key_argparser, modify_api_key
+from mcli.cli.m_set_unset.feature_flag import use_feature_flag
 from mcli.cli.m_set_unset.user import configure_user_argparser, modify_user
-from mcli.cli.m_use.m_use import use_feature_flag
 
 
 def set_entrypoint(**kwargs):
     del kwargs
     mock_parser = configure_argparser(parser=argparse.ArgumentParser())
     mock_parser.print_help()
     return 0
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/m_unset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ mcli unset Entrypoint """
 import argparse
 
+from mcli.cli.m_set_unset.feature_flag import use_feature_flag
 from mcli.cli.m_set_unset.user import modify_user
-from mcli.cli.m_use.m_use import use_feature_flag
 
 
 def unset_entrypoint(**kwargs):
     del kwargs
     mock_parser = configure_argparser(parser=argparse.ArgumentParser())
     mock_parser.print_help()
     return 0
```

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a0/mcli/cli/m_util/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,34 @@
 from rich.style import Style
 from rich.table import Table
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIErrorMessages, MAPIException, cli_error_handler
 from mcli.api.model.cluster_details import ClusterDetails, ClusterUtilizationByRun
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay
-from mcli.cli.m_util.kube_util import get_row_color
 from mcli.utils.utils_logging import print_timedelta
 
 logger = logging.getLogger(__name__)
 
 
+def get_row_color(node: dict) -> Optional[str]:
+    """Get the row color using the serialized NodeInfo data
+    """
+    gpus_used = int(node.get("gpus_used", 0))
+    gpus_available = int(node.get("gpus_available", 0))
+
+    if gpus_used == 0 and gpus_available == 0:
+        return "bright_black"  # gray
+
+    if gpus_available > 0:
+        return "green"
+
+    return None
+
+
 @dataclass
 class UtilizationInfo(MCLIDisplayItem):
     pos: int
     name: str
     run_name: str
     user: str
     age: str
```

### Comparing `mosaicml-cli-0.3.9/mcli/config.py` & `mosaicml-cli-0.4.0a0/mcli/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Global Singleton Config Store"""
 from __future__ import annotations
 
 import logging
 import os
 from dataclasses import asdict, dataclass, field
-from datetime import datetime, timedelta
+from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set
 
 import ruamel.yaml
 import yaml
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 
 from mcli.api.exceptions import MCLIConfigError
-from mcli.models import Cluster, MCLIEnvVar
-from mcli.utils.utils_modules import check_if_module_exists
+from mcli.models import Cluster
 from mcli.utils.utils_serializable_dataclass import SerializableDataclass
 from mcli.utils.utils_yaml import StringDumpYAML
 
 logger = logging.getLogger(__name__)
 
 
 def env_path_override_config(config_value: str):
@@ -55,21 +54,16 @@
 
 MCLI_CONFIG_PATH: Path = MCLI_CONFIG_DIR / 'mcli_config'
 env_path_override_config('MCLI_CONFIG_PATH')
 
 MCLI_KUBECONFIG: Path = MCLI_CONFIG_DIR / 'kube_config'
 env_path_override_config('MCLI_KUBECONFIG')
 
-COMPOSER_INSTALLED: bool = check_if_module_exists('composer')
-
 UPDATE_CHECK_FREQUENCY_DAYS: float = 2
 
-PAGER_LIMIT: int = 50  # When `mcli get` returns more than PAGER_LIMIT entries, a pager should be used
-
-JOB_TTL: int = int(timedelta(days=14).total_seconds())
 MCLI_MODE_ENV: str = 'MCLI_MODE'
 env_str_override_config(MCLI_MODE_ENV)
 
 MCLI_INTERACTIVE_ENV: str = 'MCLI_INTERACTIVE'
 env_str_override_config(MCLI_INTERACTIVE_ENV)
 
 MCLI_TIMEOUT_ENV = 'MCLI_TIMEOUT'
@@ -77,18 +71,14 @@
 
 MCLI_DISABLE_UPGRADE_CHECK_ENV: str = 'MCLI_DISABLE_UPGRADE_CHECK'
 env_str_override_config(MCLI_DISABLE_UPGRADE_CHECK_ENV)
 
 # Used for local dev and testing
 MOSAICML_API_KEY_ENV: str = 'MOSAICML_API_KEY'
 
-SUPPORT_TOKEN_KEY_ENV: str = 'MOSAICML_SUPPORT_TOKEN_KEY'
-
-MCLOUD_OBSCURE_FALLBACK: str = 'PLEASE_NO_MCLOUD_THANKS'
-
 logging.getLogger('urllib3.connectionpool').disabled = True
 
 logger = logging.getLogger(__name__)
 
 ADMIN_MODE = False
 
 
@@ -101,56 +91,42 @@
     return default_timeout
 
 
 class FeatureFlag(Enum):
     """Enum for mcli feature flags
     """
     ALPHA_TESTER = 'ALPHA_TESTER'
-    MLPERF_MODE = 'MLPERF_MODE'
-    USE_DEMO_NODES = 'USE_DEMO_NODES'
-    USE_MCLOUD = 'USE_MCLOUD'
-
     MCLOUD_INTERACTIVE = 'MCLOUD_INTERACTIVE'
 
-    def validate_compatibility(self) -> None:
-        conf = MCLIConfig.load_config(safe=True)
-        if self == FeatureFlag.USE_DEMO_NODES and conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-            raise MCLIConfigError(Messages.INVALID_FEATURES_DEMO_NODES_AND_MCLOUD)
-        if self == FeatureFlag.USE_MCLOUD and conf.feature_enabled(FeatureFlag.USE_DEMO_NODES):
-            raise MCLIConfigError(Messages.INVALID_FEATURES_MCLOUD_AND_DEMO_NODES)
-
     @staticmethod
     def get_external_features() -> Set[FeatureFlag]:
-        return {FeatureFlag.USE_MCLOUD}
+        return set()
 
 
 class MCLIMode(Enum):
     """Enum for mcli user modes
     """
     PROD = 'PROD'
     DEV = 'DEV'
     INTERNAL = 'INTERNAL'
     LOCAL = 'LOCAL'
     LEGACY = 'LEGACY'
     STAGING = 'STAGING'
 
+    def is_legacy(self) -> bool:
+        """True if this mode is a legacy mode
+        """
+        return self == MCLIMode.LEGACY
+
     def is_internal(self) -> bool:
         """True if this mode is an internal mode
         """
         internal_modes = {MCLIMode.DEV, MCLIMode.INTERNAL, MCLIMode.LOCAL, MCLIMode.STAGING}
         return self in internal_modes
 
-    def is_mcloud_enabled(self) -> bool:
-        """True if this mode is enabled use with mcloud
-        """
-        mcloud_disabled = {
-            MCLIMode.LEGACY,
-        }
-        return self not in mcloud_disabled
-
     def available_feature_flags(self) -> List[FeatureFlag]:
         if self.is_internal():
             # All features are available to internal users
             return list(FeatureFlag)
 
         return list(FeatureFlag.get_external_features())
 
@@ -207,17 +183,14 @@
 
     # set to default for now to not break existing users' configs
     MOSAICML_API_KEY: str = ''  # pylint: disable=invalid-name Global Stored within Singleton
 
     feature_flags: Dict[str, bool] = field(default_factory=dict)
     last_update_check: datetime = field(default_factory=datetime.now)
 
-    # Global Environment Variables
-    environment_variables: List[MCLIEnvVar] = field(default_factory=list)
-
     # Registered Clusters
     clusters: List[Cluster] = field(default_factory=list)
 
     # MCloud environments w/ API keys
     # Most users will be in PROD, so this will likely only be touched internally
     mcloud_envs: Dict[str, str] = field(default_factory=dict)
 
@@ -237,18 +210,14 @@
 
     @classmethod
     def empty(cls) -> MCLIConfig:
         conf = MCLIConfig()
         return conf
 
     @property
-    def dev_mode(self) -> bool:
-        return self.mcli_mode == MCLIMode.DEV
-
-    @property
     def internal(self) -> bool:
         return self.mcli_mode.is_internal()
 
     @property
     def mcli_mode(self) -> MCLIMode:
         return MCLIMode.from_env()
 
@@ -308,45 +277,36 @@
             return api_key_env
         elif self.mcli_mode.is_alternate():
             return self.mcloud_envs.get(self.mcli_mode.value, '')
         elif self.MOSAICML_API_KEY:
             return self.MOSAICML_API_KEY
         return ''
 
-    @staticmethod
-    def _remove_deprecated_cluster_details(clusters: List[Dict[str, str]]) -> List[Dict[str, str]]:
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.serverside.clusters.cluster import GenericK8sCluster
-
-        valid_clusters: List[Dict[str, str]] = []
-        for cluster in clusters:
-            if cluster.get('kubernetes_context', '').endswith('research-01'):
-                continue
-            if 'kubernetes_context' in cluster and cluster[
-                    'kubernetes_context'] not in GenericK8sCluster.get_k8s_context_map():
-                continue
-            if 'environment_overrides' in cluster:
-                del cluster['environment_overrides']
-            valid_clusters.append(cluster)
-        return valid_clusters
-
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> MCLIConfig:
         # TODO: Remove after full deprecation transition
         if 'dev_mode' in data:
             del data['dev_mode']
         if 'internal' in data:
             del data['internal']
         # TODO(END): Remove after full deprecation transition
 
         # Backwards compatibility: platforms should be synonymous with clusters
         if 'platforms' in data:
             data['clusters'] = data['platforms']
             del data['platforms']
-        data['clusters'] = cls._remove_deprecated_cluster_details(data.get('clusters', []))
+
+        if 'environment_variables' in data:
+            del data['environment_variables']
+
+        data['clusters'] = []
+
+        # Remove any unknown feature flags
+        known_feature_flags = {f.value for f in FeatureFlag}
+        data['feature_flags'] = {k: v for k, v in data.get('feature_flags', {}).items() if k in known_feature_flags}
 
         return super().from_dict(data)
 
     @classmethod
     def load_config(cls, safe: bool = False) -> MCLIConfig:
         """Loads the MCLIConfig from local disk
 
@@ -389,65 +349,29 @@
         return True
 
     def _get_formatted_dump(self) -> CommentedMap:
         """Gets the ruamel yaml formatted dump of the config
         """
         raw_data = self.to_disk()
 
-        # Moves clusters to last item
-        clusters = raw_data['clusters']
+        # Remove clusters
         del raw_data['clusters']
-        raw_data['clusters'] = clusters
-
-        # Remove invalid clusters
 
         data: CommentedMap = ruamel.yaml.load(
             yaml.dump(raw_data),
             ruamel.yaml.RoundTripLoader,
         )
-        data.yaml_set_start_comment('MCLI Config Data\n')
-        data.yaml_set_comment_before_after_key(
-            key='environment_variables',
-            before='\nAll Global Environment variables go here',
-        )
-        data.yaml_set_comment_before_after_key(
-            key='clusters',
-            before='\nAll Clusters configured for MCLI',
-        )
         return data
 
-    @property
-    def mcloud_enabled(self) -> bool:
-        if os.environ.get(MCLOUD_OBSCURE_FALLBACK, "FALSE").upper() == "TRUE":
-            # Disabled if the obscure fallback env var is on
-            return False
-
-        if not self.mcli_mode.is_mcloud_enabled():
-            # Disabled if MCloud is disabled for the mode
-            return False
-
-        if self.internal:
-            # All internal users should otherwise be enabled
-            return True
-
-        if self.mcli_mode == MCLIMode.PROD:
-            # Prod users check feature flag
-            return self.feature_flags.get(FeatureFlag.USE_MCLOUD.value, True)
-
-        return False
-
     def feature_enabled(self, feature: FeatureFlag) -> bool:
         """Checks if the feature flag is enabled
 
         Args:
             feature (FeatureFlag): The feature to check
         """
-        if feature is FeatureFlag.USE_MCLOUD:
-            # Handle complicated mcloud enabling logic elsewhere
-            return self.mcloud_enabled
 
         if not self.internal and feature not in FeatureFlag.get_external_features():
             # Only enable select features for external use
             return False
 
         if feature.value in self.feature_flags:
             enabled = self.feature_flags.get(feature.value, False)
@@ -466,18 +390,9 @@
     return conf.feature_enabled(feature=feature)
 
 
 class Messages():
     MCLI_NOT_INITIALIZED = 'MCLI not yet initialized. Please run `mcli init` first.'
     API_KEY_MISSING = 'No API key found. Please create one and set it using `mcli set api-key`.'
 
-    INVALID_FEATURES_DEMO_NODES_AND_MCLOUD = (
-        f'{FeatureFlag.USE_DEMO_NODES.value} feature cannot be set when the {FeatureFlag.USE_MCLOUD.value}'
-        f' feature is already activated. Run `mcli unset feature {FeatureFlag.USE_MCLOUD.value}` before trying to'
-        ' use demo nodes feature')
-    INVALID_FEATURES_MCLOUD_AND_DEMO_NODES = (
-        f'{FeatureFlag.USE_MCLOUD.value} feature cannot be set when the {FeatureFlag.USE_DEMO_NODES.value}'
-        f' feature is already activated. Run `mcli unset feature {FeatureFlag.USE_DEMO_NODES.value}`'
-        ' before trying to use MCLOUD')
-
 
 MESSAGE = Messages()
```

### Comparing `mosaicml-cli-0.3.9/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a0/mcli/api/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ Reimport all MCLI Models """
 # pylint: disable=useless-import-alias
+from mcli.api.model.inference_deployment import InferenceDeployment as InferenceDeployment
+from mcli.api.model.run import Run as Run
 from mcli.models.mcli_cluster import Cluster as Cluster
 from mcli.models.mcli_envvar import MCLIEnvVar as MCLIEnvVar
-from mcli.models.mcli_integration import IntegrationType as IntegrationType
-from mcli.models.mcli_integration import MCLIIntegration as MCLIIntegration
 from mcli.models.mcli_secret import SECRET_MOUNT_PATH_PARENT as SECRET_MOUNT_PATH_PARENT
 from mcli.models.mcli_secret import MCLIGenericSecret as MCLIGenericSecret
 from mcli.models.mcli_secret import Secret as Secret
 from mcli.models.mcli_secret import SecretType as SecretType
-from mcli.models.run_config import ComputeConfig as ComputeConfig
 from mcli.models.run_config import FinalRunConfig as FinalRunConfig
 from mcli.models.run_config import RunConfig as RunConfig
 from mcli.models.run_config import SchedulingConfig as SchedulingConfig
 
 #pylint: disable=line-too-long
 from mcli.models.inference_deployment_config import InferenceDeploymentConfig as InferenceDeploymentConfig  # isort: skip
 from mcli.models.inference_deployment_config import FinalInferenceDeploymentConfig as FinalInferenceDeploymentConfig  # isort: skip
```

### Comparing `mosaicml-cli-0.3.9/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a0/mcli/models/inference_deployment_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional
 
 import yaml
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
-from mcli.models.run_config import _clean_run_name, _validate_cluster_exists
+from mcli.models.run_config import _clean_run_name
 from mcli.utils.utils_config import BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, uuid_generator
 from mcli.utils.utils_string_functions import validate_image
 
 logger = logging.getLogger(__name__)
 
 DEPLOYMENT_CONFIG_UID_LENGTH = 6
 
@@ -101,17 +101,14 @@
         Returns:
             :class:`~mcli.models.deployment_config.FinalDeploymentConfig`:The object created using values from the input
         Raises:
             :class:`~mcli.api.exceptions.MCLIConfigError`: If MCLI config is not present or is missing information
             :class:`~mcli.api.exceptions.MCLIDeploymentConfigValidationError`: If deployment_config is not valid
         """
 
-        if deployment_config.cluster:
-            _validate_cluster_exists(deployment_config.cluster)
-
         model_as_dict = asdict(deployment_config)
 
         missing_fields = [field for field, value in model_as_dict.items() if value is None]
         for missing in missing_fields:
             model_as_dict.pop(missing, None)
 
         # required for FinalDeploymentConfig, even though not required for mcloud
```

### Comparing `mosaicml-cli-0.3.9/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a0/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a0/mcli/models/mcli_secret.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """ MCLI Abstraction for Secrets """
 from __future__ import annotations
 
 import functools
-from abc import ABC, abstractmethod
-from dataclasses import asdict, dataclass
+from abc import ABC
+from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar
+from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 import yaml
 
 from mcli.api.exceptions import MAPI_DESERIALIZATION_ERROR
 from mcli.api.schema.generic_model import DeserializableModel
-from mcli.models import Cluster
-from mcli.serverside.job.mcli_k8s_job import MCLIK8sJob
-from mcli.utils.utils_kube import base64_decode, base64_encode, read_secret
-from mcli.utils.utils_kube_labels import label
 from mcli.utils.utils_serializable_dataclass import SerializableDataclass, T_SerializableDataclass
 from mcli.utils.utils_types import CommonEnum
 
 SECRET_MOUNT_PATH_PARENT = Path('/secrets')
 EnumType = TypeVar('EnumType', bound=Enum)  # pylint: disable=invalid-name
 
 MAPI_TO_MCLI_SECRET_TYPE = {
@@ -110,76 +106,19 @@
 
     def __lt__(self, other: Secret):
         if not isinstance(other, Secret):
             raise TypeError(f'Cannot compare order of ``Secret`` and {type(other)}')
         return self.name > other.name
 
     @property
-    def kubernetes_type(self) -> str:
-        """The corresponding Kubernetes secret type for this class of secrets
-        """
-        return 'Opaque'
-
-    @property
     def mapi_data(self) -> Dict[str, Any]:
         """Data used to create the secret in MAPI
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def add_to_job(self, kubernetes_job: MCLIK8sJob) -> bool:
-        """Add a secret to a job
-        """
-
-    @property
-    def required_packing_fields(self) -> Set[str]:
-        """ All required fields for packing up the secret """
-        return set()
-
-    def unpack(self, data: Dict[str, str]):
-        """Unpack the Kubernetes secret `data` field to fill in required secret values
-
-        All required packing fields must be present.
-        By default looks for all required fields and base64 decodes them
-
-        Args:
-            data (Dict[str, str]): Kubernetes `data` field as a JSON
-        """
-
-        missing_fields = self.required_packing_fields - data.keys()
-        if missing_fields:
-            raise ValueError('Missing required field(s) to unpack Secret: '
-                             f'{",".join(missing_fields)}')
-
-        for field_ in self.required_packing_fields:
-            setattr(self, field_, base64_decode(data[field_]))
-
-    def pack(self) -> Dict[str, str]:
-        """The `data` field for the corresponding kubernetes secret
-        Validated to ensure fully completed
-
-        By default base64 encodes all required fields
-        """
-        filled_fields = asdict(self)
-        data = {k: v for k, v in filled_fields.items() if k in self.required_packing_fields}
-        for key, value in data.items():
-            if not isinstance(value, str):
-                raise TypeError(f'All keys in a secret must be strings, got {key}: {type(value)}')
-            data[key] = base64_encode(value)
-        return data
-
-    def pull(self, cluster: Cluster):
-        with Cluster.use(cluster):
-            # Read the secret if it exists
-            secret = read_secret(self.name, cluster.namespace)
-            if not secret:
-                raise RuntimeError(f'Could not find secret {self.name} in cluster {cluster.name}')
-            assert isinstance(secret['data'], dict)
-            self.unpack(secret['data'])
-
     @classmethod
     def from_dict(cls: Type[T_SerializableDataclass], data: Dict[str, Any]) -> Secret:
         if not isinstance(data, dict):
             raise TypeError(f'Secret data must be structured as a dictionary. Got: {type(data)}')
 
         secret_type_string = data.pop('secret_type', None)
         if not secret_type_string:
@@ -188,30 +127,14 @@
         secret_type = SecretType.ensure_enum(secret_type_string)
         assert isinstance(secret_type, SecretType)
 
         secret = secret_type_to_class(secret_type)(secret_type=secret_type, **data)
         assert isinstance(secret, Secret)
         return secret  # type: ignore
 
-    @property
-    def kubernetes_labels(self) -> Dict[str, str]:
-        """Labels to add to all Kubernetes secrets
-        """
-        labels = {
-            label.mosaic.SECRET_TYPE: self.secret_type.value.replace('_', '-'),
-            **label.mosaic.version.get_version_labels(),
-        }
-        return labels
-
-    @property
-    def kubernetes_annotations(self) -> Dict[str, str]:
-        """Annotations to add to all Kubernetes secrets
-        """
-        return {}
-
     @staticmethod
     def _mapi_required_properties() -> Tuple[str]:
         """Required properties for mapi response"""
         return tuple(['name', 'type', 'metadata'])
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> Secret:
@@ -255,20 +178,7 @@
 
 
 @dataclass
 class MCLIGenericSecret(Secret):
     """Secret class for generic secrets
     """
     value: Optional[str] = None
-
-    @property
-    def disk_skipped_fields(self) -> List[str]:
-        return ['value']
-
-    @property
-    def required_packing_fields(self) -> Set[str]:
-        return set(self.disk_skipped_fields)
-
-    def add_to_job(self, kubernetes_job: MCLIK8sJob) -> bool:
-        del kubernetes_job
-        # Missing context on how it should be added to a job
-        raise NotImplementedError
```

### Comparing `mosaicml-cli-0.3.9/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a0/mcli/models/run_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """ Run Input """
 from __future__ import annotations
 
+import copy
 import logging
+from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Sequence
+from typing import Any, Dict, Generic, List, Optional, Sequence, TypeVar
 
 import yaml
 from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIRunConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
-from mcli.models.mcli_cluster import Cluster
-from mcli.utils.utils_config import (BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, Translation,
-                                     uuid_generator)
-from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, ensure_rfc1123_compatibility, validate_image,
+from mcli.utils.utils_config import BaseSubmissionConfig, uuid_generator
+from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, camel_case_to_snake_case,
+                                               ensure_rfc1123_compatibility, snake_case_to_camel_case, validate_image,
                                                validate_rfc1123_name)
 
 logger = logging.getLogger(__name__)
 RUN_CONFIG_UID_LENGTH = 6
 VALID_OPTIMIZATION_LEVELS = frozenset([0, 1, 2, 3])
 MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
 DEFAULT_PRIORITY_NAME = 'medium'
@@ -263,14 +264,110 @@
 
             translated_input[translated_name] = value
         return {
             'runInput': translated_input,
         }
 
 
+T = TypeVar('T')  # pylint: disable=invalid-name
+U = TypeVar('U')
+
+
+class Translation(ABC, Generic[T, U]):
+    """ABC for MAPI/MCLI translations"""
+
+    @classmethod
+    @abstractmethod
+    def to_mapi(cls, value: T) -> U:
+        ...
+
+    @classmethod
+    @abstractmethod
+    def from_mapi(cls, value: U) -> T:
+        ...
+
+
+class EnvVarTranslation(Translation[List[Dict[str, str]], List[Dict[str, str]]]):
+    """Translate environment variable configs"""
+
+    MAPI_KEY = 'envKey'
+    MAPI_VALUE = 'envValue'
+
+    MCLI_KEY = 'key'
+    MCLI_VALUE = 'value'
+
+    @classmethod
+    def to_mapi(cls, value: List[Dict[str, str]]) -> List[Dict[str, str]]:
+        env_vars = []
+        for env_var in value:
+            try:
+                key = env_var[cls.MCLI_KEY]
+                val = env_var[cls.MCLI_VALUE]
+            except KeyError as e:
+                raise KeyError('Environment variables should be specified as a list '
+                               f'of dictionaries with keys: "{cls.MCLI_KEY}" and "{cls.MCLI_VALUE}". '
+                               f'Got: {", ".join(list(env_var.keys()))}') from e
+
+            env_vars.append({cls.MAPI_KEY: key, cls.MAPI_VALUE: val})
+        return env_vars
+
+    @classmethod
+    def from_mapi(cls, value: List[Dict[str, str]]) -> List[Dict[str, str]]:
+        env_vars = []
+        for env_var in value:
+            try:
+                key = env_var[cls.MAPI_KEY]
+                val = env_var[cls.MAPI_VALUE]
+            except KeyError:
+                logger.warning(f'Received incompatible environment variable: {env_var}')
+                continue
+            env_vars.append({cls.MCLI_KEY: key, cls.MCLI_VALUE: val})
+        return env_vars
+
+
+class IntegrationTranslation(Translation[List[Dict[str, Any]], List[Dict[str, Any]]]):
+    """Translate integration configs"""
+
+    MAPI_TYPE = 'type'
+    MAPI_PARAMS = 'params'
+
+    MCLI_TYPE = 'integration_type'
+
+    @classmethod
+    def to_mapi(cls, value: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+        value = copy.deepcopy(value)
+        integrations_list = []
+        for integration in value:
+            integration_type = integration.pop(cls.MCLI_TYPE)
+
+            translated_integration = {}
+            for param, val in integration.items():
+                # Translate keys to camel case for MAPI parameters
+                translated_key = snake_case_to_camel_case(param)
+                translated_integration[translated_key] = val
+
+            integrations_dict = {cls.MAPI_TYPE: integration_type, cls.MAPI_PARAMS: translated_integration}
+            integrations_list.append(integrations_dict)
+        return integrations_list
+
+    @classmethod
+    def from_mapi(cls, value: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+        integrations_list = []
+        for integration in value:
+            translated_integration = {cls.MCLI_TYPE: integration[cls.MAPI_TYPE]}
+            params = integration.get(cls.MAPI_PARAMS, {})
+            for param, val in params.items():
+                # Translate keys to camel case for MAPI parameters
+                translated_key = camel_case_to_snake_case(param)
+                translated_integration[translated_key] = val
+
+            integrations_list.append(translated_integration)
+        return integrations_list
+
+
 class SchedulingTranslation(Translation[SchedulingConfig, Dict[str, Any]]):
     """Translate scheduling configs to and from MAPI"""
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> SchedulingConfig:
         extracted: SchedulingConfig = {'priority': None}
         for k, v in value.items():
@@ -324,41 +421,14 @@
 
     logger.warning(f'Invalid run name "{run_name}": Run names must be less than {MAX_RUN_NAME_LENGTH} '
                    'characters and contain only lower-case letters, numbers, or "-". '
                    f'Converting to a valid name: {new_run_name}')
     return new_run_name
 
 
-def _validate_cluster_exists(cluster: str):
-    """Validate that the cluster exists, if not throw a MCLIValidationError
-    """
-    try:
-        _ = Cluster.get_by_name(cluster)
-    except KeyError as e:
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.config import FeatureFlag, MCLIConfig
-
-        conf = MCLIConfig.load_config(True)
-        if not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-            cluster_names = ', '.join([c.name for c in conf.clusters])
-            if cluster_names:
-                raise MCLIRunConfigValidationError(
-                    f'Invalid cluster requested: {cluster}. '
-                    'If you think this should be a valid cluster, try creating the cluster '
-                    f'first with:\n\nmcli create cluster {cluster}\n\n'
-                    f'Otherwise, choose one of: {cluster_names}') from e
-            else:
-                raise MCLIRunConfigValidationError(
-                    f'Invalid cluster requested: {cluster}. '
-                    'User has not created any clusters. '
-                    'If you think this should be a valid cluster, try creating the cluster '
-                    f'first with:\n\nmcli create cluster {cluster}') from e
-        raise
-
-
 @dataclass
 class RunConfig(BaseSubmissionConfig):
     """A run configuration for the MosaicML platform
 
     Values in here are not yet validated and some required values may be missing.
 
     Args:
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/s3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,91 @@
-"""Creators for docker secrets"""
-from enum import Enum
+"""Creators for s3 secrets"""
+from pathlib import Path
 from typing import Callable, Optional
 
 from mcli.models import SecretType
-from mcli.objects.secrets import MCLIDockerRegistrySecret
+from mcli.objects.secrets import MCLIS3Secret
 from mcli.objects.secrets.create.base import SecretCreator, SecretValidationError
-from mcli.utils.utils_interactive import choose_one, secret_prompt, simple_prompt
-from mcli.utils.utils_string_functions import validate_email_address, validate_url
+from mcli.objects.secrets.create.generic import FileSecretFiller, FileSecretValidator
+from mcli.utils.utils_interactive import file_prompt
+from mcli.utils.utils_string_functions import validate_existing_filename
 
 
-class ContainerRegistries(Enum):
-    DOCKERHUB = ("DockerHub", "https://index.docker.io/v1/")
-    GHCR = ("Github (GHCR)", "https://ghcr.io")
-    OTHER = ("Other", "")
-
-    def __init__(self, display: str, url: str):
-        self.display = display
-        self.url = url
-
-
-class DockerSecretFiller():
-    """Interactive filler for docker secret data
+class S3SecretFiller(FileSecretFiller):
+    """Interactive filler for s3 secret data
     """
 
     @staticmethod
-    def fill_str(prompt: str, default: Optional[str] = None, validate: Optional[Callable[[str], bool]] = None):
-        return simple_prompt(prompt, default=default, validate=validate)
+    def fill_file(prompt: str, validate: Callable[[str], bool]) -> str:
+        return file_prompt(prompt, validate=validate)
 
     @classmethod
-    def fill_username(cls) -> str:
-        return cls.fill_str('What is your username?')
+    def fill_config(cls, validate: Callable[[str], bool]) -> str:
+        return cls.fill_file(
+            'Where is your S3 config file located?',
+            validate,
+        )
 
     @classmethod
-    def fill_password(cls) -> str:
-        return secret_prompt('What is your password/API token?')
-
-    @classmethod
-    def fill_server(cls, validate: Callable[[str], bool]) -> str:
-        chosen = choose_one(message="Which container registry would you like to use?",
-                            options=list(ContainerRegistries),
-                            formatter=lambda o: o.display,
-                            default=ContainerRegistries.DOCKERHUB)
-        server = chosen.url
-        if chosen is ContainerRegistries.OTHER:
-            server = cls.fill_str('What is the URL for this registry?', validate=validate)
-        return server
+    def fill_credentials(cls, validate: Callable[[str], bool]) -> str:
+        return cls.fill_file(
+            'Where is your S3 credentials file located?',
+            validate,
+        )
 
 
-class DockerSecretValidator():
-    """Validation methods for docker secret data
+class S3SecretValidator(FileSecretValidator):
+    """Validation methods for secret data
 
     Raises:
         SecretValidationError: Raised for any validation error for secret data
     """
 
     @staticmethod
-    def validate_email(email: str) -> bool:
-        is_valid_email = validate_email_address(email)
-        if not is_valid_email:
-            raise SecretValidationError(f'{email} does not appear to be a valid email address.')
-        return True
+    def validate_file_exists(path: str) -> bool:
 
-    @staticmethod
-    def validate_server(url: str) -> bool:
-        is_valid_url = validate_url(url)
-        if not is_valid_url:
-            raise SecretValidationError(f'{url} does not appear to be a valid URL.')
+        if not validate_existing_filename(path):
+            raise SecretValidationError(f'File does not exist. File path {path} does not exist or is not a file.')
         return True
 
 
-class DockerSecretCreator(DockerSecretFiller, DockerSecretValidator):
-    """Creates docker secrets for the CLI
+class S3SecretCreator(S3SecretFiller, S3SecretValidator):
+    """Creates s3 secrets for the CLI
     """
 
     def create(self,
                name: Optional[str] = None,
-               username: Optional[str] = None,
-               password: Optional[str] = None,
-               email: Optional[str] = None,
-               server: Optional[str] = None,
-               **kwargs) -> MCLIDockerRegistrySecret:
-        del kwargs
+               mount_directory: Optional[str] = None,
+               credentials_file: Optional[str] = None,
+               config_file: Optional[str] = None) -> MCLIS3Secret:
+
+        # Validate mount directory and files
+        if mount_directory:
+            self.validate_mount_absolute(mount_directory)
 
-        if server:
-            self.validate_server(server)
+        if credentials_file:
+            self.validate_file_exists(credentials_file)
 
-        if email:
-            self.validate_email(email)
+        if config_file:
+            self.validate_file_exists(config_file)
 
-        # Get base secret
         base_creator = SecretCreator()
-        secret = base_creator.create(SecretType.docker_registry, name)
-        assert isinstance(secret, MCLIDockerRegistrySecret)
+        secret = base_creator.create(SecretType.s3, name=name)
+        assert isinstance(secret, MCLIS3Secret)
+
+        if not config_file:
+            config_file = self.fill_config(self.validate_file_exists)
+
+        if not credentials_file:
+            credentials_file = self.fill_credentials(self.validate_file_exists)
+
+        if not mount_directory:
+            mount_directory = self.get_mount_path(secret.name)
+        secret.mount_directory = mount_directory
+
+        with open(Path(config_file).expanduser().absolute(), 'r', encoding='utf8') as fh:
+            secret.config = fh.read()
 
-        secret.server = server or self.fill_server(self.validate_server)
-        secret.username = username or self.fill_username()
-        secret.password = password or self.fill_password()
-        secret.email = email
+        with open(Path(credentials_file).expanduser().absolute(), 'r', encoding='utf8') as fh:
+            secret.credentials = fh.read()
 
         return secret
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/gcp.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     Raises:
         SecretValidationError: Raised for any validation error for secret data
     """
 
     @staticmethod
     def validate_file_exists(path: str) -> bool:
-
         if not validate_existing_filename(path):
             raise SecretValidationError(f'File does not exist. File path {path} does not exist or is not a file.')
         return True
 
 
 class GCPSecretCreator(GCPSecretFiller, GCPSecretValidator):
     """Creates gcp secrets for the CLI
@@ -50,27 +49,27 @@
         name: Optional[str] = None,
         mount_path: Optional[str] = None,
         credentials_file: Optional[str] = None,
     ) -> MCLIGCPSecret:
 
         # Validate mount path and files
         if mount_path:
-            self.validate_mount(mount_path)
+            self.validate_mount_absolute(mount_path)
 
         if credentials_file:
             self.validate_file_exists(credentials_file)
 
         base_creator = SecretCreator()
         secret = base_creator.create(SecretType.gcp, name=name)
         assert isinstance(secret, MCLIGCPSecret)
 
         if not credentials_file:
             credentials_file = self.fill_credentials(self.validate_file_exists)
 
         if not mount_path:
-            mount_path = self.get_valid_mount_path(secret.name)
+            mount_path = self.get_mount_path(secret.name)
         secret.mount_path = mount_path
 
         with open(Path(credentials_file).expanduser().absolute(), 'r', encoding='utf8') as fh:
             secret.value = fh.read()
 
         return secret
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/generic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 """Creators for generic secrets"""
 import re
 import uuid
 from pathlib import Path
-from typing import Callable, Optional, Set, Tuple
+from typing import Callable, Optional, Tuple
 
-from mcli.cli.m_create.env_var import EnvVarValidator
+from mcli.api.exceptions import ValidationError
 from mcli.models.mcli_secret import SECRET_MOUNT_PATH_PARENT, MCLIGenericSecret, SecretType
-from mcli.objects.secrets import MCLIEnvVarSecret, MCLIMountedSecret, MCLIS3Secret
-from mcli.objects.secrets.create.base import SecretCreator, SecretValidationError, SecretValidator
+from mcli.objects.secrets import MCLIEnvVarSecret, MCLIMountedSecret
+from mcli.objects.secrets.create.base import SecretCreator, SecretValidationError
 from mcli.utils.utils_interactive import file_prompt, secret_prompt, simple_prompt
 from mcli.utils.utils_string_functions import (KEY_VALUE_PATTERN, ensure_rfc1123_compatibility, validate_absolute_path,
-                                               validate_existing_filename)
+                                               validate_env_key, validate_existing_filename, validate_key_value_pair)
 
 
-class GenericSecretFiller():
-    """Interactive filler for secret data
-    """
-
-    @staticmethod
-    def fill_value() -> str:
-        return secret_prompt('What value would you like to store?')
-
-
-class GenericSecretValidator():
-    """Validation methods for generic secret data
-    """
-    pass
-
-
-class GenericSecretCreator(GenericSecretFiller, GenericSecretValidator):
+class GenericSecretCreator:
     """Creates base generic secrets for the CLI
     """
 
     def create(self,
                name: Optional[str] = None,
                value: Optional[str] = None,
                make_name_unique: bool = False) -> MCLIGenericSecret:
 
         base_creator = SecretCreator()
         secret = base_creator.create(SecretType.generic, name=name, make_name_unique=make_name_unique)
         assert isinstance(secret, MCLIGenericSecret)
 
         if not secret.value:
-            secret.value = value or self.fill_value()
+            secret.value = value or secret_prompt('What value would you like to store?')
 
         return secret
 
 
 class EnvVarSecretFiller():
     """Interactive filler for secret data
     """
 
     @staticmethod
     def fill_key(validate: Callable[[str], bool]) -> str:
         return simple_prompt('If an environment variable is KEY=VALUE, what should be the KEY?', validate=validate)
 
 
-class EnvVarSecretValidator(SecretValidator, EnvVarValidator):
+class EnvVarValidationError(ValidationError):
+    """Env var could not be configured with the provided values
+    """
+
+
+class EnvVarSecretValidator:
     """Validation methods for env var secret data
 
     Raises:
         SecretValidationError: Raised for any validation error for secret data
     """
 
+    @staticmethod
+    def validate_env_pair(env_pair: str) -> bool:
+        if not validate_key_value_pair(env_pair):
+            raise EnvVarValidationError(
+                'Environment variable must be specified like KEY=VALUE, where KEY must include only characters '
+                f'in [0-9A-Za-z_]. Got: {env_pair}')
+        return True
+
+    @staticmethod
+    def validate_key_valid(key: str) -> bool:
+        if not validate_env_key(key):
+            raise EnvVarValidationError('Invalid environment variable. Can only contain the characters [0-9A-Za-z_]')
+        return True
+
 
 class EnvVarSecretCreator(EnvVarSecretFiller, EnvVarSecretValidator):
     """Creates env var secrets for the CLI
     """
 
     @staticmethod
     def get_env(env_pair: str) -> Tuple[str, str]:
@@ -83,21 +87,17 @@
         key: Optional[str] = None,
     ) -> MCLIEnvVarSecret:
 
         if env_pair:
             self.validate_env_pair(env_pair)
             key, value = self.get_env(env_pair)
 
-        # Validate key
-        if key:
-            self.validate_env_key_available(key)
-
         # Fill key
         if not key:
-            key = self.fill_key(self.validate_key)
+            key = self.fill_key(self.validate_key_valid)
 
         # Make a name if not provided
         make_name_unique = False
         if not name:
             name = ensure_rfc1123_compatibility(key)
             make_name_unique = True
 
@@ -114,71 +114,36 @@
 
     @staticmethod
     def fill_secret_path(validate: Callable[[str], bool]) -> str:
         del validate
         return file_prompt('Which file would you like to store as a secret?')
 
 
-class FileSecretValidator(SecretValidator):
+class FileSecretValidator:
     """Validation methods for mounted secret data
 
     Raises:
         SecretValidationError: Raised for any validation error for secret data
     """
 
-    def __init__(self):
-        super().__init__()
-        self.existing_mounts = self.get_existing_mounts()
-
-    def get_existing_mounts(self) -> Set[str]:
-        secret_paths = {
-            s.mount_path for s in self.existing_secrets if isinstance(s, MCLIMountedSecret) and s.mount_path
-        }
-        s3_mounts = {
-            s.mount_directory for s in self.existing_secrets if isinstance(s, MCLIS3Secret) and s.mount_directory
-        }
-        return secret_paths | s3_mounts
-
-    def get_valid_mount_path(self, name: str, unique: bool = False) -> str:
+    def get_mount_path(self, name: str, unique: bool = False) -> str:
         if not unique:
-            proposed = str(SECRET_MOUNT_PATH_PARENT / name)
+            return str(SECRET_MOUNT_PATH_PARENT / name)
         else:
-            proposed = str(SECRET_MOUNT_PATH_PARENT / name / f'-{str(uuid.uuid4())[:6]}')
-
-        try:
-            self.validate_mount_available(proposed, self.existing_mounts)
-        except SecretValidationError:
-            if not unique:
-                # Try getting a unique path
-                proposed = self.get_valid_mount_path(name, True)
-            else:
-                # If that fails for some reason, just fail
-                raise
-        return proposed
+            return str(SECRET_MOUNT_PATH_PARENT / name / f'-{str(uuid.uuid4())[:6]}')
 
     @staticmethod
     def validate_mount_absolute(path: str) -> bool:
         is_valid = validate_absolute_path(path)
         if not is_valid:
             raise SecretValidationError('Invalid mount point. Mount must be an absolute path, '
                                         f'not {path}.')
         return True
 
     @staticmethod
-    def validate_mount_available(path: str, existing_paths: Set[str]) -> bool:
-        if path in existing_paths:
-            path_str = '\n'.join(sorted(list(existing_paths)))
-            raise SecretValidationError(f'Duplicate path. Mount path {path} already in use.'
-                                        f'Please choose something not in: {path_str}.')
-        return True
-
-    def validate_mount(self, path: str) -> bool:
-        return self.validate_mount_absolute(path) and self.validate_mount_available(path, self.existing_mounts)
-
-    @staticmethod
     def validate_path_exists(path: str) -> bool:
         if not validate_existing_filename(path):
             raise SecretValidationError(f'File does not exist. File path {path} does not exist or is not a file.')
         return True
 
 
 class FileSecretCreator(FileSecretFiller, FileSecretValidator):
@@ -193,15 +158,15 @@
     ) -> MCLIMountedSecret:
 
         if secret_path:
             self.validate_path_exists(secret_path)
 
         # Validate mount path
         if mount_path:
-            self.validate_mount(mount_path)
+            self.validate_mount_absolute(mount_path)
 
         # Fill secret file
         if not secret_path:
             secret_path = self.fill_secret_path(self.validate_path_exists)
 
         secret_file = Path(secret_path).expanduser().absolute()
 
@@ -217,9 +182,9 @@
 
         # Create generic secret
         generic_creator = GenericSecretCreator()
         generic_secret = generic_creator.create(name, value, make_name_unique=make_name_unique)
 
         # Get a mount path based on the secret's name
         if mount_path is None:
-            mount_path = self.get_valid_mount_path(generic_secret.name)
+            mount_path = self.get_mount_path(generic_secret.name)
         return MCLIMountedSecret.from_generic_secret(generic_secret, mount_path=mount_path)
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/oci.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                name: Optional[str] = None,
                mount_directory: Optional[str] = None,
                key_file: Optional[str] = None,
                config_file: Optional[str] = None) -> MCLIOCISecret:
 
         # Validate mount directory and files
         if mount_directory:
-            self.validate_mount(mount_directory)
+            self.validate_mount_absolute(mount_directory)
 
         if key_file:
             self.validate_file_exists(key_file)
 
         if config_file:
             self.validate_file_exists(config_file)
 
@@ -77,15 +77,15 @@
         if not config_file:
             config_file = self.fill_config(self.validate_file_exists)
 
         if not key_file:
             key_file = self.fill_key_file(self.validate_file_exists)
 
         if not mount_directory:
-            mount_directory = self.get_valid_mount_path(secret.name)
+            mount_directory = self.get_mount_path(secret.name)
         secret.mount_directory = mount_directory
 
         oci_config_parser = configparser.ConfigParser()
         try:
             oci_config_parser.read(Path(config_file).expanduser().absolute(), encoding='utf8')
         except Exception as ex:
             raise SecretValidationError(
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/ssh.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,36 +46,14 @@
 class SSHSecretValidator(FileSecretValidator):
     """Validation methods for SSH secret data
 
     Raises:
         SecretValidationError: Raised for any validation error for secret data
     """
 
-    def validate_only_git_ssh(self) -> bool:
-        for secret in self.existing_secrets:
-            if secret.secret_type == SecretType.git:
-                raise SecretValidationError(
-                    f'Git SSH secret already exists: {secret.name}. '
-                    'Only one Git SSH secret is allowed. Try adding the secret as an '
-                    '`ssh` secret instead using `mcli create secret ssh`. '
-                    f'Otherwise, delete the git secret with `mcli delete secret {secret.name}` and '
-                    'create a new one.')
-        return True
-
-    def validate_only_sftp_ssh(self) -> bool:
-        for secret in self.existing_secrets:
-            if secret.secret_type == SecretType.sftp:
-                raise SecretValidationError(
-                    f'SFTP secret already exists: {secret.name}. '
-                    'Only one SFTP secret is allowed. Try adding the secret as an '
-                    '`ssh` secret instead using `mcli create secret ssh`. '
-                    f'Otherwise, delete the sftp secret with `mcli delete secret {secret.name}` and '
-                    'create a new one.')
-        return True
-
     @staticmethod
     def validate_private_key(key_path: str) -> bool:
 
         if not validate_existing_filename(key_path):
             raise SecretValidationError(f'File does not exist. File path {key_path} does not exist or is not a file.')
         return True
 
@@ -99,25 +77,17 @@
                host_name: Optional[str] = None,
                no_host_check: Optional[bool] = None) -> MCLISSHSecret:
 
         if no_host_check:
             logger.warning(
                 f'{WARN} WARNING: Disabling host checking when adding SSH keys is a security risk. Use with caution.')
 
-        # Validate only one git secret
-        if git:
-            self.validate_only_git_ssh()
-
-        # Validate only one sftp secret
-        if sftp:
-            self.validate_only_sftp_ssh()
-
         # Validate mount and ssh key
         if mount_path:
-            self.validate_mount(mount_path)
+            self.validate_mount_absolute(mount_path)
 
         if ssh_private_key:
             self.validate_private_key(ssh_private_key)
 
         # Fill ssh private key
         if not ssh_private_key:
             ssh_private_key = self.fill_private_key(self.validate_private_key)
@@ -157,14 +127,14 @@
         secret = base_creator.create(secret_type, name=name, make_name_unique=make_name_unique)
         assert isinstance(secret, MCLISSHSecret)
 
         if isinstance(secret, MCLISFTPSSHSecret):
             secret.known_hosts = known_hosts
 
         if not mount_path:
-            mount_path = self.get_valid_mount_path(secret.name)
+            mount_path = self.get_mount_path(secret.name)
         secret.mount_path = mount_path
 
         with open(Path(ssh_private_key).expanduser().absolute(), 'r', encoding='utf8') as fh:
             secret.value = fh.read()
 
         return secret
```

### Comparing `mosaicml-cli-0.3.9/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a0/mcli/objects/secrets/create/docker_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-""" Creates an EnvVar Secret """
-from __future__ import annotations
+"""Creators for docker secrets"""
+from enum import Enum
+from typing import Optional
 
-from dataclasses import dataclass
-from typing import Any, Dict, Optional, Set, Type
+from mcli.models import SecretType
+from mcli.objects.secrets import MCLIDockerRegistrySecret
+from mcli.objects.secrets.create.base import SecretCreator
+from mcli.utils.utils_interactive import choose_one, secret_prompt, simple_prompt
 
-from kubernetes import client
 
-from mcli.models import MCLIGenericSecret, SecretType
-from mcli.serverside.job.mcli_k8s_job import MCLIK8sJob
+class ContainerRegistries(Enum):
+    DOCKERHUB = ("DockerHub", "https://index.docker.io/v1/")
+    GHCR = ("Github (GHCR)", "https://ghcr.io")
+    OTHER = ("Other", "")
 
+    def __init__(self, display: str, url: str):
+        self.display = display
+        self.url = url
 
-@dataclass
-class MCLIEnvVarSecret(MCLIGenericSecret):
-    """Secret class for generic secrets that will be added as environment variables
+
+class DockerSecretFiller():
+    """Interactive filler for docker secret data
     """
-    key: Optional[str] = None
 
-    @property
-    def mapi_data(self) -> Dict[str, Any]:
-        return {
-            'envVarSecret': {
-                'name': self.name,
-                'metadata': {
-                    'key': self.key
-                },
-                'value': self.value,
-            },
-        }
-
-    @property
-    def required_packing_fields(self) -> Set[str]:
-        return set(self.disk_skipped_fields + ['key'])
+    @classmethod
+    def fill_username(cls) -> str:
+        return simple_prompt('What is your username?')
+
+    @classmethod
+    def fill_password(cls) -> str:
+        return secret_prompt('What is your password/API token?')
 
     @classmethod
-    def from_generic_secret(
-        cls: Type[MCLIEnvVarSecret],
-        generic_secret: MCLIGenericSecret,
-        key: str,
-    ) -> MCLIEnvVarSecret:
-        return cls(
-            name=generic_secret.name,
-            value=generic_secret.value,
-            secret_type=SecretType.environment,
-            key=key,
-        )
-
-    def add_to_job(self, kubernetes_job: MCLIK8sJob) -> bool:
-        secret_env = client.V1EnvVar(
-            name=self.key,
-            value_from=client.V1EnvVarSource(secret_key_ref=client.V1SecretKeySelector(
-                name=self.name,
-                key='value',
-                optional=False,
-            ),),
-        )
+    def fill_server(cls) -> str:
+        chosen = choose_one(message="Which container registry would you like to use?",
+                            options=list(ContainerRegistries),
+                            formatter=lambda o: o.display,
+                            default=ContainerRegistries.DOCKERHUB)
+        server = chosen.url
+        if chosen is ContainerRegistries.OTHER:
+            server = simple_prompt('What is the URL for this registry?')
+        return server
+
+
+class DockerSecretCreator(DockerSecretFiller):
+    """Creates docker secrets for the CLI
+    """
+
+    def create(self,
+               name: Optional[str] = None,
+               username: Optional[str] = None,
+               password: Optional[str] = None,
+               email: Optional[str] = None,
+               server: Optional[str] = None,
+               **kwargs) -> MCLIDockerRegistrySecret:
+        del kwargs
+
+        # Get base secret
+        base_creator = SecretCreator()
+        secret = base_creator.create(SecretType.docker_registry, name)
+        assert isinstance(secret, MCLIDockerRegistrySecret)
+
+        secret.server = server or self.fill_server()
+        secret.username = username or self.fill_username()
+        secret.password = password or self.fill_password()
+        secret.email = email
 
-        kubernetes_job.add_env_var(secret_env)
-        return True
+        return secret
```

### Comparing `mosaicml-cli-0.3.9/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a0/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a0/mcli/sdk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,11 +11,7 @@
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, stop_run, stop_runs, update_run_metadata,
                            wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
-
-if not MCLIConfig.load_config(safe=True).feature_enabled(FeatureFlag.USE_MCLOUD):
-    from mcli.api.kube.runs import (create_run, delete_runs, follow_run_logs, get_run_logs, get_runs, stop_runs,
-                                    wait_for_run_status)
```

### Comparing `mosaicml-cli-0.3.9/mcli/serverside/clusters/gpu_type.py` & `mosaicml-cli-0.4.0a0/mcli/models/gpu_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,36 +16,14 @@
     K80 = 'k80'
     RTX3080 = '3080'
     RTX3090 = '3090'
     TPUv2 = 'tpuv2'  # pylint: disable=invalid-name
     TPUv3 = 'tpuv3'  # pylint: disable=invalid-name
 
     @staticmethod
-    def get_gpu_memory_gb(gpu_type: GPUType) -> int:
-        if 'gb' in gpu_type.value:
-            try:
-                mem = gpu_type.value.split('_')[1].replace('gb', '')
-                return mem
-            except Exception:  # pylint: disable=broad-except
-                pass
-        if gpu_type == GPUType.RTX3080:
-            return 10
-        elif gpu_type == GPUType.RTX3090:
-            return 24
-        elif gpu_type == GPUType.TPUv2:
-            return 64
-        elif gpu_type == GPUType.TPUv3:
-            return 128
-        elif gpu_type == GPUType.T4:
-            return 16
-        elif gpu_type == GPUType.K80:
-            return 24
-        return 0
-
-    @staticmethod
     def get_available_gpu_types() -> List[str]:
         return [x.value for x in GPUType]
 
     @classmethod
     def from_string(cls, gpu_type: str) -> GPUType:
         if isinstance(gpu_type, int):
             # Secondary catch for gpu_type for 30 series enums
```

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import questionary
 from typing_extensions import Literal
 
 from mcli.api.exceptions import InputDisabledError, ValidationError
 from mcli.utils.utils_logging import err_console
 
 T_Option = TypeVar('T_Option')  # pylint: disable=invalid-name
-T_Option_Str = Union[T_Option, str]  # pylint: disable=invalid-name
 
 logger = logging.getLogger(__name__)
 
 
 def validate_true(_: Any) -> bool:
     return True
 
@@ -80,38 +79,14 @@
 
     def __exit__(self, exc_type, value, traceback):
         assert self.prev is not None
         self.set_disabled(self.prev)
         return False
 
 
-def prompt(*args, **kwargs):
-    """DEPRECATED prompt command
-    """
-    raise NotImplementedError('This function is no longer implemented. Please switch to the other interactive prompts')
-
-
-def list_options(
-    input_text: str,
-    options: List[T_Option],
-    *,
-    allow_custom_response: bool = False,
-    multiple_ok: bool = False,
-    default_response: Optional[T_Option] = None,
-    pre_helptext: Optional[str] = 'Interactive selection...',
-    helptext: str = 'put a number or enter your own option',
-    validate: Callable[[Union[str, T_Option]], bool] = validate_true,
-    print_option: Callable[[Union[str, T_Option]], str] = str,
-    print_response: bool = True,
-) -> Union[T_Option, str, List[T_Option], List[str], List[T_Option_Str[T_Option]]]:
-    """DEPRECATED selection command
-    """
-    raise NotImplementedError('This function is no longer implemented. Please switch to the other interactive prompts')
-
-
 def check_input_disabled(func):
     """Decorator to check if input is disabled and error
 
     Args:
         func: Function to be wrapped
 
     Raises:
```

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,32 +64,14 @@
                                         console=err_console,
                                         highlighter=NullHighlighter())
 
 console_handler.setFormatter(logging.Formatter(fmt='%(message)s'))
 console_handler.markup = True
 
 
-def log_tree(tree: Tree, level: str, logger: logging.Logger) -> None:
-
-    mapping = {
-        'DEBUG': logging.DEBUG,
-        'INFO': logging.INFO,
-        'WARN': logging.WARN,
-        'ERROR': logging.ERROR,
-    }
-    try:
-        level_val: int = mapping[level.upper()]
-        if level_val >= logger.level:
-            logger.log(level_val, '')
-            rprint(tree)
-            logger.log(level_val, '')
-    except KeyError as key_error:
-        raise ValueError(f'Invalid log level {level}. Should be one of {list(mapping.keys())}') from key_error
-
-
 def get_indented_list(items: List[str], indent: int = 0, indent_marker: str = ' ', marker: str = '- ') -> str:
     """Get an indented list of items as a multi-line string
 
     Args:
         items: List of items
         indent: Number of indents for the list block
         indent_marker: Marker for the indent. Defaults to ' '.
@@ -122,18 +104,14 @@
 
     text = ' '.join([strip(line) for line in text.splitlines() if strip(line) != ''])
     wrapped = textwrap.wrap(text, console.width - 2 * indent)
     block = textwrap.indent('\n'.join(wrapped), prefix=marker * indent)
     return block
 
 
-def set_indent(text: str, indent: int, marker: str = ' ') -> str:
-    return textwrap.indent(textwrap.dedent(text), prefix=marker * indent)
-
-
 def print_timedelta(delta: timedelta):
     # strftime cannot be used with timedelta
 
     seconds = delta.total_seconds()
     if seconds < 60:
         return f'{int(seconds)}s'
     elif seconds < 3600:
```

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_string_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 from urllib.parse import urlparse
 
 from mcli.utils.utils_interactive import ValidationError
 
 MAX_KUBERNETES_LENGTH = 63
 
 
-def validate_alphanumeric_dash_characters(text: str) -> bool:
-    """ Validates lowercase alphanumeric with a dash """
-    return re.match(r'[a-z\-]+', text) is not None  # type: ignore
-
-
 @dataclass
 class StringVerificationResult():
     """ Used to return the result of a string verification
 
     Overrides __len__ to be truthy based on validity
     Overrides __eq__ to cast when being compared to bools
     """
@@ -167,31 +162,14 @@
         start with an alphanumeric character
         end with an alphanumeric character
     """
 
     return validate_dns_subdomain_name(text=secret_name)
 
 
-def validate_secret_key(secret_key: str) -> StringVerificationResult:
-    """
-    Ensures that secret keys are valid based on k8s spec
-
-        contain no more than 253 characters
-        contain only alphanumeric characters, '-' or '.' or '_'
-    """
-    verification_result = rfc_verification(
-        text=secret_key,
-        length=253,
-        special_characters=r'\-\._A-Z',
-        start_alnum_verification=False,
-        end_alnum_verification=False,
-    )
-    return verification_result
-
-
 def validate_api_plaintext(api_plaintext: str) -> bool:
     """Ensure a plaintext api key for the MosaicML platform is valid
 
     See https://github.com/mosaicml/mcloud/blob/dev/mapi/src/graphql/apikey/controller/ApiKeyController.ts
     """
     if api_plaintext.startswith('test.mosaicml'):
         # Testing API key may be valid, so let it pass
```

### Comparing `mosaicml-cli-0.3.9/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a0/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/mcli/version.py` & `mosaicml-cli-0.4.0a0/mcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.3.9"
-
+__version__ = "0.4.0a0"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.3.9/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.9
+Version: 0.4.0a0
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.9/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a0/mosaicml_cli.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 argcomplete>=2.0.0
+arrow>=1.2.2
 backoff>=2.2.1
-kubernetes>=21.7.0
+docker>=5.0.3
+gql[websockets]>=3.4.0
 prompt_toolkit>=3.0.29
+protobuf>=4.22.0
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
-toml>=0.10.2
 typing_extensions>=4.0.1
-arrow>=1.2.2
-docker>=5.0.3
-gql[websockets]>=3.4.0
-protobuf>=4.22.0
 
 [all]
+sphinx-markdown-tables>=0.0.15
+sphinx-argparse>=0.3.1
+sphinx_external_toc>=0.3.0
+sphinxcontrib-qthelp>=1.0.3
+sphinxcontrib-htmlhelp>=2.0.0
 pylint>=2.12.2
+sphinxcontrib-images>=0.9.4
+sphinx-copybutton>=0.5.0
+sphinxcontrib-applehelp>=1.0.2
 sphinx>=4.4.0
-sphinx-panels>=0.6.0
+sphinxemoji>=0.2.0
 sphinxext-opengraph>=0.6.1
+sphinxcontrib-devhelp>=1.0.2
+toml>=0.10.2
+sphinx-panels>=0.6.0
+pytest-cov>=4.0.0
 sphinxcontrib-jsmath>=1.0.1
-pytest>=6.2.5
-isort>=5.9.3
 pytest-mock>=3.7.0
 sphinxcontrib-serializinghtml>=1.1.5
-sphinxcontrib-devhelp>=1.0.2
-sphinx-argparse>=0.3.1
 myst-parser>=0.16.1
-sphinxemoji>=0.2.0
-sphinxcontrib-katex>=0.8.6
-pyright>=1.1.256
-pre-commit>=2.17.0
-yapf==0.33.0
-sphinxcontrib-applehelp>=1.0.2
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-htmlhelp>=2.0.0
-sphinx-markdown-tables>=0.0.15
-sphinx-copybutton>=0.5.0
-sphinxcontrib-qthelp>=1.0.3
-radon>=5.1.0
-sphinx-rtd-theme>=1.0.0
 sphinx-design
-pytest-cov>=4.0.0
 furo>=2022.3.4
-sphinx_external_toc>=0.3.0
+sphinx-rtd-theme>=1.0.0
+pre-commit>=2.17.0
+radon>=5.1.0
+yapf>=0.33.0
+pyright>=1.1.256
+pytest>=6.2.5
+sphinxcontrib-katex>=0.8.6
+isort>=5.9.3
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
-pytest>=6.2.5
-pytest-mock>=3.7.0
 pytest-cov>=4.0.0
+pytest-mock>=3.7.0
+pytest>=6.2.5
 radon>=5.1.0
-yapf==0.33.0
+toml>=0.10.2
+yapf>=0.33.0
 
 [sphinx]
 furo>=2022.3.4
 sphinx>=4.4.0
 sphinx-argparse>=0.3.1
 sphinx-copybutton>=0.5.0
 sphinx-markdown-tables>=0.0.15
```

### Comparing `mosaicml-cli-0.3.9/pyproject.toml` & `mosaicml-cli-0.4.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.9/setup.py` & `mosaicml-cli-0.4.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,41 +14,40 @@
 """
 
 # pylint: disable-next=exec-used,consider-using-with
 exec(open('mcli/version.py', 'r', encoding='utf-8').read())
 
 install_requires = [
     'argcomplete>=2.0.0',
+    'arrow>=1.2.2',
     'backoff>=2.2.1',
-    'kubernetes>=21.7.0',
+    'docker>=5.0.3',
+    'gql[websockets]>=3.4.0',
     'prompt_toolkit>=3.0.29',
+    'protobuf>=4.22.0',
     'pyyaml>=5.4.1',
     'questionary>=1.10.0',
     'rich>=10.16.2',
     'ruamel.yaml>=0.17.21',
-    'toml>=0.10.2',
     'typing_extensions>=4.0.1',
-    'arrow>=1.2.2',
-    'docker>=5.0.3',
-    'gql[websockets]>=3.4.0',
-    'protobuf>=4.22.0',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'isort>=5.9.3',
     'pre-commit>=2.17.0',
     'pylint>=2.12.2',
     'pyright>=1.1.256',
-    'pytest>=6.2.5',
-    'pytest-mock>=3.7.0',
     'pytest-cov>=4.0.0',
+    'pytest-mock>=3.7.0',
+    'pytest>=6.2.5',
     'radon>=5.1.0',
-    'yapf==0.33.0',
+    'toml>=0.10.2',
+    'yapf>=0.33.0',
 ]
 
 extra_deps['sphinx'] = [
     'furo>=2022.3.4',
     'sphinx>=4.4.0',
     'sphinx-argparse>=0.3.1',
     'sphinx-copybutton>=0.5.0',
```

### Comparing `mosaicml-cli-0.3.9/tests/test_config.py` & `mosaicml-cli-0.4.0a0/tests/test_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 from contextlib import contextmanager
 
 import pytest
 
-from mcli.config import (MCLI_INTERACTIVE_ENV, MCLI_MODE_ENV, MCLOUD_OBSCURE_FALLBACK, MOSAICML_API_ENDPOINT,
-                         MOSAICML_API_ENDPOINT_DEV, MOSAICML_API_ENDPOINT_ENV, MOSAICML_API_ENDPOINT_LOCAL,
-                         MOSAICML_API_KEY_ENV, FeatureFlag, MCLIConfig, MCLIConfigError, MCLIMode)
-from mcli.models.mcli_cluster import Cluster
+from mcli.config import (MCLI_INTERACTIVE_ENV, MCLI_MODE_ENV, MOSAICML_API_ENDPOINT, MOSAICML_API_ENDPOINT_DEV,
+                         MOSAICML_API_ENDPOINT_ENV, MOSAICML_API_ENDPOINT_LOCAL, MOSAICML_API_KEY_ENV, FeatureFlag,
+                         MCLIConfig, MCLIConfigError, MCLIMode)
 
 
 @contextmanager
 def clear_envs(*envs):
     values = {}
     for k in envs:
         values[k] = os.environ.pop(k, None)
@@ -24,22 +23,21 @@
 def test_backwards_compatible_mcli_config(cluster_key, mocker):
     """MCLIConfig should be able to load backwards compatible mcli configs
     """
     mocker.patch('mcli.config.MCLIConfig.internal', new_callable=mocker.PropertyMock, return_value=True)
     data = {
         'feature_flags': {
             'UNKNOWN_FLAG_SHOULDNT_BREAK_THINGS': True,
-            'USE_MCLOUD': True
+            'ALPHA_TESTER': True
         },
         cluster_key: [
             {
                 'kubernetes_context': 'microk8s',
                 'name': 'microk8s',
                 'namespace': 'microk8s',
-                'environment_overrides': 'dfjhgsjkdfnkvnskdf'  # this should be removed
             },
             # these should be ignored
             {
                 'kubernetes_context': 'unknown',
                 'name': 'unknown',
                 'namespace': 'unknown',
             },
@@ -49,18 +47,15 @@
         ],
         # these should be removed
         'dev_mode': True,
         'internal': True,
     }
     mcli_config = MCLIConfig.from_dict(data)
     assert mcli_config.feature_flags
-    assert mcli_config.feature_enabled(FeatureFlag.USE_MCLOUD)
-    assert not mcli_config.feature_enabled(FeatureFlag.USE_DEMO_NODES)
-
-    assert mcli_config.clusters == [Cluster(name='microk8s', kubernetes_context='microk8s', namespace='microk8s')]
+    assert mcli_config.feature_enabled(FeatureFlag.ALPHA_TESTER)
 
 
 def test_uninitialized(new_mcli_setup):
     """Test MCLIConfig fails to load for a new setup, raising a custom exception
     """
     with pytest.raises(MCLIConfigError):
         MCLIConfig.load_config()
@@ -69,45 +64,28 @@
 def test_initialized(base_mcli_setup):
     """Test MCLIConfig successfully loads
     """
     config = MCLIConfig.load_config()
 
     # defaults
     assert not config.internal
-    assert config.mcli_mode == MCLIMode.LEGACY  # TODO: Tests should not be using legacy
+    assert config.mcli_mode == MCLIMode.PROD
     assert config.endpoint == MOSAICML_API_ENDPOINT
-    assert not config.feature_enabled(FeatureFlag.USE_MCLOUD)
 
 
 def test_config_save_load(new_mcli_setup):
     """Test basic save and load
     """
     conf = MCLIConfig.empty()
     conf.save_config()
 
     conf2 = MCLIConfig.load_config()
     assert conf.to_dict() == conf2.to_dict()
 
 
-def test_config_invalid_clusters(new_mcli_setup):
-    """Test that invalid clusters are removed
-    """
-    clusters = [
-        Cluster(name='r1z1', kubernetes_context='r1z1', namespace='user'),
-        Cluster(name='invalid', kubernetes_context='invalid', namespace='user')
-    ]
-    conf = MCLIConfig.empty()
-    conf.clusters = clusters
-    conf.save_config()
-
-    conf2 = MCLIConfig.load_config()
-    assert len(conf2.clusters) == 1
-    assert conf2.clusters[0].name == 'r1z1'
-
-
 def test_mcli_mode(new_mcli_setup):
     with clear_envs(MCLI_MODE_ENV, 'DOGEMODE'):
         conf = MCLIConfig.empty()
         assert conf.mcli_mode == MCLIMode.PROD
 
         os.environ[MCLI_MODE_ENV] = MCLIMode.DEV.value
         assert conf.mcli_mode == MCLIMode.DEV
@@ -197,35 +175,7 @@
             os.environ[MCLI_INTERACTIVE_ENV] = value
             assert conf.allow_interactive is False
 
         del os.environ[MCLI_INTERACTIVE_ENV]
 
         os.environ[MCLI_MODE_ENV] = MCLIMode.INTERNAL.value
         assert conf.allow_interactive is True
-
-
-def test_mcloud_enabled(new_mcli_setup):
-    with clear_envs(MCLI_MODE_ENV):
-        conf = MCLIConfig.empty()
-        assert conf.mcloud_enabled is True
-
-        # Set user to any internal
-        for mode in [MCLIMode.INTERNAL, MCLIMode.DEV, MCLIMode.LOCAL]:
-            os.environ[MCLI_MODE_ENV] = mode.value
-            assert conf.mcloud_enabled is True
-
-        # Set user to prod and ensure it's configured by the feature flag
-        os.environ[MCLI_MODE_ENV] = MCLIMode.PROD.value
-        conf.feature_flags[FeatureFlag.USE_MCLOUD.value] = False
-        assert conf.mcloud_enabled is False
-        conf.feature_flags[FeatureFlag.USE_MCLOUD.value] = True
-        assert conf.mcloud_enabled is True
-
-        # Set "Legacy" mcli mode
-        os.environ[MCLI_MODE_ENV] = MCLIMode.LEGACY.value
-        assert conf.mcloud_enabled is False
-
-        # Fallback works
-        del os.environ[MCLI_MODE_ENV]
-        for value in ("true", "TRUE"):
-            os.environ[MCLOUD_OBSCURE_FALLBACK] = value
-            assert conf.mcloud_enabled is False
```

### Comparing `mosaicml-cli-0.3.9/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a0/tests/test_upgrade.py`

 * *Files identical despite different names*

