# Comparing `tmp/ml-starter-0.0.22.tar.gz` & `tmp/ml-starter-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.22.tar", last modified: Thu Apr 20 14:32:00 2023, max compression
+gzip compressed data, was "ml-starter-0.0.23.tar", last modified: Thu Apr 20 20:36:47 2023, max compression
```

## Comparing `ml-starter-0.0.22.tar` & `ml-starter-0.0.23.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.583649 ml-starter-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:31:44.000000 ml-starter-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 14:32:00.583649 ml-starter-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 14:31:44.000000 ml-starter-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.555648 ml-starter-0.0.22/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.559648 ml-starter-0.0.22/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.563649 ml-starter-0.0.22/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.567649 ml-starter-0.0.22/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.571648 ml-starter-0.0.22/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.575648 ml-starter-0.0.22/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.579649 ml-starter-0.0.22/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.579649 ml-starter-0.0.22/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 14:31:44.000000 ml-starter-0.0.22/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:32:00.583649 ml-starter-0.0.22/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 14:32:00.000000 ml-starter-0.0.22/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 14:31:44.000000 ml-starter-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 14:31:44.000000 ml-starter-0.0.22/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 14:31:44.000000 ml-starter-0.0.22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 14:32:00.583649 ml-starter-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 14:31:44.000000 ml-starter-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 20:36:36.000000 ml-starter-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 20:36:47.259864 ml-starter-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 20:36:36.000000 ml-starter-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.235862 ml-starter-0.0.23/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22561 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.239862 ml-starter-0.0.23/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.243863 ml-starter-0.0.23/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.247863 ml-starter-0.0.23/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.251863 ml-starter-0.0.23/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.255864 ml-starter-0.0.23/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 20:36:36.000000 ml-starter-0.0.23/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:36:47.259864 ml-starter-0.0.23/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 20:36:47.000000 ml-starter-0.0.23/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 20:36:36.000000 ml-starter-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 20:36:36.000000 ml-starter-0.0.23/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 20:36:36.000000 ml-starter-0.0.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 20:36:47.259864 ml-starter-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 20:36:36.000000 ml-starter-0.0.23/setup.py
```

### Comparing `ml-starter-0.0.22/PKG-INFO` & `ml-starter-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.22
+Version: 0.0.23
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.22/README.md` & `ml-starter-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/api.py` & `ml-starter-0.0.23/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/core/config.py` & `ml-starter-0.0.23/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/core/env.py` & `ml-starter-0.0.23/ml/core/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 """
 
 
 import os
 from pathlib import Path
 from typing import Set
 
-import torch.distributed as dist
-
 
 class _StrEnvVar:
     def __init__(self, key: str, *, default: str | None = None) -> None:
         self.key = key
         self.default = default
 
     def get(self) -> str:
@@ -147,14 +145,7 @@
 # Disables using accelerator on Mac.
 DisableMetal = _BoolEnvVar("DISABLE_METAL", default=False)
 is_metal_disabled = DisableMetal.get
 
 # Disables using the GPU.
 DisableGPU = _BoolEnvVar("DISABLE_GPU", default=False)
 is_gpu_disabled = DisableGPU.get
-
-
-def get_distributed_backend() -> dist.Backend:
-    # Used to change the distributed backend to something other than NCCL.
-    # For example, if you're on a system with some strange NCCL errors, you
-    # can try changing this environment variable to `gloo`.
-    return dist.Backend(os.environ.get("TORCH_DISTRIBUTED_BACKEND", "nccl"))
```

### Comparing `ml-starter-0.0.22/ml/core/registry.py` & `ml-starter-0.0.23/ml/core/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     @classmethod
     def build_entry(cls, raw_config: DictConfig) -> Entry | None:
         if cls.config_key() not in raw_config:
             return None
         reg_cfg = raw_config[cls.config_key()]
         reg_name = get_name(cls.config_key(), reg_cfg)
         reg_cls, _ = cls.lookup(reg_name)
-        with Timer(f"building {reg_name} from '{cls.REGISTRY_LOCATIONS[reg_name]}'"):
+        with Timer(f"building {reg_name}"):
             reg_obj = reg_cls(reg_cfg)
         if isinstance(reg_obj, BaseObjectWithPointers):
             reg_obj.set_raw_config(raw_config)
         return reg_obj
 
     @classmethod
     def build_entry_non_null(cls, raw_config: DictConfig) -> Entry:
@@ -363,15 +363,15 @@
         if cls.config_key() not in raw_config:
             return None
         reg_cfgs = cast(ListConfig, raw_config[cls.config_key()])
         reg_objs = []
         for reg_cfg in reg_cfgs:
             reg_name = get_name(cls.config_key(), reg_cfg)
             reg_cls, _ = cls.lookup(reg_name)
-            with Timer(f"building {reg_name} from '{cls.REGISTRY_LOCATIONS[reg_name]}'"):
+            with Timer(f"building {reg_name}"):
                 reg_obj = reg_cls(reg_cfg)
             reg_obj.set_raw_config(raw_config)
             reg_objs.append(reg_obj)
         return reg_objs
 
 
 class register_model(register_base["BaseModel", "BaseModelConfig"]):  # pylint: disable=invalid-name
```

### Comparing `ml-starter-0.0.22/ml/core/state.py` & `ml-starter-0.0.23/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/loggers/base.py` & `ml-starter-0.0.23/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/loggers/meter.py` & `ml-starter-0.0.23/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/loggers/multi.py` & `ml-starter-0.0.23/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/loggers/stdout.py` & `ml-starter-0.0.23/ml/loggers/stdout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import datetime
+import itertools
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable
 
 from torch import Tensor
 
 from ml.core.config import conf_field
 from ml.core.registry import register_logger
 from ml.core.state import Phase, State
 from ml.loggers.base import BaseLogger, BaseLoggerConfig
-from ml.utils.colors import colorize
+from ml.utils.colors import Color, colorize
 from ml.utils.datetime import format_timedelta
 from ml.utils.distributed import is_distributed
 
+LEVEL_COLORS: list[Color] = ["light-cyan", "cyan"]
+
 
 @dataclass
 class StdoutLoggerConfig(BaseLoggerConfig):
     precision: int = conf_field(4, help="Scalar precision to log")
 
 
 def format_number(value: int | float, precision: int) -> str:
@@ -71,19 +74,35 @@
         if not (phase_log_values := self.log_values.get(state.phase)):
             return
 
         # Gets elapsed time since last write.
         elapsed_time = datetime.datetime.now() - self.start_time
         elapsed_time_str = format_timedelta(elapsed_time)
 
-        def get_section_string(name: str, section: dict[str, Any]) -> str:
-            p1, p2 = colorize('"', "magenta"), colorize('"', "blue")
-            get_line = lambda kv: f"{p1}{kv[0]}{p2}: {as_str(kv[1](), self.config.precision)}"
-            inner_str = ", ".join(map(get_line, sorted(section.items())))
-            return '"' + colorize(name, "cyan") + '": {' + inner_str + "}"
+        def get_section_string(name: str, section: dict[str, Any], level: int = 0) -> str:
+            sub_sections: dict[str, dict[str, Any]] = {}
+            section_keys = list(section.keys())
+            for k in section_keys:
+                ks = k.split("/", maxsplit=1)
+                if len(ks) == 2:
+                    kk, rest = ks
+                    if kk not in sub_sections:
+                        sub_sections[kk] = {}
+                    sub_sections[kk][rest] = section[k]
+                    section.pop(k)
+
+            get_line = lambda kv: f'"{kv[0]}": {as_str(kv[1](), self.config.precision)}'
+            inner_str = ", ".join(
+                itertools.chain(
+                    map(get_line, sorted(section.items())),
+                    (get_section_string(k, v, level + 1) for k, v in sorted(sub_sections.items())),
+                )
+            )
+            level_color = LEVEL_COLORS[min(level, len(LEVEL_COLORS) - 1)]
+            return '"' + colorize(name, level_color) + '": {' + inner_str + "}"
 
         def colorize_phase(phase: Phase) -> str:
             match phase:
                 case "train":
                     return colorize(phase, "green", bold=True)
                 case "valid":
                     return colorize(phase, "yellow", bold=True)
```

### Comparing `ml-starter-0.0.22/ml/loggers/tensorboard.py` & `ml-starter-0.0.23/ml/loggers/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import atexit
 import datetime
 import functools
 import logging
 import os
 import re
 import subprocess
+import threading
 import time
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, Iterator, cast
 
 import torch
@@ -19,15 +20,14 @@
 from ml.core.config import conf_field
 from ml.core.registry import register_logger
 from ml.core.state import Phase, State
 from ml.loggers.base import BaseLogger, BaseLoggerConfig
 from ml.loggers.multi import TARGET_FPS, TARGET_SAMPLE_RATE
 from ml.utils.distributed import is_distributed, is_master
 from ml.utils.networking import get_unused_port
-from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 WRITE_PROC_TEXT_EVERY_N_SECONDS: int = 60 * 2
 
 
 def format_as_string(value: Any) -> str:
@@ -133,69 +133,72 @@
 
         self.line_str: str | None = None
         self.last_tensorboard_write_time = time.time()
 
     def initialize(self, log_directory: Path) -> None:
         super().initialize(log_directory)
 
+        # If on master, launch TensorBoard subprocess in a separate thread.
+        if is_master():
+            threading.Thread(target=self.worker_thread, daemon=False).start()
+
+    def worker_thread(self) -> None:
         if "TENSORBOARD_PORT" in os.environ:
             port, use_localhost = int(os.environ["TENSORBOARD_PORT"]), True
         else:
             port, use_localhost = get_unused_port(), False
 
         def make_localhost(s: str) -> str:
             if use_localhost:
                 s = re.sub(rf"://(.+?):{port}", f"://localhost:{port}", s)
             return s
 
-        if is_master():
-            if not self.config.start_in_subprocess or is_distributed():
-                tensorboard_command_strs = [
-                    "tensorboard serve \\",
-                    f"  --logdir {self.tensorboard_log_directory} \\",
-                    "  --bind_all \\",
-                    f"  --port {port} \\",
-                    "  --reload_interval 15",
-                ]
-                logger.info("Tensorboard command:\n%s", make_localhost(make_bold(tensorboard_command_strs)))
-
-            else:
-                command: list[str] = [
-                    "tensorboard",
-                    "serve",
-                    "--logdir",
-                    str(self.tensorboard_log_directory),
-                    "--bind_all",
-                    "--port",
-                    str(port),
-                    "--reload_interval",
-                    "15",
-                ]
-                logger.info("Tensorboard command: %s", " ".join(command))
-
-                with Timer("starting tensorboard", spinner=True):
-                    proc = subprocess.Popen(  # pylint: disable=consider-using-with
-                        command,
-                        stdout=subprocess.PIPE,
-                        stderr=subprocess.STDOUT,
-                    )
-
-                    # Gets the output line that shows the running address.
-                    assert proc is not None and proc.stdout is not None
-                    for line in proc.stdout:
-                        line_str = line.decode("utf-8")
-                        if line_str.startswith("TensorBoard"):
-                            self.line_str = make_localhost(line_str)
-                            break
+        if not self.config.start_in_subprocess or is_distributed():
+            tensorboard_command_strs = [
+                "tensorboard serve \\",
+                f"  --logdir {self.tensorboard_log_directory} \\",
+                "  --bind_all \\",
+                f"  --port {port} \\",
+                "  --reload_interval 15",
+            ]
+            logger.info("Tensorboard command:\n%s", make_localhost(make_bold(tensorboard_command_strs)))
+
+        else:
+            command: list[str] = [
+                "tensorboard",
+                "serve",
+                "--logdir",
+                str(self.tensorboard_log_directory),
+                "--bind_all",
+                "--port",
+                str(port),
+                "--reload_interval",
+                "15",
+            ]
+            logger.info("Tensorboard command: %s", " ".join(command))
+
+            proc = subprocess.Popen(  # pylint: disable=consider-using-with
+                command,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT,
+            )
+
+            # Gets the output line that shows the running address.
+            assert proc is not None and proc.stdout is not None
+            for line in proc.stdout:
+                line_str = line.decode("utf-8")
+                if line_str.startswith("TensorBoard"):
+                    self.line_str = make_localhost(line_str)
+                    break
 
-                if self.line_str is not None:
-                    logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str]))
+            if self.line_str is not None:
+                logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str]))
 
-                # Close the process when the program terminates.
-                atexit.register(proc.kill)
+            # Close the process when the program terminates.
+            atexit.register(proc.kill)
 
     @property
     def tensorboard_log_directory(self) -> Path:
         return self.log_directory / "tensorboard" / self.config.log_id
 
     @functools.cached_property
     def train_writer(self) -> SummaryWriter:
```

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/base.py` & `ml-starter-0.0.23/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.23/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.23/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/linear.py` & `ml-starter-0.0.23/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.23/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.23/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/models/activations.py` & `ml-starter-0.0.23/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/models/base.py` & `ml-starter-0.0.23/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/models/embeddings.py` & `ml-starter-0.0.23/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/models/init.py` & `ml-starter-0.0.23/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/models/norms.py` & `ml-starter-0.0.23/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/optimizers/adam.py` & `ml-starter-0.0.23/ml/optimizers/adam.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     weight_decay: float = conf_field(0.0, help="Weight decay regularization to use")
     amsgrad: bool = conf_field(False, help="Whether to use the AMSGrad variant of the algorithm")
 
 
 @register_optimizer("adam", AdamOptimizerConfig)
 class AdamOptimizer(BaseOptimizer[AdamOptimizerConfig]):
     def get(self, model: nn.Module) -> Adam:
+        b1, b2 = self.config.betas
+
         return Adam(
             model.parameters(),
             lr=self.config.lr,
-            betas=self.config.betas,
+            betas=(b1, b2),
             eps=self.config.eps,
             weight_decay=self.config.weight_decay,
             amsgrad=self.config.amsgrad,
             **self.common_kwargs,
         )
```

### Comparing `ml-starter-0.0.22/ml/optimizers/adamw.py` & `ml-starter-0.0.23/ml/optimizers/adamw.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,17 +78,18 @@
         }
 
 
 @register_optimizer("adamw", AdamWOptimizerConfig)
 class AdamWOptimizer(BaseOptimizer[AdamWOptimizerConfig]):
     def get(self, model: nn.Module) -> AdamW:
         params = model.parameters()
+        b1, b2 = self.config.betas
 
         return AdamW(
             params if self.config.weight_decay_bias else separate_weight_decayable_params(params),
             lr=self.config.lr,
-            betas=self.config.betas,
+            betas=(b1, b2),
             eps=self.config.eps,
             weight_decay=self.config.weight_decay,
             amsgrad=self.config.amsgrad,
             **self.common_kwargs,
         )
```

### Comparing `ml-starter-0.0.22/ml/optimizers/adan.py` & `ml-starter-0.0.23/ml/optimizers/adan.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
     eps: float = conf_field(1e-4, help="Epsilon term")
     weight_decay: float = conf_field(1e-5, help="Weight decay regularization to use")
 
 
 @register_optimizer("adan", AdanOptimizerConfig)
 class AdanOptimizer(BaseOptimizer[AdanOptimizerConfig]):
     def get(self, model: nn.Module) -> Adan:
+        b1, b2, b3 = self.config.betas
+
         return Adan(
             model.parameters(),
             lr=self.config.lr,
-            betas=self.config.betas,
+            betas=(b1, b2, b3),
             eps=self.config.eps,
             weight_decay=self.config.weight_decay,
             **self.common_kwargs,
         )
```

### Comparing `ml-starter-0.0.22/ml/optimizers/base.py` & `ml-starter-0.0.23/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/optimizers/sgd.py` & `ml-starter-0.0.23/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/optimizers/shampoo.py` & `ml-starter-0.0.23/ml/optimizers/shampoo.py`

 * *Files 7% similar despite different names*

```diff
@@ -150,20 +150,24 @@
 
         return loss
 
 
 @dataclass
 class ShampooOptimizerConfig(BaseOptimizerConfig):
     lr: float = conf_field(1e-3, help="Learning rate")
-    betas: tuple[float, float] = conf_field((0.9, 0.999), help="Beta coefficients")
-    eps: float = conf_field(1e-4, help="Epsilon term to add to the denominator for stability")
-    weight_decay: float = conf_field(1e-5, help="Weight decay regularization to use")
-    amsgrad: bool = conf_field(False, help="Whether to use the AMSGrad variant of the algorithm")
+    momentum: float = conf_field(0.0, help="Momentum")
+    weight_decay: float = conf_field(0.0, help="Weight decay")
+    epsilon: float = conf_field(1e-4, help="Epsilon")
+    update_freq: int = conf_field(1, help="Update frequency")
 
 
 @register_optimizer("shampoo", ShampooOptimizerConfig)
 class ShampooOptimizer(BaseOptimizer[ShampooOptimizerConfig]):
     def get(self, model: nn.Module) -> Shampoo:
         return Shampoo(
             model.parameters(),
             lr=self.config.lr,
+            momentum=self.config.momentum,
+            weight_decay=self.config.weight_decay,
+            epsilon=self.config.epsilon,
+            update_freq=self.config.update_freq,
         )
```

### Comparing `ml-starter-0.0.22/ml/scripts/cli.py` & `ml-starter-0.0.23/ml/scripts/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import logging
 import shlex
 import sys
 from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
-from omegaconf import DictConfig
-
-from ml.core.env import add_global_tag
-from ml.core.registry import Objects, add_project_dir
-from ml.scripts import compiler, mp_train, resolve, stage, train
-from ml.utils.cli import parse_cli
-from ml.utils.colors import colorize
 from ml.utils.distributed import get_rank_optional, get_world_size_optional
 from ml.utils.logging import configure_logging
-from ml.utils.random import set_random_seed
+from ml.utils.timer import Timer
+
+if TYPE_CHECKING:
+    from omegaconf import DictConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def cli_main(project_root: Path | str | None = None) -> None:
     configure_logging(rank=get_rank_optional(), world_size=get_world_size_optional())
     logger.info("Command: %s", shlex.join(sys.argv))
 
+    # Import here to avoid slow startup time.
+    with Timer("importing", spinner=True):
+        from ml.core.env import add_global_tag
+        from ml.core.registry import Objects, add_project_dir
+        from ml.scripts import compiler, mp_train, resolve, stage, train
+        from ml.utils.cli import parse_cli
+        from ml.utils.colors import colorize
+        from ml.utils.random import set_random_seed
+
     if project_root is not None:
         add_project_dir(Path(project_root).resolve())
 
     set_random_seed()
 
     without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
         "compile": compiler.compile_main,
```

### Comparing `ml-starter-0.0.22/ml/scripts/compiler.py` & `ml-starter-0.0.23/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/scripts/stage.py` & `ml-starter-0.0.23/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/scripts/train.py` & `ml-starter-0.0.23/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/base.py` & `ml-starter-0.0.23/ml/tasks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,20 @@
 
         # Logs epoch statistics (only if at least one epoch seen).
         if self.epoch_timer.steps > 0:
             logs["epoch"] = self.epoch_timer.steps
             logs["hours/epoch"] = self.epoch_timer.hours_per_step
 
         # Logs step statistics.
-        logs["steps"] = self.step_timer.steps
+        logs["steps/total"] = self.step_timer.steps
         logs["steps/second"] = self.step_timer.steps_per_second
         logs["steps/hour"] = self.step_timer.steps_per_hour
 
         # Logs sample statistics.
-        logs["samples"] = self.sample_timer.steps
+        logs["samples/total"] = self.sample_timer.steps
         logs["samples/second"] = self.sample_timer.steps_per_second
         logs["samples/hour"] = self.sample_timer.steps_per_hour
 
         logs["dt/iter"] = self.iter_timer.iter_seconds
         return logs
```

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.23/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.23/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/collate.py` & `ml-starter-0.0.23/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.23/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.23/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.23/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.23/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.23/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/utils.py` & `ml-starter-0.0.23/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.23/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/environments/base.py` & `ml-starter-0.0.23/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/environments/utils.py` & `ml-starter-0.0.23/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/environments/worker.py` & `ml-starter-0.0.23/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/losses/reduce.py` & `ml-starter-0.0.23/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/rl/base.py` & `ml-starter-0.0.23/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/rl/replay.py` & `ml-starter-0.0.23/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/tasks/sl/base.py` & `ml-starter-0.0.23/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/base.py` & `ml-starter-0.0.23/ml/trainers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,15 @@
             if isinstance(ckpt, (str, Path)):
                 try:
                     ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only))
                 except UnpicklingError:
                     if weights_only:
                         logger.warning("Failed to load checkpoint using `weights_only` flag, retrying without it")
                         ckpt = cast(dict, torch.load(cast(str | Path, ckpt), weights_only=False))
+                        raise  # TODO: Remove later
                     else:
                         raise
 
             task.on_after_load_checkpoint(ckpt)
             if "model" in ckpt:
                 model.load_state_dict(ckpt["model"])
             else:
@@ -375,44 +376,45 @@
     def save_checkpoint(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer | None = None,
         lr_sched: SchedulerAdapter | None = None,
-    ) -> None:
+    ) -> Path:
+        ckpt_path = self.get_ckpt_path(state)
         if is_master():
             with Timer("saving checkpoint", spinner=True):
-                ckpt_path = self.get_ckpt_path(state)
                 logger.info("Saving checkpoint to %s", ckpt_path)
                 last_ckpt_path = self.get_ckpt_path()
                 ckpt_path.parent.mkdir(exist_ok=True, parents=True)
                 state_dict: dict[str, Any] = {
                     "model": model.state_dict(),
                     "task": task.state_dict(),
                     "optim": None if optim is None else optim.state_dict(),
                     "lr_sched": None if lr_sched is None else lr_sched.state_dict(),
                     "state": asdict(state),
                 }
                 if self._raw_config is not None:
-                    state_dict["config"] = OmegaConf.to_container(self._raw_config)
+                    state_dict["config"] = OmegaConf.to_container(self._raw_config, enum_to_str=True)
                 self.update_state_dict(state_dict)
                 if last_ckpt_path.exists():
                     if self.checkpoint_config.only_save_most_recent:
                         base_ckpt = last_ckpt_path.resolve()
                         if base_ckpt.is_file():
                             base_ckpt.unlink()
                     last_ckpt_path.unlink()
                 torch.save(state_dict, ckpt_path)
                 try:
                     last_ckpt_path.symlink_to(ckpt_path)
                 except FileExistsError:
                     logger.exception("Exception while trying to update %s", ckpt_path)
                 self.add_lock_file("ckpt", exists_ok=True)
                 task.on_after_save_checkpoint(ckpt_path)
+        return ckpt_path
 
     @abstractmethod
     def launch(self) -> None:
         """Launches a multiprocess command."""
 
     @abstractmethod
     def train(self, model: ModelT, task: TaskT, optimizer: BaseOptimizer, lr_scheduler: BaseLRScheduler) -> None:
```

### Comparing `ml-starter-0.0.22/ml/trainers/ddp.py` & `ml-starter-0.0.23/ml/trainers/ddp.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,29 @@
 from abc import ABC
 from typing import Callable, Generic
 
 import torch.multiprocessing as mp
 from omegaconf import DictConfig
 from torch import nn
 
-from ml.core.env import get_distributed_backend
 from ml.core.registry import Objects
 from ml.scripts.train import train_main
 from ml.trainers.base import ModelT, MultiprocessConfig, TaskT
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfigT
 from ml.utils.distributed import (
     get_world_size,
-    init_process_group,
     set_init_method,
     set_master_addr,
     set_master_port,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
 from ml.utils.networking import get_unused_port
+from ml.utils.torch_distributed import get_distributed_backend, init_process_group
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def process_main(cfg: MultiprocessConfig, raw_config: DictConfig) -> None:
     set_master_addr(cfg.master_addr)
     set_master_port(cfg.master_port)
```

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.23/ml/trainers/mixins/cpu_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,17 +236,17 @@
     ) -> None:
         super().on_step_start(state, train_batch, task, model, optim, lr_sched)
 
         monitor = self._cpu_stats_monitor
         stats = monitor.get_if_set() if self.config.cpu_stats_only_log_once else monitor.get()
 
         if stats is not None:
+            self.logger.log_scalar("cpu/child_procs", stats.num_child_procs, namespace="trainer")
             self.logger.log_scalar("cpu/percent", stats.cpu_percent, namespace="trainer")
             self.logger.log_scalar("cpu/child_percent", stats.child_cpu_percent, namespace="trainer")
             self.logger.log_scalar("mem/percent", stats.mem_percent, namespace="trainer")
-            self.logger.log_scalar("mem/rss", stats.mem_rss, namespace="trainer")
-            self.logger.log_scalar("mem/vms", stats.mem_vms, namespace="trainer")
             self.logger.log_scalar("mem/shared", stats.mem_shared, namespace="trainer")
+            self.logger.log_scalar("mem/child_percent", stats.child_mem_percent, namespace="trainer")
+            self.logger.log_scalar("mem/rss/cur", stats.mem_rss, namespace="trainer")
             self.logger.log_scalar("mem/rss/total", stats.mem_rss_total, namespace="trainer")
+            self.logger.log_scalar("mem/vms/cur", stats.mem_vms, namespace="trainer")
             self.logger.log_scalar("mem/vms/total", stats.mem_vms_total, namespace="trainer")
-            self.logger.log_scalar("mem/child_percent", stats.child_mem_percent, namespace="trainer")
-            self.logger.log_scalar("child_procs", stats.num_child_procs, namespace="trainer")
```

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.23/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.23/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.23/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.23/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.23/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.23/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.23/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/rl.py` & `ml-starter-0.0.23/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/sl.py` & `ml-starter-0.0.23/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/trainers/slurm.py` & `ml-starter-0.0.23/ml/trainers/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,35 +27,35 @@
 from typing import Callable, Generic, TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
 from torch import nn
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
-from ml.core.env import get_distributed_backend, get_stage_dir
+from ml.core.env import get_stage_dir
 from ml.core.registry import Objects, project_dirs
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.scripts.train import train_main
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
     get_world_size,
-    init_process_group,
     is_master,
     set_init_method,
     set_master_addr,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
 from ml.utils.staging import stage_environment
+from ml.utils.torch_distributed import get_distributed_backend, init_process_group
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 SBATCH_TEMPLATE: str = """
 #!/bin/bash
 #SBATCH --job-name={job_name}
 #SBATCH --partition={partition}
