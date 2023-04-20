# Comparing `tmp/caikit-0.1.3.tar.gz` & `tmp/caikit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.1.3.tar", last modified: Mon Apr 17 22:12:49 2023, max compression
+gzip compressed data, was "caikit-0.1.4.tar", last modified: Thu Apr 20 19:39:06 2023, max compression
```

## Comparing `caikit-0.1.3.tar` & `caikit-0.1.4.tar`

### file list

```diff
@@ -1,295 +1,294 @@
--rw-r--r--   0        0        0       60 2023-04-17 22:12:38.150926 caikit-0.1.3/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0     1272 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-04-17 22:12:38.154926 caikit-0.1.3/.gitignore
--rw-r--r--   0        0        0      310 2023-04-17 22:12:38.154926 caikit-0.1.3/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-17 22:12:38.154926 caikit-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-17 22:12:38.154926 caikit-0.1.3/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-17 22:12:38.154926 caikit-0.1.3/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-17 22:12:38.154926 caikit-0.1.3/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-17 22:12:38.154926 caikit-0.1.3/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-17 22:12:38.154926 caikit-0.1.3/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     6510 2023-04-17 22:12:38.154926 caikit-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-17 22:12:38.154926 caikit-0.1.3/LICENSE
--rw-r--r--   0        0        0       18 2023-04-17 22:12:38.154926 caikit-0.1.3/OWNERS
--rw-r--r--   0        0        0     3757 2023-04-17 22:12:38.154926 caikit-0.1.3/README.md
--rw-r--r--   0        0        0    44878 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit-overview.png
--rw-r--r--   0        0        0      323 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/__init__.py
--rw-r--r--   0        0        0     1861 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1104 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/config.py
--rw-r--r--   0        0        0     1010 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/config.yml
--rw-r--r--   0        0        0      962 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29207 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13676 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20773 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/model_manager.py
--rw-r--r--   0        0        0    51860 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module.py
--rw-r--r--   0        0        0     7643 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5493 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1032 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0     1787 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/config_utils.py
--rw-r--r--   0        0        0      637 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18275 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     5439 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/extension_utils.py
--rw-r--r--   0        0        0     4935 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1864 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32214 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     5353 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/config/config.yml
--rw-r--r--   0        0        0     1716 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13853 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6068 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12138 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4194 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    20064 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5611 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12289 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5768 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    10121 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10301 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4911 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8296 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12008 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14523 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10554 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1696 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/config_parser.py
--rw-r--r--   0        0        0     6692 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0     1686 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/log_config.py
--rw-r--r--   0        0        0    17900 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      837 2023-04-17 22:12:38.162926 caikit-0.1.3/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1154 2023-04-17 22:12:43.871383 caikit-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-17 22:12:38.162926 caikit-0.1.3/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-17 22:12:38.162926 caikit-0.1.3/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/base.py
--rw-r--r--   0        0        0     8909 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    12691 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26013 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    13533 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     2909 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     3080 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_config.py
--rw-r--r--   0        0        0      521 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_imports.py
--rw-r--r--   0        0        0    18331 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17317 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module.py
--rw-r--r--   0        0        0     4751 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8441 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0     1953 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_config_utils.py
--rw-r--r--   0        0        0    14999 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4408 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_extension_utils.py
--rw-r--r--   0        0        0     4972 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    15618 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      176 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1852 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2411 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1404 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2498 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      202 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/config.py
--rw-r--r--   0        0        0      141 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      933 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/studio_models/studio_block
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6439 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11774 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18079 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5053 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     3326 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3280 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18350 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     1372 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7923 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    12985 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3533 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7386 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29936 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    10451 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     3785 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_configs.py
--rw-r--r--   0        0        0     5041 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26086 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1025 2023-04-17 22:12:38.170926 caikit-0.1.3/tox.ini
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-20 19:38:57.270401 caikit-0.1.4/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0     1272 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-20 19:38:57.270401 caikit-0.1.4/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-04-20 19:38:57.270401 caikit-0.1.4/.gitignore
+-rw-r--r--   0        0        0      310 2023-04-20 19:38:57.270401 caikit-0.1.4/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-20 19:38:57.270401 caikit-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-20 19:38:57.270401 caikit-0.1.4/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-20 19:38:57.270401 caikit-0.1.4/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-20 19:38:57.274402 caikit-0.1.4/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-20 19:38:57.274402 caikit-0.1.4/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-20 19:38:57.274402 caikit-0.1.4/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     6510 2023-04-20 19:38:57.274402 caikit-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-20 19:38:57.274402 caikit-0.1.4/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-20 19:38:57.274402 caikit-0.1.4/OWNERS
+-rw-r--r--   0        0        0     3757 2023-04-20 19:38:57.274402 caikit-0.1.4/README.md
+-rw-r--r--   0        0        0    44878 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit-overview.png
+-rw-r--r--   0        0        0      323 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/__init__.py
+-rw-r--r--   0        0        0     1837 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1104 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/config/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/config/config.py
+-rw-r--r--   0        0        0     1010 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/config/config.yml
+-rw-r--r--   0        0        0      962 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29207 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13676 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20448 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    51878 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/module.py
+-rw-r--r--   0        0        0     7643 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-20 19:38:57.274402 caikit-0.1.4/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5500 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1001 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0     1787 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/config_utils.py
+-rw-r--r--   0        0        0      637 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18275 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1864 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     5353 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/config/config.yml
+-rw-r--r--   0        0        0     1716 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13853 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4703 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6068 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12138 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4194 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    20064 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5611 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12289 2023-04-20 19:38:57.278402 caikit-0.1.4/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     6831 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10177 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10301 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4911 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8296 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12008 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    14523 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10554 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1696 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/utils/config_parser.py
+-rw-r--r--   0        0        0     6692 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0     1686 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/utils/log_config.py
+-rw-r--r--   0        0        0    17900 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-20 19:38:57.282402 caikit-0.1.4/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0     3693 2023-04-20 19:38:57.282402 caikit-0.1.4/docs/adrs/README.md
+-rw-r--r--   0        0        0      837 2023-04-20 19:38:57.282402 caikit-0.1.4/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1154 2023-04-20 19:39:01.446621 caikit-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-20 19:38:57.282402 caikit-0.1.4/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-20 19:38:57.282402 caikit-0.1.4/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3783 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/base.py
+-rw-r--r--   0        0        0     8909 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    12691 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    13533 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     2909 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     3080 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/test_config.py
+-rw-r--r--   0        0        0      521 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/test_imports.py
+-rw-r--r--   0        0        0    18315 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17317 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/test_module.py
+-rw-r--r--   0        0        0     4751 2023-04-20 19:38:57.282402 caikit-0.1.4/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8441 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0     1953 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_config_utils.py
+-rw-r--r--   0        0        0    14999 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    15618 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      176 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2411 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1404 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2498 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      202 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/config.py
+-rw-r--r--   0        0        0      141 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.286402 caikit-0.1.4/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6439 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11774 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18079 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5053 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     1654 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     3326 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3280 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18350 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0      846 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1372 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7923 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    12985 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3533 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7386 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    29936 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    10451 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     3785 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/utils/test_configs.py
+-rw-r--r--   0        0        0     5041 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-20 19:38:57.290402 caikit-0.1.4/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1025 2023-04-20 19:38:57.290402 caikit-0.1.4/tox.ini
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.4/PKG-INFO
```

### Comparing `caikit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.1.4/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.github/workflows/build-library.yml` & `caikit-0.1.4/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.github/workflows/lint-code.yml` & `caikit-0.1.4/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.github/workflows/publish-library.yml` & `caikit-0.1.4/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/.pylintrc` & `caikit-0.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/CODE-OF-CONDUCT.md` & `caikit-0.1.4/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/CONTRIBUTING.md` & `caikit-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/LICENSE` & `caikit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/README.md` & `caikit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit-overview.png` & `caikit-0.1.4/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/__init__.py` & `caikit-0.1.4/caikit/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Caikit Core AI Framework library.  This is the base framework for core AI/ML libraries, such
-as NLP and Vision.
+"""Caikit Core AI Framework library.  This is the base framework for core AI/ML libraries.
 """
 
 # the import order cannot adhere to the linter here because we must do things like
 # disable warnings, initialize the JVM and configure logging in a specific order
 # pylint: disable=wrong-import-position,wrong-import-order
 
 # Standard
