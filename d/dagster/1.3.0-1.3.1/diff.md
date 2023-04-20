# Comparing `tmp/dagster-1.3.0.tar.gz` & `tmp/dagster-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.0.tar", last modified: Wed Apr 19 19:01:52 2023, max compression
+gzip compressed data, was "dagster-1.3.1.tar", last modified: Thu Apr 20 20:39:23 2023, max compression
```

## Comparing `dagster-1.3.0.tar` & `dagster-1.3.1.tar`

### file list

```diff
@@ -1,625 +1,625 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-19 19:01:29.000000 dagster-1.3.0/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-19 19:01:29.000000 dagster-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 19:01:29.000000 dagster-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-19 19:01:52.727803 dagster-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-04-19 19:01:29.000000 dagster-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/
--rw-r--r--   0 root         (0) root         (0)    25230 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27263 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8207 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    33891 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5141 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28486 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    17554 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    58020 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7997 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10380 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)    22609 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_group.py
--rw-r--r--   0 root         (0) root         (0)     3817 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36853 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    46445 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    17185 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    58973 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24065 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    15537 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45721 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10877 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20634 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40545 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9563 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17810 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14491 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11914 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6695 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20403 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39915 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31183 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21562 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16178 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44593 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22927 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)    46583 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32712 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/mode.py
--rw-r--r--   0 root         (0) root         (0)    55735 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    21561 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11938 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19242 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)    18917 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    44376 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    34900 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/pipeline_definition.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)     9054 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/preset.py
--rw-r--r--   0 root         (0) root         (0)    30644 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    23982 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    19736 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    19180 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8118 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    25522 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14975 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    37627 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    35100 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    43829 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14153 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    73361 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15807 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    65032 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.683803 dagster-1.3.0/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41958 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    25196 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14370 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.683803 dagster-1.3.0/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    27186 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27826 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    34437 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    43261 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    20099 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context_creation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     6480 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_job_result.py
--rw-r--r--   0 root         (0) root         (0)     9184 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8734 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23056 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7095 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16478 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27380 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10255 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    38667 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    60978 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15617 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    16031 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19527 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)    25987 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/results.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15452 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14347 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33996 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    33186 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    69685 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4341 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)    17332 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     5205 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/pipeline_index.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104545 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11577 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17327 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    18194 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.695803 dagster-1.3.0/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.695803 dagster-1.3.0/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4019 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12052 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)    17447 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/pipeline_snapshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.699803 dagster-1.3.0/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.699803 dagster-1.3.0/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16259 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    11527 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14277 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    77841 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18916 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)     9985 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26262 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17376 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23190 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)    23993 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/pipeline_run.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15584 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8629 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46721 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3660 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15907 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27288 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18883 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7393 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/utility_solids.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5451 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26703 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5450 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6882 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9124 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4422 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17726 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8371 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    35694 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.655803 dagster-1.3.0/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11665 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38179 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18538 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22252 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    52644 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26106 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      638 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32009 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    33924 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23212 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    23704 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    11139 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10483 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    23902 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24986 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1290 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-19 19:01:52.731804 dagster-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6429 2023-04-19 19:01:30.000000 dagster-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.236790 dagster-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-20 20:39:02.000000 dagster-1.3.1/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-20 20:39:02.000000 dagster-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-20 20:39:02.000000 dagster-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-20 20:39:23.236790 dagster-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-04-20 20:39:02.000000 dagster-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.152789 dagster-1.3.1/dagster/
+-rw-r--r--   0 root         (0) root         (0)    25230 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27263 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8207 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    33891 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5141 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.160790 dagster-1.3.1/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28486 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.160790 dagster-1.3.1/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14686 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18799 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    17554 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    58149 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10380 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)    22609 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_group.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36853 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    46445 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    17185 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    58973 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24065 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15537 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45721 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10877 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20634 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40545 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17810 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14491 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11914 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20547 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31183 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21562 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44593 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22927 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)    46583 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32712 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/mode.py
+-rw-r--r--   0 root         (0) root         (0)    55735 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    21561 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    20633 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19242 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    44192 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    34900 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/pipeline_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9054 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/preset.py
+-rw-r--r--   0 root         (0) root         (0)    30644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.184790 dagster-1.3.1/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    23982 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    19736 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    19180 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8118 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    25522 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14975 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    37627 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    35100 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    44640 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    74443 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15807 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.184790 dagster-1.3.1/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    65032 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.188790 dagster-1.3.1/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41958 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    25196 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.188790 dagster-1.3.1/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    27186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27826 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34437 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    43261 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    20099 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context_creation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_job_result.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8734 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14650 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23056 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7095 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27380 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10255 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    38667 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    60978 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15617 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    16031 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19527 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)    25987 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/results.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15452 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14347 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33996 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    33186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    69685 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)    17332 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/pipeline_index.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104545 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11577 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17327 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18194 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20631 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.200790 dagster-1.3.1/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4019 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12052 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)    17447 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/pipeline_snapshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.204790 dagster-1.3.1/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.204790 dagster-1.3.1/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8073 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16259 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    11527 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    77841 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18916 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9985 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26262 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17376 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23190 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)    23993 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/pipeline_run.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15584 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46721 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15907 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27288 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18883 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7393 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/utility_solids.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5451 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26703 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9124 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17726 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8371 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    35694 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.148790 dagster-1.3.1/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11665 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38179 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    22252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    52644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26106 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32009 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    33924 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.232790 dagster-1.3.1/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23212 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    23704 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.232790 dagster-1.3.1/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10483 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    23902 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.236790 dagster-1.3.1/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.152789 dagster-1.3.1/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24986 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-20 20:39:23.236790 dagster-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-04-20 20:39:02.000000 dagster-1.3.1/setup.py
```

### Comparing `dagster-1.3.0/COPYING` & `dagster-1.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/LICENSE` & `dagster-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/PKG-INFO` & `dagster-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.0
+Version: 1.3.1
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.0/README.md` & `dagster-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/__init__.py` & `dagster-1.3.1/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_annotations.py` & `dagster-1.3.1/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/get_server_id.py` & `dagster-1.3.1/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/list_repositories.py` & `dagster-1.3.1/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/notebook_data.py` & `dagster-1.3.1/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.1/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_partition.py` & `dagster-1.3.1/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_pipeline.py` & `dagster-1.3.1/dagster/_api/snapshot_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_repository.py` & `dagster-1.3.1/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_schedule.py` & `dagster-1.3.1/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_api/snapshot_sensor.py` & `dagster-1.3.1/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_check/README.md` & `dagster-1.3.1/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_check/__init__.py` & `dagster-1.3.1/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/__init__.py` & `dagster-1.3.1/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/api.py` & `dagster-1.3.1/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/asset.py` & `dagster-1.3.1/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/config_scaffolder.py` & `dagster-1.3.1/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/debug.py` & `dagster-1.3.1/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/dev.py` & `dagster-1.3.1/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/instance.py` & `dagster-1.3.1/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/job.py` & `dagster-1.3.1/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/load_handle.py` & `dagster-1.3.1/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/project.py` & `dagster-1.3.1/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/run.py` & `dagster-1.3.1/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/schedule.py` & `dagster-1.3.1/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/sensor.py` & `dagster-1.3.1/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/utils.py` & `dagster-1.3.1/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.1/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/__init__.py` & `dagster-1.3.1/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/config_schema.py` & `dagster-1.3.1/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/config_type.py` & `dagster-1.3.1/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/errors.py` & `dagster-1.3.1/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/evaluate_value_result.py` & `dagster-1.3.1/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/field.py` & `dagster-1.3.1/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/field_utils.py` & `dagster-1.3.1/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/post_process.py` & `dagster-1.3.1/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/primitive_mapping.py` & `dagster-1.3.1/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.1/dagster/_config/pythonic_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DagsterInvalidConfigDefinitionError,
     DagsterInvalidConfigError,
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidPythonicConfigDefinitionError,
 )
 from dagster._core.execution.context.init import InitResourceContext
