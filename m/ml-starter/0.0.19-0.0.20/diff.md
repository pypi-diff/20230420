# Comparing `tmp/ml-starter-0.0.19.tar.gz` & `tmp/ml-starter-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.19.tar", last modified: Mon Apr 17 18:43:27 2023, max compression
+gzip compressed data, was "ml-starter-0.0.20.tar", last modified: Thu Apr 20 01:13:51 2023, max compression
```

## Comparing `ml-starter-0.0.19.tar` & `ml-starter-0.0.20.tar`

### file list

```diff
@@ -1,150 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.382779 ml-starter-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 18:43:12.000000 ml-starter-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-17 18:43:27.382779 ml-starter-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-17 18:43:12.000000 ml-starter-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.354779 ml-starter-0.0.19/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.358779 ml-starter-0.0.19/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.358779 ml-starter-0.0.19/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.358779 ml-starter-0.0.19/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.358779 ml-starter-0.0.19/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.362779 ml-starter-0.0.19/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.362779 ml-starter-0.0.19/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.362779 ml-starter-0.0.19/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.366779 ml-starter-0.0.19/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.366779 ml-starter-0.0.19/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.366779 ml-starter-0.0.19/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.370779 ml-starter-0.0.19/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.370779 ml-starter-0.0.19/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.370779 ml-starter-0.0.19/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.370779 ml-starter-0.0.19/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.374779 ml-starter-0.0.19/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.378779 ml-starter-0.0.19/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.378779 ml-starter-0.0.19/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-17 18:43:12.000000 ml-starter-0.0.19/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:27.382779 ml-starter-0.0.19/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 18:43:27.000000 ml-starter-0.0.19/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-17 18:43:12.000000 ml-starter-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 18:43:12.000000 ml-starter-0.0.19/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 18:43:12.000000 ml-starter-0.0.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 18:43:27.382779 ml-starter-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 18:43:12.000000 ml-starter-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.652442 ml-starter-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 01:13:37.000000 ml-starter-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 01:13:51.652442 ml-starter-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 01:13:37.000000 ml-starter-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.624442 ml-starter-0.0.20/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.628442 ml-starter-0.0.20/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.628442 ml-starter-0.0.20/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.628442 ml-starter-0.0.20/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.632442 ml-starter-0.0.20/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.632442 ml-starter-0.0.20/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.632442 ml-starter-0.0.20/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.636442 ml-starter-0.0.20/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.636442 ml-starter-0.0.20/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.636442 ml-starter-0.0.20/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.640442 ml-starter-0.0.20/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.640442 ml-starter-0.0.20/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.640442 ml-starter-0.0.20/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.640442 ml-starter-0.0.20/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.640442 ml-starter-0.0.20/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.644442 ml-starter-0.0.20/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.648442 ml-starter-0.0.20/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.652442 ml-starter-0.0.20/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-20 01:13:37.000000 ml-starter-0.0.20/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:13:51.652442 ml-starter-0.0.20/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 01:13:51.000000 ml-starter-0.0.20/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 01:13:37.000000 ml-starter-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 01:13:37.000000 ml-starter-0.0.20/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 01:13:37.000000 ml-starter-0.0.20/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 01:13:51.652442 ml-starter-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 01:13:37.000000 ml-starter-0.0.20/setup.py
```

### Comparing `ml-starter-0.0.19/PKG-INFO` & `ml-starter-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.19
+Version: 0.0.20
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.19/README.md` & `ml-starter-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/api.py` & `ml-starter-0.0.20/ml/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 There wasn't an explicit dictating which functions to include here, it was just
 whichever functions seemed like they would be generally useful to have on
 hand quickly.
 """
 
 __all__ = [
     "ActivationType",
+    "add_project_dir",
     "as_cpu_tensor",
     "as_numpy_array",
     "assert_no_nans",
     "AsyncEnvironmentWorker",
     "AsyncIterableDataset",
     "AsyncWorkerPool",
     "atomic_save",
@@ -43,14 +44,15 @@
     "collate_non_null",
     "collate",
     "CollateMode",
     "colorize",
     "conf_field",
     "configure_logging",
     "DDPTrainer",
+    "DictIndex",
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
     "get_args",
     "get_cache_dir",
     "get_data_dir",
@@ -89,14 +91,16 @@
     "MultiIterDataset",
     "NormType",
     "open_atomic",
     "Output",
     "pad_all",
     "pad_sequence",
     "Phase",
+    "project_dir_paths",
+    "read_video",
     "reduce",
     "register_logger",
     "register_lr_scheduler",
     "register_model",
     "register_optimizer",
     "register_task",
     "register_trainer",
@@ -129,32 +133,33 @@
     "SyncWorkerPool",
     "test_dataset",
     "timeout",
     "Timer",
     "transforms",
     "VanillaTrainer",
     "VanillaTrainerConfig",
-    "VIDEO_READERS",
-    "VIDEO_WRITERS",
     "VideoFileDataset",
     "WorkerPool",
+    "write_video",
 ]
 
 from ml.core.common_types import Batch, Loss, Output
 from ml.core.config import conf_field
 from ml.core.env import (
     get_cache_dir,
     get_data_dir,
     get_eval_run_dir,
     get_exp_name,
     get_model_dir,
     get_run_dir,
     is_debugging,
 )
 from ml.core.registry import (
+    add_project_dir,
+    project_dir_paths,
     register_logger,
     register_lr_scheduler,
     register_model,
     register_optimizer,
     register_task,
     register_trainer,
 )
@@ -218,15 +223,15 @@
     SupervisedLearningVanillaTrainer,
 )
 from ml.trainers.slurm import SlurmTrainer, SlurmTrainerConfig, set_slurm_master_addr, set_slurm_rank_and_world_size
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
-from ml.utils.caching import cached_object
+from ml.utils.caching import DictIndex, cached_object
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
 from ml.utils.data import get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.distributed import (
@@ -243,8 +248,8 @@
 from ml.utils.io import instantiate_config, load_model_and_task
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
 from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
-from ml.utils.video import READERS as VIDEO_READERS, WRITERS as VIDEO_WRITERS
+from ml.utils.video import read_video, write_video
```

### Comparing `ml-starter-0.0.19/ml/core/config.py` & `ml-starter-0.0.20/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/core/env.py` & `ml-starter-0.0.20/ml/core/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -148,18 +148,13 @@
 DisableMetal = _BoolEnvVar("DISABLE_METAL", default=False)
 is_metal_disabled = DisableMetal.get
 
 # Disables using the GPU.
 DisableGPU = _BoolEnvVar("DISABLE_GPU", default=False)
 is_gpu_disabled = DisableGPU.get
 
-# Sets the root project directory.
-ProjectRoot = _PathEnvVar("PROJECT_ROOT")
-get_project_root = ProjectRoot.maybe_get
-set_project_root = ProjectRoot.set
-
 
 def get_distributed_backend() -> dist.Backend:
     # Used to change the distributed backend to something other than NCCL.
     # For example, if you're on a system with some strange NCCL errors, you
     # can try changing this environment variable to `gloo`.
     return dist.Backend(os.environ.get("TORCH_DISTRIBUTED_BACKEND", "nccl"))
```

### Comparing `ml-starter-0.0.19/ml/core/registry.py` & `ml-starter-0.0.20/ml/core/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generic, Iterator, TypeVar, cast
 
 from omegaconf import DictConfig, ListConfig, OmegaConf
 from omegaconf.basecontainer import BaseContainer
 
 from ml.core.config import BaseConfig, BaseObject, BaseObjectWithPointers
-from ml.core.env import get_project_root
 from ml.utils.colors import colorize
-from ml.utils.paths import get_relative_path
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
     from ml.loggers.base import BaseLogger, BaseLoggerConfig
     from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
     from ml.models.base import BaseModel, BaseModelConfig
     from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
@@ -40,21 +38,45 @@
 ROOT_DIR: Path = Path(__file__).parent.parent.resolve()
 
 # Maximum number of days to keep a staging directory around. This should
 # correspond to the maximum number of days that an experiment could run.
 MAX_STAGING_DAYS = 31
 
 
-@functools.lru_cache
-def base_dirs() -> list[Path]:
-    base_dirs = [ROOT_DIR]
-    project_root_dir = get_project_root()
-    if project_root_dir is not None:
-        base_dirs.append(project_root_dir)
-    return base_dirs
+class _ProjectDirs:
+    def __init__(self) -> None:
+        self.__dir_set: set[Path] = {ROOT_DIR}
+        self.__dir_list: list[Path] = [ROOT_DIR]
+
+    @property
+    def paths(self) -> list[Path]:
+        return self.__dir_list
+
+    def add(self, path: Path) -> None:
+        if path in self.__dir_set:
+            return
+        path = path.resolve()
+        self.__dir_set.add(path)
+        self.__dir_list.append(path)
+
+    def relative_path(self, p: Path, parent: bool = False) -> Path:
+        for d in self.__dir_list:
+            try:
+                return p.relative_to(d.parent if parent else d)
+            except ValueError:
+                pass
+        raise ValueError(f"Path {p} is not relative to any of {self.__dir_list}")
+
+
+# Project directories singleton.
+project_dirs = _ProjectDirs()
+
+# Some aliases for the project directory accessors.
+add_project_dir = project_dirs.add
+project_dir_paths = project_dirs.paths
 
 
 def get_name(key: str, config: BaseContainer) -> str:
     if not isinstance(config, DictConfig):
         raise ValueError(f"Expected {key} config to be a dictionary, got {type(config)}")
     if NAME_KEY not in config:
         raise ValueError(f"Malformed {key} config; missing expected key {NAME_KEY}")
@@ -88,15 +110,15 @@
     @classmethod
     @abstractmethod
     def config_key(cls) -> str:
         """Returns the key for the current item from the config."""
 
     @classmethod
     def registry_path(cls) -> Path:
-        return (get_project_root() or Path(__file__).parent.resolve()) / ".cache" / f"{cls.config_key()}.json"
+        return project_dirs.paths[-1] / ".cache" / f"{cls.config_key()}.json"
 
     @classmethod
     @functools.lru_cache(None)
     def load_registry_locations(cls) -> None:
         registry_path = cls.registry_path()
         if not registry_path.exists():
             return
@@ -121,15 +143,15 @@
             json.dump(registry_locations, f, indent=2)
 
     @classmethod
     @functools.lru_cache(None)
     def manual_import(cls, path: Path) -> None:
         with Timer(f"importing '{path}'"):
             try:
-                rel_path = get_relative_path(path, base_dirs(), True)
+                rel_path = project_dirs.relative_path(path, parent=True)
                 module_name = ".".join(list(rel_path.parts[:-1]) + [rel_path.stem])
                 if module_name not in sys.modules:
                     spec = importlib.util.spec_from_file_location(module_name, str(path))
                     assert spec is not None
                     module = importlib.util.module_from_spec(spec)
                     sys.modules[module_name] = module
                     loader = spec.loader
@@ -178,15 +200,15 @@
                         subfiles.append(subfile)
                         yield subfile
                     elif subpath.is_dir():
                         yield from iter_directory(subpath)
 
         # Next sweep over the search directory and check for prefix matches.
         search_dir = cls.search_directory()
-        search_dirs = [base_dir / search_dir for base_dir in base_dirs()]
+        search_dirs = [base_dir / search_dir for base_dir in project_dirs.paths]
         search_dirs = [search_dir for search_dir in search_dirs if search_dir.is_dir()]
         for path in iter_directory(*search_dirs):
             if path.stem.lower().startswith(lower_name) or lower_name.startswith(path.stem.lower()):
                 cls.manual_import(path)
                 if name in cls.REGISTRY:
                     return
```

### Comparing `ml-starter-0.0.19/ml/core/state.py` & `ml-starter-0.0.20/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/loggers/base.py` & `ml-starter-0.0.20/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/loggers/meter.py` & `ml-starter-0.0.20/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/loggers/multi.py` & `ml-starter-0.0.20/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/loggers/stdout.py` & `ml-starter-0.0.20/ml/loggers/stdout.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             return
 
         # Gets elapsed time since last write.
         elapsed_time = datetime.datetime.now() - self.start_time
         elapsed_time_str = format_timedelta(elapsed_time)
 
         def get_section_string(name: str, section: dict[str, Any]) -> str:
-            get_line = lambda kv: f'"{kv[0]}": {as_str(kv[1](), self.config.precision)}'
+            p1, p2 = colorize('"', "magenta"), colorize('"', "blue")
+            get_line = lambda kv: f"{p1}{kv[0]}{p2}: {as_str(kv[1](), self.config.precision)}"
             inner_str = ", ".join(map(get_line, sorted(section.items())))
             return '"' + colorize(name, "cyan") + '": {' + inner_str + "}"
 
         def colorize_phase(phase: Phase) -> str:
             match phase:
                 case "train":
                     return colorize(phase, "green", bold=True)
```

### Comparing `ml-starter-0.0.19/ml/loggers/tensorboard.py` & `ml-starter-0.0.20/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/base.py` & `ml-starter-0.0.20/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.20/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.20/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/linear.py` & `ml-starter-0.0.20/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.20/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.20/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/models/activations.py` & `ml-starter-0.0.20/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/models/base.py` & `ml-starter-0.0.20/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/models/embeddings.py` & `ml-starter-0.0.20/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/models/init.py` & `ml-starter-0.0.20/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/models/norms.py` & `ml-starter-0.0.20/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/adam.py` & `ml-starter-0.0.20/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/adamw.py` & `ml-starter-0.0.20/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/adan.py` & `ml-starter-0.0.20/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/base.py` & `ml-starter-0.0.20/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/sgd.py` & `ml-starter-0.0.20/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/optimizers/shampoo.py` & `ml-starter-0.0.20/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/scripts/cli.py` & `ml-starter-0.0.20/ml/scripts/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import shlex
 import sys
 from pathlib import Path
 from typing import Callable
 
 from omegaconf import DictConfig
 
-from ml.core.env import add_global_tag, set_project_root
-from ml.core.registry import Objects
+from ml.core.env import add_global_tag
+from ml.core.registry import Objects, add_project_dir
 from ml.scripts import compiler, mp_train, resolve, stage, train
 from ml.utils.cli import parse_cli
 from ml.utils.colors import colorize
 from ml.utils.distributed import get_rank_optional, get_world_size_optional
 from ml.utils.logging import configure_logging
 from ml.utils.random import set_random_seed
 
@@ -19,15 +19,15 @@
 
 
 def cli_main(project_root: Path | str | None = None) -> None:
     configure_logging(rank=get_rank_optional(), world_size=get_world_size_optional())
     logger.info("Command: %s", shlex.join(sys.argv))
 
     if project_root is not None:
-        set_project_root(Path(project_root).resolve())
+        add_project_dir(Path(project_root).resolve())
 
     set_random_seed()
 
     without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
         "compile": compiler.compile_main,
         "mp_train": mp_train.mp_train_main,
         "stage": stage.stage_main,
```

### Comparing `ml-starter-0.0.19/ml/scripts/compiler.py` & `ml-starter-0.0.20/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/scripts/stage.py` & `ml-starter-0.0.20/ml/scripts/stage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import logging
 
 from omegaconf import DictConfig, OmegaConf
 
-from ml.core.env import get_project_root, get_stage_dir
+from ml.core.env import get_stage_dir
+from ml.core.registry import project_dirs
 from ml.utils.staging import stage_environment
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def stage_main(config: DictConfig) -> None:
     """Stages the current configuration.
 
     Args:
         config: The configuration object.