```

### Comparing `caikit-0.1.3/caikit/core/augmentors/__init__.py` & `caikit-0.1.4/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/base.py` & `caikit-0.1.4/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.1.4/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.1.4/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/schemes/base.py` & `caikit-0.1.4/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.1.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.1.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/blocks/__init__.py` & `caikit-0.1.4/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/blocks/base.py` & `caikit-0.1.4/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/config/__init__.py` & `caikit-0.1.4/caikit/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/config/config.py` & `caikit-0.1.4/caikit/core/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/config/config.yml` & `caikit-0.1.4/caikit/core/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/__init__.py` & `caikit-0.1.4/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/base.py` & `caikit-0.1.4/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.1.4/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/data_backends/base.py` & `caikit-0.1.4/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.1.4/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/dataobject.py` & `caikit-0.1.4/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/enums.py` & `caikit-0.1.4/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/producer.py` & `caikit-0.1.4/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.1.4/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/__init__.py` & `caikit-0.1.4/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/converter.py` & `caikit-0.1.4/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.1.4/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/data_stream.py` & `caikit-0.1.4/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/resolver.py` & `caikit-0.1.4/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/data_model/streams/validator.py` & `caikit-0.1.4/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/model_manager.py` & `caikit-0.1.4/caikit/core/model_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,19 +90,15 @@
 
         Returns:
             subclass of blocks.base.BlockBase
                 Model object that is loaded, configured, and ready for prediction.
         """
         error.type_check("<COR98255724E>", bool, load_singleton=load_singleton)
 
-        # This is mainly done for the caikit Studio integration so that the models are loadable from
-        # a volume mount such as `/opt/caikit/nlpmodels`. Note if the path exists we assume the
-        # customer is trying to load their own model (e.g,. a standard models saved to disk, or
-        # a custom model downloaded from Studio data assets. In that case we keep module_path
-        # intact.
+        # This allows a user to load their own model (e.g. model saved to disk)
         load_path = lib_config.load_path
         if load_path is not None and isinstance(module_path, str):
             if not os.path.exists(module_path):
                 module_path = os.path.join(load_path, module_path)
 
         # Ensure that we have a loadable directory.
         error.type_check("<COR98255419E>", str, BytesIO, bytes, module_path=module_path)
```

### Comparing `caikit-0.1.3/caikit/core/module.py` & `caikit-0.1.4/caikit/core/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             self._metadata = {}
         return self._metadata
 
     @classmethod
     @alog.logged_function(log.debug)
     def bootstrap(cls, *args, **kwargs):
         """Bootstrap a block. This method can be used to initialize the block