@@ -229,19 +229,19 @@
             tasks_per_node=tasks_per_node,
             cpus_per_task=cpus_per_task,
             gres=gres,
             gpu_bind=gpu_bind,
             output_path=slurm_log_dir / "slurm_out.txt",
             error_path=slurm_log_dir / "slurm_err.%j.txt",
             extra_sbatch_lines="\n".join(f"#SBATCH {line}" for line in sbatch_lines),
+            stage_dir=stage_dir,
             pythonpath=python_path,
             master_port=self.config.master_port,
             config_path=self.exp_dir / "config.yaml",
             lock_file_path=self.exp_dir / ".lock_running",
-            stage_dir=stage_dir,
         )
 
         with open(sbatch_path, "w", encoding="utf-8") as f:
             f.write(sbatch_file)
         logger.info("Wrote sbatch file to %s", sbatch_path)
 
         # Call `sbatch` on the given file.
```

### Comparing `ml-starter-0.0.22/ml/trainers/vanilla.py` & `ml-starter-0.0.23/ml/trainers/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,13 +281,12 @@
         lr_sched: SchedulerAdapter,
     ) -> State:
         if (ckpt_path := self.get_ckpt_path()).exists():
             return self.load_checkpoint(ckpt_path, task, model, optim, lr_sched)
         return State.init_state()
 
     def _log_prefetcher_stats(self, pf: Prefetcher) -> None:
-        self.logger.log_scalar("num_queued_samples", pf.num_queued_samples, namespace="trainer")
         self.logger.log_scalar("dt/get_batch", pf.get_batch_time, namespace="timers")
         self.logger.log_scalar("dt/to_device", pf.to_device_time, namespace="timers")
 
     def launch(self) -> None:
         raise NotImplementedError(f"{self.__class__.__name__} doesn't support multiprocess training")
```

### Comparing `ml-starter-0.0.22/ml/utils/argparse.py` & `ml-starter-0.0.23/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/atomic.py` & `ml-starter-0.0.23/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/augmentation.py` & `ml-starter-0.0.23/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/caching.py` & `ml-starter-0.0.23/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/call_train.py` & `ml-starter-0.0.23/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/cli.py` & `ml-starter-0.0.23/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/colors.py` & `ml-starter-0.0.23/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/compiler.py` & `ml-starter-0.0.23/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/data.py` & `ml-starter-0.0.23/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/datetime.py` & `ml-starter-0.0.23/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/device/auto.py` & `ml-starter-0.0.23/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/device/base.py` & `ml-starter-0.0.23/ml/utils/device/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 import contextlib
 import functools
+import threading
 from abc import ABC, abstractmethod
 from dataclasses import is_dataclass
 from typing import Any, Callable, ContextManager, Iterable, Iterator, Mapping, Sequence
 
 import numpy as np
 import torch
 from torch import Tensor, nn
