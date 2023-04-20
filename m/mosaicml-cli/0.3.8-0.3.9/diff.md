# Comparing `tmp/mosaicml-cli-0.3.8.tar.gz` & `tmp/mosaicml-cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.3.8.tar", last modified: Tue Apr 18 23:55:06 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.3.9.tar", last modified: Thu Apr 20 19:06:23 2023, max compression
```

## Comparing `mosaicml-cli-0.3.8.tar` & `mosaicml-cli-0.3.9.tar`

### file list

```diff
@@ -1,272 +1,273 @@
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.610104 mosaicml-cli-0.3.8/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-18 23:55:06.609742 mosaicml-cli-0.3.8/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     7799 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/README.md
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.516259 mosaicml-cli-0.3.8/mcli/
--rw-r--r--   0 wai        (502) staff       (20)       54 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.516990 mosaicml-cli-0.3.8/mcli/api/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.517698 mosaicml-cli-0.3.8/mcli/api/cluster/
--rw-r--r--   0 wai        (502) staff       (20)      134 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/cluster/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4141 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.519151 mosaicml-cli-0.3.8/mcli/api/engine/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/engine/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    26222 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/engine/engine.py
--rw-r--r--   0 wai        (502) staff       (20)      787 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/engine/utils.py
--rw-r--r--   0 wai        (502) staff       (20)    11677 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/exceptions.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.521838 mosaicml-cli-0.3.8/mcli/api/inference_deployments/
--rw-r--r--   0 wai        (502) staff       (20)      879 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3402 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     3292 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     6105 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     1044 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     1126 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.522050 mosaicml-cli-0.3.8/mcli/api/kube/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.524101 mosaicml-cli-0.3.8/mcli/api/kube/runs/
--rw-r--r--   0 wai        (502) staff       (20)      856 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4900 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_create_run.py
--rw-r--r--   0 wai        (502) staff       (20)     5042 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_delete_runs.py
--rw-r--r--   0 wai        (502) staff       (20)    14458 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_get_run_logs.py
--rw-r--r--   0 wai        (502) staff       (20)    16261 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_get_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     5981 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_stop_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     6210 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/kube/runs/api_watch_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.524656 mosaicml-cli-0.3.8/mcli/api/mint/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.8/mcli/api/mint/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6595 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/mint/shell.py
--rw-r--r--   0 wai        (502) staff       (20)     2216 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.8/mcli/api/mint/tty.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.525582 mosaicml-cli-0.3.8/mcli/api/model/
--rw-r--r--   0 wai        (502) staff       (20)      209 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/model/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6186 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/model/cluster_details.py
--rw-r--r--   0 wai        (502) staff       (20)     2909 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/model/inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     8057 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/model/run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.527367 mosaicml-cli-0.3.8/mcli/api/runs/
--rw-r--r--   0 wai        (502) staff       (20)     1102 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/runs/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2750 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_create_run.py
--rw-r--r--   0 wai        (502) staff       (20)     3926 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     9281 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 wai        (502) staff       (20)    10440 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     5099 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     3937 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 wai        (502) staff       (20)    10619 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.527808 mosaicml-cli-0.3.8/mcli/api/schema/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/schema/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      636 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.528864 mosaicml-cli-0.3.8/mcli/api/secrets/
--rw-r--r--   0 wai        (502) staff       (20)      309 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/secrets/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2365 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.8/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     3697 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)      508 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/api/types.py
--rw-r--r--   0 wai        (502) staff       (20)     2354 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/typing_future.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.529340 mosaicml-cli-0.3.8/mcli/api/users/
--rw-r--r--   0 wai        (502) staff       (20)      139 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/api/users/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2694 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.8/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.529739 mosaicml-cli-0.3.8/mcli/cli/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/__init__.py
--rwxr-xr-x   0 wai        (502) staff       (20)     7182 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/cli.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.530511 mosaicml-cli-0.3.8/mcli/cli/common/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/common/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2670 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 wai        (502) staff       (20)     7238 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.530883 mosaicml-cli-0.3.8/mcli/cli/m_clean/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_clean/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      950 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_clean/m_clean.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.531263 mosaicml-cli-0.3.8/mcli/cli/m_connect/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.8/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1541 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.8/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.532479 mosaicml-cli-0.3.8/mcli/cli/m_create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    11513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_create/cluster.py
--rw-r--r--   0 wai        (502) staff       (20)     7167 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_create/env_var.py
--rw-r--r--   0 wai        (502) staff       (20)     4217 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_create/m_create.py
--rw-r--r--   0 wai        (502) staff       (20)    24927 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.532992 mosaicml-cli-0.3.8/mcli/cli/m_delete/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    14072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_delete/delete.py
--rw-r--r--   0 wai        (502) staff       (20)     8562 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.533268 mosaicml-cli-0.3.8/mcli/cli/m_deploy/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3896 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.534120 mosaicml-cli-0.3.8/mcli/cli/m_describe/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4409 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     9943 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     1860 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.535831 mosaicml-cli-0.3.8/mcli/cli/m_get/
--rw-r--r--   0 wai        (502) staff       (20)      549 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/clusters.py
--rw-r--r--   0 wai        (502) staff       (20)     6452 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/display.py
--rw-r--r--   0 wai        (502) staff       (20)     1315 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/envvars.py
--rw-r--r--   0 wai        (502) staff       (20)     5361 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     4866 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/m_get.py
--rw-r--r--   0 wai        (502) staff       (20)     9517 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/runs.py
--rw-r--r--   0 wai        (502) staff       (20)     3567 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     1580 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_get/users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.536356 mosaicml-cli-0.3.8/mcli/cli/m_init/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_init/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4113 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_init/m_init.py
--rw-r--r--   0 wai        (502) staff       (20)     9374 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.537147 mosaicml-cli-0.3.8/mcli/cli/m_interactive/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     9005 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.8/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 wai        (502) staff       (20)    16203 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_interactive/m_interactive.py
--rw-r--r--   0 wai        (502) staff       (20)     4601 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_interactive/temp_mcloud_interactive.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.537439 mosaicml-cli-0.3.8/mcli/cli/m_log/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_log/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8633 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.537726 mosaicml-cli-0.3.8/mcli/cli/m_ping/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1742 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.537989 mosaicml-cli-0.3.8/mcli/cli/m_predict/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.538282 mosaicml-cli-0.3.8/mcli/cli/m_root/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_root/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.538583 mosaicml-cli-0.3.8/mcli/cli/m_run/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_run/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    10034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.539520 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2973 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 wai        (502) staff       (20)     1927 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 wai        (502) staff       (20)     1408 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 wai        (502) staff       (20)      881 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.539877 mosaicml-cli-0.3.8/mcli/cli/m_stop/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3847 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.540192 mosaicml-cli-0.3.8/mcli/cli/m_use/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_use/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_use/m_use.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.540834 mosaicml-cli-0.3.8/mcli/cli/m_util/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/cli/m_util/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     9853 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_util/kube_util.py
--rw-r--r--   0 wai        (502) staff       (20)     1147 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_util/m_util.py
--rw-r--r--   0 wai        (502) staff       (20)     6515 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/cli/m_util/util.py
--rw-r--r--   0 wai        (502) staff       (20)    16462 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.542069 mosaicml-cli-0.3.8/mcli/models/
--rw-r--r--   0 wai        (502) staff       (20)     1199 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8555 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/inference_deployment_config.py
--rw-r--r--   0 wai        (502) staff       (20)     3693 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/mcli_cluster.py
--rw-r--r--   0 wai        (502) staff       (20)      563 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/models/mcli_envvar.py
--rw-r--r--   0 wai        (502) staff       (20)     3386 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/mcli_integration.py
--rw-r--r--   0 wai        (502) staff       (20)     9400 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/mcli_secret.py
--rw-r--r--   0 wai        (502) staff       (20)    17234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/models/run_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.542371 mosaicml-cli-0.3.8/mcli/objects/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/objects/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.543737 mosaicml-cli-0.3.8/mcli/objects/integrations/
--rw-r--r--   0 wai        (502) staff       (20)      660 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      671 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/apt_packages.py
--rw-r--r--   0 wai        (502) staff       (20)     1287 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/comet.py
--rw-r--r--   0 wai        (502) staff       (20)     2597 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/git_repo.py
--rw-r--r--   0 wai        (502) staff       (20)     3491 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/local.py
--rw-r--r--   0 wai        (502) staff       (20)     2126 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/mosaicml_agent.py
--rw-r--r--   0 wai        (502) staff       (20)      810 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/pip_packages.py
--rw-r--r--   0 wai        (502) staff       (20)     2742 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/integrations/wandb.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.545548 mosaicml-cli-0.3.8/mcli/objects/secrets/
--rw-r--r--   0 wai        (502) staff       (20)     1090 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4913 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/cluster_secret.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.550876 mosaicml-cli-0.3.8/mcli/objects/secrets/create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3953 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/base.py
--rw-r--r--   0 wai        (502) staff       (20)     3461 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     2406 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     7554 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 wai        (502) staff       (20)     3855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     6701 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 wai        (502) staff       (20)     3782 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     1634 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/env_var.py
--rw-r--r--   0 wai        (502) staff       (20)     1122 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     2893 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/mounted.py
--rw-r--r--   0 wai        (502) staff       (20)     2855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/oci.py
--rw-r--r--   0 wai        (502) staff       (20)     2577 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     3952 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.552189 mosaicml-cli-0.3.8/mcli/proto/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/proto/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.553297 mosaicml-cli-0.3.8/mcli/sdk/
--rw-r--r--   0 wai        (502) staff       (20)     1298 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/sdk/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.554012 mosaicml-cli-0.3.8/mcli/serverside/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.559122 mosaicml-cli-0.3.8/mcli/serverside/clusters/
--rw-r--r--   0 wai        (502) staff       (20)      381 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    11245 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster.py
--rw-r--r--   0 wai        (502) staff       (20)    23072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster_instances.py
--rw-r--r--   0 wai        (502) staff       (20)     4005 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster_pv_setup.py
--rw-r--r--   0 wai        (502) staff       (20)     2793 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/gpu_type.py
--rw-r--r--   0 wai        (502) staff       (20)     2824 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/instance_type.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.576416 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/
--rw-r--r--   0 wai        (502) staff       (20)     1603 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      548 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/microk8s.py
--rw-r--r--   0 wai        (502) staff       (20)     2219 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r10z1.py
--rw-r--r--   0 wai        (502) staff       (20)     2822 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r1z1.py
--rw-r--r--   0 wai        (502) staff       (20)     2495 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r1z4.py
--rw-r--r--   0 wai        (502) staff       (20)     2759 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r3z1.py
--rw-r--r--   0 wai        (502) staff       (20)     5355 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r4z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1049 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1161 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z10.py
--rw-r--r--   0 wai        (502) staff       (20)     2497 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z2.py
--rw-r--r--   0 wai        (502) staff       (20)     1062 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z3.py
--rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z4.py
--rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z5.py
--rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z6.py
--rw-r--r--   0 wai        (502) staff       (20)     1214 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z7.py
--rw-r--r--   0 wai        (502) staff       (20)     1242 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z9.py
--rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z1.py
--rw-r--r--   0 wai        (502) staff       (20)     1071 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z2.py
--rw-r--r--   0 wai        (502) staff       (20)     1054 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z3.py
--rw-r--r--   0 wai        (502) staff       (20)     1061 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r99z1.py
--rw-r--r--   0 wai        (502) staff       (20)      310 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/clusters/volumekind.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.582502 mosaicml-cli-0.3.8/mcli/serverside/job/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    15654 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_job.py
--rw-r--r--   0 wai        (502) staff       (20)      465 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_config_map_typing.py
--rw-r--r--   0 wai        (502) staff       (20)     6471 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_job.py
--rw-r--r--   0 wai        (502) staff       (20)     8090 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_job_typing.py
--rw-r--r--   0 wai        (502) staff       (20)     7524 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
--rw-r--r--   0 wai        (502) staff       (20)      459 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_service_typing.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.584163 mosaicml-cli-0.3.8/mcli/serverside/runners/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/runners/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5770 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/serverside/runners/runner.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.601019 mosaicml-cli-0.3.8/mcli/utils/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/utils/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5306 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/utils/utils_cli.py
--rw-r--r--   0 wai        (502) staff       (20)     6073 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.8/mcli/utils/utils_config.py
--rw-r--r--   0 wai        (502) staff       (20)      740 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/utils/utils_date.py
--rw-r--r--   0 wai        (502) staff       (20)    10453 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_docker.py
--rw-r--r--   0 wai        (502) staff       (20)    12947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_epilog.py
--rw-r--r--   0 wai        (502) staff       (20)      751 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_file.py
--rw-r--r--   0 wai        (502) staff       (20)    11769 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_interactive.py
--rw-r--r--   0 wai        (502) staff       (20)    49322 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_kube.py
--rw-r--r--   0 wai        (502) staff       (20)     6980 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_kube_labels.py
--rw-r--r--   0 wai        (502) staff       (20)     4832 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_logging.py
--rw-r--r--   0 wai        (502) staff       (20)      359 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_modules.py
--rw-r--r--   0 wai        (502) staff       (20)     6614 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/utils/utils_pypi.py
--rw-r--r--   0 wai        (502) staff       (20)     6513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_rancher.py
--rw-r--r--   0 wai        (502) staff       (20)     3115 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/utils/utils_rich.py
--rw-r--r--   0 wai        (502) staff       (20)     8533 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_run_status.py
--rw-r--r--   0 wai        (502) staff       (20)     4350 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 wai        (502) staff       (20)     1103 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/mcli/utils/utils_spinner.py
--rw-r--r--   0 wai        (502) staff       (20)    11437 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_string_functions.py
--rw-r--r--   0 wai        (502) staff       (20)     3954 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/mcli/utils/utils_types.py
--rw-r--r--   0 wai        (502) staff       (20)     1001 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/mcli/utils/utils_yaml.py
--rw-r--r--   0 wai        (502) staff       (20)     3884 2023-04-18 23:54:06.000000 mosaicml-cli-0.3.8/mcli/version.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.604676 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     7226 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wai        (502) staff       (20)        1 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wai        (502) staff       (20)       75 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 wai        (502) staff       (20)     1552 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 wai        (502) staff       (20)       11 2023-04-18 23:55:06.000000 mosaicml-cli-0.3.8/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 wai        (502) staff       (20)    31312 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/pyproject.toml
--rw-r--r--   0 wai        (502) staff       (20)       38 2023-04-18 23:55:06.610307 mosaicml-cli-0.3.8/setup.cfg
--rw-r--r--   0 wai        (502) staff       (20)     2991 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/setup.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.606655 mosaicml-cli-0.3.8/tests/
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-18 23:55:06.608775 mosaicml-cli-0.3.8/tests/submit/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/tests/submit/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6393 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/tests/submit/test_cluster.py
--rw-r--r--   0 wai        (502) staff       (20)     9266 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/tests/submit/test_cluster_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     7973 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.8/tests/test_config.py
--rw-r--r--   0 wai        (502) staff       (20)       62 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.8/tests/test_simple.py
--rw-r--r--   0 wai        (502) staff       (20)     6116 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.8/tests/test_upgrade.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.957165 mosaicml-cli-0.3.9/
+-rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-20 19:06:23.956825 mosaicml-cli-0.3.9/PKG-INFO
+-rw-r--r--   0 wai        (502) staff       (20)     7799 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/README.md
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.824750 mosaicml-cli-0.3.9/mcli/
+-rw-r--r--   0 wai        (502) staff       (20)       54 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.826116 mosaicml-cli-0.3.9/mcli/api/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.826844 mosaicml-cli-0.3.9/mcli/api/cluster/
+-rw-r--r--   0 wai        (502) staff       (20)      134 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/cluster/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4141 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.827918 mosaicml-cli-0.3.9/mcli/api/engine/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/engine/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    26222 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/engine/engine.py
+-rw-r--r--   0 wai        (502) staff       (20)      787 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/engine/utils.py
+-rw-r--r--   0 wai        (502) staff       (20)    11677 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/exceptions.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.856766 mosaicml-cli-0.3.9/mcli/api/inference_deployments/
+-rw-r--r--   0 wai        (502) staff       (20)      879 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3421 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)     3292 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     6124 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     1044 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)     1126 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.857132 mosaicml-cli-0.3.9/mcli/api/kube/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.858600 mosaicml-cli-0.3.9/mcli/api/kube/runs/
+-rw-r--r--   0 wai        (502) staff       (20)      856 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4900 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_create_run.py
+-rw-r--r--   0 wai        (502) staff       (20)     5042 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_delete_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)    14458 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_run_logs.py
+-rw-r--r--   0 wai        (502) staff       (20)    16261 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     5981 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_stop_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     6210 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/kube/runs/api_watch_run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.859645 mosaicml-cli-0.3.9/mcli/api/mint/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/api/mint/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6870 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/mint/shell.py
+-rw-r--r--   0 wai        (502) staff       (20)     2216 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.9/mcli/api/mint/tty.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.860595 mosaicml-cli-0.3.9/mcli/api/model/
+-rw-r--r--   0 wai        (502) staff       (20)      209 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6186 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/cluster_details.py
+-rw-r--r--   0 wai        (502) staff       (20)     2987 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 wai        (502) staff       (20)     8057 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/model/run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.862591 mosaicml-cli-0.3.9/mcli/api/runs/
+-rw-r--r--   0 wai        (502) staff       (20)     1102 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/runs/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2750 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 wai        (502) staff       (20)     3926 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     7971 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 wai        (502) staff       (20)    10440 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     5099 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     3937 2023-04-11 22:36:33.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 wai        (502) staff       (20)    10619 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.863066 mosaicml-cli-0.3.9/mcli/api/schema/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/schema/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      636 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.864260 mosaicml-cli-0.3.9/mcli/api/secrets/
+-rw-r--r--   0 wai        (502) staff       (20)      309 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/secrets/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2365 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     3697 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)      508 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/api/types.py
+-rw-r--r--   0 wai        (502) staff       (20)     2354 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/typing_future.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.864854 mosaicml-cli-0.3.9/mcli/api/users/
+-rw-r--r--   0 wai        (502) staff       (20)      139 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/api/users/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2694 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.865288 mosaicml-cli-0.3.9/mcli/cli/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/__init__.py
+-rwxr-xr-x   0 wai        (502) staff       (20)     7182 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/cli.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.867688 mosaicml-cli-0.3.9/mcli/cli/common/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/common/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2670 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 wai        (502) staff       (20)     7238 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.868707 mosaicml-cli-0.3.9/mcli/cli/m_clean/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_clean/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      950 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_clean/m_clean.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.869362 mosaicml-cli-0.3.9/mcli/cli/m_connect/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1541 2023-02-27 22:51:58.000000 mosaicml-cli-0.3.9/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.871643 mosaicml-cli-0.3.9/mcli/cli/m_create/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    11513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/cluster.py
+-rw-r--r--   0 wai        (502) staff       (20)     7167 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/env_var.py
+-rw-r--r--   0 wai        (502) staff       (20)     4217 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 wai        (502) staff       (20)    24927 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.872616 mosaicml-cli-0.3.9/mcli/cli/m_delete/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    14072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 wai        (502) staff       (20)     8562 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.873226 mosaicml-cli-0.3.9/mcli/cli/m_deploy/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3896 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.874786 mosaicml-cli-0.3.9/mcli/cli/m_describe/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4409 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     9943 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     1860 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.879197 mosaicml-cli-0.3.9/mcli/cli/m_get/
+-rw-r--r--   0 wai        (502) staff       (20)      549 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     8477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 wai        (502) staff       (20)     6452 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/display.py
+-rw-r--r--   0 wai        (502) staff       (20)     1315 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/envvars.py
+-rw-r--r--   0 wai        (502) staff       (20)     5467 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 wai        (502) staff       (20)     4866 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 wai        (502) staff       (20)     9517 2023-04-18 21:58:44.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/runs.py
+-rw-r--r--   0 wai        (502) staff       (20)     3567 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     1580 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_get/users.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.879935 mosaicml-cli-0.3.9/mcli/cli/m_init/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4113 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 wai        (502) staff       (20)     9374 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.880843 mosaicml-cli-0.3.9/mcli/cli/m_interactive/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     9005 2023-03-06 19:03:52.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 wai        (502) staff       (20)    16203 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/m_interactive.py
+-rw-r--r--   0 wai        (502) staff       (20)     4601 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_interactive/temp_mcloud_interactive.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881147 mosaicml-cli-0.3.9/mcli/cli/m_log/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     8633 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881472 mosaicml-cli-0.3.9/mcli/cli/m_ping/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1742 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.881785 mosaicml-cli-0.3.9/mcli/cli/m_predict/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.882103 mosaicml-cli-0.3.9/mcli/cli/m_root/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.882417 mosaicml-cli-0.3.9/mcli/cli/m_run/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    10034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.883410 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     2973 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 wai        (502) staff       (20)     1927 2023-04-04 20:22:39.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 wai        (502) staff       (20)     1408 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 wai        (502) staff       (20)      881 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.883783 mosaicml-cli-0.3.9/mcli/cli/m_stop/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3847 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.884231 mosaicml-cli-0.3.9/mcli/cli/m_use/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_use/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_use/m_use.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.885029 mosaicml-cli-0.3.9/mcli/cli/m_util/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     9853 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/kube_util.py
+-rw-r--r--   0 wai        (502) staff       (20)     1147 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 wai        (502) staff       (20)     6515 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/cli/m_util/util.py
+-rw-r--r--   0 wai        (502) staff       (20)    16462 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.886444 mosaicml-cli-0.3.9/mcli/models/
+-rw-r--r--   0 wai        (502) staff       (20)     1199 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     8555 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 wai        (502) staff       (20)     3693 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_cluster.py
+-rw-r--r--   0 wai        (502) staff       (20)      563 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/models/mcli_envvar.py
+-rw-r--r--   0 wai        (502) staff       (20)     3386 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_integration.py
+-rw-r--r--   0 wai        (502) staff       (20)     9400 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/mcli_secret.py
+-rw-r--r--   0 wai        (502) staff       (20)    17234 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/models/run_config.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.886888 mosaicml-cli-0.3.9/mcli/objects/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.888435 mosaicml-cli-0.3.9/mcli/objects/integrations/
+-rw-r--r--   0 wai        (502) staff       (20)      660 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      671 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/apt_packages.py
+-rw-r--r--   0 wai        (502) staff       (20)     1287 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/comet.py
+-rw-r--r--   0 wai        (502) staff       (20)     2597 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/git_repo.py
+-rw-r--r--   0 wai        (502) staff       (20)     3491 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/local.py
+-rw-r--r--   0 wai        (502) staff       (20)     2126 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/mosaicml_agent.py
+-rw-r--r--   0 wai        (502) staff       (20)      810 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/pip_packages.py
+-rw-r--r--   0 wai        (502) staff       (20)     2742 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/integrations/wandb.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.890277 mosaicml-cli-0.3.9/mcli/objects/secrets/
+-rw-r--r--   0 wai        (502) staff       (20)     1090 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     4913 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/cluster_secret.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.895446 mosaicml-cli-0.3.9/mcli/objects/secrets/create/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     3953 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 wai        (502) staff       (20)     3461 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 wai        (502) staff       (20)     2406 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 wai        (502) staff       (20)     7554 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 wai        (502) staff       (20)     3855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 wai        (502) staff       (20)     2998 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 wai        (502) staff       (20)     6701 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 wai        (502) staff       (20)     3782 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 wai        (502) staff       (20)     1634 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 wai        (502) staff       (20)     1122 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 wai        (502) staff       (20)     2893 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 wai        (502) staff       (20)     2855 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/oci.py
+-rw-r--r--   0 wai        (502) staff       (20)     2577 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/s3.py
+-rw-r--r--   0 wai        (502) staff       (20)     3952 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.896776 mosaicml-cli-0.3.9/mcli/proto/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/proto/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     1477 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.897426 mosaicml-cli-0.3.9/mcli/sdk/
+-rw-r--r--   0 wai        (502) staff       (20)     1298 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/sdk/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.898437 mosaicml-cli-0.3.9/mcli/serverside/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/__init__.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.903585 mosaicml-cli-0.3.9/mcli/serverside/clusters/
+-rw-r--r--   0 wai        (502) staff       (20)      381 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    11245 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster.py
+-rw-r--r--   0 wai        (502) staff       (20)    23072 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_instances.py
+-rw-r--r--   0 wai        (502) staff       (20)     4005 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_pv_setup.py
+-rw-r--r--   0 wai        (502) staff       (20)     2793 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/gpu_type.py
+-rw-r--r--   0 wai        (502) staff       (20)     2824 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/instance_type.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.921675 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/
+-rw-r--r--   0 wai        (502) staff       (20)     1603 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)      548 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/microk8s.py
+-rw-r--r--   0 wai        (502) staff       (20)     2219 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r10z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     2822 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     2495 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z4.py
+-rw-r--r--   0 wai        (502) staff       (20)     2759 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r3z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     5355 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r4z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     1049 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     1161 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z10.py
+-rw-r--r--   0 wai        (502) staff       (20)     2497 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z2.py
+-rw-r--r--   0 wai        (502) staff       (20)     1062 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z3.py
+-rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z4.py
+-rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z5.py
+-rw-r--r--   0 wai        (502) staff       (20)     1047 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z6.py
+-rw-r--r--   0 wai        (502) staff       (20)     1214 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z7.py
+-rw-r--r--   0 wai        (502) staff       (20)     1242 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z9.py
+-rw-r--r--   0 wai        (502) staff       (20)     1034 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z1.py
+-rw-r--r--   0 wai        (502) staff       (20)     1071 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z2.py
+-rw-r--r--   0 wai        (502) staff       (20)     1054 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z3.py
+-rw-r--r--   0 wai        (502) staff       (20)     1061 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r99z1.py
+-rw-r--r--   0 wai        (502) staff       (20)      310 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/clusters/volumekind.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.926609 mosaicml-cli-0.3.9/mcli/serverside/job/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)    15654 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_job.py
+-rw-r--r--   0 wai        (502) staff       (20)      465 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_config_map_typing.py
+-rw-r--r--   0 wai        (502) staff       (20)     6471 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job.py
+-rw-r--r--   0 wai        (502) staff       (20)     8090 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job_typing.py
+-rw-r--r--   0 wai        (502) staff       (20)     7524 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
+-rw-r--r--   0 wai        (502) staff       (20)      459 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_service_typing.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.927972 mosaicml-cli-0.3.9/mcli/serverside/runners/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/runners/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     5770 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/serverside/runners/runner.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.948090 mosaicml-cli-0.3.9/mcli/utils/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     5306 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_cli.py
+-rw-r--r--   0 wai        (502) staff       (20)     6073 2023-04-18 16:53:02.000000 mosaicml-cli-0.3.9/mcli/utils/utils_config.py
+-rw-r--r--   0 wai        (502) staff       (20)      740 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_date.py
+-rw-r--r--   0 wai        (502) staff       (20)    10453 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_docker.py
+-rw-r--r--   0 wai        (502) staff       (20)    12947 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_epilog.py
+-rw-r--r--   0 wai        (502) staff       (20)      751 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_file.py
+-rw-r--r--   0 wai        (502) staff       (20)    11769 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_interactive.py
+-rw-r--r--   0 wai        (502) staff       (20)    49322 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_kube.py
+-rw-r--r--   0 wai        (502) staff       (20)     6980 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_kube_labels.py
+-rw-r--r--   0 wai        (502) staff       (20)     4832 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_logging.py
+-rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 wai        (502) staff       (20)      359 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_modules.py
+-rw-r--r--   0 wai        (502) staff       (20)     6614 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_pypi.py
+-rw-r--r--   0 wai        (502) staff       (20)     6513 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_rancher.py
+-rw-r--r--   0 wai        (502) staff       (20)     3115 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_rich.py
+-rw-r--r--   0 wai        (502) staff       (20)     8533 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_run_status.py
+-rw-r--r--   0 wai        (502) staff       (20)     4350 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 wai        (502) staff       (20)     1103 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/mcli/utils/utils_spinner.py
+-rw-r--r--   0 wai        (502) staff       (20)    11437 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 wai        (502) staff       (20)     3954 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/mcli/utils/utils_types.py
+-rw-r--r--   0 wai        (502) staff       (20)     1001 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/mcli/utils/utils_yaml.py
+-rw-r--r--   0 wai        (502) staff       (20)     3885 2023-04-20 18:58:54.000000 mosaicml-cli-0.3.9/mcli/version.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.951930 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/
+-rw-r--r--   0 wai        (502) staff       (20)      696 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wai        (502) staff       (20)     7263 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wai        (502) staff       (20)        1 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wai        (502) staff       (20)       75 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wai        (502) staff       (20)     1552 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 wai        (502) staff       (20)       11 2023-04-20 19:06:23.000000 mosaicml-cli-0.3.9/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 wai        (502) staff       (20)    31087 2023-04-20 18:58:30.000000 mosaicml-cli-0.3.9/pyproject.toml
+-rw-r--r--   0 wai        (502) staff       (20)       38 2023-04-20 19:06:23.957367 mosaicml-cli-0.3.9/setup.cfg
+-rw-r--r--   0 wai        (502) staff       (20)     2991 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/setup.py
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.954109 mosaicml-cli-0.3.9/tests/
+drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-04-20 19:06:23.955987 mosaicml-cli-0.3.9/tests/submit/
+-rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/__init__.py
+-rw-r--r--   0 wai        (502) staff       (20)     6393 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/test_cluster.py
+-rw-r--r--   0 wai        (502) staff       (20)     9266 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/submit/test_cluster_secrets.py
+-rw-r--r--   0 wai        (502) staff       (20)     7973 2023-04-18 23:46:04.000000 mosaicml-cli-0.3.9/tests/test_config.py
+-rw-r--r--   0 wai        (502) staff       (20)       62 2023-02-02 22:40:35.000000 mosaicml-cli-0.3.9/tests/test_simple.py
+-rw-r--r--   0 wai        (502) staff       (20)     6116 2023-03-21 22:39:53.000000 mosaicml-cli-0.3.9/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.3.8/PKG-INFO` & `mosaicml-cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.8/README.md` & `mosaicml-cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.3.9/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/engine/engine.py` & `mosaicml-cli-0.3.9/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/engine/utils.py` & `mosaicml-cli-0.3.9/mcli/api/engine/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/exceptions.py` & `mosaicml-cli-0.3.9/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
     publicDNS