-        from artifacts created outside of caikitNLP
+        from artifacts created outside of a particular caikit library
         """
         error(
             "<COR92634438E>",
             NotImplementedError("This is not available in this module."),
         )
 
     @classmethod
```

### Comparing `caikit-0.1.3/caikit/core/module_backend_config.py` & `caikit-0.1.4/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/module_backends/__init__.py` & `caikit-0.1.4/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/module_backends/backend_types.py` & `caikit-0.1.4/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/module_backends/base.py` & `caikit-0.1.4/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/module_backends/local_backend.py` & `caikit-0.1.4/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/module_config.py` & `caikit-0.1.4/caikit/core/module_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # First Party
 import aconfig
 import alog
 
 # Local
 from . import toolkit
-from .toolkit import error_handler
+from .toolkit.errors import error_handler
 
 log = alog.use_channel("MODULE")
 error = error_handler.get(log)
 
 
 class ModuleConfig(aconfig.Config):
     """Config object used by all blocks for config loading, saving, etc."""
```

### Comparing `caikit-0.1.3/caikit/core/module_meta.py` & `caikit-0.1.4/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/resources/__init__.py` & `caikit-0.1.4/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/resources/base.py` & `caikit-0.1.4/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/__init__.py` & `caikit-0.1.4/caikit/core/toolkit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 """Contains many helpers, utilities, and commonly re-used code in the `caikit.core` library. Users
 may find helpful methods in here for more advanced use of this library.
 """
 # Local
 from . import compatibility, logging
 from .errors import *
-from .extension_utils import *
 from .fileio import *
 from .isa import *
 from .quality_evaluation import (
     EvalTypes,
     F1Metrics,
     F1MetricsContainer,
     QualityEvaluator,
```

### Comparing `caikit-0.1.3/caikit/core/toolkit/compatibility.py` & `caikit-0.1.4/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/config_utils.py` & `caikit-0.1.4/caikit/core/toolkit/config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/errors/__init__.py` & `caikit-0.1.4/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.1.4/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.1.4/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/fileio.py` & `caikit-0.1.4/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/isa.py` & `caikit-0.1.4/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/logging.py` & `caikit-0.1.4/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.1.4/caikit/core/toolkit/quality_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Evaluate quality of caikitNLP models.
+"""Evaluate quality of models.
 """
 
 # Standard
 from dataclasses import dataclass
 from typing import Dict, Optional
 import enum
 import math
```

### Comparing `caikit-0.1.3/caikit/core/toolkit/serializers.py` & `caikit-0.1.4/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/toolkit/wip_decorator.py` & `caikit-0.1.4/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/workflows/__init__.py` & `caikit-0.1.4/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/core/workflows/base.py` & `caikit-0.1.4/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/__init__.py` & `caikit-0.1.4/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/common/__init__.py` & `caikit-0.1.4/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.1.4/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/common/data_model/producer.py` & `caikit-0.1.4/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/runtime/__init__.py` & `caikit-0.1.4/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.1.4/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.1.4/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/__init__.py` & `caikit-0.1.4/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/config/config.yml` & `caikit-0.1.4/caikit/runtime/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/dump_services.py` & `caikit-0.1.4/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/grpc_server.py` & `caikit-0.1.4/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/interceptors/__init__.py` & `caikit-0.1.4/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.1.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/metrics/__init__.py` & `caikit-0.1.4/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.1.4/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/metrics/throughput.py` & `caikit-0.1.4/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/__init__.py` & `caikit-0.1.4/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/batcher.py` & `caikit-0.1.4/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/loaded_model.py` & `caikit-0.1.4/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/model_loader.py` & `caikit-0.1.4/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/model_manager.py` & `caikit-0.1.4/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/model_sizer.py` & `caikit-0.1.4/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/model_management/training_manager.py` & `caikit-0.1.4/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/__init__.py` & `caikit-0.1.4/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.1.4/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.1.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.1.4/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.1.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.1.4/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.1.4/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.1.4/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.1.4/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.1.4/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_factory.py` & `caikit-0.1.4/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.1.4/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.1.4/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/create_service.py` & `caikit-0.1.4/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.1.4/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/primitives.py` & `caikit-0.1.4/caikit/runtime/service_generation/primitives.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 This file contains our logic about what constitutes a "primitive" for RPC generation purposes
 """
 
 # Standard