-from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX
+from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX, cached_method
 
 from .attach_other_object_to_context import (
     IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
 )
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
@@ -643,14 +643,15 @@
     def _nested_resources(self):
         return self._state__internal__.nested_resources
 
     @property
     def _resolved_config_dict(self):
         return self._state__internal__.resolved_config_dict
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
             resource_fn=self._initialize_and_run,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
@@ -899,14 +900,15 @@
 
     @property
     def nested_resources(
         self,
     ) -> Mapping[str, CoercibleToResource]:
         return self._state__internal__.nested_resources
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
             resource_fn=self._state__internal__.resource_fn,
             config_schema=self._state__internal__.config_schema,
             description=self._state__internal__.description,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
@@ -966,14 +968,15 @@
     """
 
     @property
     @abstractmethod
     def wrapped_resource(self) -> ResourceDefinition:
         raise NotImplementedError()
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
             resource_fn=self.wrapped_resource.resource_fn,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
@@ -1012,14 +1015,15 @@
     @classmethod
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialIOManager[Self]":
         """Returns a partially initialized copy of the IO manager, with remaining config fields
         set at runtime.
         """
         return PartialIOManager(cls, data=kwargs)
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
         return ConfigurableIOManagerFactoryResourceDefinition(
             resource_fn=self._initialize_and_run,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
@@ -1028,14 +1032,15 @@
 
 class PartialIOManager(Generic[TResValue], PartialResource[TResValue]):
     def __init__(
         self, resource_cls: Type[ConfigurableResourceFactory[TResValue]], data: Dict[str, Any]
     ):
         PartialResource.__init__(self, resource_cls, data)
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
         return ConfigurableIOManagerFactoryResourceDefinition(
             resource_fn=self._state__internal__.resource_fn,
             config_schema=self._state__internal__.config_schema,
             description=self._state__internal__.description,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self._state__internal__.nested_resources,
@@ -1260,14 +1265,15 @@
         raise NotImplementedError()
 
     def create_io_manager(self, context) -> IOManager:
         raise NotImplementedError(
             "Because we override resource_fn in the adapter, this is never called."
         )
 
+    @cached_method
     def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
         return ConfigurableIOManagerFactoryResourceDefinition(
             resource_fn=self.wrapped_io_manager.resource_fn,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
```

### Comparing `dagster-1.3.0/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.1/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.1/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.1/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/snap.py` & `dagster-1.3.1/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/source.py` & `dagster-1.3.1/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/stack.py` & `dagster-1.3.1/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/traversal_context.py` & `dagster-1.3.1/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/type_printer.py` & `dagster-1.3.1/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_config/validate.py` & `dagster-1.3.1/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/assets.py` & `dagster-1.3.1/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/code_pointer.py` & `dagster-1.3.1/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/container_context/config.py` & `dagster-1.3.1/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/debug.py` & `dagster-1.3.1/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/decorator_utils.py` & `dagster-1.3.1/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/__init__.py` & `dagster-1.3.1/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.1/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.1/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_group.py` & `dagster-1.3.1/dagster/_core/definitions/asset_group.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_in.py` & `dagster-1.3.1/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.1/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_out.py` & `dagster-1.3.1/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.1/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.1/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/assets.py` & `dagster-1.3.1/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/assets_job.py` & `dagster-1.3.1/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.1/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.1/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/composition.py` & `dagster-1.3.1/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/config.py` & `dagster-1.3.1/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/configurable.py` & `dagster-1.3.1/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/data_time.py` & `dagster-1.3.1/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/data_version.py` & `dagster-1.3.1/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.1/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.1/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.1/dagster/_core/definitions/definitions_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,21 @@
             and schedule.has_loadable_target()
             and schedule.job in unsatisfied_jobs
         )
         else schedule
         for schedule in schedules
     ]
     updated_sensors = [
-        sensor.with_updated_job(unsatisfied_job_to_resource_bound_job[id(sensor.job)])
-        if sensor.has_loadable_targets() and sensor.job in unsatisfied_jobs
+        sensor.with_updated_jobs(
+            [
+                unsatisfied_job_to_resource_bound_job[id(job)] if job in unsatisfied_jobs else job
+                for job in sensor.jobs
+            ]
+        )
+        if sensor.has_loadable_targets() and any(job in unsatisfied_jobs for job in sensor.jobs)
         else sensor
         for sensor in sensors
     ]
 
     return _AttachedObjects(jobs_with_resources, updated_schedules, updated_sensors)
```

### Comparing `dagster-1.3.0/dagster/_core/definitions/dependency.py` & `dagster-1.3.1/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/events.py` & `dagster-1.3.1/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.1/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.1/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.1/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.1/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.1/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/inference.py` & `dagster-1.3.1/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/input.py` & `dagster-1.3.1/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.1/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/job_definition.py` & `dagster-1.3.1/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.1/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.1/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.1/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/materialize.py` & `dagster-1.3.1/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.1/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.1/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/mode.py` & `dagster-1.3.1/dagster/_core/definitions/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.1/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/node_container.py` & `dagster-1.3.1/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/node_definition.py` & `dagster-1.3.1/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/observe.py` & `dagster-1.3.1/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/op_definition.py` & `dagster-1.3.1/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.1/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/output.py` & `dagster-1.3.1/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/partition.py` & `dagster-1.3.1/dagster/_core/definitions/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -833,24 +833,21 @@
 
     def _key_to_partition(
         self,
         partition_key: str,
         current_time: Optional[datetime],
         dynamic_partitions_store: Optional[DynamicPartitionsStore],
     ) -> Partition[T_cov]:
-        matches = [
-            p
-            for p in self.partitions_def.get_partitions(
-                current_time=current_time, dynamic_partitions_store=dynamic_partitions_store
-            )
-            if p.name == partition_key
-        ]
-        if len(matches) == 0:
-            raise DagsterUnknownPartitionError(f"No partition for partition key `{partition_key}`.")
-        return matches[0]
+        partition = self.partitions_def.get_partition(
+            partition_key,
+            current_time=current_time,
+            dynamic_partitions_store=dynamic_partitions_store,
+        )
+
+        return partition
 
     @classmethod
     def from_flexible_config(
         cls,
         config: Optional[Union[ConfigMapping, Mapping[str, object], "PartitionedConfig"]],
         partitions_def: PartitionsDefinition,
     ) -> "PartitionedConfig":
```

### Comparing `dagster-1.3.0/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.1/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.1/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/pipeline_base.py` & `dagster-1.3.1/dagster/_core/definitions/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/pipeline_definition.py` & `dagster-1.3.1/dagster/_core/definitions/pipeline_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/policy.py` & `dagster-1.3.1/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/preset.py` & `dagster-1.3.1/dagster/_core/definitions/preset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.1/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.1/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.1/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.1/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.1/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.1/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.1/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/run_config.py` & `dagster-1.3.1/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.1/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/run_request.py` & `dagster-1.3.1/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.1/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.1/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/selector.py` & `dagster-1.3.1/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.1/dagster/_core/definitions/sensor_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,31 +459,41 @@
         jobs (Optional[Sequence[GraphDefinition, JobDefinition, UnresolvedAssetJob]]): (experimental) A list of jobs to execute when this sensor fires.
         default_status (DefaultSensorStatus): Whether the sensor starts as running or not. The default
             status can be overridden from Dagit or via the GraphQL API.
         asset_selection (AssetSelection): (Experimental) an asset selection to launch a run for if
             the sensor condition is met. This can be provided instead of specifying a job.
     """
 