-
-    Raises:
-        RuntimeError: If the project root is not set.
     """
 
     # Stages the currently-imported files.
-    project_root = get_project_root()
-    if project_root is None:
-        raise RuntimeError("Project root is not set.")
-    out_dir = stage_environment(project_root, get_stage_dir())
+    out_dir = stage_environment(project_dirs.paths[1:], get_stage_dir())
     logger.info("Staged environment to %s", out_dir)
 
     # Stages the raw config.
     config_dir = out_dir / "configs"
     config_dir.mkdir(exist_ok=True, parents=True)
     config_id = len(list(config_dir.glob("config_*.yaml")))
     config_path = config_dir / f"config_{config_id}.yaml"
```

### Comparing `ml-starter-0.0.19/ml/scripts/train.py` & `ml-starter-0.0.20/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/base.py` & `ml-starter-0.0.20/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.20/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.20/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/collate.py` & `ml-starter-0.0.20/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.20/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.20/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.20/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.20/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.20/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/utils.py` & `ml-starter-0.0.20/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.20/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/environments/base.py` & `ml-starter-0.0.20/ml/tasks/environments/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,7 +60,11 @@
 
         Args:
             state: The most recent state
 
         Returns:
             If the environment has finished
         """
+
+    @property
+    def fps(self) -> int:
+        return 30
```

### Comparing `ml-starter-0.0.19/ml/tasks/environments/utils.py` & `ml-starter-0.0.20/ml/tasks/environments/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 import tqdm
 from torch import Tensor
 
 from ml.tasks.environments.base import Environment
 from ml.utils.logging import configure_logging
