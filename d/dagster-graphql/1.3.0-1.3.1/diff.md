# Comparing `tmp/dagster-graphql-1.3.0.tar.gz` & `tmp/dagster-graphql-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.0.tar", last modified: Wed Apr 19 19:09:39 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.1.tar", last modified: Thu Apr 20 20:47:19 2023, max compression
```

## Comparing `dagster-graphql-1.3.0.tar` & `dagster-graphql-1.3.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.736932 dagster-graphql-1.3.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-19 19:09:39.736932 dagster-graphql-1.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.652931 dagster-graphql-1.3.0/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.660931 dagster-graphql-1.3.0/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21649 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.676931 dagster-graphql-1.3.0/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.680931 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11579 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8860 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7594 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12620 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15390 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8258 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10803 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.708932 dagster-graphql-1.3.0/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40174 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    14982 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18079 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16228 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    11017 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     4947 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    22897 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.708932 dagster-graphql-1.3.0/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20899 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17864 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.720932 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11072 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39733 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.728932 dagster-graphql-1.3.0/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25590 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36131 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4051 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.732932 dagster-graphql-1.3.0/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7971 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.736932 dagster-graphql-1.3.0/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6376 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:09:39.652931 dagster-graphql-1.3.0/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4100 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 19:09:39.000000 dagster-graphql-1.3.0/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 19:09:39.736932 dagster-graphql-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-19 19:01:29.000000 dagster-graphql-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.691717 dagster-graphql-1.3.1/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.695718 dagster-graphql-1.3.1/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21649 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.707718 dagster-graphql-1.3.1/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.711718 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11579 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12620 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15390 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10803 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.735718 dagster-graphql-1.3.1/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40174 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    14982 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18079 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16228 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     4947 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    22897 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.735718 dagster-graphql-1.3.1/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20899 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    16816 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.743718 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11072 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39733 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25590 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36131 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4051 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29755 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.691717 dagster-graphql-1.3.1/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/setup.py
```

### Comparing `dagster-graphql-1.3.0/LICENSE` & `dagster-graphql-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/PKG-INFO` & `dagster-graphql-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.0
+Version: 1.3.1
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.0/dagster_graphql/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/cli.py` & `dagster-graphql-1.3.1/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/client/client.py` & `dagster-graphql-1.3.1/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.1/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/client/query.py` & `dagster-graphql-1.3.1/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.1/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.1/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/partition_sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -384,55 +384,27 @@
     isPrimaryDimension = graphene.NonNull(graphene.Boolean)
     dynamicPartitionsDefinitionName = graphene.Field(graphene.String)
 
     class Meta:
         name = "DimensionDefinitionType"
 
 
-class GrapheneTimePartitionsDefinitionMetadata(graphene.ObjectType):
-    startTime = graphene.NonNull(graphene.Float)
-    endTime = graphene.NonNull(graphene.Float)
-    startKey = graphene.NonNull(graphene.String)
-    endKey = graphene.NonNull(graphene.String)
-
-    class Meta:
-        name = "TimePartitionsDefinitionMetadata"
-
-
 class GraphenePartitionDefinition(graphene.ObjectType):
     description = graphene.NonNull(graphene.String)
     type = graphene.NonNull(GraphenePartitionDefinitionType)
     dimensionTypes = non_null_list(GrapheneDimensionDefinitionType)
-    timeWindowMetadata = graphene.Field(GrapheneTimePartitionsDefinitionMetadata)
     name = graphene.Field(graphene.String)
 
     class Meta:
         name = "PartitionDefinition"
 
-    def __init__(self, partition_def_data: ExternalPartitionsDefinitionData):
-        def _get_time_partitions_metadata(partition_def_data):
-            check.inst_param(
-                partition_def_data, "partition_def_data", ExternalTimeWindowPartitionsDefinitionData
-            )
-
-            partitions_def = partition_def_data.get_partitions_definition()
-            return GrapheneTimePartitionsDefinitionMetadata(
-                startTime=partitions_def.start.timestamp(),
-                endTime=partitions_def.get_current_timestamp(),
-                startKey=partitions_def.get_first_partition_key(),
-                endKey=partitions_def.get_last_partition_key(),
-            )
-
-        super().__init__(
-            description=str(partition_def_data.get_partitions_definition()),
-            type=GraphenePartitionDefinitionType.from_partition_def_data(partition_def_data),
-            name=partition_def_data.name
-            if isinstance(partition_def_data, ExternalDynamicPartitionsDefinitionData)
-            else None,
-            dimensionTypes=[
+    def resolve_dimensionTypes(self, _graphene_info):
+        partition_def_data = self._partition_def_data
+        return (
+            [
                 GrapheneDimensionDefinitionType(
                     name=dim.name,
                     description=str(dim.external_partitions_def_data.get_partitions_definition()),
                     type=GraphenePartitionDefinitionType.from_partition_def_data(
                         dim.external_partitions_def_data
                     ),
                     isPrimaryDimension=dim.name
@@ -456,17 +428,24 @@
                         partition_def_data
                     ),
                     isPrimaryDimension=True,
                     dynamicPartitionsDefinitionName=partition_def_data.name
                     if isinstance(partition_def_data, ExternalDynamicPartitionsDefinitionData)
                     else None,
                 )
-            ],
-            timeWindowMetadata=_get_time_partitions_metadata(partition_def_data)
-            if isinstance(partition_def_data, ExternalTimeWindowPartitionsDefinitionData)
+            ]
+        )
+
+    def __init__(self, partition_def_data: ExternalPartitionsDefinitionData):
+        self._partition_def_data = partition_def_data
+        super().__init__(
+            description=str(partition_def_data.get_partitions_definition()),
+            type=GraphenePartitionDefinitionType.from_partition_def_data(partition_def_data),
+            name=partition_def_data.name
+            if isinstance(partition_def_data, ExternalDynamicPartitionsDefinitionData)
             else None,
         )
 
 
 class GrapheneDimensionPartitionKeys(graphene.ObjectType):
     name = graphene.NonNull(graphene.String)
     partition_keys = non_null_list(graphene.String)
```

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.1/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.1/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.1/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.0
+Version: 1.3.1
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.0/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.1/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.0/setup.py` & `dagster-graphql-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.0",
+        "dagster==1.3.1",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

