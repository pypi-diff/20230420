# Comparing `tmp/ml-starter-0.0.21.tar.gz` & `tmp/ml-starter-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.21.tar", last modified: Thu Apr 20 01:32:38 2023, max compression
+gzip compressed data, was "ml-starter-0.0.22.tar", last modified: Thu Apr 20 14:32:00 2023, max compression
```

## Comparing `ml-starter-0.0.21.tar` & `ml-starter-0.0.22.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.231950 ml-starter-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 01:32:25.000000 ml-starter-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 01:32:38.231950 ml-starter-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 01:32:25.000000 ml-starter-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.215950 ml-starter-0.0.21/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.215950 ml-starter-0.0.21/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.219950 ml-starter-0.0.21/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.219950 ml-starter-0.0.21/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.219950 ml-starter-0.0.21/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.219950 ml-starter-0.0.21/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.219950 ml-starter-0.0.21/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.223950 ml-starter-0.0.21/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.227950 ml-starter-0.0.21/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.227950 ml-starter-0.0.21/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.231950 ml-starter-0.0.21/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.231950 ml-starter-0.0.21/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 01:32:25.000000 ml-starter-0.0.21/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:32:38.231950 ml-starter-0.0.21/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 01:32:38.000000 ml-starter-0.0.21/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 01:32:25.000000 ml-starter-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 01:32:25.000000 ml-starter-0.0.21/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 01:32:25.000000 ml-starter-0.0.21/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 01:32:38.231950 ml-starter-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 01:32:25.000000 ml-starter-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.583649 ml-starter-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:31:44.000000 ml-starter-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 14:32:00.583649 ml-starter-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 14:31:44.000000 ml-starter-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.555648 ml-starter-0.0.22/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.575648 ml-starter-0.0.22/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.579649 ml-starter-0.0.22/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.579649 ml-starter-0.0.22/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.583649 ml-starter-0.0.22/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 14:31:44.000000 ml-starter-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 14:31:44.000000 ml-starter-0.0.22/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 14:31:44.000000 ml-starter-0.0.22/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 14:32:00.583649 ml-starter-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 14:31:44.000000 ml-starter-0.0.22/setup.py
```

### Comparing `ml-starter-0.0.21/PKG-INFO` & `ml-starter-0.0.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.21
+Version: 0.0.22
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.21/README.md` & `ml-starter-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/api.py` & `ml-starter-0.0.22/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/core/config.py` & `ml-starter-0.0.22/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/core/env.py` & `ml-starter-0.0.22/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/core/registry.py` & `ml-starter-0.0.22/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/core/state.py` & `ml-starter-0.0.22/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/loggers/base.py` & `ml-starter-0.0.22/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/loggers/meter.py` & `ml-starter-0.0.22/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/loggers/multi.py` & `ml-starter-0.0.22/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/loggers/stdout.py` & `ml-starter-0.0.22/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/loggers/tensorboard.py` & `ml-starter-0.0.22/ml/loggers/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ml.core.config import conf_field
 from ml.core.registry import register_logger
 from ml.core.state import Phase, State
 from ml.loggers.base import BaseLogger, BaseLoggerConfig
 from ml.loggers.multi import TARGET_FPS, TARGET_SAMPLE_RATE
 from ml.utils.distributed import is_distributed, is_master
 from ml.utils.networking import get_unused_port
+from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 WRITE_PROC_TEXT_EVERY_N_SECONDS: int = 60 * 2
 
 
 def format_as_string(value: Any) -> str:
@@ -167,28 +168,31 @@
                     "--port",
                     str(port),
                     "--reload_interval",
                     "15",
                 ]
                 logger.info("Tensorboard command: %s", " ".join(command))
 