-from ml.utils.video import WRITERS as VIDEO_WRITERS, Writer
+from ml.utils.video import Writer, write_video
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def test_environment(
     env: Environment,
     max_steps: int = 100,
@@ -48,8 +48,8 @@
                 yield env.render(state)
 
     # Save the video if a path is provided, otherwise just iterate through the
     # samples from the environment.
     if save_path is None:
         iter_environment()
     else:
-        VIDEO_WRITERS[writer](iter_environment(), save_path)
+        write_video(writer, iter_environment(), save_path)
```

### Comparing `ml-starter-0.0.19/ml/tasks/environments/worker.py` & `ml-starter-0.0.20/ml/tasks/environments/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             if self._proc.is_alive():
                 logger.warning("Process failed to finish after %.2f seconds; killing", self.cleanup_time)
                 if isinstance(self._proc, threading.Thread):
                     self._proc._stop()
                 else:
                     self._proc.kill()
         except Exception:
-            logger.exception("Exception while cleaning up task")
+            pass
 
     @classmethod
     def _thread(
         cls,
         env: "Environment[RLState, RLAction]",
         seed: int,
         action_queue: "Queue[RLAction | SpecialAction]",
@@ -348,15 +348,15 @@
             clear_queue(self.state_queue)
             for action_queue in self.action_queues:
                 clear_queue(action_queue)
                 action_queue.put("close")
             for proc in self._procs:
                 proc.join()
         except Exception:
-            logger.exception("Exception while cleaning up worker pool")
+            pass
 
     def reset(self) -> None:
         clear_queue(self.state_queue)
         for action_queue in self.action_queues:
             clear_queue(action_queue)
             action_queue.put("reset")
```

### Comparing `ml-starter-0.0.19/ml/tasks/losses/reduce.py` & `ml-starter-0.0.20/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/rl/base.py` & `ml-starter-0.0.20/ml/tasks/rl/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SpecialState,
     SyncEnvironmentWorker,
     WorkerPool,
     cast_worker_mode,
     get_worker_pool,
 )
 from ml.tasks.rl.replay import MultiReplaySamples, ReplayDataset, ReplaySamples
-from ml.utils.video import WRITERS as VIDEO_WRITERS, Writer, standardize_image
+from ml.utils.video import Writer, standardize_image, write_video
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class EnvironmentConfig:
     num_env_workers: int = conf_field(1, help="Number of environment workers (0 to run synchronously)")
@@ -440,9 +440,9 @@
 
             images_np = [standardize_image(image) for image in iter_images()]
             return torch.from_numpy(np.stack(images_np))
 
         if return_states:
             raise ValueError("Cannot return states when saving to a file")
 
-        VIDEO_WRITERS[writer](iter_images(), save_path)
+        write_video(writer, iter_images(), save_path, fps=environment.fps)
         return None
```

### Comparing `ml-starter-0.0.19/ml/tasks/rl/replay.py` & `ml-starter-0.0.20/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/tasks/sl/base.py` & `ml-starter-0.0.20/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/base.py` & `ml-starter-0.0.20/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/ddp.py` & `ml-starter-0.0.20/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.20/ml/trainers/mixins/cpu_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     monitor_event: Event,
     start_event: Event,
     pid: int,
 ) -> None:
     start_event.set()
 
     proc, cur_pid = psutil.Process(pid), os.getpid()