-from typing import Dict, List, Type, Union
+from typing import Dict, List, Type, Union, get_args, get_origin
 import inspect
 import sys
 import typing
 
 # First Party
 import alog
 
@@ -78,14 +78,42 @@
                 primitives[arg] = arg_type
         else:
             log.debug("Skipping non-primitive argument [%s], type [%s]", arg, arg_type)
 
     return primitives
 
 
+def extract_data_model_type_from_union(arg_type: Type) -> Type:
+    """Helper function that determines the right data model type to use from a Union"""
+
+    # Decompose this type using typing to determine if it's a useful typing hint
+    typing_origin = get_origin(arg_type)
+    typing_args = get_args(arg_type)
+
+    # If this is a data model type, no need to do anything
+    if isinstance(arg_type, type) and issubclass(arg_type, DataBase):
+        return arg_type
+
+    # Handle Unions by looking for a data model object in the union
+    if typing_origin is Union:
+        dm_types = [
+            arg
+            for arg in typing_args
+            if inspect.isclass(arg) and issubclass(arg, DataBase)
+        ]
+        if dm_types:
+            log.debug2(
+                "Found data model types in Union: [%s], taking first one", dm_types
+            )
+            return extract_data_model_type_from_union(dm_types[0])
+
+    # anything else is an invalid output type
+    raise RuntimeError(f"Invalid arg type for output : {arg_type}")
+
+
 def is_primitive_method(
     method: CaikitCoreModuleMethodSignature, primitive_data_model_types: List[str]
 ) -> bool:
     """Determine if the arguments to the module's run function meet the criteria
     for being a "primitive" interface this means that all **non-optional** arguments
     types must be either (a) a primitive data model type for the given library or
     (b) a language-primitive type.
```

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/serializers.py` & `caikit-0.1.4/caikit/runtime/service_generation/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,23 +193,24 @@
             self._task_to_req_name(), parameters_dict, default_parameters
         )
 
         # Validate that the return_type of all modules in the grouping matches
         return_types = {method.return_type for method in method_signatures}
         assert len(return_types) == 1, f"Found multiple return types for task [{task}]"
         return_type = list(return_types)[0]
-        self.return_type = return_type
+        self.return_type = primitives.extract_data_model_type_from_union(return_type)
 
         # Create the rpc name based on the module type
         self.name = self._task_to_rpc_name()
 
     @property
     def module_list(self) -> List[Type[ModuleBase]]:
         """Returns the list of all caikit.core.modules that this RPC will be for. These should all