-                proc = subprocess.Popen(  # pylint: disable=consider-using-with
-                    command,
-                    stdout=subprocess.PIPE,
-                    stderr=subprocess.STDOUT,
-                )
-
-                # Gets the output line that shows the running address.
-                assert proc is not None and proc.stdout is not None
-                for line in proc.stdout:
-                    line_str = line.decode("utf-8")
-                    if line_str.startswith("TensorBoard"):
-                        self.line_str = make_localhost(line_str)
-                        logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str]))
-                        break
+                with Timer("starting tensorboard", spinner=True):
+                    proc = subprocess.Popen(  # pylint: disable=consider-using-with
+                        command,
+                        stdout=subprocess.PIPE,
+                        stderr=subprocess.STDOUT,
+                    )
+
+                    # Gets the output line that shows the running address.
+                    assert proc is not None and proc.stdout is not None
+                    for line in proc.stdout:
+                        line_str = line.decode("utf-8")
+                        if line_str.startswith("TensorBoard"):
+                            self.line_str = make_localhost(line_str)
+                            break
+
+                if self.line_str is not None:
+                    logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str]))
 
                 # Close the process when the program terminates.
                 atexit.register(proc.kill)
 
     @property
     def tensorboard_log_directory(self) -> Path:
         return self.log_directory / "tensorboard" / self.config.log_id
```

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/base.py` & `ml-starter-0.0.22/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.22/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.22/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/linear.py` & `ml-starter-0.0.22/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.22/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.22/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/models/activations.py` & `ml-starter-0.0.22/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/models/base.py` & `ml-starter-0.0.22/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/models/embeddings.py` & `ml-starter-0.0.22/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/models/init.py` & `ml-starter-0.0.22/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/models/norms.py` & `ml-starter-0.0.22/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/adam.py` & `ml-starter-0.0.22/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/adamw.py` & `ml-starter-0.0.22/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/adan.py` & `ml-starter-0.0.22/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/base.py` & `ml-starter-0.0.22/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/sgd.py` & `ml-starter-0.0.22/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/optimizers/shampoo.py` & `ml-starter-0.0.22/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/scripts/cli.py` & `ml-starter-0.0.22/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/scripts/compiler.py` & `ml-starter-0.0.22/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/scripts/stage.py` & `ml-starter-0.0.22/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/scripts/train.py` & `ml-starter-0.0.22/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/base.py` & `ml-starter-0.0.22/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.22/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.22/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/collate.py` & `ml-starter-0.0.22/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.22/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.22/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.22/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.22/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.22/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/utils.py` & `ml-starter-0.0.22/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.22/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/environments/base.py` & `ml-starter-0.0.22/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/environments/utils.py` & `ml-starter-0.0.22/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/environments/worker.py` & `ml-starter-0.0.22/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/losses/reduce.py` & `ml-starter-0.0.22/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/rl/base.py` & `ml-starter-0.0.22/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/rl/replay.py` & `ml-starter-0.0.22/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/tasks/sl/base.py` & `ml-starter-0.0.22/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/base.py` & `ml-starter-0.0.22/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/ddp.py` & `ml-starter-0.0.22/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.22/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.22/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.22/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.22/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.22/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.22/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.22/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.22/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/rl.py` & `ml-starter-0.0.22/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/sl.py` & `ml-starter-0.0.22/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/slurm.py` & `ml-starter-0.0.22/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/trainers/vanilla.py` & `ml-starter-0.0.22/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/argparse.py` & `ml-starter-0.0.22/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/atomic.py` & `ml-starter-0.0.22/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/augmentation.py` & `ml-starter-0.0.22/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/caching.py` & `ml-starter-0.0.22/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/call_train.py` & `ml-starter-0.0.22/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/cli.py` & `ml-starter-0.0.22/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/colors.py` & `ml-starter-0.0.22/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/compiler.py` & `ml-starter-0.0.22/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/data.py` & `ml-starter-0.0.22/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/datetime.py` & `ml-starter-0.0.22/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/device/auto.py` & `ml-starter-0.0.22/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/device/base.py` & `ml-starter-0.0.22/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/device/cpu.py` & `ml-starter-0.0.22/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/device/gpu.py` & `ml-starter-0.0.22/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/device/metal.py` & `ml-starter-0.0.22/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/distributed.py` & `ml-starter-0.0.22/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/io.py` & `ml-starter-0.0.22/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/large_models.py` & `ml-starter-0.0.22/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/logging.py` & `ml-starter-0.0.22/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/meter.py` & `ml-starter-0.0.22/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/staging.py` & `ml-starter-0.0.22/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/timer.py` & `ml-starter-0.0.22/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml/utils/video.py` & `ml-starter-0.0.22/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.22/ml_starter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.21
+Version: 0.0.22
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.21/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.22/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/pyproject.toml` & `ml-starter-0.0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.21/setup.py` & `ml-starter-0.0.22/setup.py`

 * *Files identical despite different names*