-    def with_updated_job(self, new_job: ExecutableDefinition) -> "SensorDefinition":
-        """Returns a copy of this schedule with the job replaced.
+    def with_updated_jobs(self, new_jobs: Sequence[ExecutableDefinition]) -> "SensorDefinition":
+        """Returns a copy of this sensor with the jobs replaced.
 
         Args:
             job (ExecutableDefinition): The job that should execute when this
                 schedule runs.
         """
         return SensorDefinition(
             name=self.name,
             evaluation_fn=self._evaluation_fn,
             minimum_interval_seconds=self.minimum_interval_seconds,
             description=self.description,
-            job=new_job,
+            jobs=new_jobs if len(new_jobs) > 1 else None,
+            job=new_jobs[0] if len(new_jobs) == 1 else None,
             default_status=self.default_status,
             asset_selection=self.asset_selection,
         )
 
+    def with_updated_job(self, new_job: ExecutableDefinition) -> "SensorDefinition":
+        """Returns a copy of this sensor with the job replaced.
+
+        Args:
+            job (ExecutableDefinition): The job that should execute when this
+                schedule runs.
+        """
+        return self.with_updated_jobs([new_job])
+
     def __init__(
         self,
         name: Optional[str] = None,
         *,
         evaluation_fn: Optional[RawSensorEvaluationFunction] = None,
         job_name: Optional[str] = None,
         minimum_interval_seconds: Optional[int] = None,
@@ -619,14 +629,21 @@
                 return self._targets[0].target
             elif len(self._targets) > 1:
                 raise DagsterInvalidDefinitionError(
                     "Job property not available when SensorDefinition has multiple jobs."
                 )
         raise DagsterInvalidDefinitionError("No job was provided to SensorDefinition.")
 
+    @public
+    @property
+    def jobs(self) -> List[Union[JobDefinition, GraphDefinition, UnresolvedAssetJobDefinition]]:
+        if self._targets and all(isinstance(target, DirectTarget) for target in self._targets):
+            return [target.target for target in self._targets]
+        raise DagsterInvalidDefinitionError("No job was provided to SensorDefinition.")
+
     @property
     def sensor_type(self) -> SensorType:
         return SensorType.STANDARD
 
     def evaluate_tick(self, context: "SensorEvaluationContext") -> "SensorExecutionData":
         """Evaluate sensor using the provided context.