-        be of the same ai-problem, e.g. my_caikit_library.[blocks | workflows].classification"""
+        be of the same ai-problem, e.g. my_caikit_library.[blocks | workflows].classification
+        """
         return self._module_list
 
     @property
     def request(self) -> "_RequestMessage":
         return self._req
 
     def _task_to_req_name(self) -> str:
```

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.1.4/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.1.4/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/__init__.py` & `caikit-0.1.4/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.1.4/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.1.4/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.1.4/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.1.4/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.1.4/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/types/__init__.py` & `caikit-0.1.4/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/types/aborted_exception.py` & `caikit-0.1.4/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.1.4/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.1.4/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/utils/__init__.py` & `caikit-0.1.4/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/utils/config_parser.py` & `caikit-0.1.4/caikit/runtime/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/utils/import_util.py` & `caikit-0.1.4/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/utils/log_config.py` & `caikit-0.1.4/caikit/runtime/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/utils/servicer_util.py` & `caikit-0.1.4/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/work_management/__init__.py` & `caikit-0.1.4/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/work_management/abortable_action.py` & `caikit-0.1.4/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/work_management/call_aborter.py` & `caikit-0.1.4/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.1.4/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/examples/start_runtime_with_sample_lib.py` & `caikit-0.1.4/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/pyproject.toml` & `caikit-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.1.3"
+version = "0.1.4"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.1.3/scripts/fmt.sh` & `caikit-0.1.4/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/__init__.py` & `caikit-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/base.py` & `caikit-0.1.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/conftest.py` & `caikit-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.1.4/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.1.4/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/blocks/__init__.py` & `caikit-0.1.4/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/blocks/test_base.py` & `caikit-0.1.4/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.1.4/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/streams/test_converter.py` & `caikit-0.1.4/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.1.4/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.1.4/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/streams/test_resolver.py` & `caikit-0.1.4/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/streams/test_validator.py` & `caikit-0.1.4/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/test_base.py` & `caikit-0.1.4/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/test_dataobject.py` & `caikit-0.1.4/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/data_model/test_producer.py` & `caikit-0.1.4/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/helpers.py` & `caikit-0.1.4/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/module_backends/test_backend_types.py` & `caikit-0.1.4/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_config.py` & `caikit-0.1.4/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_imports.py` & `caikit-0.1.4/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_model_manager.py` & `caikit-0.1.4/tests/core/test_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         with open(zipfile, "rb") as f:
             cls.resource_archive_buffer = f.read()
 
     @pytest.fixture
     def global_load_path(self):
         """Set load_path prior to importing caikit.core."""
         # Set test load path
-        test_load_path = os.path.join(self.fixtures_dir, "studio_models")
+        test_load_path = os.path.join(self.fixtures_dir, "models")
 
         # Save the original load path so that it can be undone
         std_load_path = lib_config.load_path
 
         # Overwrite the load path with the test fixtures path
         lib_config.load_path = test_load_path
 
@@ -195,15 +195,15 @@
         model_path = os.path.join(self.fixtures_dir, "invalid.zip")
         with self.assertRaises(FileNotFoundError):
             caikit.core.load(model_path)
 
     @pytest.mark.usefixtures("global_load_path")
     def test_load_path(self):
         """Test that loading a model from a path defined in the load_path config variable works."""
-        model = caikit.core.load("studio_block")
+        model = caikit.core.load("foo")
         self.assertIsInstance(model, caikit.core.BlockBase)
 
     def test_import_block_registry(self):
         """Make sure that the BLOCK_REGISTRY can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
         # Local
         from caikit.core.model_manager import BLOCK_REGISTRY
```