+    createdByEmail
   }}
 }}"""
 
 
 @overload
 def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
                                 timeout: Optional[float] = 10,
```

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
     publicDNS
+    createdByEmail
   }}
 }}"""
 
 
 @overload
 def get_inference_deployments(
     deployments: Optional[Union[List[str], List[InferenceDeployment]]] = None,
```

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.3.9/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/__init__.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_create_run.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_delete_runs.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_get_run_logs.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_get_runs.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_stop_runs.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/kube/runs/api_watch_run.py` & `mosaicml-cli-0.3.9/mcli/api/kube/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/mint/shell.py` & `mosaicml-cli-0.3.9/mcli/api/mint/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import shutil
 import ssl
 import sys
-from typing import Dict, Optional
+from typing import Dict, Optional, cast
 
 from websockets.client import WebSocketClientProtocol
 from websockets.client import connect as ws_connect
 from websockets.exceptions import ConnectionClosedError, ConnectionClosedOK, InvalidStatusCode
 
 from mcli.api.exceptions import MintException
 from mcli.api.mint import tty
 from mcli.proto.mint_pb2 import MINTMessage, TerminalSize, UserInput
 from mcli.utils.utils_logging import FAIL, WARN
+from mcli.utils.utils_message_decoding import MessageDecoder
 
 logger = logging.getLogger(__name__)
 
 
 class MintShell:
     """Interactive shell into MINT (Mosaic Interactive service)
 
@@ -87,17 +88,19 @@
                 else:
                     # This can be very short, since its main purpose is to not block the event loop
                     await asyncio.sleep(0.01)
 
         async def write_stdout(ws: WebSocketClientProtocol):
             """Reads from the websocket and writes to stdout
             """
+            decoder = MessageDecoder()
             async for msg in ws:
                 if msg:
-                    sys.stdout.write(str(msg))
+                    decoded = decoder.decode(cast(bytes, msg))
+                    sys.stdout.write(decoded)
                     sys.stdout.flush()
 
         async def monitor_terminal_size(ws: WebSocketClientProtocol):
             """Monitors terminal size and sends it to the server when it changes
 
             This sends the width x height tuple as a byte string so MINT can parse it
             """
@@ -116,14 +119,16 @@
             # Useful for debugging. If logging is set to DEBUG level, this will log debug statements
             "logger": logger,
             # Set the close timeout to a small value. When the server closes connection, it often
             # does not respond to the client's close request. This keeps the waiting to a minimum.
             # If we start having reasons for the client to initiate the close, we may need to modify
             # this value.
             "close_timeout": 0.25,
+            # Give enough time for MINT to get a connection from the agent
+            "open_timeout": 30,
         }
         if uri.startswith("wss:"):
             connect_params["ssl"] = ssl.SSLContext(ssl.PROTOCOL_TLS)
 
         try:
             async with ws_connect(**connect_params) as ws:
                 # Start the read and write tasks to run until the connection closes
```

### Comparing `mosaicml-cli-0.3.8/mcli/api/mint/tty.py` & `mosaicml-cli-0.3.9/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.3.9/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.3.9/mcli/api/model/inference_deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     deployment_uid: str
     name: str
     status: str
     created_at: datetime
     updated_at: datetime
     config: FinalInferenceDeploymentConfig
+    created_by: str
     public_dns: str = ""
 
     deleted_at: Optional[datetime] = None
     submitted_config: Optional[InferenceDeploymentConfig] = None
 
     _required_properties: Tuple[str] = tuple(
         ['id', 'name', 'status', 'createdAt', 'updatedAt', 'inferenceDeploymentInput', 'publicDNS'])
@@ -58,9 +59,10 @@
         return cls(deployment_uid=response['id'],
                    name=response['name'],
                    created_at=convert_datetime(response['createdAt']),
                    updated_at=convert_datetime(response['updatedAt']),
                    deleted_at=deleted_at,
                    status=response['status'],
                    public_dns=response['publicDNS'],
+                   created_by=response['createdByEmail'],
                    config=FinalInferenceDeploymentConfig.from_mapi_response(response['inferenceDeploymentInput']),
                    submitted_config=submit_config)
```

### Comparing `mosaicml-cli-0.3.8/mcli/api/model/run.py` & `mosaicml-cli-0.3.9/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/__init__.py` & `mosaicml-cli-0.3.9/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_get_run_logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Get a run's logs from the MosaicML platform"""
 from __future__ import annotations
 
 import base64
 from concurrent.futures import Future
-from typing import Any, Dict, Generator, Optional, Tuple, Union, overload
+from typing import Any, Dict, Generator, Optional, Union, overload
 
 import gql
 from typing_extensions import Literal
 
 from mcli.api.engine.engine import MAPIConnection
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
+from mcli.utils.utils_message_decoding import MessageDecoder
 
 QUERY_FUNCTION = 'getRunLogs'
 VARIABLE_DATA_NAME = 'getRunLogsInput'
 QUERY = f"""
 subscription Subscription(${VARIABLE_DATA_NAME}: GetRunLogsInput!) {{
     {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME})
 }}"""
@@ -180,72 +181,37 @@
             yield message
 
 
 def _get_logs(query: str, variables: Dict[str, Any]) -> Generator[Future[str], None, None]:
 
     gql_query = gql.gql(query)
     connection = MAPIConnection.get_current_connection()
-    decoder = MessageDecoder()
+    decoder = LogsDecoder()
 
     for message in connection.subscribe(
             query=gql_query,
             variables=variables,
             callback=decoder.parse_message,
             retry_callback=decoder.update_offset,
     ):
         yield message
 
 
-def careful_decode(byte_str: bytes) -> Tuple[str, bytes]:
-    try:
-        return byte_str.decode('utf8'), b''
-    except UnicodeDecodeError as e:
-        if e.start == 0:
-            # Error is at the start. Let's just ignore these bytes
-            return careful_decode(byte_str[e.end:])
-        else:
-            remaining = byte_str[e.start:]
-            decoded = byte_str[:e.start].decode('utf8')
-            return decoded, remaining
-
-
-class MessageDecoder:
-    """Decode messages from MAPI getRunLogs
+class LogsDecoder(MessageDecoder):
+    """Decode log messages and update read offset
     """
 
-    def __init__(self):
-        self.remaining = b''
-        # prev can be used to maintain things that come after the final linebreak.
-        # Leaving this off for now, but maybe we'd want it?
-        self.prev = ''
-        # Number of bytes read from the subscription so far so that reconnection of stream can start
-        # at correct offset in the case of web socket errors in long lived subscriptions.
-        # There may be slight misalignment when reconnecting if self.remaining is not 0
-        # or if unicode decode error is at the start of the string.
-        self.num_bytes_read = 0
+    def update_offset(self, variables: Dict[str, Any]) -> Dict[str, Any]:
+        variables['getRunLogsInput']['offset'] = self.num_bytes_read
+        return variables
 
     def parse_message(self, data: Dict[str, str]) -> str:
         """Get the next message from the GraphQL logging subscription
         """
 
         # Convert from base64 string to a bytestring
         b64_message = data['getRunLogs']
 
         b64_bytes = b64_message.encode('utf8')
         message_bytes = base64.b64decode(b64_bytes)
 
-        # Add any previous hanging bytes
-        byte_str: bytes = self.remaining + message_bytes
-
-        # Decode whatever we can
-        decoded, self.remaining = careful_decode(byte_str)
-
-        # Combine with previous, if needed
-        decoded, self.prev = self.prev + decoded, ''
-
-        self.num_bytes_read = self.num_bytes_read + len(byte_str)
-
-        return decoded
-
-    def update_offset(self, variables: Dict[str, Any]) -> Dict[str, Any]:
-        variables['getRunLogsInput']['offset'] = self.num_bytes_read
-        return variables
+        return self.decode(message_bytes)
```

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.3.9/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.3.9/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.3.9/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.3.9/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.3.9/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/typing_future.py` & `mosaicml-cli-0.3.9/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.3.9/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/cli.py` & `mosaicml-cli-0.3.9/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.3.9/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.3.9/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_clean/m_clean.py` & `mosaicml-cli-0.3.9/mcli/cli/m_clean/m_clean.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.3.9/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_create/cluster.py` & `mosaicml-cli-0.3.9/mcli/cli/m_create/cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_create/env_var.py` & `mosaicml-cli-0.3.9/mcli/cli/m_create/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.3.9/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.3.9/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.3.9/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.3.9/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.3.9/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.3.9/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.3.9/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/__init__.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/display.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/envvars.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/envvars.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from mcli.sdk import InferenceDeployment
 from mcli.utils.utils_cli import SubmissionType
 
 
 class InferenceDeploymentColumns(Enum):
     ID = 'id'
     NAME = 'name'
+    USER = 'user'
     CLUSTER = 'cluster'
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
     CREATED_TIME = 'created_time'
     STATUS = 'status'
 
 
@@ -29,24 +30,26 @@
 class InferenceDeploymentDisplayItem(MCLIDisplayItem):
     """Tuple that extracts deployment data for display purposes.
     """
     name: str
     gpu_num: str
     created_time: str
     status: str
+    user: str
     cluster: Optional[str] = None
     gpu_type: Optional[str] = None
     id: Optional[str] = None
 
     @classmethod
     def from_deployment(cls,
                         deployment: InferenceDeployment,
                         include_ids: bool = False) -> InferenceDeploymentDisplayItem:
         extracted: Dict[str, str] = {
             InferenceDeploymentColumns.NAME.value: deployment.name,
+            InferenceDeploymentColumns.USER.value: deployment.created_by,
             InferenceDeploymentColumns.GPU_NUM.value: str(deployment.config.gpu_num),
             InferenceDeploymentColumns.CREATED_TIME.value: format_timestamp(deployment.created_at),
             InferenceDeploymentColumns.STATUS.value: deployment.status,
             InferenceDeploymentColumns.CLUSTER.value: deployment.config.cluster,
             InferenceDeploymentColumns.GPU_TYPE.value: deployment.config.gpu_type
         }
         if include_ids:
```

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_get/users.py` & `mosaicml-cli-0.3.9/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.3.9/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.3.9/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.3.9/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.3.9/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_interactive/temp_mcloud_interactive.py` & `mosaicml-cli-0.3.9/mcli/cli/m_interactive/temp_mcloud_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.3.9/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.3.9/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.3.9/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.3.9/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.3.9/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.3.9/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.3.9/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_use/m_use.py` & `mosaicml-cli-0.3.9/mcli/cli/m_use/m_use.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_util/kube_util.py` & `mosaicml-cli-0.3.9/mcli/cli/m_util/kube_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.3.9/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/cli/m_util/util.py` & `mosaicml-cli-0.3.9/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/config.py` & `mosaicml-cli-0.3.9/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/__init__.py` & `mosaicml-cli-0.3.9/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.3.9/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/mcli_cluster.py` & `mosaicml-cli-0.3.9/mcli/models/mcli_cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.3.9/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/mcli_integration.py` & `mosaicml-cli-0.3.9/mcli/models/mcli_integration.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/mcli_secret.py` & `mosaicml-cli-0.3.9/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/models/run_config.py` & `mosaicml-cli-0.3.9/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/__init__.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/apt_packages.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/apt_packages.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/comet.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/comet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/git_repo.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/git_repo.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/local.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/mosaicml_agent.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/mosaicml_agent.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/pip_packages.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/pip_packages.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/integrations/wandb.py` & `mosaicml-cli-0.3.9/mcli/objects/integrations/wandb.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/cluster_secret.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/cluster_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.3.9/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.3.9/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/sdk/__init__.py` & `mosaicml-cli-0.3.9/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster_instances.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_instances.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/cluster_pv_setup.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/cluster_pv_setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/gpu_type.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/instance_type.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/instance_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/__init__.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/microk8s.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/microk8s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r10z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r10z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r1z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r1z4.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r1z4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r3z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r3z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r4z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r4z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z10.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z2.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z3.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z4.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z5.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z5.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z6.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z6.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z7.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z7.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r7z9.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r7z9.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z2.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r8z3.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r8z3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/clusters/overrides/r99z1.py` & `mosaicml-cli-0.3.9/mcli/serverside/clusters/overrides/r99z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/job/mcli_job.py` & `mosaicml-cli-0.3.9/mcli/serverside/job/mcli_job.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_job.py` & `mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_job_typing.py` & `mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_job_typing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py` & `mosaicml-cli-0.3.9/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/serverside/runners/runner.py` & `mosaicml-cli-0.3.9/mcli/serverside/runners/runner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_cli.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_config.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_date.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_docker.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_file.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_file.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_kube.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_kube_labels.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_kube_labels.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_logging.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_rancher.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_rancher.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_rich.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_types.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.3.9/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/mcli/version.py` & `mosaicml-cli-0.3.9/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,13 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
+
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.3.8/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.3.9/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.8/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.3.9/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 mcli/utils/utils_docker.py
 mcli/utils/utils_epilog.py
 mcli/utils/utils_file.py
 mcli/utils/utils_interactive.py
 mcli/utils/utils_kube.py
 mcli/utils/utils_kube_labels.py
 mcli/utils/utils_logging.py
+mcli/utils/utils_message_decoding.py
 mcli/utils/utils_modules.py
 mcli/utils/utils_pypi.py
 mcli/utils/utils_rancher.py
 mcli/utils/utils_rich.py
 mcli/utils/utils_run_status.py
 mcli/utils/utils_serializable_dataclass.py
 mcli/utils/utils_spinner.py
```

### Comparing `mosaicml-cli-0.3.8/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.3.9/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 typing_extensions>=4.0.1
 arrow>=1.2.2
 docker>=5.0.3
 gql[websockets]>=3.4.0
 protobuf>=4.22.0
 
 [all]
-sphinxemoji>=0.2.0
-pytest-cov>=4.0.0
-sphinx_external_toc>=0.3.0
+pylint>=2.12.2
+sphinx>=4.4.0
+sphinx-panels>=0.6.0
+sphinxext-opengraph>=0.6.1
+sphinxcontrib-jsmath>=1.0.1
 pytest>=6.2.5
-sphinx-copybutton>=0.5.0
-sphinx-rtd-theme>=1.0.0
-sphinxcontrib-devhelp>=1.0.2
+isort>=5.9.3
+pytest-mock>=3.7.0
 sphinxcontrib-serializinghtml>=1.1.5
-furo>=2022.3.4
-pyright>=1.1.256
+sphinxcontrib-devhelp>=1.0.2
+sphinx-argparse>=0.3.1
 myst-parser>=0.16.1
+sphinxemoji>=0.2.0
+sphinxcontrib-katex>=0.8.6
+pyright>=1.1.256
+pre-commit>=2.17.0
+yapf==0.33.0
+sphinxcontrib-applehelp>=1.0.2
 sphinxcontrib-images>=0.9.4
 sphinxcontrib-htmlhelp>=2.0.0
-sphinx>=4.4.0
-isort>=5.9.3
-sphinxcontrib-jsmath>=1.0.1
-sphinx-panels>=0.6.0
 sphinx-markdown-tables>=0.0.15
+sphinx-copybutton>=0.5.0
+sphinxcontrib-qthelp>=1.0.3
 radon>=5.1.0
-sphinxext-opengraph>=0.6.1
-sphinxcontrib-applehelp>=1.0.2
+sphinx-rtd-theme>=1.0.0
 sphinx-design
-sphinxcontrib-katex>=0.8.6
-yapf==0.33.0
-sphinx-argparse>=0.3.1
-pylint>=2.12.2
-pre-commit>=2.17.0
-pytest-mock>=3.7.0
-sphinxcontrib-qthelp>=1.0.3
+pytest-cov>=4.0.0
+furo>=2022.3.4
+sphinx_external_toc>=0.3.0
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest>=6.2.5
```

### Comparing `mosaicml-cli-0.3.8/pyproject.toml` & `mosaicml-cli-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -666,21 +666,14 @@
 # character used as a quote delimiter is used inconsistently within a module.
 check-quote-consistency="no"
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps="no"
 
-[tool.pylint.typecheck]
-
-# List of members which are set dynamically and missed by pylint inference
-# system, and so shouldn't trigger E1101 when accessed. Python regular
-# expressions are accepted.
-generated-members="^_.*"
-
 
 [tool.pylint.logging]
 
 # The type of string formatting that logging methods do. `old` means using %
 # formatting, `new` is for `{}` formatting.
 logging-format-style="new"
```

### Comparing `mosaicml-cli-0.3.8/setup.py` & `mosaicml-cli-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/tests/submit/test_cluster.py` & `mosaicml-cli-0.3.9/tests/submit/test_cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/tests/submit/test_cluster_secrets.py` & `mosaicml-cli-0.3.9/tests/submit/test_cluster_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/tests/test_config.py` & `mosaicml-cli-0.3.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.8/tests/test_upgrade.py` & `mosaicml-cli-0.3.9/tests/test_upgrade.py`

 * *Files identical despite different names*