-from torch.utils.data.dataloader import (
-    DataLoader,
-    _BaseDataLoaderIter,
-    _MultiProcessingDataLoaderIter,
-)
+from torch.utils.data.dataloader import DataLoader, _BaseDataLoaderIter
 
 from ml.core.common_types import Batch
 from ml.utils.timer import Timer
 
 
 def allow_nonblocking(device_a: torch.device, device_b: torch.device) -> bool:
     return device_a.type in ("cpu", "cuda") and device_b.type in ("cpu", "cuda")
 
 
-def get_tasks_outstanding(dataloader_iter: _BaseDataLoaderIter) -> int:
-    if isinstance(dataloader_iter, _MultiProcessingDataLoaderIter):
-        try:
-            return dataloader_iter._worker_result_queue.qsize()
-        except NotImplementedError:
-            return -2
-    return -1
-
-
 def recursive_apply(item: Any, func: Callable[[Tensor], Tensor]) -> Any:
     """Applies a function recursively to tensors in an item.
 
     Args:
         item: The item to apply the function to
         func: The function to apply (for the tensor)
 
@@ -66,29 +54,44 @@
         raise_stop_iter: bool = False,
     ) -> None:
         super().__init__()
 
         self.to_device_func = to_device_func
         self.dataloader = dataloader
         self.raise_stop_iter = raise_stop_iter
-        self.dataloader_iter = iter(self.dataloader)
         self.next_sample = None
         self.get_batch_time = 0.0
         self.to_device_time = 0.0
-        self.num_queued_samples = -1
+
+        # Start the dataloader in a separate thread.
+        self._dataloader_iter_ready = threading.Event()
+        self._dataloader_iter: _BaseDataLoaderIter | None = None
+        threading.Thread(target=self.start_dataloader).start()
+
+    def start_dataloader(self) -> None:
+        self._dataloader_iter = iter(self.dataloader)
+        self._dataloader_iter_ready.set()
+        self.prefetch()
+
+    @property
+    def dataloader_iter(self) -> _BaseDataLoaderIter:
+        if self._dataloader_iter is None:
+            with Timer("starting dataloader", spinner=True):
+                self._dataloader_iter_ready.wait()
+                assert self._dataloader_iter is not None
+        return self._dataloader_iter
 
     def prefetch(self) -> None:
         try:
             with Timer("getting sample from dataloader") as timer:
                 next_sample = next(self.dataloader_iter)
             self.get_batch_time = timer.elapsed_time
             with Timer("moving sample to device") as timer:
                 self.next_sample = self.to_device_func(next_sample)
             self.to_device_time = timer.elapsed_time
-            self.num_queued_samples = get_tasks_outstanding(self.dataloader_iter)
         except StopIteration:
             self.next_sample = None
 
     def recursive_chunk(self, item: Any, chunks: int) -> list[Any]:
         """Applies a function recursively to tensors in an item.
 
         Args:
@@ -119,27 +122,30 @@
         return item
 
     @classmethod
     def recursive_apply(cls, item: Any, func: Callable[[Tensor], Tensor]) -> Any:
         return recursive_apply(item, func)
 
     def __iter__(self) -> Iterator[Batch]:
-        self.prefetch()
+        # Yields one sample quickly.
+        next_sample = next(self.dataloader_iter)
+        yield self.to_device_func(next_sample)
 
         try:
+            self.prefetch()
             while True:
                 if self.next_sample is None:
                     raise StopIteration
                 sample = self.next_sample
                 self.prefetch()
                 yield sample
 
         except StopIteration:
             # Resets the dataloader if the iteration has completed.
-            self.dataloader_iter = iter(self.dataloader)
+            self._dataloader_iter = iter(self.dataloader)
             if self.raise_stop_iter:
                 raise
 
 
 class InfinitePrefetcher(Iterable[Batch]):
     def __init__(self, prefetcher: Prefetcher[Batch]) -> None:
         self.prefetcher = prefetcher
```

### Comparing `ml-starter-0.0.22/ml/utils/device/cpu.py` & `ml-starter-0.0.23/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/device/gpu.py` & `ml-starter-0.0.23/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/device/metal.py` & `ml-starter-0.0.23/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/io.py` & `ml-starter-0.0.23/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/large_models.py` & `ml-starter-0.0.23/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/logging.py` & `ml-starter-0.0.23/ml/utils/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 import math
 import sys