### Comparing `caikit-0.1.3/tests/core/test_module.py` & `caikit-0.1.4/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_module_backend_config.py` & `caikit-0.1.4/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_module_metadata.py` & `caikit-0.1.4/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/test_no_write_permissions.py` & `caikit-0.1.4/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_compatibility.py` & `caikit-0.1.4/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_config_utils.py` & `caikit-0.1.4/tests/core/toolkit/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_error_handler.py` & `caikit-0.1.4/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_fileio.py` & `caikit-0.1.4/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.1.4/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_serializers.py` & `caikit-0.1.4/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.1.4/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/workflows/__init__.py` & `caikit-0.1.4/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/core/workflows/test_base.py` & `caikit-0.1.4/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/data_model_helpers.py` & `caikit-0.1.4/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.1.4/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_block.zip` & `caikit-0.1.4/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_block/config.yml` & `caikit-0.1.4/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.1.4/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_resource.zip` & `caikit-0.1.4/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_workflow.zip` & `caikit-0.1.4/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.1.4/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/fixtures.py` & `caikit-0.1.4/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/invalid.zip` & `caikit-0.1.4/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/linux.txt` & `caikit-0.1.4/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/primitive_party.proto` & `caikit-0.1.4/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.1.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.1.4/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.1.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 A sample block for sample things!
 """
+# Standard
+from typing import Union
+
 # Local
 from ...config import lib_config
 from ...data_model.sample import OtherOutputType, SampleInputType, SampleTrainingType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
@@ -12,15 +15,15 @@
 @caikit.core.block("33221100-0405-0607-0809-0a0b02dd0e0f", "OtherBlock", "0.0.1")
 class OtherBlock(caikit.core.BlockBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
-    def run(self, sample_input: SampleInputType) -> OtherOutputType:
+    def run(self, sample_input: SampleInputType) -> Union[OtherOutputType, str]:
         return OtherOutputType(f"goodbye: {sample_input.name} {self.batch_size} times")
 
     @classmethod
     def load(cls, model_path, **kwargs):
         loader = ModuleLoader(model_path)
         config = loader.config
         return cls(config["train"]["batch_size"], config["train"]["learning_rate"])
```

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.1.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.1.4/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.1.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/generated/__init__.py` & `caikit-0.1.4/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/metrics/__init__.py` & `caikit-0.1.4/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.1.4/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/metrics/test_throughput.py` & `caikit-0.1.4/tests/runtime/metrics/test_throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/__init__.py` & `caikit-0.1.4/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/test_batcher.py` & `caikit-0.1.4/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/test_model_loader.py` & `caikit-0.1.4/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/test_model_manager.py` & `caikit-0.1.4/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.1.4/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/model_management/test_training_manager.py` & `caikit-0.1.4/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.4/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.1.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.1.4/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/test_create_service.py` & `caikit-0.1.4/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.1.4/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.1.4/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/__init__.py` & `caikit-0.1.4/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.1.4/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.1.4/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.1.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.1.4/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.1.4/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/test_grpc_server.py` & `caikit-0.1.4/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/test_service_factory.py` & `caikit-0.1.4/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/utils/__init__.py` & `caikit-0.1.4/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/utils/test_configs.py` & `caikit-0.1.4/tests/runtime/utils/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/utils/test_import_util.py` & `caikit-0.1.4/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/utils/test_servicer_util.py` & `caikit-0.1.4/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/work_management/__init__.py` & `caikit-0.1.4/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.1.4/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.1.4/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.1.4/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/tox.ini` & `caikit-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.1.3/PKG-INFO` & `caikit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.1.3
+Version: 0.1.4
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.0.0
 Requires-Dist: alchemy-logging>=1.0.4
 Requires-Dist: anytree>=2.7.0,<3.0
```