```

### Comparing `dagster-1.3.0/dagster/_core/definitions/source_asset.py` & `dagster-1.3.1/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.1/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/target.py` & `dagster-1.3.1/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.1/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.1/dagster/_core/definitions/time_window_partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 from dagster._utils.partitions import DEFAULT_HOURLY_FORMAT_WITHOUT_TIMEZONE
 from dagster._utils.schedules import (
     cron_string_iterator,
     is_valid_cron_schedule,
     reverse_cron_string_iterator,
 )
 
-from ..errors import DagsterInvalidDefinitionError, DagsterInvalidDeserializationVersionError
+from ..errors import (
+    DagsterInvalidDefinitionError,
+    DagsterInvalidDeserializationVersionError,
+    DagsterUnknownPartitionError,
+)
 from .partition import (
     DEFAULT_DATE_FORMAT,
     Partition,
     PartitionedConfig,
     PartitionsDefinition,
     PartitionsSubset,
     ScheduleType,
@@ -240,14 +244,54 @@
                 break
 
         if self.end_offset < 0:
             partitions = partitions[: self.end_offset]
 
         return partitions
 
+    def _get_validated_time_window_for_partition_key(
+        self, partition_key: str, current_time: Optional[datetime] = None
+    ) -> Optional[TimeWindow]:
+        """Returns a TimeWindow for the given partition key if it is valid, otherwise returns None.
+        """
+        try:
+            time_window = self.time_window_for_partition_key(partition_key)
+        except ValueError:
+            return None
+
+        first_partition_window = self.get_first_partition_window(current_time=current_time)
+        last_partition_window = self.get_last_partition_window(current_time=current_time)
+        if (
+            first_partition_window is None
+            or last_partition_window is None
+            or time_window.start < first_partition_window.start
+            or time_window.start > last_partition_window.start
+            or time_window.start.strftime(self.fmt) != partition_key
+        ):
+            return None
+
+        return time_window
+
+    def get_partition(
+        self,
+        partition_key: str,
+        current_time: Optional[datetime] = None,
+        dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
+    ) -> Partition[TimeWindow]:
+        time_window = self._get_validated_time_window_for_partition_key(
+            partition_key, current_time=current_time
+        )
+
+        if time_window is None:
+            raise DagsterUnknownPartitionError(
+                f"Could not find a partition with key `{partition_key}`"
+            )
+
+        return Partition(value=time_window, name=partition_key)
+
     def __str__(self) -> str:
         schedule_str = (
             self.schedule_type.value.capitalize() if self.schedule_type else self.cron_schedule
         )
         partition_def_str = (
             f"{schedule_str}, starting {self.start.strftime(self.fmt)} {self.timezone}."
         )
@@ -709,30 +753,16 @@
 
     def has_partition_key(
         self,
         partition_key: str,
         current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> bool:
-        try:
-            time_window = self.time_window_for_partition_key(partition_key)
-        except ValueError:
-            return False
-
-        first_partition_window = self.get_first_partition_window(current_time=current_time)
-        last_partition_window = self.get_last_partition_window(current_time=current_time)
-        if (
-            first_partition_window is None
-            or last_partition_window is None
-            or time_window.start < first_partition_window.start
-            or time_window.start > last_partition_window.start
-        ):
-            return False
-
-        return time_window.start.strftime(self.fmt) == partition_key
+        time_window = self._get_validated_time_window_for_partition_key(partition_key, current_time)
+        return True if time_window else False
 
 
 class DailyPartitionsDefinition(TimeWindowPartitionsDefinition):
     """A set of daily partitions.
 
     The first partition in the set will start at the start_date at midnight. The last partition
     in the set will end before the current time, unless the end_offset argument is set to a
```

### Comparing `dagster-1.3.0/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.1/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/utils.py` & `dagster-1.3.1/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.1/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/errors.py` & `dagster-1.3.1/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/event_api.py` & `dagster-1.3.1/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/events/__init__.py` & `dagster-1.3.1/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/events/log.py` & `dagster-1.3.1/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/events/utils.py` & `dagster-1.3.1/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/api.py` & `dagster-1.3.1/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.1/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/backfill.py` & `dagster-1.3.1/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/build_resources.py` & `dagster-1.3.1/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/compute_logs.py` & `dagster-1.3.1/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/compute.py` & `dagster-1.3.1/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/hook.py` & `dagster-1.3.1/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/init.py` & `dagster-1.3.1/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/input.py` & `dagster-1.3.1/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/invocation.py` & `dagster-1.3.1/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/logger.py` & `dagster-1.3.1/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/output.py` & `dagster-1.3.1/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context/system.py` & `dagster-1.3.1/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/context_creation_pipeline.py` & `dagster-1.3.1/dagster/_core/execution/context_creation_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.1/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.1/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/execute_job_result.py` & `dagster-1.3.1/dagster/_core/execution/execute_job_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/execution_result.py` & `dagster-1.3.1/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/host_mode.py` & `dagster-1.3.1/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/job_backfill.py` & `dagster-1.3.1/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/memoization.py` & `dagster-1.3.1/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/active.py` & `dagster-1.3.1/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/compute.py` & `dagster-1.3.1/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.1/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.1/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.1/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.1/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/handle.py` & `dagster-1.3.1/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.1/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.1/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/objects.py` & `dagster-1.3.1/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.1/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/plan.py` & `dagster-1.3.1/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/state.py` & `dagster-1.3.1/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/step.py` & `dagster-1.3.1/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/plan/utils.py` & `dagster-1.3.1/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.1/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.1/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/resources_init.py` & `dagster-1.3.1/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/results.py` & `dagster-1.3.1/dagster/_core/execution/results.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/retries.py` & `dagster-1.3.1/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.1/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/stats.py` & `dagster-1.3.1/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/tags.py` & `dagster-1.3.1/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.1/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.1/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/execution/with_resources.py` & `dagster-1.3.1/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/base.py` & `dagster-1.3.1/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.1/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/in_process.py` & `dagster-1.3.1/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/init.py` & `dagster-1.3.1/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/multiprocess.py` & `dagster-1.3.1/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.1/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/__init__.py` & `dagster-1.3.1/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/code_location.py` & `dagster-1.3.1/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/external.py` & `dagster-1.3.1/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/external_data.py` & `dagster-1.3.1/dagster/_core/host_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.1/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.1/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/handle.py` & `dagster-1.3.1/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/historical.py` & `dagster-1.3.1/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/origin.py` & `dagster-1.3.1/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/pipeline_index.py` & `dagster-1.3.1/dagster/_core/host_representation/pipeline_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/host_representation/represented.py` & `dagster-1.3.1/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/instance/__init__.py` & `dagster-1.3.1/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/instance/config.py` & `dagster-1.3.1/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/instance/ref.py` & `dagster-1.3.1/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/instance_for_test.py` & `dagster-1.3.1/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/launcher/base.py` & `dagster-1.3.1/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.1/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.1/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/log_manager.py` & `dagster-1.3.1/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/nux.py` & `dagster-1.3.1/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/origin.py` & `dagster-1.3.1/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/run_coordinator/base.py` & `dagster-1.3.1/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.1/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.1/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/scheduler/__init__.py` & `dagster-1.3.1/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/scheduler/execution.py` & `dagster-1.3.1/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/scheduler/instigation.py` & `dagster-1.3.1/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.1/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/secrets/env_file.py` & `dagster-1.3.1/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/selector/subset_selector.py` & `dagster-1.3.1/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/__init__.py` & `dagster-1.3.1/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/config_types.py` & `dagster-1.3.1/dagster/_core/snap/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/dagster_types.py` & `dagster-1.3.1/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.1/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.1/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/mode.py` & `dagster-1.3.1/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/node.py` & `dagster-1.3.1/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/snap/pipeline_snapshot.py` & `dagster-1.3.1/dagster/_core/snap/pipeline_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.1/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/README.md` & `dagster-1.3.1/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/env.py` & `dagster-1.3.1/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.1/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/base_storage.py` & `dagster-1.3.1/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.1/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.1/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.1/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/config.py` & `dagster-1.3.1/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.1/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/base.py` & `dagster-1.3.1/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.1/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.1/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.1/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.1/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.1/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/file_manager.py` & `dagster-1.3.1/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/input_manager.py` & `dagster-1.3.1/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/io_manager.py` & `dagster-1.3.1/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.1/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.1/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/migration/utils.py` & `dagster-1.3.1/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.1/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/output_manager.py` & `dagster-1.3.1/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.1/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/pipeline_run.py` & `dagster-1.3.1/dagster/_core/storage/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/root.py` & `dagster-1.3.1/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.1/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/base.py` & `dagster-1.3.1/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.1/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/migration.py` & `dagster-1.3.1/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/schema.py` & `dagster-1.3.1/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.1/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/base.py` & `dagster-1.3.1/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.1/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.1/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.1/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/sql.py` & `dagster-1.3.1/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/sqlite.py` & `dagster-1.3.1/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.1/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/tags.py` & `dagster-1.3.1/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.1/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.1/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.1/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/system_config/objects.py` & `dagster-1.3.1/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/telemetry.py` & `dagster-1.3.1/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/telemetry_upload.py` & `dagster-1.3.1/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/test_utils.py` & `dagster-1.3.1/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.1/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/config_schema.py` & `dagster-1.3.1/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/dagster_type.py` & `dagster-1.3.1/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/decorator.py` & `dagster-1.3.1/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.1/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.1/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/python_dict.py` & `dagster-1.3.1/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/python_set.py` & `dagster-1.3.1/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/python_tuple.py` & `dagster-1.3.1/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/types/transform_typing.py` & `dagster-1.3.1/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/utility_solids.py` & `dagster-1.3.1/dagster/_core/utility_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/utils.py` & `dagster-1.3.1/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.1/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/config_schema.py` & `dagster-1.3.1/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/context.py` & `dagster-1.3.1/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/load.py` & `dagster-1.3.1/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/load_target.py` & `dagster-1.3.1/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/permissions.py` & `dagster-1.3.1/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_core/workspace/workspace.py` & `dagster-1.3.1/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/__init__.py` & `dagster-1.3.1/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/asset_daemon.py` & `dagster-1.3.1/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/backfill.py` & `dagster-1.3.1/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/cli/__init__.py` & `dagster-1.3.1/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/controller.py` & `dagster-1.3.1/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/daemon.py` & `dagster-1.3.1/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.1/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/sensor.py` & `dagster-1.3.1/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/types.py` & `dagster-1.3.1/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_daemon/workspace.py` & `dagster-1.3.1/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_generate/download.py` & `dagster-1.3.1/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_generate/generate.py` & `dagster-1.3.1/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.1/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.1/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/__init__.py` & `dagster-1.3.1/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/client.py` & `dagster-1.3.1/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/compile.py` & `dagster-1.3.1/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/impl.py` & `dagster-1.3.1/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/protos/api.proto` & `dagster-1.3.1/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/server.py` & `dagster-1.3.1/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/server_watcher.py` & `dagster-1.3.1/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/types.py` & `dagster-1.3.1/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_grpc/utils.py` & `dagster-1.3.1/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_legacy/__init__.py` & `dagster-1.3.1/dagster/_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_loggers/__init__.py` & `dagster-1.3.1/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_module_alias_map.py` & `dagster-1.3.1/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_scheduler/scheduler.py` & `dagster-1.3.1/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_scheduler/stale.py` & `dagster-1.3.1/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_serdes/__init__.py` & `dagster-1.3.1/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_serdes/config_class.py` & `dagster-1.3.1/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_serdes/ipc.py` & `dagster-1.3.1/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_serdes/serdes.py` & `dagster-1.3.1/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_serdes/utils.py` & `dagster-1.3.1/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_seven/__init__.py` & `dagster-1.3.1/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_seven/abc.py` & `dagster-1.3.1/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_seven/compat/pendulum.py` & `dagster-1.3.1/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/__init__.py` & `dagster-1.3.1/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/alert.py` & `dagster-1.3.1/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/backcompat.py` & `dagster-1.3.1/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/backoff.py` & `dagster-1.3.1/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/cached_method.py` & `dagster-1.3.1/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.1/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/dagster_type.py` & `dagster-1.3.1/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/error.py` & `dagster-1.3.1/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/external.py` & `dagster-1.3.1/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/forked_pdb.py` & `dagster-1.3.1/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/hosted_user_process.py` & `dagster-1.3.1/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/indenting_printer.py` & `dagster-1.3.1/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/interrupts.py` & `dagster-1.3.1/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/log.py` & `dagster-1.3.1/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/merger.py` & `dagster-1.3.1/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/net.py` & `dagster-1.3.1/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/schedules.py` & `dagster-1.3.1/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/tags.py` & `dagster-1.3.1/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/temp_file.py` & `dagster-1.3.1/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/test/__init__.py` & `dagster-1.3.1/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.1/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.1/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.1/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/timing.py` & `dagster-1.3.1/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/typing_api.py` & `dagster-1.3.1/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster/_utils/yaml_utils.py` & `dagster-1.3.1/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster.egg-info/PKG-INFO` & `dagster-1.3.1/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.0
+Version: 1.3.1
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.0/dagster.egg-info/SOURCES.txt` & `dagster-1.3.1/dagster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/dagster.egg-info/requires.txt` & `dagster-1.3.1/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.0/setup.py` & `dagster-1.3.1/setup.py`

 * *Files identical despite different names*