-    logger.info("Starting CPU stats monitor for PID %d with PID %d", pid, cur_pid)
+    logger.debug("Starting CPU stats monitor for PID %d with PID %d", pid, cur_pid)
 
     get_children = lambda: {p.pid: p for p in proc.children(recursive=True) if p.pid != cur_pid}
     child_procs = get_children()
 
     while True:
         try:
             # Updates child processes, preserving the previous child process
@@ -128,14 +128,15 @@
             logger.info("No parent process; probably cleaning up")
 
         time.sleep(ping_interval)
 
 
 class CPUStatsMonitor:
     def __init__(self, ping_interval: float, manager: SyncManager) -> None:
+        self._ping_interval = ping_interval
         self._manager = manager
         self._monitor_event = manager.Event()
         self._start_event = manager.Event()
         self._cpu_stats_smem = self._manager.Value(
             CPUStats,
             CPUStats(
                 cpu_percent=0.0,
@@ -147,42 +148,53 @@
                 mem_vms_total=0,
                 child_cpu_percent=0.0,
                 child_mem_percent=0.0,
                 num_child_procs=0,
             ),
         )
         self._cpu_stats: CPUStatsInfo | None = None
-
-        self._proc = mp.Process(
-            target=worker,
-            args=(ping_interval, self._cpu_stats_smem, self._monitor_event, self._start_event, os.getpid()),
-            daemon=False,
-        )
+        self._proc: mp.Process | None = None
 
     def get_if_set(self) -> CPUStatsInfo | None:
         if self._monitor_event.is_set():
             self._monitor_event.clear()
             return CPUStatsInfo.from_stats(self._cpu_stats_smem.get())
         return None
 
     def get(self) -> CPUStatsInfo | None:
         if (stats := self.get_if_set()) is not None:
             self._cpu_stats = stats
         return self._cpu_stats
 
     def start(self, wait: bool = False) -> None:
+        if self._proc is not None:
+            raise RuntimeError("CPU stats monitor already started")
+        if self._monitor_event.is_set():
+            self._monitor_event.clear()
+        if self._start_event.is_set():
+            self._start_event.clear()
+        self._cpu_stats = None
+        self._proc = mp.Process(
+            target=worker,
+            args=(self._ping_interval, self._cpu_stats_smem, self._monitor_event, self._start_event, os.getpid()),
+            daemon=False,
+        )
         self._proc.start()
         if wait:
             self._start_event.wait()
 
     def stop(self) -> None:
+        if self._proc is None:
+            raise RuntimeError("CPU stats monitor not started")
         if self._proc.is_alive():
             self._proc.terminate()
             logger.debug("Terminated CPU stats monitor; joining...")
             self._proc.join()
+        self._proc = None
+        self._cpu_stats = None
 
 
 class CPUStatsMixin(MonitorProcessMixin[CPUStatsConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for getting CPU statistics."""
 
     def __init__(self, config: CPUStatsConfigT) -> None:
         super().__init__(config)
```

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.20/ml/trainers/mixins/gpu_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,25 +123,28 @@
     smems: list[ValueProxy[GPUStats]],
     main_event: Event,
     events: list[Event],
     start_event: Event,
 ) -> None:
     start_event.set()
 
+    logger.debug("Starting GPU stats monitor with PID %d", os.getpid())
+
     for gpu_stat in gen_gpu_stats(ping_interval):
         if gpu_stat.index >= len(smems):
             logger.warning("GPU index %d is out of range", gpu_stat.index)
             continue
         smems[gpu_stat.index].set(gpu_stat)
         events[gpu_stat.index].set()
         main_event.set()
 
 
 class GPUStatsMonitor:
     def __init__(self, ping_interval: float, manager: SyncManager) -> None:
+        self._ping_interval = ping_interval
         self._manager = manager
 
         num_gpus = get_num_gpus()
         self._main_event = manager.Event()
         self._events = [manager.Event() for _ in range(num_gpus)]
         self._start_event = manager.Event()
 
@@ -154,20 +157,15 @@
                     temperature=0.0,
                     utilization=0.0,
                 ),
             )
             for i in range(num_gpus)
         ]
         self._gpu_stats: dict[int, GPUStatsInfo] = {}
-
-        self._proc = mp.Process(
-            target=worker,
-            args=(ping_interval, self._smems, self._main_event, self._events, self._start_event),
-            daemon=False,
-        )
+        self._proc: mp.Process | None = None
 
     def get_if_set(self) -> dict[int, GPUStatsInfo]:
         gpu_stats: dict[int, GPUStatsInfo] = {}
         if self._main_event.is_set():
             self._main_event.clear()
             for i, event in enumerate(self._events):
                 if event.is_set():
@@ -176,23 +174,41 @@
         return gpu_stats
 
     def get(self) -> dict[int, GPUStatsInfo]:
         self._gpu_stats.update(self.get_if_set())
         return self._gpu_stats
 
     def start(self, wait: bool = False) -> None:
+        if self._proc is not None:
+            raise RuntimeError("GPUStatsMonitor already started")
+        if self._main_event.is_set():
+            self._main_event.clear()
+        for event in self._events:
+            if event.is_set():
+                event.clear()
+        if self._start_event.is_set():
+            self._start_event.clear()
+        self._gpu_stats.clear()
+        self._proc = mp.Process(
+            target=worker,
+            args=(self._ping_interval, self._smems, self._main_event, self._events, self._start_event),
+            daemon=False,
+        )
         self._proc.start()
         if wait:
             self._start_event.wait()
 
     def stop(self) -> None:
+        if self._proc is None:
+            raise RuntimeError("GPUStatsMonitor not started")
         if self._proc.is_alive():
             self._proc.terminate()
             logger.debug("Terminated GPU stats monitor; joining...")
             self._proc.join()
+        self._proc = None
 
 
 class GPUStatsMixin(MonitorProcessMixin[GPUStatsConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for getting GPU statistics."""
 
     def __init__(self, config: GPUStatsConfigT) -> None:
         super().__init__(config)
```

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.20/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.20/ml/trainers/mixins/heartbeat.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     heartbeat_event: Event,
     start_event: Event,
     pid: int,
     on_heartbeat: Callable[[int, Event], None],
 ) -> None:
     start_event.set()
 
+    logger.debug("Starting heartbeat monitor for PID %d with PID %d", pid, os.getpid())
+
     while True:
         try:
             heartbeat_event.set()
             time.sleep(heartbeat_interval)
             if heartbeat_event.is_set():
                 on_heartbeat(pid, heartbeat_event)
 
@@ -61,38 +63,49 @@
 class HeartbeatMonitor:
     def __init__(
         self,
         heartbeat_interval: float,
         manager: SyncManager,
         on_heartbeat: Callable[[int, Event], None] | None,
     ) -> None:
+        self._heartbeat_interval = heartbeat_interval
+        self._on_heartbeat = on_heartbeat
         self._manager = manager
         self._heartbeat_event = manager.Event()
         self._start_event = manager.Event()
-
-        self._proc = mp.Process(
-            target=worker,
-            args=(heartbeat_interval, self._heartbeat_event, self._start_event, os.getpid(), on_heartbeat),
-            daemon=False,
-        )
+        self._proc: mp.Process | None = None
 
     def beat(self) -> None:
         if self._heartbeat_event.is_set():
             self._heartbeat_event.clear()
 
     def start(self, wait: bool = False) -> None:
+        if self._proc is not None:
+            raise RuntimeError("Heartbeat already started")
+        if self._heartbeat_event.is_set():
+            self._heartbeat_event.clear()
+        if self._start_event.is_set():
+            self._start_event.clear()
+        self._proc = mp.Process(
+            target=worker,
+            args=(self._heartbeat_interval, self._heartbeat_event, self._start_event, os.getpid(), self._on_heartbeat),
+            daemon=False,
+        )
         self._proc.start()
         if wait:
             self._start_event.wait()
 
     def stop(self) -> None:
+        if self._proc is None:
+            raise RuntimeError("Heartbeat not started")
         if self._proc.is_alive():
             self._proc.terminate()
             logger.debug("Terminated heartbeat process; joining...")
             self._proc.join()
+        self._proc = None
 
 
 class HeartbeatMonitorMixin(MonitorProcessMixin[HeartbeatConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for running a heartbeat process."""
 
     def __init__(self, config: HeartbeatConfigT) -> None:
         super().__init__(config)
```

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.20/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.20/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.20/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/rl.py` & `ml-starter-0.0.20/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/trainers/sl.py` & `ml-starter-0.0.20/ml/trainers/sl.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         try:
             with contextlib.ExitStack() as ctx:
                 profile = self.get_profile()
                 if profile is not None:
                     ctx.enter_context(profile)
 
-                with Timer("initial validation step(s)", spinner=True):
+                with Timer("initial validation step(s)"):
                     if (num_init_valid_steps := self.config.validation.num_init_valid_steps) is not None:
                         for _ in range(num_init_valid_steps):
                             self.val_step(
                                 task_model=task_model,
                                 batch=next(valid_pf_iter),
                                 state=state,
                                 task=task,
```

### Comparing `ml-starter-0.0.19/ml/trainers/slurm.py` & `ml-starter-0.0.20/ml/trainers/slurm.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,25 @@
 import os
 import re
 import signal
 import subprocess
 import sys
 from abc import ABC
 from dataclasses import dataclass
+from pathlib import Path
 from types import FrameType
 from typing import Callable, Generic, TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
 from torch import nn
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
-from ml.core.env import ProjectRoot, get_distributed_backend, get_stage_dir
-from ml.core.registry import Objects
+from ml.core.env import get_distributed_backend, get_stage_dir
+from ml.core.registry import Objects, project_dirs
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.scripts.train import train_main
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.distributed import (
     get_master_addr,
@@ -69,15 +70,15 @@
 #SBATCH --gpu-bind={gpu_bind}
 #SBATCH --output={output_path}
 #SBATCH --error={error_path}
 #SBATCH --open-mode=append
 {extra_sbatch_lines}
 
 # Sets the environment variables.
-export PROJECT_ROOT={project_root}
+export STAGE_DIR={stage_dir}
 export PYTHONPATH={pythonpath}
 export MASTER_PORT={master_port}
 
 # Set some debugging flags.
 export TORCH_DISTRIBUTED_DEBUG=DETAIL
 export TORCH_SHOW_CPP_STACKTRACES=1
 export NCCL_DEBUG=1
@@ -198,19 +199,15 @@
 
         # Writes all Slurm stuff (including logs) to this folder.
         slurm_log_dir = self.exp_dir / "logs"
         slurm_log_dir.mkdir(exist_ok=True, parents=True)
         sbatch_path = self.exp_dir / "sbatch.sh"
 
         # Stages all files to a new directory.
-        project_root = ProjectRoot.get()
-        if project_root is None:
-            raise ValueError("Project root not found; cannot stage files")
-        stage_dir = stage_environment(project_root, get_stage_dir())
-        new_project_root = stage_dir / ProjectRoot.get().name
+        stage_dir = stage_environment(project_dirs.paths[1:], get_stage_dir())
 
         # Gets the python path with the new output directory.
         python_path_parts = [str(stage_dir)] + os.environ.get("PYTHONPATH", "").split(":")
         python_path = ":".join(p for p in python_path_parts if p)
 
         # Comment miscellaneous stuff here.
         comments: list[str] = []
@@ -232,15 +229,14 @@
             tasks_per_node=tasks_per_node,
             cpus_per_task=cpus_per_task,
             gres=gres,
             gpu_bind=gpu_bind,
             output_path=slurm_log_dir / "slurm_out.txt",
             error_path=slurm_log_dir / "slurm_err.%j.txt",
             extra_sbatch_lines="\n".join(f"#SBATCH {line}" for line in sbatch_lines),
-            project_root=new_project_root,
             pythonpath=python_path,
             master_port=self.config.master_port,
             config_path=self.exp_dir / "config.yaml",
             lock_file_path=self.exp_dir / ".lock_running",
             stage_dir=stage_dir,
         )
 
@@ -272,14 +268,20 @@
         self.add_lock_file("scheduled", exists_ok=False)
 
 
 def slurm_main() -> None:
     args = sys.argv[1:]
     assert len(args) == 1, f"Unexpected arguments to `slurm_main`: {sys.argv}"
 
+    # Adds the stage directories as project directories.
+    stage_dir = Path(os.environ["STAGE_DIR"])
+    for sub_dir in stage_dir.iterdir():
+        if sub_dir.is_dir():
+            project_dirs.add(sub_dir)
+
     # Loads the raw config.
     raw_config = OmegaConf.load(args[0])
 
     # Sets environment variables from Clurm environment variables.
     set_slurm_master_addr()
     rank, world_size = set_slurm_rank_and_world_size()
```

### Comparing `ml-starter-0.0.19/ml/trainers/vanilla.py` & `ml-starter-0.0.20/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/argparse.py` & `ml-starter-0.0.20/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/atomic.py` & `ml-starter-0.0.20/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/augmentation.py` & `ml-starter-0.0.20/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/caching.py` & `ml-starter-0.0.20/ml/utils/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                     pickle.dump(obj, fb)
                     return obj
             raise NotImplementedError(f"Can't save extension {self.ext}")
 
         return call_function_cached
 
 
-class Index(Generic[Tk, Tv]):
+class DictIndex(Generic[Tk, Tv]):
     def __init__(self, items: Mapping[Tk, Sequence[Tv]]) -> None:
         """Indexes a dictionary with values that are lists.
 
         This lazily indexes all the values in the provided dictionary, flattens
         them out and allows them to be looked up by a specific index. This is
         analogous to PyTorch's ConcatDataset.
```

### Comparing `ml-starter-0.0.19/ml/utils/call_train.py` & `ml-starter-0.0.20/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/cli.py` & `ml-starter-0.0.20/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/colors.py` & `ml-starter-0.0.20/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/compiler.py` & `ml-starter-0.0.20/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/data.py` & `ml-starter-0.0.20/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/datetime.py` & `ml-starter-0.0.20/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/device/auto.py` & `ml-starter-0.0.20/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/device/base.py` & `ml-starter-0.0.20/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/device/cpu.py` & `ml-starter-0.0.20/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/device/gpu.py` & `ml-starter-0.0.20/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/device/metal.py` & `ml-starter-0.0.20/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/distributed.py` & `ml-starter-0.0.20/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/io.py` & `ml-starter-0.0.20/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/large_models.py` & `ml-starter-0.0.20/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/logging.py` & `ml-starter-0.0.20/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/meter.py` & `ml-starter-0.0.20/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/staging.py` & `ml-starter-0.0.20/ml/utils/staging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 import datetime
 import hashlib
 import logging
 import os
 import shutil
 import sys
 from pathlib import Path
+from typing import Sequence
 from uuid import uuid4
 
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 # Date format for staging environments.
 DATE_FORMAT = "%Y-%m-%d"
 
 
 def stage_environment(
-    project_root: Path,
+    project_roots: str | Path | Sequence[str | Path],
     stage_dir: Path,
     date_format: str = DATE_FORMAT,
 ) -> Path:
     """Stages the current environment to a root directory.
 
     Args:
-        project_root: The root directory of the project.
+        project_roots: The root directory of the project.
         stage_dir: The root directory for staging environments.
         date_format: The date format to use for the staging directory.
 
     Returns:
         The stage environment path
+
+    Raises:
+        ValueError: If no project root is found.
     """
 
+    if isinstance(project_roots, (str, Path)):
+        project_roots = [Path(project_roots)]
+
+    if not project_roots:
+        raise ValueError("No project root directories")
+
     with Timer("getting files to stage", spinner=True):
-        fpaths: list[tuple[Path, Path]] = []
-        for module in sys.modules.values():
-            if (fpath_str := getattr(module, "__file__", None)) is None:
-                continue
-            fpath = Path(fpath_str).resolve()
-            try:
-                rel_fpath = fpath.relative_to(project_root.parent)
-                fpaths.append((fpath, rel_fpath))
-            except ValueError:
-                pass
+        for project_root in project_roots:
+            fpaths: list[tuple[Path, Path]] = []
+            for module in sys.modules.values():
+                if (fpath_str := getattr(module, "__file__", None)) is None:
+                    continue
+                fpath = Path(fpath_str).resolve()
+                try:
+                    rel_fpath = fpath.relative_to(Path(project_root).parent)
+                    fpaths.append((fpath, rel_fpath))
+                except ValueError:
+                    pass
 
     assert fpaths, "Couldn't find any file paths to stage!"
 
     with Timer("computing hash of current environment", spinner=True):
         hashobj = hashlib.md5()
         for fpath, _ in fpaths:
             with open(fpath, "rb") as f:
```

### Comparing `ml-starter-0.0.19/ml/utils/timer.py` & `ml-starter-0.0.20/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/ml/utils/video.py` & `ml-starter-0.0.20/ml/utils/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import math
 import re
 import shutil
+import warnings
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
-from typing import AsyncGenerator, Callable, Iterator, Literal
+from typing import AsyncGenerator, Iterator, Literal
 
 import cv2
 import ffmpeg
 import matplotlib.animation as ani
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
@@ -142,14 +143,15 @@
         image = make_human_viewable_resolution(image)
 
     return image.permute(1, 2, 0).detach().cpu().numpy()
 
 
 def read_video_ffmpeg(
     in_file: str | Path,
+    *,
     output_fmt: str = "rgb24",
     channels: int = 3,
 ) -> Iterator[np.ndarray]:
     """Function that reads a video to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: The input video to read
@@ -174,14 +176,15 @@
 
     stream.stdout.close()
     stream.wait()
 
 
 async def read_video_with_timestamps_ffmpeg(
     in_file: str | Path,
+    *,
     output_fmt: str = "rgb24",
     channels: int = 3,
     target_dims: tuple[int | None, int | None] | None = None,
 ) -> AsyncGenerator[tuple[np.ndarray, float], None]:
     """Like `read_video_ffmpeg` but also returns timestamps.
 
     Args:
@@ -273,14 +276,15 @@
             return
         yield buffer
 
 
 def write_video_opencv(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
+    *,
     fps: int | Fraction = 30,
     codec: str = "MP4V",
 ) -> None:
     """Function that writes a video from a stream of numpy arrays using OpenCV.
 
     Args:
         itr: The image iterator, yielding images with shape (H, W, C).
@@ -308,14 +312,15 @@
     stream.release()
     cv2.destroyAllWindows()
 
 
 def write_video_ffmpeg(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
+    *,
     fps: int | Fraction = 30,
     out_fps: int | Fraction = 30,
     vcodec: str = "libx264",
     input_fmt: str = "rgb24",
     output_fmt: str = "yuv420p",
 ) -> None:
     """Function that writes an video from a stream of numpy arrays using FFMPEG.
@@ -351,14 +356,15 @@
     stream.stdin.close()
     stream.wait()
 
 
 def write_video_matplotlib(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
+    *,
     dpi: int = 50,
     fps: int | Fraction = 30,
     title: str = "Video",
     comment: str | None = None,
     writer: str = "ffmpeg",
 ) -> None:
     """Function that writes an video from a stream of input tensors.
@@ -411,23 +417,47 @@
             im.set_data(as_uint8(standardize_image(img)))
             mpl_writer.grab_frame()
 
 
 Reader = Literal["ffmpeg", "opencv"]
 Writer = Literal["ffmpeg", "matplotlib", "opencv"]
 
-READERS: dict[Reader, Callable[[str | Path], Iterator[np.ndarray]]] = {
-    "ffmpeg": read_video_ffmpeg,
-    "opencv": read_video_opencv,
-}
-
-WRITERS: dict[Writer, Callable[[Iterator[np.ndarray | Tensor], str | Path], None]] = {
-    "ffmpeg": write_video_ffmpeg,
-    "matplotlib": write_video_matplotlib,
-    "opencv": write_video_opencv,
-}
-
-# Remove the FFMPEG reader and writer if FFMPEG is not available in the system.
-if not shutil.which("ffmpeg"):
-    READERS.pop("ffmpeg")
-    WRITERS.pop("ffmpeg")
-    WRITERS.pop("matplotlib")
+
+def read_video(reader: Reader, in_file: str | Path) -> Iterator[np.ndarray]:
+    if reader == "ffmpeg":
+        if not shutil.which("ffmpeg"):
+            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
+            reader = "opencv"
+        else:
+            return read_video_ffmpeg(in_file)
+
+    if reader == "opencv":
+        return read_video_opencv(in_file)
+
+    raise ValueError(f"Invalid reader: {reader}")
+
+
+def write_video(
+    writer: Writer,
+    itr: Iterator[np.ndarray | Tensor],
+    out_file: str | Path,
+    *,
+    fps: int | Fraction = 30,
+) -> None:
+    if writer == "ffmpeg":
+        if not shutil.which("ffmpeg"):
+            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
+            writer = "opencv"
+        else:
+            return write_video_ffmpeg(itr, out_file, fps=fps)
+
+    if writer == "matplotlib":
+        if not shutil.which("ffmpeg"):
+            warnings.warn("FFMPEG is not available in the system. Falling back to OpenCV.")
+            writer = "opencv"
+        else:
+            return write_video_matplotlib(itr, out_file, fps=fps)
+
+    if writer == "opencv":
+        return write_video_opencv(itr, out_file, fps=fps)
+
+    raise ValueError(f"Invalid writer: {writer}")
```

### Comparing `ml-starter-0.0.19/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.20/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.19
+Version: 0.0.20
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.19/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.20/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 ml/utils/distributed.py
 ml/utils/io.py
 ml/utils/large_models.py
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
-ml/utils/paths.py
 ml/utils/random.py
 ml/utils/staging.py
 ml/utils/timer.py
 ml/utils/video.py
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
```

### Comparing `ml-starter-0.0.19/pyproject.toml` & `ml-starter-0.0.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.19/setup.py` & `ml-starter-0.0.20/setup.py`

 * *Files identical despite different names*