-from typing import Any
 
 import tqdm
-from torch import Tensor
 
 from ml.core.env import is_debugging
 from ml.utils.colors import Color, colorize, get_colorize_parts
 
 # Logging level to show on all ranks.
 INFOALL: int = logging.INFO + 1
 
@@ -123,13 +121,7 @@
     handler.addFilter(RankFilter(rank=rank))
     root_logger.addHandler(handler)
     root_logger.setLevel(logging.DEBUG if is_debugging() else logging.INFO)
 
     # Avoid junk logs from other libraries.
     logging.getLogger("matplotlib").setLevel(logging.WARNING)
     logging.getLogger("PIL").setLevel(logging.WARNING)
-
-
-def get_log_item(item: Any) -> Any:
-    if isinstance(item, Tensor):
-        return item.detach().cpu().item()
-    return item
```

### Comparing `ml-starter-0.0.22/ml/utils/meter.py` & `ml-starter-0.0.23/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/staging.py` & `ml-starter-0.0.23/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml/utils/timer.py` & `ml-starter-0.0.23/ml/utils/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 class Timer:
     """Defines a simple timer for logging an event."""
 
     def __init__(
         self,
         description: str,
-        min_seconds_to_print: float = 1.0,
+        min_seconds_to_print: float = 5.0,
         logger: logging.Logger | None = None,
         spinner: bool = False,
     ) -> None:
         self.description = description
         self.min_seconds_to_print = min_seconds_to_print
         self._start_time: float | None = None
         self._elapsed_time: float | None = None
```

### Comparing `ml-starter-0.0.22/ml/utils/video.py` & `ml-starter-0.0.23/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.23/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.22
+Version: 0.0.23
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.22/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.23/ml_starter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/random.py
 ml/utils/staging.py
 ml/utils/timer.py
+ml/utils/torch_distributed.py
 ml/utils/video.py
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
 ml/utils/device/cpu.py
 ml/utils/device/gpu.py
 ml/utils/device/metal.py
```

### Comparing `ml-starter-0.0.22/pyproject.toml` & `ml-starter-0.0.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.22/setup.py` & `ml-starter-0.0.23/setup.py`

 * *Files identical despite different names*

