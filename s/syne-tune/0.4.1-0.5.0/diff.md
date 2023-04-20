# Comparing `tmp/syne_tune-0.4.1.tar.gz` & `tmp/syne_tune-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.4.1.tar", last modified: Thu Mar 16 14:17:10 2023, max compression
+gzip compressed data, was "syne_tune-0.5.0.tar", last modified: Thu Apr 20 13:27:06 2023, max compression
```

## Comparing `syne_tune-0.4.1.tar` & `syne_tune-0.5.0.tar`

### file list

```diff
@@ -1,276 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-16 14:16:57.000000 syne_tune-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-16 14:16:57.000000 syne_tune-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-16 14:16:57.000000 syne_tune-0.4.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-03-16 14:17:10.872910 syne_tune-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-03-16 14:16:57.000000 syne_tune-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-16 14:17:10.872910 syne_tune-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-03-16 14:16:57.000000 syne_tune-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.852910 syne_tune-0.4.1/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.852910 syne_tune-0.4.1/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.852910 syne_tune-0.4.1/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43889 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.856910 syne_tune-0.4.1/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36478 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    55879 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.860910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.864910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.864910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.864910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.864910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.864910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20877 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    30724 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    41953 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.868910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    15446 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34001 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.872910 syne_tune-0.4.1/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 14:16:57.000000 syne_tune-0.4.1/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:17:10.852910 syne_tune-0.4.1/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-03-16 14:17:10.000000 syne_tune-0.4.1/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-03-16 14:17:10.000000 syne_tune-0.4.1/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:17:10.000000 syne_tune-0.4.1/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-16 14:17:10.000000 syne_tune-0.4.1/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 14:17:10.000000 syne_tune-0.4.1/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-20 13:26:53.000000 syne_tune-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 13:26:53.000000 syne_tune-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 13:26:53.000000 syne_tune-0.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-04-20 13:27:06.302595 syne_tune-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-04-20 13:26:53.000000 syne_tune-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 13:27:06.302595 syne_tune-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-20 13:26:53.000000 syne_tune-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.282595 syne_tune-0.5.0/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.286595 syne_tune-0.5.0/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43889 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36483 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.290595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.294595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20877 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31946 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42535 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.298595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15446 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34001 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.302595 syne_tune-0.5.0/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 13:26:53.000000 syne_tune-0.5.0/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:27:06.282595 syne_tune-0.5.0/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 13:27:06.000000 syne_tune-0.5.0/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.4.1/LICENSE` & `syne_tune-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/PKG-INFO` & `syne_tune-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne_tune
-Version: 0.4.1
+Version: 0.5.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Provides-Extra: kde
 Provides-Extra: gpsearchers
 Provides-Extra: benchmarks
 Provides-Extra: blackbox-repository
 Provides-Extra: aws
 Provides-Extra: yahpo
 Provides-Extra: dev
+Provides-Extra: moo
 Provides-Extra: extra
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
@@ -49,21 +50,22 @@
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to get the latest version from git: 
+or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
+pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -73,62 +75,63 @@
 
 ## Getting started
 
 To enable tuning, you have to report metrics from a training script so that they can be communicated later to Syne Tune,
 this can be accomplished by just calling `report(epoch=epoch, loss=loss)` as shown in the example below:
 
 ```python
-# train_height.py
+# train_height_simple.py
 import logging
 import time
 
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
-
     parser = ArgumentParser()
     parser.add_argument('--steps', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
-
     args, _ = parser.parse_known_args()
     report = Reporter()
-
     for step in range(args.steps):
-        dummy_score = (0.1 + args.width * step / 100) ** (-1) + args.height * 0.1
-        # Feed the score back to Syne Tune.
-        report(step=step, mean_loss=dummy_score, epoch=step + 1)
         time.sleep(0.1)
+        dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
+        # Feed the score back to Syne Tune.
+        report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
 
 ```python
+# launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
 
 # hyperparameter search space to consider
 config_space = {
-    'steps': 100,
     'width': randint(1, 20),
     'height': randint(1, 20),
+    'epochs': 100,
 }
 
 tuner = Tuner(
     trial_backend=LocalBackend(entry_point='train_height.py'),
     scheduler=ASHA(
-        config_space, metric='mean_loss', resource_attr='epoch', max_t=100,
+        config_space,
+        metric='mean_loss',
+        resource_attr='epoch',
+        max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
-    stop_criterion=StoppingCriterion(max_wallclock_time=15),
+    stop_criterion=StoppingCriterion(max_wallclock_time=30),
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
@@ -146,15 +149,16 @@
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
-HyperTune | Li, et al. (2022) | model-based | yes | yes | no 
+HyperTune | Li, et al. (2022) | model-based | yes | yes | no
+DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
@@ -172,87 +176,101 @@
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
-You will find the following examples in [examples/](examples/) folder illustrating different functionalities provided
-by Syne Tune:
+You will find many examples in the [examples/](examples/) folder illustrating
+different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
   [train_height_example.py](examples/training_scripts/height_example/train_height.py) for several baselines  
-* [launch_height_ray.py](examples/launch_height_ray.py):
-  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
-  scheduler
 * [launch_height_moasha.py](examples/launch_height_moasha.py):
   shows how to tune a script reporting multiple-objectives with multiobjective Asynchronous Hyperband (MOASHA)
 * [launch_height_standalone_scheduler.py](examples/launch_height_standalone_scheduler.py):
   launches HPO locally with a custom scheduler that cuts any trial that is not
   in the top 80%
 * [launch_height_sagemaker_remotely.py](examples/launch_height_sagemaker_remotely.py):
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
+* [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
+  launches Bayesian contrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
   launches HPO on SageMaker to tune a entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
+* [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
+  shows how results can be visualized on the fly with TensorBoard
+* [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
+  demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
-launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
-employs an easy-to-use benchmark convention
+  launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
+  employs an easy-to-use benchmark convention
 * [launch_huggingface_classification.py](examples/launch_huggingface_classification.py):
   launches HPO on SageMaker to tune a SageMaker Hugging Face estimator for sentiment classification
 * [launch_tuning_gluonts.py](examples/launch_tuning_gluonts.py):
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
+* [launch_height_ray.py](examples/launch_height_ray.py):
+  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
+  scheduler
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
 * [How can I run on AWS and SageMaker?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-on-aws-and-sagemaker)
 * [What are the metrics reported by default when calling the `Reporter`?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-metrics-reported-by-default-when-calling-the-reporter)
 * [How can I utilize multiple GPUs?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-utilize-multiple-gpus)
 * [What is the default mode when performing optimization?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-is-the-default-mode-when-performing-optimization)
 * [How are trials evaluated on a local machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-are-trials-evaluated-on-a-local-machine)
-* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [Where can I find the output of the tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-the-tuning)
+* [How can I change the default output folder where tuning results are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-change-the-default-output-folder-where-tuning-results-are-stored)
+* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [How can I enable trial checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-enable-trial-checkpointing)
+* [How can I retrieve the best checkpoint obtained after tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-retrieve-the-best-checkpoint-obtained-after-tuning)
 * [Which schedulers make use of checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#which-schedulers-make-use-of-checkpointing)
 * [Is the tuner checkpointed?](https://syne-tune.readthedocs.io/en/latest/faq.html#is-the-tuner-checkpointed)
 * [Where can I find the output of my trials?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-my-trials)
 * [How can I plot the results of a tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-plot-the-results-of-a-tuning)
 * [How can I specify additional tuning metadata?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-additional-tuning-metadata)
 * [How do I append additional information to the results which are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-append-additional-information-to-the-results-which-are-stored) 
 * [I don’t want to wait, how can I launch the tuning on a remote machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#i-dont-want-to-wait-how-can-i-launch-the-tuning-on-a-remote-machine)
 * [How can I run many experiments in parallel?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-many-experiments-in-parallel)
 * [How can I access results after tuning remotely?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-access-results-after-tuning-remotely)
 * [How can I specify dependencies to remote launcher or when using the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-dependencies-to-remote-launcher-or-when-using-the-sagemaker-backend)
 * [How can I benchmark different methods?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-benchmark-different-methods)
 * [What different schedulers do you support? What are the main differences between them?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-different-schedulers-do-you-support-what-are-the-main-differences-between-them)
 * [How do I define the search space?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-define-the-search-space) 
+* [How do I set arguments of multi-fidelity schedulers?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-set-arguments-of-multi-fidelity-schedulers)
 * [How can I visualize the progress of my tuning experiment with Tensorboard?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-visualize-the-progress-of-my-tuning-experiment-with-tensorboard)
 * [How can I add a new scheduler?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-scheduler)
 * [How can I add a new tabular or surrogate benchmark?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-tabular-or-surrogate-benchmark)
+* [How can I reduce delays in starting trials with the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-reduce-delays-in-starting-trials-with-the-sageMaker-backend)
+* [How can I pass lists or dictionaries to the training script?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-pass-lists-or-dictionaries-to-the-training-script)
+* [How can I write extra results for an experiment?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-write-extra-results-for-an-experiment)
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
-* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
-* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
-* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
+* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
+* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
+* [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
+* [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.4.1/README.md` & `syne_tune-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to get the latest version from git: 
+or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
+pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -48,62 +49,63 @@
 
 ## Getting started
 
 To enable tuning, you have to report metrics from a training script so that they can be communicated later to Syne Tune,
 this can be accomplished by just calling `report(epoch=epoch, loss=loss)` as shown in the example below:
 
 ```python
-# train_height.py
+# train_height_simple.py
 import logging
 import time
 
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
-
     parser = ArgumentParser()
     parser.add_argument('--steps', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
-
     args, _ = parser.parse_known_args()
     report = Reporter()
-
     for step in range(args.steps):
-        dummy_score = (0.1 + args.width * step / 100) ** (-1) + args.height * 0.1
-        # Feed the score back to Syne Tune.
-        report(step=step, mean_loss=dummy_score, epoch=step + 1)
         time.sleep(0.1)
+        dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
+        # Feed the score back to Syne Tune.
+        report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
 
 ```python
+# launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
 
 # hyperparameter search space to consider
 config_space = {
-    'steps': 100,
     'width': randint(1, 20),
     'height': randint(1, 20),
+    'epochs': 100,
 }
 
 tuner = Tuner(
     trial_backend=LocalBackend(entry_point='train_height.py'),
     scheduler=ASHA(
-        config_space, metric='mean_loss', resource_attr='epoch', max_t=100,
+        config_space,
+        metric='mean_loss',
+        resource_attr='epoch',
+        max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
-    stop_criterion=StoppingCriterion(max_wallclock_time=15),
+    stop_criterion=StoppingCriterion(max_wallclock_time=30),
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
@@ -121,15 +123,16 @@
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
-HyperTune | Li, et al. (2022) | model-based | yes | yes | no 
+HyperTune | Li, et al. (2022) | model-based | yes | yes | no
+DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
@@ -147,87 +150,101 @@
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
-You will find the following examples in [examples/](examples/) folder illustrating different functionalities provided
-by Syne Tune:
+You will find many examples in the [examples/](examples/) folder illustrating
+different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
   [train_height_example.py](examples/training_scripts/height_example/train_height.py) for several baselines  
-* [launch_height_ray.py](examples/launch_height_ray.py):
-  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
-  scheduler
 * [launch_height_moasha.py](examples/launch_height_moasha.py):
   shows how to tune a script reporting multiple-objectives with multiobjective Asynchronous Hyperband (MOASHA)
 * [launch_height_standalone_scheduler.py](examples/launch_height_standalone_scheduler.py):
   launches HPO locally with a custom scheduler that cuts any trial that is not
   in the top 80%
 * [launch_height_sagemaker_remotely.py](examples/launch_height_sagemaker_remotely.py):
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
+* [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
+  launches Bayesian contrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
   launches HPO on SageMaker to tune a entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
+* [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
+  shows how results can be visualized on the fly with TensorBoard
+* [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
+  demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
-launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
-employs an easy-to-use benchmark convention
+  launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
+  employs an easy-to-use benchmark convention
 * [launch_huggingface_classification.py](examples/launch_huggingface_classification.py):
   launches HPO on SageMaker to tune a SageMaker Hugging Face estimator for sentiment classification
 * [launch_tuning_gluonts.py](examples/launch_tuning_gluonts.py):
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
+* [launch_height_ray.py](examples/launch_height_ray.py):
+  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
+  scheduler
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
 * [How can I run on AWS and SageMaker?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-on-aws-and-sagemaker)
 * [What are the metrics reported by default when calling the `Reporter`?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-metrics-reported-by-default-when-calling-the-reporter)
 * [How can I utilize multiple GPUs?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-utilize-multiple-gpus)
 * [What is the default mode when performing optimization?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-is-the-default-mode-when-performing-optimization)
 * [How are trials evaluated on a local machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-are-trials-evaluated-on-a-local-machine)
-* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [Where can I find the output of the tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-the-tuning)
+* [How can I change the default output folder where tuning results are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-change-the-default-output-folder-where-tuning-results-are-stored)
+* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [How can I enable trial checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-enable-trial-checkpointing)
+* [How can I retrieve the best checkpoint obtained after tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-retrieve-the-best-checkpoint-obtained-after-tuning)
 * [Which schedulers make use of checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#which-schedulers-make-use-of-checkpointing)
 * [Is the tuner checkpointed?](https://syne-tune.readthedocs.io/en/latest/faq.html#is-the-tuner-checkpointed)
 * [Where can I find the output of my trials?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-my-trials)
 * [How can I plot the results of a tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-plot-the-results-of-a-tuning)
 * [How can I specify additional tuning metadata?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-additional-tuning-metadata)
 * [How do I append additional information to the results which are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-append-additional-information-to-the-results-which-are-stored) 
 * [I don’t want to wait, how can I launch the tuning on a remote machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#i-dont-want-to-wait-how-can-i-launch-the-tuning-on-a-remote-machine)
 * [How can I run many experiments in parallel?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-many-experiments-in-parallel)
 * [How can I access results after tuning remotely?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-access-results-after-tuning-remotely)
 * [How can I specify dependencies to remote launcher or when using the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-dependencies-to-remote-launcher-or-when-using-the-sagemaker-backend)
 * [How can I benchmark different methods?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-benchmark-different-methods)
 * [What different schedulers do you support? What are the main differences between them?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-different-schedulers-do-you-support-what-are-the-main-differences-between-them)
 * [How do I define the search space?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-define-the-search-space) 
+* [How do I set arguments of multi-fidelity schedulers?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-set-arguments-of-multi-fidelity-schedulers)
 * [How can I visualize the progress of my tuning experiment with Tensorboard?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-visualize-the-progress-of-my-tuning-experiment-with-tensorboard)
 * [How can I add a new scheduler?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-scheduler)
 * [How can I add a new tabular or surrogate benchmark?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-tabular-or-surrogate-benchmark)
+* [How can I reduce delays in starting trials with the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-reduce-delays-in-starting-trials-with-the-sageMaker-backend)
+* [How can I pass lists or dictionaries to the training script?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-pass-lists-or-dictionaries-to-the-training-script)
+* [How can I write extra results for an experiment?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-write-extra-results-for-an-experiment)
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
-* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
-* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
-* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
+* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
+* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
+* [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
+* [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.4.1/setup.py` & `syne_tune-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,25 +34,27 @@
 )
 required_yahpo = load_requirements(
     "syne_tune/blackbox_repository/conversion_scripts/scripts/requirements-yahpo.txt"
 )
 required_benchmarks = load_benchmark_requirements()
 required_dev = load_requirements("requirements-dev.txt")
 required_aws = load_requirements("requirements-aws.txt")
+required_moo = load_requirements("requirements-moo.txt")
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 required_extra = (
     required_ray
     + required_gpsearchers
     + required_benchmarks
     + required_blackbox_repository
     + required_kde
     + required_dev
     + required_aws
     + required_yahpo
+    + required_moo
 )
 
 # Botorch only supports python version >= 3.8
 if sys.version_info >= (3, 8):
     required_extra += required_botorch
 
 setup(
@@ -74,14 +76,15 @@
         "kde": required_kde,
         "gpsearchers": required_gpsearchers,
         "benchmarks": required_benchmarks,
         "blackbox-repository": required_blackbox_repository,
         "aws": required_aws,
         "yahpo": required_yahpo,
         "dev": required_dev,
+        "moo": required_moo,
         "extra": required_extra,
     },
     install_requires=required_core,
     include_package_data=True,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `syne_tune-0.4.1/syne_tune/__init__.py` & `syne_tune-0.5.0/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/__init__.py` & `syne_tune-0.5.0/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/local_backend.py` & `syne_tune-0.5.0/syne_tune/backend/local_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.5.0/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.5.0/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.5.0/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.5.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.5.0/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.5.0/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,20 @@
 from syne_tune.backend.simulator_backend.events import (
     SimulatorState,
     StartEvent,
     CompleteEvent,
     StopEvent,
     OnTrialResultEvent,
 )
-from syne_tune.constants import ST_CHECKPOINT_DIR, ST_WORKER_TIMESTAMP, ST_TUNER_TIME
-from syne_tune.tuner import DEFAULT_SLEEP_TIME
+from syne_tune.constants import (
+    ST_CHECKPOINT_DIR,
+    ST_WORKER_TIMESTAMP,
+    ST_TUNER_TIME,
+    TUNER_DEFAULT_SLEEP_TIME,
+)
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_DELAY = 0.05
 
 
@@ -125,15 +129,15 @@
     """
 
     def __init__(
         self,
         entry_point: str,
         elapsed_time_attr: str,
         simulator_config: Optional[SimulatorConfig] = None,
-        tuner_sleep_time: float = DEFAULT_SLEEP_TIME,
+        tuner_sleep_time: float = TUNER_DEFAULT_SLEEP_TIME,
         debug_resource_attr: Optional[str] = None,
     ):
         super().__init__(entry_point=entry_point, rotate_gpus=False)
         self.elapsed_time_attr = elapsed_time_attr
         if simulator_config is None:
             self.simulator_config = SimulatorConfig()
         else:
```

### Comparing `syne_tune-0.4.1/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.5.0/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
+from typing import Optional
 import logging
 
-from syne_tune.tuner_callback import StoreResultsCallback
+from syne_tune.results_callback import StoreResultsCallback, ExtraResultsComposer
 from syne_tune.backend.simulator_backend.simulator_backend import SimulatorBackend
 from syne_tune import Tuner
 from syne_tune.constants import ST_TUNER_TIME
 from syne_tune import StoppingCriterion
 from syne_tune.optimizer.schedulers.fifo import FIFOScheduler
 
 logger = logging.getLogger(__name__)
@@ -42,21 +43,28 @@
     a decision based on ``max_wallclock_time``. By default,
     :class:`~syne_tune.StoppingCriterion` takes ``TuningStatus`` as an input,
     which counts real time and knows nothing about simulated time. To this
     end, we modify ``stop_criterion`` of the tuner to instead depend on the
     ``ST_TUNER_TIME`` fields in the results received. This allows us to keep
     both :class:`~syne_tune.Tuner` and ``TuningStatus`` independent of the time
     keeper.
+
+    :param extra_results_composer: Optional. If given, this is called in
+        :meth:`on_trial_result`, and the resulting dictionary is appended as
+        extra columns to the results dataframe
     """
 
-    def __init__(self):
+    def __init__(self, extra_results_composer: Optional[ExtraResultsComposer] = None):
         # Note: ``results_update_interval`` is w.r.t. real time, not
         # simulated time. Storing results intermediately is not important for
         # the simulator backend, so the default is larger
-        super().__init__(add_wallclock_time=True)
+        super().__init__(
+            add_wallclock_time=True,
+            extra_results_composer=extra_results_composer,
+        )
         self._tuner_sleep_time = None
         self._time_keeper = None
         self._tuner = None
         self._backup_stop_criterion = None
 
     def _modify_stop_criterion(self, tuner: "Tuner"):
         stop_criterion = tuner.stop_criterion
```

### Comparing `syne_tune-0.4.1/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.5.0/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/time_keeper.py` & `syne_tune-0.5.0/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/backend/trial_backend.py` & `syne_tune-0.5.0/syne_tune/backend/trial_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 
 class TrialBackend:
     """
     Interface for backend to execute evaluations of trials.
 
     :param delete_checkpoints: If ``True``, the checkpoints written by a trial
         are deleted once the trial is stopped or is registered as
-        completed. Also, as part of :meth:`stop_all` called at the end of the
-        tuning loop, all remaining checkpoints are deleted. Defaults to
-        ``False``.
+        completed. Checkpoints of paused trials may also be removed, if the
+        scheduler supports early checkpoint removal. Also, as part of
+        :meth:`stop_all` called at the end of the tuning loop, all remaining
+        checkpoints are deleted. Defaults to ``False`` (no checkpoints are
+        removed).
     :param pass_args_as_json: Normally, the hyperparameter configuration is
         passed as command line arguments to the trial evaluation script. This
         works if all hyperparameters have elementary types. If
         ``pass_args_as_json == True``, the configuration is instead written into
         a JSON file, whose name is passed as command line argument
         :const:`~syne_tune.constants.ST_CONFIG_JSON_FNAME_ARG`. The trial
         evaluation script then loads the configuration from this file. This allows
```

### Comparing `syne_tune-0.4.1/syne_tune/backend/trial_status.py` & `syne_tune-0.5.0/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.5.0/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/callbacks/__init__.py` & `syne_tune-0.5.0/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.5.0/syne_tune/callbacks/tensorboard_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,19 @@
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["writer"]
         return state
 
     def __setstate__(self, state):
-        super().__init__(
+        self.__init__(
             ignore_metrics=state["ignore_metrics"],
             target_metric=state["target_metric"],
             mode="min" if state["metric_sign"] == 1 else "max",
+            log_hyperparameters=state["log_hyperparameters"],
         )
         self.results = state["results"]
         self.curr_best_value = state["curr_best_value"]
         self.curr_best_config = state["curr_best_config"]
         self.start_time_stamp = state["start_time_stamp"]
         self.iter = state["iter"]
```

### Comparing `syne_tune-0.4.1/syne_tune/config_space.py` & `syne_tune-0.5.0/syne_tune/config_space.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/constants.py` & `syne_tune-0.5.0/syne_tune/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,11 +68,25 @@
 ST_CONFIG_JSON_FNAME_ARG = "st_config_json_filename"
 """Name of config key for config JSON file"""  # pylint: disable=W0105
 
 ST_REMOTE_UPLOAD_DIR_NAME = "tuner"
 """Name for ``upload_dir`` in ``RemoteTuner``"""  # pylint: disable=W0105
 
 
+# File names
+
+ST_RESULTS_DATAFRAME_FILENAME = "results.csv.zip"
+"""Name for results dataframe stored in ``StoreResultsCallback``"""  # pylint: disable=W0105
+
+ST_METADATA_FILENAME = "metadata.json"
+"""Name for metadata file stored in ``Tuner``"""  # pylint: disable=W0105
+
+ST_TUNER_DILL_FILENAME = "tuner.dill"
+"""Name for final tuner object file stored in ``Tuner``"""  # pylint: disable=W0105
+
 # Limits
 
 MAX_METRICS_SUPPORTED_BY_SAGEMAKER = 40
 """Max number of metrics allowed for estimator"""  # pylint: disable=W0105
+
+TUNER_DEFAULT_SLEEP_TIME = 5.0
+"""Default value for ``sleep_time``"""  # pylint: disable=W0105
```

### Comparing `syne_tune-0.4.1/syne_tune/experiments.py` & `syne_tune-0.5.0/syne_tune/experiments.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,36 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import List, Dict, Callable, Optional, Union, Any
 import json
 import logging
+from dataclasses import dataclass
 from datetime import datetime
 from json.decoder import JSONDecodeError
-import pandas as pd
-from dataclasses import dataclass
 from pathlib import Path
+from typing import List, Dict, Callable, Optional, Union, Any, Tuple
+
+import numpy as np
+import pandas as pd
 
-from syne_tune.constants import ST_TUNER_TIME, ST_TUNER_CREATION_TIMESTAMP
 from syne_tune import Tuner
-from syne_tune.util import experiment_path, s3_experiment_path
+from syne_tune.constants import (
+    ST_TUNER_TIME,
+    ST_TUNER_CREATION_TIMESTAMP,
+    ST_METADATA_FILENAME,
+    ST_RESULTS_DATAFRAME_FILENAME,
+    ST_TUNER_DILL_FILENAME,
+)
+from syne_tune.optimizer.schedulers.multiobjective.utils import hypervolume_cumulative
 from syne_tune.try_import import try_import_aws_message
+from syne_tune.util import experiment_path, s3_experiment_path
 
 try:
     import boto3
     from botocore.exceptions import ClientError
 except ImportError:
     print(try_import_aws_message())
 
@@ -57,71 +66,164 @@
 
     def creation_date(self):
         """
         :return: Timestamp when :class:`~syne_tune.Tuner` was created
         """
         return datetime.fromtimestamp(self.metadata[ST_TUNER_CREATION_TIMESTAMP])
 
-    def plot(self, **plt_kwargs):
+    def plot_hypervolume(
+        self,
+        metrics_to_plot: Union[List[int], List[str]] = None,
+        reference_point: np.ndarray = None,
+        figure_path: str = None,
+        **plt_kwargs,
+    ):
+        """Plot best hyervolume value as function of wallclock time
+
+        :param reference_point: Reference point for hypervolume calculations.
+            If None, the maximum values of each metric is used.
+        :param figure_path: If specified, defines the path where the figure will be saved.
+            If None, the figure is shown
+        :param plt_kwargs: Arguments to :func:`matplotlib.pyplot.plot`
+        """
+        import matplotlib.pyplot as plt
+
+        if metrics_to_plot is None:
+            metrics_to_plot = self.metric_names()
+
+        assert (
+            len(metrics_to_plot) > 1
+        ), "Only one metric defined, cannot compute hypervolume"
+
+        metrics, metric_names, metric_modes = zip(
+            *[self._metric_name_mode(metric) for metric in metrics_to_plot]
+        )
+        assert np.all(
+            [metric_mode == "max" for metric_mode in metric_modes]
+        ), f"All metrics must be maximized but the following modes were selected: {metric_modes}"
+
+        if self.results is not None and len(self.results) > 0:
+            results_df = self.results.sort_values(ST_TUNER_TIME)
+
+            x = self.results.loc[:, ST_TUNER_TIME]
+            results_array = results_df[list(metric_names)].values
+            hypervolume_indicator = hypervolume_cumulative(
+                results_array, reference_point
+            )
+
+            fig, ax = plt.subplots()
+            ax.plot(x, hypervolume_indicator, **plt_kwargs)
+            ax.set_xlabel("wallclock time (secs)")
+            ax.set_ylabel("Hypervolume indicator")
+            ax.set_title(f"Hypervolume over time {self.name}")
+            if figure_path is not None:
+                fig.savefig(figure_path)
+            else:
+                fig.show()
+
+    def plot(
+        self, metric_to_plot: Union[str, int] = 0, figure_path: str = None, **plt_kwargs
+    ):
         """Plot best metric value as function of wallclock time
 
+        :param metric_to_plot: Indicates which metric to plot, can be the index or a name of the metric.
+            default to 0 - first metric defined
+        :param figure_path: If specified, defines the path where the figure will be saved.
+            If None, the figure is shown
         :param plt_kwargs: Arguments to :func:`matplotlib.pyplot.plot`
         """
         import matplotlib.pyplot as plt
 
-        metric = self.metric_names()[0]
+        metric, metric_name, metric_mode = self._metric_name_mode(
+            metric_to_plot, verbose=True
+        )
+
         df = self.results
         if df is not None and len(df) > 0:
             df = df.sort_values(ST_TUNER_TIME)
             x = df.loc[:, ST_TUNER_TIME]
             y = (
-                df.loc[:, metric].cummax()
-                if self.metric_mode() == "max"
-                else df.loc[:, metric].cummin()
+                df.loc[:, metric_name].cummax()
+                if metric_mode == "max"
+                else df.loc[:, metric_name].cummin()
             )
-            plt.plot(x, y, **plt_kwargs)
-            plt.xlabel("wallclock time (secs)")
-            plt.ylabel(metric)
-            plt.title(f"Best result over time {self.name}")
-            plt.show()
+            fig, ax = plt.subplots()
+            ax.plot(x, y, **plt_kwargs)
+            ax.set_xlabel("wallclock time (secs)")
+            ax.set_ylabel(metric_name)
+            ax.set_title(f"Best result over time {self.name}")
+            if figure_path is not None:
+                fig.savefig(figure_path)
+            else:
+                fig.show()
 
-    def metric_mode(self) -> str:
+    def metric_mode(self) -> Union[str, List[str]]:
         return self.metadata["metric_mode"]
 
     def metric_names(self) -> List[str]:
         return self.metadata["metric_names"]
 
     def entrypoint_name(self) -> str:
         return self.metadata["entrypoint"]
 
-    def best_config(self) -> Dict[str, Any]:
+    def best_config(self, metric: Union[str, int] = 0) -> Dict[str, Any]:
         """
-        Return the best config found for the first metric defined in the scheduler.
+        Return the best config found for the specified metric
+        :param metric: Indicates which metric to use, can be the index or a name of the metric.
+            default to 0 - first metric defined in the Scheduler
         :return: Configuration corresponding to best metric value
         """
-        metric_names = self.metric_names()
-        metric_mode = self.metric_mode()
-
-        if len(metric_names) > 1:
-            logging.warning(
-                "Several metrics exists so the best is not defined, this will "
-                f"return the best w.r.t. the first metric of {metric_names}."
-            )
-        metric_name = metric_names[0]
+        metric, metric_name, metric_mode = self._metric_name_mode(metric, verbose=True)
 
         # locate best result
         if metric_mode == "min":
             best_index = self.results.loc[:, metric_name].argmin()
         else:
             best_index = self.results.loc[:, metric_name].argmax()
         res = dict(self.results.loc[best_index])
 
         # Don't include internal fields
         return {k: v for k, v in res.items() if not k.startswith("st_")}
 
+    def _metric_name_mode(
+        self, metric: Union[str, int], verbose: bool = False
+    ) -> Tuple[int, str, str]:
+        """
+        Determine the metric, name and its mode given ambiguous input.
+        :param metric: Index or name of the selected metric
+        :param verbose: If True, prints a warning message when only one metric is selected from many
+        """
+        if isinstance(metric, str):
+            assert (
+                metric in self.metric_names()
+            ), f"Attepted to use {metric} while available metrics are {self.metric_names()}"
+            metric_name = metric
+            metric = self.metric_names().index(metric)
+        elif isinstance(metric, int):
+            assert metric < len(
+                self.metric_names()
+            ), f"Attepted to use metric index={metric} with {len(self.metric_names())} availale metrics"
+            metric_name = self.metric_names()[metric]
+        else:
+            raise AttributeError(
+                f"metic must be <int> or <str> but {type(metric)} was provided"
+            )
+
+        if len(self.metric_names()) > 1 and verbose:
+            logging.warning(
+                "Several metrics exists, this will "
+                f"use metric={metric_name} (index={metric}) out of {self.metric_names()}."
+            )
+
+        metric_mode = self.metric_mode()
+        if len(metric_mode) > 1:
+            metric_mode = metric_mode[metric]
+
+        return metric, metric_name, metric_mode
+
 
 def download_single_experiment(
     tuner_name: str,
     s3_bucket: Optional[str] = None,
     experiment_name: Optional[str] = None,
 ):
     """Downloads results from S3 of a tuning experiment
@@ -136,15 +238,20 @@
     ).rstrip("/")
     tgt_dir = experiment_path(tuner_name=tuner_name)
     tgt_dir.mkdir(exist_ok=True, parents=True)
     s3 = boto3.client("s3")
     parts_path = s3_path.replace("s3://", "").split("/")
     s3_bucket = parts_path[0]
     s3_key = "/".join(parts_path[1:])
-    for file in ["metadata.json", "results.csv.zip", "tuner.dill"]:
+    result_files = [
+        ST_METADATA_FILENAME,
+        ST_RESULTS_DATAFRAME_FILENAME,
+        ST_TUNER_DILL_FILENAME,
+    ]
+    for file in result_files:
         try:
             logging.info(f"downloading {file} on {s3_path}")
             s3.download_file(s3_bucket, f"{s3_key}/{file}", str(tgt_dir / file))
         except ClientError as e:
             logging.info(f"could not find {file} on {s3_path}")
 
 
@@ -162,32 +269,33 @@
     :param load_tuner: Whether to load the tuner in addition to metadata and results
     :param local_path: Path containing the experiment to load. If not specified,
         ``~/{SYNE_TUNE_FOLDER}/`` is used.
     :param experiment_name: If given, this is used as first directory.
     :return: Result object
     """
     path = experiment_path(tuner_name, local_path)
-    metadata_path = path / "metadata.json"
+    metadata_path = path / ST_METADATA_FILENAME
     if not (metadata_path.exists()) and download_if_not_found:
         logging.info(
             f"experiment {tuner_name} not found locally, trying to get it from s3."
         )
         download_single_experiment(
             tuner_name=tuner_name, experiment_name=experiment_name
         )
     try:
         with open(metadata_path, "r") as f:
             metadata = json.load(f)
     except FileNotFoundError:
         metadata = None
     try:
-        if (path / "results.csv.zip").exists():
-            results = pd.read_csv(path / "results.csv.zip")
+        results_fname = ST_RESULTS_DATAFRAME_FILENAME
+        if (path / results_fname).exists():
+            results = pd.read_csv(path / results_fname)
         else:
-            results = pd.read_csv(path / "results.csv")
+            results = pd.read_csv(path / results_fname[:-4])
     except Exception:
         results = None
     if load_tuner:
         try:
             tuner = Tuner.load(str(path))
         except FileNotFoundError:
             tuner = None
@@ -232,15 +340,15 @@
         experiments.
     :param root: Root path for experiment results. Default is
         ``experiment_path()``
     :return: Dictionary from tuner name to metadata dict
     """
     path_filter = _impute_filter(path_filter)
     res = dict()
-    for metadata_path in root.glob("**/metadata.json"):
+    for metadata_path in root.glob(f"**/{ST_METADATA_FILENAME}"):
         path = metadata_path.parent
         if path_filter(str(path)):
             try:
                 tuner_name = path.name
                 with open(metadata_path, "r") as f:
                     metadata = json.load(f)
                     # we check that the metadata is valid by verifying that is a dict containing Syne Tune time-stamp
@@ -272,15 +380,15 @@
         :func:`experiment_path`
     :param load_tuner: Whether to load the tuner in addition to metadata and results
     :return: List of result objects
     """
     path_filter = _impute_filter(path_filter)
     experiment_filter = _impute_filter(experiment_filter)
     res = []
-    for metadata_path in root.glob("**/metadata.json"):
+    for metadata_path in root.glob(f"**/{ST_METADATA_FILENAME}"):
         path = metadata_path.parent
         tuner_name = path.name
         if path_filter(str(metadata_path)):
             result = load_experiment(
                 tuner_name, load_tuner, local_path=str(path.parent)
             )
             if (
```

### Comparing `syne_tune-0.4.1/syne_tune/num_gpu.py` & `syne_tune-0.5.0/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/baselines.py` & `syne_tune-0.5.0/syne_tune/optimizer/baselines.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     HyperbandScheduler,
     PopulationBasedTraining,
 )
 from syne_tune.optimizer.schedulers.multiobjective import MOASHA
 from syne_tune.optimizer.schedulers.searchers.regularized_evolution import (
     RegularizedEvolution,
 )
-from syne_tune.optimizer.schedulers.searchers.multi_objective_regularized_evolution import (
+from syne_tune.optimizer.schedulers.multiobjective.multi_objective_regularized_evolution import (
     MultiObjectiveRegularizedEvolution,
 )
 from syne_tune.optimizer.schedulers.synchronous import (
     SynchronousGeometricHyperbandScheduler,
     GeometricDifferentialEvolutionHyperbandScheduler,
 )
 from syne_tune.optimizer.schedulers.transfer_learning import (
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/scheduler.py` & `syne_tune-0.5.0/syne_tune/optimizer/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from dataclasses import dataclass
 from typing import Optional, List, Dict, Any, Union
 import logging
 
 from syne_tune.backend.trial_status import Trial
-from syne_tune.config_space import non_constant_hyperparameter_keys, cast_config_values
+from syne_tune.config_space import (
+    non_constant_hyperparameter_keys,
+    cast_config_values,
+    config_space_to_json_dict,
+)
+from syne_tune.util import dump_json_with_numpy
 
 logger = logging.getLogger(__name__)
 
 
 class SchedulerDecision:
     """
     Possible return values of :meth:`TrialScheduler.on_trial_result`, signals the
@@ -272,7 +277,28 @@
             Here, "min" should be the default. For a genuine multi-objective
             scheduler, a list of modes is returned
         """
         if hasattr(self, "mode"):
             return self.mode
         else:
             raise NotImplementedError
+
+    def metadata(self) -> Dict[str, Any]:
+        """
+        :return: Metadata for the scheduler
+        """
+        config_space_json = dump_json_with_numpy(
+            config_space_to_json_dict(self.config_space)
+        )
+        return {
+            "metric_names": self.metric_names(),
+            "metric_mode": self.metric_mode(),
+            "scheduler_name": str(self.__class__.__name__),
+            "config_space": config_space_json,
+        }
+
+    def is_multiobjective_scheduler(self) -> bool:
+        """
+        Return True if a scheduler is multi-objective.
+        """
+        # This is set to False as a default but should be overriden by any classes that implement MO Schedulers
+        return False
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/fifo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import copy
 import logging
 from dataclasses import dataclass
-from typing import Optional, List, Dict, Any
+from typing import Optional, List, Dict, Any, Tuple, Callable
 
 import numpy as np
 
 from syne_tune.backend.trial_status import Trial
 from syne_tune.optimizer.scheduler import SchedulerDecision
 from syne_tune.optimizer.schedulers.fifo import FIFOScheduler
 from syne_tune.optimizer.schedulers.multi_fidelity import MultiFidelitySchedulerMixin
@@ -26,15 +26,24 @@
 )
 from syne_tune.optimizer.schedulers.hyperband_pasha import PASHARungSystem
 from syne_tune.optimizer.schedulers.hyperband_promotion import PromotionRungSystem
 from syne_tune.optimizer.schedulers.hyperband_rush import (
     RUSHPromotionRungSystem,
     RUSHStoppingRungSystem,
 )
-from syne_tune.optimizer.schedulers.hyperband_stopping import StoppingRungSystem
+from syne_tune.optimizer.schedulers.hyperband_stopping import (
+    StoppingRungSystem,
+    PausedTrialsResult,
+)
+from syne_tune.optimizer.schedulers.hyperband_checkpoint_removal import (
+    create_callback_for_checkpoint_removal,
+)
+from syne_tune.optimizer.schedulers.remove_checkpoints import (
+    RemoveCheckpointsSchedulerMixin,
+)
 from syne_tune.optimizer.schedulers.searchers.dyhpo.hyperband_dyhpo import (
     DyHPORungSystem,
     DEFAULT_SH_PROBABILITY,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
     check_and_merge_defaults,
     Integer,
@@ -47,14 +56,16 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bracket_distribution import (
     DefaultHyperbandBracketDistribution,
 )
 from syne_tune.optimizer.schedulers.utils.successive_halving import (
     successive_halving_rung_levels,
 )
+from syne_tune.tuning_status import TuningStatus
+from syne_tune.tuner_callback import TunerCallback
 
 logger = logging.getLogger(__name__)
 
 
 RUNG_SYSTEMS = {
     "stopping": StoppingRungSystem,
     "promotion": PromotionRungSystem,
@@ -76,14 +87,15 @@
     "searcher_data",
     "cost_attr",
     "register_pending_myopic",
     "do_snapshots",
     "rung_system_per_bracket",
     "rung_levels",
     "rung_system_kwargs",
+    "early_checkpoint_removal_kwargs",
 }
 
 _DEFAULT_OPTIONS = {
     "resource_attr": "epoch",
     "grace_period": 1,
     "brackets": 1,
     "type": "stopping",
@@ -106,14 +118,15 @@
     "type": Categorical(tuple(RUNG_SYSTEMS.keys())),
     "searcher_data": Categorical(("rungs", "all", "rungs_and_last")),
     "cost_attr": String(),
     "register_pending_myopic": Boolean(),
     "do_snapshots": Boolean(),
     "rung_system_per_bracket": Boolean(),
     "rung_system_kwargs": Dictionary(),
+    "early_checkpoint_removal_kwargs": Dictionary(),
 }
 
 
 def is_continue_decision(trial_decision: str) -> bool:
     return trial_decision == SchedulerDecision.CONTINUE
 
 
@@ -141,15 +154,17 @@
     def restart(self, time_stamp: float):
         self.time_stamp = time_stamp
         self.reported_result = None
         self.keep_case = False
         self.trial_decision = SchedulerDecision.CONTINUE
 
 
-class HyperbandScheduler(FIFOScheduler, MultiFidelitySchedulerMixin):
+class HyperbandScheduler(
+    FIFOScheduler, MultiFidelitySchedulerMixin, RemoveCheckpointsSchedulerMixin
+):
     r"""Implements different variants of asynchronous Hyperband
 
     See ``type`` for the different variants. One implementation detail is
     when using multiple brackets, task allocation to bracket is done randomly,
     based on a distribution which can be configured.
 
     For definitions of concepts (bracket, rung, milestone), see
@@ -371,14 +386,22 @@
           probability given here, we instead try to promote a trial as if
           ``type == "promotion"``. If no trial can be promoted, we fall back to
           the DyHPO logic. Use this to make DyHPO robust against starting too
           many new trials, because all paused ones score poorly (this happens
           especially at the beginning).
 
     :type rung_system_kwargs: Dict[str, Any], optional
+    :param early_checkpoint_removal_kwargs: If given, speculative early removal
+        of checkpoints is done, see
+        :class:`~syne_tune.callbacks.hyperband_remove_checkpoints_callback.HyperbandRemoveCheckpointsCallback`.
+        The constructor arguments for the ``HyperbandRemoveCheckpointsCallback``
+        must be given here, if they cannot be inferred (key ``max_num_checkpoints``
+        is mandatory). This feature is used only for scheduler types which pause
+        and resume trials.
+    :type early_checkpoint_removal_kwargs: Dict[str, Any], optional
     """
 
     def __init__(self, config_space: Dict[str, Any], **kwargs):
         # Before we can call the superclass constructor, we need to set a few
         # members (see also ``_extend_search_options``).
         # To do this properly, we first check values and impute defaults for
         # ``kwargs``.
@@ -479,14 +502,27 @@
         self._active_trials = dict()
         # _cost_offset:
         # Is used for promotion-based (pause/resume) scheduling if the eval
         # function reports cost values. For a trial which has been paused at
         # least once, this records the sum of costs for reaching its last
         # recent milestone.
         self._cost_offset = dict()
+        self._initialize_early_checkpoint_removal(
+            kwargs.get("early_checkpoint_removal_kwargs")
+        )
+
+    def _initialize_early_checkpoint_removal(
+        self, callback_kwargs: Optional[Dict[str, Any]]
+    ):
+        if callback_kwargs is not None:
+            for name in ["max_num_checkpoints"]:
+                assert (
+                    name in callback_kwargs
+                ), f"early_checkpoint_removal_kwargs must contain '{name}' entry"
+        self._early_checkpoint_removal_kwargs = callback_kwargs
 
     def does_pause_resume(self) -> bool:
         """
         :return: Is this variant doing pause and resume scheduling, in the
             sense that trials can be paused and resumed later?
         """
         return HyperbandBracketManager.does_pause_resume(self.scheduler_type)
@@ -974,14 +1010,33 @@
             resource = int(result[self._resource_attr])
             if resource > largest_update_resource:
                 super().on_trial_complete(trial, result)
         # Remove pending evaluations, in case there are still some
         self.searcher.cleanup_pending(trial_id)
         self._cleanup_trial(trial_id, trial_decision=SchedulerDecision.STOP)
 
+    def callback_for_checkpoint_removal(
+        self, stop_criterion: Callable[[TuningStatus], bool]
+    ) -> Optional[TunerCallback]:
+        if (
+            self._early_checkpoint_removal_kwargs is None
+            or not self.terminator.support_early_checkpoint_removal()
+        ):
+            return None
+        else:
+            callback_kwargs = dict(
+                self._early_checkpoint_removal_kwargs,
+                metric=self.metric,
+                resource_attr=self._resource_attr,
+                mode=self.mode,
+            )
+            return create_callback_for_checkpoint_removal(
+                callback_kwargs, stop_criterion=stop_criterion
+            )
+
 
 class HyperbandBracketManager:
     """
     Maintains rung level systems for range of brackets. Differences depending
     on ``scheduler_type`` manifest themselves mostly at the level of the rung
     level system itself.
 
@@ -1200,7 +1255,36 @@
         if k not in extra_kwargs:
             extra_kwargs[k] = rung_sys.get_first_milestone(skip_rungs)
         return trial_id, extra_kwargs
 
     def snapshot_rungs(self, bracket_id):
         rung_sys, skip_rungs = self._get_rung_system_for_bracket_id(bracket_id)
         return rung_sys.snapshot_rungs(skip_rungs)
+
+    def paused_trials(self, resource: Optional[int] = None) -> PausedTrialsResult:
+        """
+        Only for pause and resume schedulers (:meth:`does_pause_resume` returns
+        ``True``), where trials can be paused at certain rung levels only.
+        If ``resource`` is not given, returns list of all paused trials
+        ``(trial_id, rank, metric_val, level)``, where ``level`` is
+        the rung level, and ``rank`` is the rank of the trial in the rung
+        (0 for the best metric value). If ``resource`` is given, only the
+        paused trials in the rung of this level are returned.
+
+        :param resource: If given, paused trials of only this rung level are
+            returned. Otherwise, all paused trials are returned
+        :return: See above
+        """
+        return [
+            entry for rs in self._rung_systems for entry in rs.paused_trials(resource)
+        ]
+
+    def information_for_rungs(self) -> List[Tuple[int, int, float]]:
+        """
+        :return: List of ``(resource, num_entries, prom_quant)``, where
+            ``resource`` is a rung level, ``num_entries`` the number of entries
+            in the rung, and ``prom_quant`` the promotion quantile
+        """
+        return self._rung_systems[0].information_for_rungs()
+
+    def support_early_checkpoint_removal(self) -> bool:
+        return self._rung_systems[0].support_early_checkpoint_removal()
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,43 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Tuple, Dict, Any
 import logging
 
-from syne_tune.optimizer.schedulers.hyperband_promotion import PromotionRungSystem
+from syne_tune.optimizer.schedulers.hyperband_stopping import Rung
+from syne_tune.optimizer.schedulers.hyperband_promotion import (
+    PromotionRungEntry,
+    PromotionRungSystem,
+)
 
 logger = logging.getLogger(__name__)
 
 
+class CostPromotionRungEntry(PromotionRungEntry):
+    """
+    Appends ``cost_val`` to the superclass. This is the cost value
+    :math:`c(x, r)` recorded for the trial at the resource level.
+    """
+
+    def __init__(
+        self,
+        trial_id: str,
+        metric_val: float,
+        cost_val: float,
+        was_promoted: bool = False,
+    ):
+        super().__init__(trial_id, metric_val, was_promoted)
+        self.cost_val = cost_val
+
+
 class CostPromotionRungSystem(PromotionRungSystem):
     """
     Cost-aware extension of promotion-based asynchronous Hyperband (ASHA).
 
     This code is equivalent with base
     :class:`~syne_tune.optimizer.schedulers.hyperband_promotion.PromotionRungSystem`,
     except the "promotable" condition in :meth:`_find_promotable_trial` is
@@ -66,60 +87,38 @@
         cost_attr: str,
         max_t: int,
     ):
         super().__init__(
             rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
         )
         self._cost_attr = cost_attr
-        # Note: The data entry in ``_rungs`` is now a dict mapping trial_id to
-        # ``(metric_value, cost_value, was_promoted)``, where metric_value is
-        # :math:`m(x, r)`, cost value is :math:`c(x, r)`.
-
-    def _find_promotable_trial(
-        self, recorded: Dict[str, Any], prom_quant: float, resource: int
-    ) -> Optional[str]:
+
+    def _find_promotable_trial(self, rung: Rung) -> Optional[Tuple[str, int]]:
         """
-        Check whether any not yet promoted entry in ``recorded`` is
-        promotable (see header comment). If there are several such, the one
-        with the best value is chosen.
-
-        :param recorded: Dict to scan
-        :param prom_quant: Quantile for promotion
-        :param resource: Amount of resources spent on the rung.
-        :return: ``trial_id`` if found, otherwise ``None``
+        The promotability condition depends on the cost values (see header
+        comment).
         """
-        ret_id = None
-        if len(recorded) > 1:
-            sign = 2 * (self._mode == "min") - 1
-            # Sort best-first
-            sorted_record = sorted(
-                ((k,) + v for k, v in recorded.items()), key=lambda x: x[1] * sign
-            )
-            cost_threshold = sum(x[2] for x in sorted_record) * prom_quant
+        result = None
+        if len(rung) > 1:
+            cost_threshold = sum(x.cost_val for x in rung.data) * rung.prom_quant
             sum_costs = 0
-            # DEBUG
-            log_msg = (
-                f"q = {prom_quant:.2f}, threshold = {cost_threshold:.2f}\n"
-                + ", ".join(
-                    [
-                        f"{x[0]}:{x[2]:.2f}({x[1]:.3f},{int(x[3])})"
-                        for x in sorted_record
-                    ]
-                )
-            )
-            for id, _, cost, was_promoted in sorted_record:
-                sum_costs += cost
+            # ``rung.data`` is ordered, with best metric value first
+            for pos, entry in enumerate(rung.data):
+                sum_costs += entry.cost_val
                 if sum_costs > cost_threshold:
-                    log_msg += "\nNothing to promote"
-                    break
-                if not was_promoted:
-                    log_msg += f"\nPromote {id}: sum_costs = {sum_costs:.2f}"
-                    ret_id = id
+                    break  # Nothing to promote
+                if self._is_promotable_trial(entry, rung.level):
+                    result = (entry.trial_id, pos)
                     break
-            logger.debug(log_msg)  # DEBUG
-        return ret_id
+        return result
 
-    def _register_metrics_at_rung_level(self, trial_id, result, recorded):
-        metric_value = result[self._metric]
-        cost_value = result[self._cost_attr]
-        assert trial_id not in recorded  # Sanity check
-        recorded[trial_id] = (metric_value, cost_value, False)
+    def _register_metrics_at_rung_level(
+        self, trial_id: str, result: Dict[str, Any], rung: Rung
+    ):
+        assert trial_id not in rung  # Sanity check
+        rung.add(
+            CostPromotionRungEntry(
+                trial_id=trial_id,
+                metric_val=result[self._metric],
+                cost_val=result[self._cost_attr],
+            )
+        )
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,27 +77,29 @@
         """
         rankings = []
         # be careful, self._rungs is ordered with the highest resources level in the beginning
         for rung in [
             self._rungs[-self.current_rung_idx],
             self._rungs[-self.current_rung_idx + 1],
         ]:
-            if rung.data != {}:
-                trial_ids = rung.data.keys()
-                values = []
-                for trial_id in trial_ids:
-                    values.append(rung.data[trial_id][0])
-                # order specifies where the value should be placed in the sorted list
-                values_order = np.array(values).argsort()
-                # calling argsort on the order will give us the ranking
-                values_ranking = values_order.argsort()
+            if rung:
+                # Note that entries in ``rung.data`` are already sorted
+                trial_ids, values = zip(
+                    *[(x.trial_id, x.metric_val) for x in rung.data]
+                )
+                # Note: To retain the exact logic of older code (which used
+                # ``numpy.argsort``, we assume the ranks for increasing metric
+                # values, which is the opposite ordering to ``rung.data`` if
+                # ``self._mode == "max"``
+                if self._mode == "min":
+                    values_ranking = list(range(len(trial_ids)))
+                else:
+                    values_ranking = list(range(len(trial_ids) - 1, -1, -1))
                 ranking = list(zip(trial_ids, values_ranking, values))
-
                 rankings.append(ranking)
-
         return rankings
 
     def _get_sorted_top_rungs(self, rankings):
         """
         Sort the configurations in the top rung and the previous rung.
         Filter out the configurations from the previous rung that
         are not in the top rung.
@@ -107,19 +109,15 @@
         """
         # filter only the relevant configurations from the earlier rung
         top_rung_keys = set([e[0] for e in rankings[0]])
         corresponding_previous_rung_trials = filter(
             lambda e: e[0] in top_rung_keys, rankings[1]
         )
         # if we try to maximize the objective, we need to reverse the ranking
-        if self._mode == "max":
-            reverse = True
-        else:
-            reverse = False
-
+        reverse = self._mode == "max"
         sorted_top_rung = sorted(rankings[0], key=lambda e: e[1], reverse=reverse)
         sorted_previous_rung = sorted(
             corresponding_previous_rung_trials, key=lambda e: e[1], reverse=reverse
         )
         return sorted_top_rung, sorted_previous_rung
 
     def _evaluate_soft_ranking(self, sorted_top_rung, sorted_previous_rung) -> bool:
@@ -223,26 +221,23 @@
 
         if len(noisy_cfg_distances) > 0:
             self.epsilon = np.percentile(noisy_cfg_distances, 90)
             if str(self.epsilon) == "nan":
                 raise ValueError("Epsilon became nan")
 
     def _update_per_epoch_results(self, trial_id, result):
+        resource = result[self._resource_attr]
+        metric_val = result[self._metric]
         if trial_id not in self.per_epoch_results:
-            self.per_epoch_results[trial_id] = {}
-        self.per_epoch_results[trial_id][result[self._resource_attr]] = result[
-            self._metric
-        ]
-
-        if result[self._resource_attr] not in self.epoch_to_trials:
-            self.epoch_to_trials[result[self._resource_attr]] = set()
-        self.epoch_to_trials[result[self._resource_attr]].add(trial_id)
-
-        if result[self._resource_attr] > self.current_max_epoch:
-            self.current_max_epoch = result[self._resource_attr]
+            self.per_epoch_results[trial_id] = dict()
+        self.per_epoch_results[trial_id][resource] = metric_val
+        if resource not in self.epoch_to_trials:
+            self.epoch_to_trials[resource] = set()
+        self.epoch_to_trials[resource].add(trial_id)
+        self.current_max_epoch = max(self.current_max_epoch, resource)
 
     def _decide_resource_increase(self, rankings) -> bool:
         """
         Decide if to increase the resources given the current rankings.
         Currently we look at the rankings and if elements in the first list
         have the same order also in the second list, we keep the current resource
         budget. If the rankings are different, we will increase the budget.
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,272 +6,240 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional, List, Dict, Any
+from typing import List, Dict, Any, Tuple
+from numpy.random import RandomState
+import logging
+from collections import Counter
 
-from syne_tune.optimizer.schedulers.hyperband_stopping import (
-    quantile_cutoff,
-    RungSystem,
+from syne_tune.optimizer.schedulers.hyperband_promotion import (
+    PromotionRungSystem,
+)
+from syne_tune.optimizer.schedulers.searchers.dyhpo.dyhpo_searcher import (
+    DynamicHPOSearcher,
+    KEY_NEW_CONFIGURATION,
 )
 
+logger = logging.getLogger(__name__)
 
-class PromotionRungSystem(RungSystem):
-    """
-    Implements both the promotion and stopping logic for an asynchronous
-    variant of Hyperband, known as ASHA:
 
-        | Li etal
-        | A System for Massively Parallel Hyperparameter Tuning
-        | https://arxiv.org/abs/1810.05934
-
-    In ASHA, configs sit paused at milestones (rung levels) until they get
-    promoted, which means that a free task picks up their evaluation until
-    the next milestone.
-
-    The rule to decide whether a paused trial is promoted (or remains
-    paused) is the same as in
-    :class:`~syne_tune.optimizer.schedulers.hyperband_stopping.StoppingRungSystem`,
-    except that *continues* becomes *gets promoted*. If several paused trials
-    in a rung can be promoted, the one with the best metric value is chosen.
-
-    Note: Say that an evaluation is resumed from level ``resume_from``. If the
-    trial evaluation function does not implement pause & resume, it needs to
-    start training from scratch, in which case metrics are reported for every
-    epoch, also those ``< resume_from``. At least for some modes of fitting the
-    searcher model to data, this would lead to duplicate target values for the
-    same extended config :math:`(x, r)`, which we want to avoid. The solution is to
-    maintain ``resume_from`` in the data for the terminator (see :attr:`_running`).
-    Given this, we can report in :meth:`on_task_report` that the current metric
-    data should not be used for the searcher model (``ignore_data = True``), namely
-    as long as the evaluation has not yet gone beyond level ``resume_from``.
+DEFAULT_SH_PROBABILITY = 0.25
+
+
+class ScheduleDecision:
+    PROMOTE_SH = 0
+    PROMOTE_DYHPO = 1
+    START_DYHPO = 2
+
+
+_SUMMARY_SCHEDULE_RECORDS = [
+    ("promoted_by_sh", ScheduleDecision.PROMOTE_SH),
+    ("promoted_by_dyhpo", ScheduleDecision.PROMOTE_DYHPO),
+    ("started_by_dyhpo", ScheduleDecision.START_DYHPO),
+]
+
+
+class DyHPORungSystem(PromotionRungSystem):
+    """
+    Implements the logic which decides which paused trial to promote to the
+    next resource level, or alternatively which configuration to start as a
+    new trial, proposed in:
+
+        | Wistuba, M. and Kadra, A. and Grabocka, J.
+        | Dynamic and Efficient Gray-Box Hyperparameter Optimization for Deep Learning
+        | https://arxiv.org/abs/2202.09774
+
+    We do promotion-based scheduling, as in
+    :class:`~syne_tune.optimizer.schedulers.hyperband_promotion.PromotionRungSystem`.
+    In fact, we run the successive halving rule in :meth:`on_task_schedule` with
+    probability ``probability_sh``, and the DyHPO logic otherwise, or if the SH
+    rule does not promote a trial. This mechanism (not contained in the paper)
+    ensures that trials are promoted eventually, even if DyHPO only starts new
+    trials.
+
+    Since :class:`~syne_tune.optimizer.schedulers.HyperbandScheduler` was designed
+    for promotion decisions to be separate from decisions about new configs, the
+    overall workflow is a bit tricky:
+
+    * In :meth:`FIFOScheduler._suggest`, we first call
+      :code:`promote_trial_id, extra_kwargs = self._promote_trial()`. If
+      ``promote_trial_id != None``, this trial is promoted. Otherwise, we call
+      :code:`config = self.searcher.get_config(**extra_kwargs, trial_id=trial_id)`
+      and start a new trial with this config. In most cases, :meth:`_promote_trial`
+      makes a promotion decision without using the searcher.
+    * Here, we use the fact that information can be passed from
+      :meth:`_promote_trial` to ``self.searcher.get_config`` via ``extra_kwargs``.
+      Namely, :meth:``HyperbandScheduler._promote_trial` calls
+      :meth:`on_task_schedule` here, which calls
+      :meth:`~syne_tune.optimizer.schedulers.searchers.dyhpo.DynamicHPOSearcher.score_paused_trials_and_new_configs`,
+      where everything happens.
+    * First, all paused trials are scored w.r.t. the value of running them for one
+      more unit of resource. Also, a number of random configs are scored w.r.t.
+      the value of running them to the minimum resource.
+    * If the winning config is from a paused trial, this is resumed. If the
+      winning config is a new one, :meth:`on_task_schedule` returns this
+      config using a special key :const:`KEY_NEW_CONFIGURATION`. This dict
+      becomes part of ``extra_kwargs`` and is passed to ``self.searcher.get_config``
+    * :meth:`~syne_tune.optimizer.schedulers.searchers.dyhpo.DynamicHPOSearcher.get_config`
+      is trivial. It obtains an argument of name :const:`KEY_NEW_CONFIGURATION`
+      returns its value, which is the winning config to be started as new trial
+
+    We can ignore ``rung_levels`` and ``promote_quantiles``, they are not used.
+    For each trial, we only need to maintain the resource level at which it is
+    paused.
     """
 
     def __init__(
         self,
         rung_levels: List[int],
         promote_quantiles: List[float],
         metric: str,
         mode: str,
         resource_attr: str,
         max_t: int,
+        searcher: DynamicHPOSearcher,
+        probability_sh: bool,
+        random_state: RandomState,
     ):
+        assert len(rung_levels) > 0, "rung_levels must not be empty"
+        assert isinstance(
+            searcher, DynamicHPOSearcher
+        ), "searcher must be of type DynamicHPOSearcher. Use searcher='dyhpo'"
+        assert (
+            0 <= probability_sh < 1
+        ), f"probability_sh = {probability_sh}, must be in [0, 1)"
         super().__init__(
             rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
         )
-        # The data entry in ``_rungs`` is a dict mapping trial_id to
-        # (metric_value, was_promoted)
-        # ``_running`` maps ``trial_id ``to ``dict(milestone, resume_from)``.
-        # The tasks runs trial ``trial_id`` until resource reaches milestone.
-        # The ``resume_from`` field can be None. If not, the task is running a
-        # trial which has been resumed from rung level ``resume_from.`` This info
-        # is required for ``on_task_report`` to properly report ``ignore_data``.
-        self._running = dict()
-
-    def _cutoff(self, recorded: Dict[str, Any], prom_quant: float):
-        values = [x[0] for x in recorded.values()]
-        return quantile_cutoff(values, prom_quant, self._mode)
-
-    def _find_promotable_trial(
-        self, recorded: Dict[str, Any], prom_quant: float, resource: int
-    ) -> Optional[str]:
-        """
-        Check whether any not yet promoted entry in ``recorded`` is
-        promotable, i.e. its value is better or equal to the cutoff
-        based on ``prom_quant``. If there are several such, the one with the
-        best value is chosen.
-
-        :param recorded: Dict to scan
-        :param prom_quant: Quantile for promotion
-        :param resource: Resource level of rung (i.e., amount of resource
-            spent by trials at this rung)
-        :return: trial_id if found, otherwise None
-        """
-        ret_id = None
-        # Code is written for 'max' mode. For 'min', we just negate all
-        # criterion values
-        sign = 1 - 2 * (self._mode == "min")
-        cutoff = self._cutoff(recorded, prom_quant)
-        if cutoff is not None:
-            # Best id among trials paused at this rung (i.e., not yet promoted)
-            trial_id, val = max(
-                (
-                    (k, v[0])
-                    for k, v in recorded.items()
-                    if self._is_promotable_trial(k, v[0], not v[1], resource)
-                ),
-                key=lambda x: sign * x[1],
-                default=(None, 0.0),
-            )
-            if trial_id is not None and sign * (val - cutoff) >= 0:
-                ret_id = trial_id
-        return ret_id
-
-    def _is_promotable_trial(
-        self, trial_id: str, metric_value: float, is_paused: bool, resource: int
-    ) -> bool:
-        """
-        Checks whether trial in rung level is promotable in principle, used
-        as filter in ``_find_promotable_trial``. Can be used in subclasses to
-        sharpen the condition for promotion.
-
-        :param trial_id: ID of trial
-        :param metric_value: Value of target metric
-        :param is_paused: Is trial paused right now?
-        :param resource: Resource level the trial has just reported at
-        """
-        return is_paused
+        self._check_rung_levels(rung_levels)
+        self._searcher = searcher
+        self._min_resource = rung_levels[0]
+        self._probability_sh = probability_sh
+        self._random_state = random_state
+        # Maps rung level to the one below
+        self._previous_rung_level = dict(zip(rung_levels[1:] + [max_t], rung_levels))
+        # Keeps a record of outcomes of :meth:`on_task_schedule` calls. Entries
+        # are ``(trial_id, decision, milestone)``, where ``decision`` is
+        # constant from :class:`ScheduleDecision`, and ``milestone`` is the
+        # rung level which the trial reaches next
+        self._schedule_records = []
 
     @staticmethod
-    def _mark_as_promoted(recorded: Dict[str, Any], trial_id: str):
-        curr_val = recorded[trial_id]
-        assert not curr_val[-1]  # Sanity check
-        recorded[trial_id] = curr_val[:-1] + (True,)
+    def _check_rung_levels(rung_levels: List[int]):
+        if len(rung_levels) > 1:
+            rmin = rung_levels[0]
+            step = rung_levels[1] - rmin
+            should_be = list(range(rmin, rung_levels[-1] + 1, step))
+            if rmin != step or rung_levels != should_be:
+                logger.warning(
+                    "DyHPO should be run with linearly spaced rung levels, in "
+                    "that reduction_factor is not used, and grace_period == "
+                    "rung_increment, bracket == 1. Running with rung_levels = "
+                    f"{rung_levels} is not recommended"
+                )
 
-    def _effective_max_t(self):
+    def _paused_trials_and_milestones(self) -> List[Tuple[str, int, int]]:
         """
-        The following method is used in on_task_schedule to control the maximum
-        amount of resources allocated to a single configuration during the
-        optimization. For ASHA it's just a constant value.
+        Return list of all trials which are paused. Entries are
+        ``(trial_id, pos, resource)``, where ``pos`` is the position of the trial
+        in its rung, and ``resource`` is the next rung level the trial reaches
+        after being resumed.
+
+        :return: See above
         """
-        return self._max_t
+        paused_trials = []
+        next_level = self._max_t
+        for rung in self._rungs:
+            level = rung.level
+            paused_trials.extend(
+                (entry.trial_id, pos, next_level)
+                for pos, entry in enumerate(rung.data)
+                if self._is_promotable_trial(entry, level)
+            )
+            next_level = level
+        return paused_trials
 
     def on_task_schedule(self, new_trial_id: str) -> Dict[str, Any]:
         """
-        Used to implement
-        :meth:`~syne_tune.optimizer.schedulers.HyperbandScheduler._promote_trial`.
-        Searches through rungs to find a trial which can be promoted. If one is
-        found, we return the ``trial_id`` and other info (current milestone,
-        milestone to be promoted to). We also mark the trial as being promoted
-        at the rung level it sits right now.
-        """
-        trial_id = None
-        next_milestone = self._max_t
-        milestone = None
-        recorded = None
-        for rung in self._rungs:
-            _milestone = rung.level
-            prom_quant = rung.prom_quant
-            _recorded = rung.data
-            if _milestone < self._effective_max_t():
-                trial_id = self._find_promotable_trial(
-                    _recorded, prom_quant, rung.level
+        The main decision making happens here. We collect ``(trial_id, resource)``
+        for all paused trials and call ``searcher``. The searcher scores all
+        these trials along with a certain number of randomly drawn new
+        configurations.
+
+        If one of the paused trials has the best score, we return its ``trial_id``
+        along with extra information, so it gets promoted.
+        If one of the new configurations has the best score, we return this
+        configuration. In this case, a new trial is started with this configuration.
+
+        Note: For this scheduler type, ``kwargs`` must contain the trial ID of
+        the new trial to be started, in case none can be promoted.
+        """
+        if self._random_state.rand() <= self._probability_sh:
+            # Try to promote trial based on successive halving logic
+            result = super().on_task_schedule(new_trial_id)
+            if result.get("trial_id") is not None:
+                self._schedule_records.append(
+                    (
+                        result["trial_id"],
+                        ScheduleDecision.PROMOTE_SH,
+                        result["milestone"],
+                    )
                 )
-                if trial_id is not None:
-                    recorded = _recorded
-                    milestone = _milestone
-                    break
-            next_milestone = _milestone
-        ret_dict = dict()
+                return result
+        # Follow DyHPO logic
+        paused_trials = self._paused_trials_and_milestones()
+        assert new_trial_id is not None, (
+            "Internal error: kwargs must contain 'trial_id', the ID for a new "
+            "trial to be started if no paused one is resumed. Make sure to "
+            "pass this to the _promote_trial method when calling it in "
+            "_suggest"
+        )
+        result = self._searcher.score_paused_trials_and_new_configs(
+            paused_trials,
+            min_resource=self._min_resource,
+            new_trial_id=new_trial_id,
+        )
+        trial_id = result.get("trial_id")
         if trial_id is not None:
-            self._mark_as_promoted(recorded, trial_id)
+            # Trial is to be promoted
+            pos = result["pos"]  # Position of trial in its rung
+            milestone = next(r for i, _, r in paused_trials if i == trial_id)
+            resume_from = self._previous_rung_level[milestone]
+            rung = next(rung for rung in self._rungs if rung.level == resume_from)
+            self._mark_as_promoted(rung, pos, trial_id=trial_id)
             ret_dict = {
                 "trial_id": trial_id,
-                "resume_from": milestone,
-                "milestone": next_milestone,
+                "resume_from": resume_from,
+                "milestone": milestone,
             }
+            self._schedule_records.append(
+                (trial_id, ScheduleDecision.PROMOTE_DYHPO, milestone)
+            )
+        else:
+            # New trial is to be started
+            ret_dict = {KEY_NEW_CONFIGURATION: result["config"]}
+            self._schedule_records.append(
+                (new_trial_id, ScheduleDecision.START_DYHPO, self._min_resource)
+            )
         return ret_dict
 
-    def on_task_add(self, trial_id: str, skip_rungs: int, **kwargs):
-        """
-        Called when new task is started. Depending on ``kwargs["new_config"]``,
-        this could start an evaluation (``True``) or promote an existing config
-        to the next milestone (``False``). In the latter case, ``kwargs`` contains
-        additional information about the promotion (in "milestone",
-        "resume_from").
-
-        :param trial_id: ID of trial to be started
-        :param skip_rungs: This number of the smallest rung levels are not
-            considered milestones for this task
-        :param kwargs: Additional arguments
-        """
-        new_config = kwargs.get("new_config", True)
-        if new_config:
-            # New trial
-            milestone = self.get_first_milestone(skip_rungs)
-            resume_from = None
-        else:
-            # Existing trial is resumed
-            # Note that self._rungs has already been updated in
-            # on_task_schedule
-            milestone = kwargs["milestone"]
-            resume_from = kwargs["resume_from"]
-            assert resume_from < milestone  # Sanity check
-        self._running[trial_id] = {"milestone": milestone, "resume_from": resume_from}
+    @property
+    def schedule_records(self) -> List[Tuple[str, int, int]]:
+        return self._schedule_records
 
-    def _register_metrics_at_rung_level(
-        self, trial_id: str, result: Dict[str, Any], recorded: Dict[str, Any]
-    ):
-        metric_value = result[self._metric]
-        assert trial_id not in recorded  # Sanity check
-        recorded[trial_id] = (metric_value, False)
-
-    def on_task_report(
-        self, trial_id: str, result: Dict[str, Any], skip_rungs: int
-    ) -> Dict[str, Any]:
+    @staticmethod
+    def summary_schedule_keys() -> List[str]:
+        return [key for key, _ in _SUMMARY_SCHEDULE_RECORDS]
+
+    def summary_schedule_records(self) -> Dict[str, Any]:
+        histogram = Counter([x[1] for x in self._schedule_records])
+        return {name: histogram[value] for name, value in _SUMMARY_SCHEDULE_RECORDS}
+
+    def support_early_checkpoint_removal(self) -> bool:
         """
-        Decision on whether task may continue (``task_continues=True``), or
-        should be paused (``task_continues=False``).
-        ``milestone_reached`` is a flag whether resource coincides with a
-        milestone.
-        For this scheduler, we have that
-
-            ``task_continues == not milestone_reached``,
-
-        since a trial is always paused at a milestone.
-
-        ``ignore_data`` is True if a result is received from a resumed trial
-        at a level ``<= resume_from``. This happens if checkpointing is not
-        implemented (or not used), because resumed trials are started from
-        scratch then. These metric values should in general be ignored.
-
-        :param trial_id: ID of trial which reported results
-        :param result: Reported metrics
-        :param skip_rungs: This number of smallest rung levels are not
-            considered milestones for this task
-        :return: ``dict(task_continues, milestone_reached, next_milestone,
-            ignore_data)``
+        Early checkpoint removal currently not supported for DyHPO
         """
-        resource = result[self._resource_attr]
-        milestone_reached = False
-        next_milestone = None
-        milestone = self._running[trial_id]["milestone"]
-        resume_from = self._running[trial_id]["resume_from"]
-        ignore_data = (resume_from is not None) and (resource <= resume_from)
-        if resource >= milestone:
-            assert resource == milestone, (
-                f"trial_id {trial_id}: resource = {resource} > {milestone} "
-                + "milestone. Make sure to report time attributes covering "
-                + "all milestones"
-            )
-            milestone_reached = True
-            try:
-                rung_pos = next(
-                    i for i, v in enumerate(self._rungs) if v.level == milestone
-                )
-                # Register metric_value at rung level (as not promoted)
-                recorded = self._rungs[rung_pos].data
-                self._register_metrics_at_rung_level(trial_id, result, recorded)
-                next_milestone = (
-                    self._rungs[rung_pos - 1].level if rung_pos > 0 else self._max_t
-                )
-            except StopIteration:
-                # ``milestone`` not a rung level. This can happen, in particular
-                # if ``milestone == self._max_t``
-                pass
-        return {
-            "task_continues": not milestone_reached,
-            "milestone_reached": milestone_reached,
-            "next_milestone": next_milestone,
-            "ignore_data": ignore_data,
-        }
-
-    def on_task_remove(self, trial_id: str):
-        if trial_id in self._running:
-            del self._running[trial_id]
-
-    @staticmethod
-    def does_pause_resume() -> bool:
-        return True
+        return False
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import logging
-from typing import Optional, List, Dict, Any
+from typing import Optional, List
 
-from syne_tune.optimizer.schedulers.hyperband_promotion import PromotionRungSystem
-from syne_tune.optimizer.schedulers.hyperband_stopping import StoppingRungSystem
+from syne_tune.optimizer.schedulers.hyperband_promotion import (
+    PromotionRungEntry,
+    PromotionRungSystem,
+)
+from syne_tune.optimizer.schedulers.hyperband_stopping import (
+    Rung,
+    StoppingRungSystem,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class RUSHDecider:
     """
     Implements the additional decision logic according to the RUSH algorithm.
@@ -44,24 +50,24 @@
         self._num_threshold_candidates = num_threshold_candidates
         self._mode = mode
         self._thresholds = (
             dict()
         )  # thresholds at different resource levels that must be met
 
     def task_continues(
-        self, task_continues: bool, trial_id: str, metric_value: float, resource: int
+        self, task_continues: bool, trial_id: str, metric_val: float, resource: int
     ) -> bool:
         if not task_continues:
             return False
         if self._is_in_points_to_evaluate(trial_id):
             self._thresholds[resource] = self._return_better(
-                self._thresholds.get(resource), metric_value
+                self._thresholds.get(resource), metric_val
             )
             return True
-        return self._meets_threshold(metric_value, resource)
+        return self._meets_threshold(metric_val, resource)
 
     def _is_in_points_to_evaluate(self, trial_id: str) -> bool:
         return int(trial_id) < self._num_threshold_candidates
 
     def _return_better(self, val1: Optional[float], val2: Optional[float]) -> float:
         if self._mode == "min":
             better_val = min(
@@ -71,18 +77,18 @@
         else:
             better_val = max(
                 float("-inf") if val1 is None else val1,
                 float("-inf") if val2 is None else val2,
             )
         return better_val
 
-    def _meets_threshold(self, metric_value: float, resource: int) -> bool:
+    def _meets_threshold(self, metric_val: float, resource: int) -> bool:
         return (
-            self._return_better(self._thresholds.get(resource), metric_value)
-            == metric_value
+            self._return_better(self._thresholds.get(resource), metric_val)
+            == metric_val
         )
 
 
 class RUSHStoppingRungSystem(StoppingRungSystem):
     """
     Implementation for RUSH algorithm, stopping variant.
 
@@ -105,25 +111,21 @@
         super().__init__(
             rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
         )
         self._decider = RUSHDecider(num_threshold_candidates, mode)
 
     def _task_continues(
         self,
-        metric_value: float,
-        recorded: Dict[str, Any],
-        prom_quant: float,
         trial_id: str,
-        resource: int,
+        metric_val: float,
+        rung: Rung,
     ) -> bool:
-        task_continues = super()._task_continues(
-            metric_value, recorded, prom_quant, trial_id, resource
-        )
+        task_continues = super()._task_continues(trial_id, metric_val, rung)
         return self._decider.task_continues(
-            task_continues, trial_id, metric_value, resource
+            task_continues, trial_id, metric_val, rung.level
         )
 
 
 class RUSHPromotionRungSystem(PromotionRungSystem):
     """
     Implementation for RUSH algorithm, promotion variant.
 
@@ -144,16 +146,12 @@
         num_threshold_candidates: int,
     ):
         super().__init__(
             rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
         )
         self._decider = RUSHDecider(num_threshold_candidates, mode)
 
-    def _is_promotable_trial(
-        self, trial_id: str, metric_value: float, is_paused: bool, resource: int
-    ) -> bool:
-        task_continues = super()._is_promotable_trial(
-            trial_id, metric_value, is_paused, resource
-        )
+    def _is_promotable_trial(self, entry: PromotionRungEntry, resource: int) -> bool:
+        task_continues = super()._is_promotable_trial(entry, resource)
         return self._decider.task_continues(
-            task_continues, trial_id, metric_value, resource
+            task_continues, entry.trial_id, entry.metric_val, resource
         )
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,289 +6,281 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-import logging
-from dataclasses import dataclass
-from typing import List, Tuple, Dict, Any
+from typing import Optional, List, Dict, Any, Tuple
 
-import numpy as np
+from syne_tune.optimizer.schedulers.hyperband_stopping import (
+    RungEntry,
+    Rung,
+    RungSystem,
+    PausedTrialsResult,
+)
 
-logger = logging.getLogger(__name__)
 
-
-@dataclass
-class RungEntry:
+class PromotionRungEntry(RungEntry):
     """
-    :param level: Rung level :math:`r_j`
-    :param prom_quant: romotion quantile :math:`q_j`
-    :param data: Data of all previous jobs reaching the level
+    Appends ``was_promoted`` to the superclass. This is ``True`` iff the trial
+    has been promoted from this rung. Otherwise, the trial is paused at this rung.
     """
 
-    level: int
-    prom_quant: float
-    data: Dict[str, Any]
-
-
-def quantile_cutoff(values, prom_quant, mode):
-    if len(values) < 2:
-        # Cannot determine cutoff from one value
-        return None
-    q = prom_quant if mode == "min" else (1 - prom_quant)
-    return np.quantile(values, q)
+    def __init__(self, trial_id: str, metric_val: float, was_promoted: bool = False):
+        super().__init__(trial_id, metric_val)
+        self.was_promoted = was_promoted
 
 
-class RungSystem:
+class PromotionRungSystem(RungSystem):
     """
-    Terminology: Trials emit results at certain resource levels (e.g., epoch
-    numbers). Some resource levels are rung levels, this is where scheduling
-    decisions (stop, continue or pause, resume) are taken. For a running trial,
-    the next rung level (or ``max_t``) it will reach is called its next
-    milestone.
-
-    Note that ``rung_levels``, ``promote_quantiles`` can be empty. All
-    entries of ``rung_levels`` are smaller than ``max_t``.
-
-    :param rung_levels: List of rung levels (positive int, increasing)
-    :param promote_quantiles: List of promotion quantiles at each rung level
-    :param metric: Name of metric to optimize
-    :param mode: "min" or "max"
-    :param resource_attr: Name of resource attribute
-    :param max_t: Largest resource level
+    Implements the promotion logic for an asynchronous variant of Hyperband,
+    known as ASHA:
+
+        | Li etal
+        | A System for Massively Parallel Hyperparameter Tuning
+        | https://arxiv.org/abs/1810.05934
+
+    In ASHA, configs sit paused at milestones (rung levels) until they get
+    promoted, which means that a free task picks up their evaluation until
+    the next milestone.
+
+    The rule to decide whether a paused trial is promoted (or remains
+    paused) is the same as in
+    :class:`~syne_tune.optimizer.schedulers.hyperband_stopping.StoppingRungSystem`,
+    except that *continues* becomes *gets promoted*. If several paused trials
+    in a rung can be promoted, the one with the best metric value is chosen.
+
+    Note: Say that an evaluation is resumed from level ``resume_from``. If the
+    trial evaluation function does not implement pause & resume, it needs to
+    start training from scratch, in which case metrics are reported for every
+    epoch, also those ``< resume_from``. At least for some modes of fitting the
+    searcher model to data, this would lead to duplicate target values for the
+    same extended config :math:`(x, r)`, which we want to avoid. The solution is to
+    maintain ``resume_from`` in the data for the terminator (see :attr:`_running`).
+    Given this, we can report in :meth:`on_task_report` that the current metric
+    data should not be used for the searcher model (``ignore_data = True``), namely
+    as long as the evaluation has not yet gone beyond level ``resume_from``.
     """
 
     def __init__(
         self,
         rung_levels: List[int],
         promote_quantiles: List[float],
         metric: str,
         mode: str,
         resource_attr: str,
         max_t: int,
     ):
-        self.num_rungs = len(rung_levels)
-        assert len(promote_quantiles) == self.num_rungs
-        assert self.num_rungs == 0 or rung_levels[-1] < max_t
-        self._metric = metric
-        self._mode = mode
-        self._resource_attr = resource_attr
-        self._max_t = max_t
-        # The data entry in ``_rungs`` is a dict with key trial_id. The
-        # value type depends on the subclass, but it contains the
-        # metric value
-        self._rungs = [
-            RungEntry(level=x, prom_quant=y, data=dict())
-            for x, y in reversed(list(zip(rung_levels, promote_quantiles)))
-        ]
+        super().__init__(
+            rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
+        )
+        # The data entry in ``_rungs`` is a dict mapping trial_id to
+        # (metric_value, was_promoted)
+        # ``_running`` maps ``trial_id ``to ``dict(milestone, resume_from)``.
+        # The tasks runs trial ``trial_id`` until resource reaches milestone.
+        # The ``resume_from`` field can be None. If not, the task is running a
+        # trial which has been resumed from rung level ``resume_from.`` This info
+        # is required for ``on_task_report`` to properly report ``ignore_data``.
+        self._running = dict()
+
+    def _find_promotable_trial(self, rung: Rung) -> Optional[Tuple[str, int]]:
+        """
+        Check whether any not yet promoted entry in ``rung`` is
+        promotable, i.e. it lies left of (or is equal to) the pivot.
+
+        :param rung: Rung to scan
+        :return: ``(trial_id, pos)`` if found, where ``pos`` is the position
+            in ``rung.data``, otherwise ``None``
+        """
+        cutoff = rung.quantile()
+        if cutoff is None:
+            return None
+        # Find best among paused trials (not yet promoted)
+        result, metric_val = None, None
+        resource = rung.level
+        for pos, entry in enumerate(rung.data):
+            if self._is_promotable_trial(entry, resource):
+                result = (entry.trial_id, pos)
+                metric_val = entry.metric_val
+                break
+        sign = 1 - 2 * (self._mode == "min")
+        if result is not None and sign * (metric_val - cutoff) < 0:
+            # Best paused trial is not good enough to be promoted
+            result = None
+        return result
+
+    def _is_promotable_trial(self, entry: PromotionRungEntry, resource: int) -> bool:
+        """
+        Checks whether trial in rung level is promotable in principle, used
+        as filter in :meth:`_find_promotable_trial`. Can be used in subclasses
+        to sharpen the condition for promotion.
 
-    def on_task_schedule(self, new_trial_id: str) -> Dict[str, Any]:
-        """Called when new task is to be scheduled.
+        :param entry: Entry of rung in question
+        :param resource: Rung level
+        :return: Should this entry be promoted, given it fulfils the pivot
+            condition?
+        """
+        return not entry.was_promoted
 
-        For a promotion-based rung system, check whether any trial can be
-        promoted. If so, return dict with keys "trial_id", "resume_from"
-        (rung level where trial is paused), "milestone" (next rung level
-        the trial will reach, or None).
-
-        If no trial can be promoted, or if the rung system is not
-        promotion-based, the returned dictionary must not contain the
-        "trial_id" key. It is nevertheless passed back via ``extra_kwargs`` in
-        :meth:`~syne_tune.optimizer.schedulers.hyperband.HyperbandBracketManager.on_task_schedule`.
-        The default is to return an empty dictionary, but some special subclasses
-        can use this to return information in case a trial is not promoted.
-
-        If no trial can be promoted, or if the rung system is not
-        promotion-based, the returned dictionary must not contain the
-        "trial_id" key. It is nevertheless passed back via ``extra_kwargs`` in
-        :meth:`~syne_tune.optimizer.schedulers.hyperband.HyperbandBracketManager.on_task_schedule`.
-        The default is to return an empty dictionary, but some special subclasses
-        can use this to return information in case a trial is not promoted.
-
-        :param new_trial_id: ID for new trial as passed to :meth:`_suggest`.
-            Only needed by specific subclasses
-        :return: See above
+    @staticmethod
+    def _mark_as_promoted(rung: Rung, pos: int, trial_id: Optional[int] = None):
+        entry = rung.pop(pos)
+        assert not entry.was_promoted
+        if trial_id is not None:
+            assert (
+                entry.trial_id == trial_id
+            ), f"Entry at position {pos} should have trial_id = {trial_id}, but has trial_id = {entry.trial_id}"
+        entry.was_promoted = True
+        rung.add(entry)
+
+    def _effective_max_t(self):
+        """
+        The following method is used in on_task_schedule to control the maximum
+        amount of resources allocated to a single configuration during the
+        optimization. For ASHA it's just a constant value.
         """
-        raise NotImplementedError
+        return self._max_t
+
+    def on_task_schedule(self, new_trial_id: str) -> Dict[str, Any]:
+        """
+        Used to implement
+        :meth:`~syne_tune.optimizer.schedulers.HyperbandScheduler._promote_trial`.
+        Searches through rungs to find a trial which can be promoted. If one is
+        found, we return the ``trial_id`` and other info (current milestone,
+        milestone to be promoted to). We also mark the trial as being promoted
+        at the rung level it sits right now.
+        """
+        trial_id, pos = None, None
+        next_milestone = self._max_t
+        milestone = None
+        rung = None
+        for _rung in self._rungs:
+            _milestone = _rung.level
+            if _milestone < self._effective_max_t():
+                result = self._find_promotable_trial(_rung)
+                if result is not None:
+                    rung = _rung
+                    milestone = _milestone
+                    trial_id, pos = result
+                    break
+            next_milestone = _milestone
+        ret_dict = dict()
+        if trial_id is not None:
+            self._mark_as_promoted(rung, pos)
+            ret_dict = {
+                "trial_id": trial_id,
+                "resume_from": milestone,
+                "milestone": next_milestone,
+            }
+        return ret_dict
 
     def on_task_add(self, trial_id: str, skip_rungs: int, **kwargs):
-        """Called when new task is started.
+        """
+        Called when new task is started. Depending on ``kwargs["new_config"]``,
+        this could start an evaluation (``True``) or promote an existing config
+        to the next milestone (``False``). In the latter case, ``kwargs`` contains
+        additional information about the promotion (in "milestone",
+        "resume_from").
 
         :param trial_id: ID of trial to be started
         :param skip_rungs: This number of the smallest rung levels are not
             considered milestones for this task
         :param kwargs: Additional arguments
         """
-        pass
+        new_config = kwargs.get("new_config", True)
+        if new_config:
+            # New trial
+            milestone = self.get_first_milestone(skip_rungs)
+            resume_from = None
+        else:
+            # Existing trial is resumed
+            # Note that self._rungs has already been updated in
+            # on_task_schedule
+            milestone = kwargs["milestone"]
+            resume_from = kwargs["resume_from"]
+            assert resume_from < milestone  # Sanity check
+        self._running[trial_id] = {"milestone": milestone, "resume_from": resume_from}
+
+    def _register_metrics_at_rung_level(
+        self, trial_id: str, result: Dict[str, Any], rung: Rung
+    ):
+        assert trial_id not in rung  # Sanity check
+        rung.add(PromotionRungEntry(trial_id=trial_id, metric_val=result[self._metric]))
 
     def on_task_report(
         self, trial_id: str, result: Dict[str, Any], skip_rungs: int
     ) -> Dict[str, Any]:
-        """Called when a trial reports metric results.
-
-        Returns dict with keys "milestone_reached" (trial reaches its milestone),
-        "task_continues" (trial should continue; otherwise it is stopped or
-        paused), "next_milestone" (next milestone it will reach, or None).
-        For certain subclasses, there may be additional entries.
+        """
+        Decision on whether task may continue (``task_continues=True``), or
+        should be paused (``task_continues=False``).
+        ``milestone_reached`` is a flag whether resource coincides with a
+        milestone.
+        For this scheduler, we have that
+
+            ``task_continues == not milestone_reached``,
+
+        since a trial is always paused at a milestone.
+
+        ``ignore_data`` is True if a result is received from a resumed trial
+        at a level ``<= resume_from``. This happens if checkpointing is not
+        implemented (or not used), because resumed trials are started from
+        scratch then. These metric values should in general be ignored.
 
         :param trial_id: ID of trial which reported results
         :param result: Reported metrics
-        :param skip_rungs: This number of the smallest rung levels are not
+        :param skip_rungs: This number of smallest rung levels are not
             considered milestones for this task
-        :return: See above
-        """
-        raise NotImplementedError
-
-    def on_task_remove(self, trial_id: str):
-        """Called when task is removed.
-
-        :param trial_id: ID of trial which is to be removed
+        :return: ``dict(task_continues, milestone_reached, next_milestone,
+            ignore_data)``
         """
-        pass
-
-    def get_first_milestone(self, skip_rungs: int) -> int:
-        """
-        :param skip_rungs: This number of the smallest rung levels are not
-            considered milestones for this task
-        :return: First milestone to be considered
-        """
-        return (
-            self._rungs[-(skip_rungs + 1)].level
-            if skip_rungs < self.num_rungs
-            else self._max_t
-        )
-
-    def _milestone_rungs(self, skip_rungs: int) -> List[RungEntry]:
-        if skip_rungs > 0:
-            return self._rungs[:(-skip_rungs)]
-        else:
-            return self._rungs
-
-    def get_milestones(self, skip_rungs: int) -> List[int]:
-        """
-        :param skip_rungs: This number of the smallest rung levels are not
-            considered milestones for this task
-        :return: All milestones to be considered, in decreasing order; does
-            not include ``max_t``
-        """
-        milestone_rungs = self._milestone_rungs(skip_rungs)
-        return [x.level for x in milestone_rungs]
-
-    def snapshot_rungs(self, skip_rungs: int) -> List[Tuple[int, dict]]:
-        """
-        A snapshot is a list of rung levels with entries ``(level, data)``,
-        ordered from top to bottom (largest rung first).
-
-        :param skip_rungs: This number of the smallest rung levels are not
-            considered milestones for this task
-        :return: Snapshot (see above)
-        """
-        milestone_rungs = self._milestone_rungs(skip_rungs)
-        return [(x.level, x.data) for x in milestone_rungs]
-
-    @staticmethod
-    def does_pause_resume() -> bool:
-        """
-        :return: Is this variant doing pause and resume scheduling, in the
-            sense that trials can be paused and resumed later?
-        """
-        raise NotImplementedError
-
-
-class StoppingRungSystem(RungSystem):
-    r"""
-    The decision on whether a trial :math:`\mathbf{x}` continues or is stopped
-    at a rung level :math:`r`, is taken in :meth:`on_task_report`. To this end,
-    the metric value :math:`f(\mathbf{x}, r)` is inserted into :math:`r.data`.
-    Then:
-
-    .. math::
-
-       \mathrm{continues}(\mathbf{x}, r)\; \Leftrightarrow\;
-       f(\mathbf{x}, r) \le \mathrm{np.quantile}(r.data, r.prom\_quant)
-
-    in case ``mode == "min"``. See also :meth:`_task_continues`.
-    """
-
-    def _cutoff(self, recorded, prom_quant):
-        values = list(recorded.values())
-        return quantile_cutoff(values, prom_quant, self._mode)
-
-    def _task_continues(
-        self,
-        metric_value: float,
-        recorded: Dict[str, Any],
-        prom_quant: float,
-        trial_id: str,
-        resource: int,
-    ) -> bool:
-        r"""
-        :param metric_value: :math:`f(\mathbf{x}, r)` for trial
-            :math:`\mathbf{x}` at rung :math:`r`
-        :param recorded: Data for rung :math:`r` (including
-            :math:`r(\mathbf{x}, r)`)
-        :param prom_quant: Quantile threshold (for mode 'min')
-        :param trial_id: ID of trial
-        :param resource: Rung level
-        :return: Continue trial? Stop otherwise
-        """
-        cutoff = self._cutoff(recorded, prom_quant)
-        if cutoff is None:
-            return True
-        return metric_value <= cutoff if self._mode == "min" else metric_value >= cutoff
-
-    def on_task_schedule(self, new_trial_id: str) -> Dict[str, Any]:
-        return dict()
-
-    def on_task_report(
-        self, trial_id: str, result: Dict[str, Any], skip_rungs: int
-    ) -> Dict[str, Any]:
         resource = result[self._resource_attr]
-        metric_value = result[self._metric]
-        if resource == self._max_t:
-            task_continues = False
+        milestone_reached = False
+        next_milestone = None
+        milestone = self._running[trial_id]["milestone"]
+        resume_from = self._running[trial_id]["resume_from"]
+        ignore_data = (resume_from is not None) and (resource <= resume_from)
+        if resource >= milestone:
+            assert resource == milestone, (
+                f"trial_id {trial_id}: resource = {resource} > {milestone} "
+                + "milestone. Make sure to report time attributes covering "
+                + "all milestones"
+            )
             milestone_reached = True
-            next_milestone = None
-        else:
-            task_continues = True
-            milestone_reached = False
-            next_milestone = self._max_t
-            milestone_rungs = self._milestone_rungs(skip_rungs)
-            for rung in milestone_rungs:
-                milestone = rung.level
-                prom_quant = rung.prom_quant
-                recorded = rung.data
-                if not (resource < milestone or trial_id in recorded):
-                    # Note: It is important for model-based searchers that
-                    # milestones are reached exactly, not jumped over. In
-                    # particular, if a future milestone is reported via
-                    # register_pending, its reward value has to be passed
-                    # later on via update.
-                    if resource > milestone:
-                        logger.warning(
-                            f"resource = {resource} > {milestone} = milestone. "
-                            "Make sure to report time attributes covering all milestones.\n"
-                            f"Continueing, but milestone {milestone} has been skipped."
-                        )
-                    else:
-                        milestone_reached = True
-                        # Enter new metric value before checking condition
-                        recorded[trial_id] = metric_value
-                        task_continues = self._task_continues(
-                            metric_value=metric_value,
-                            recorded=recorded,
-                            prom_quant=prom_quant,
-                            trial_id=trial_id,
-                            resource=resource,
-                        )
-                    break
-                next_milestone = milestone
+            rung_pos = self._rung_pos_for_level(milestone)
+            if rung_pos is not None:
+                # Register metric_value at rung level (as not promoted)
+                rung = self._rungs[rung_pos]
+                self._register_metrics_at_rung_level(trial_id, result, rung)
+                next_milestone = (
+                    self._rungs[rung_pos - 1].level if rung_pos > 0 else self._max_t
+                )
         return {
-            "task_continues": task_continues,
+            "task_continues": not milestone_reached,
             "milestone_reached": milestone_reached,
             "next_milestone": next_milestone,
+            "ignore_data": ignore_data,
         }
 
+    def on_task_remove(self, trial_id: str):
+        if trial_id in self._running:
+            del self._running[trial_id]
+
     @staticmethod
     def does_pause_resume() -> bool:
-        return False
+        return True
+
+    def support_early_checkpoint_removal(self) -> bool:
+        return True
+
+    def paused_trials(self, resource: Optional[int] = None) -> PausedTrialsResult:
+        result = []
+        if resource is None:
+            rungs = self._rungs
+        else:
+            rung_pos = self._rung_pos_for_level(resource)
+            rungs = [] if rung_pos is None else [self._rungs[rung_pos]]
+        for rung in rungs:
+            for pos, entry in enumerate(rung.data):
+                if not entry.was_promoted:
+                    result.append((entry.trial_id, pos, entry.metric_val, rung.level))
+        return result
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,20 @@
             metrics=self._metric_dict(result),
         )
         del self._trial_info[trial.trial_id]
 
     def on_trial_remove(self, trial: Trial):
         del self._trial_info[trial.trial_id]
 
+    def is_multiobjective_scheduler(self) -> bool:
+        """
+        Return True if a scheduler is multi-objective.
+        """
+        return True
+
 
 class _Bracket:
     """Bookkeeping system to track recorded values.
 
     Rungs are created in reversed order so that we can more easily find
     the correct rung corresponding to the current iteration of the result.
     """
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/pbt.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,42 +191,37 @@
         """
         lower_quantile, upper_quantile = self._quantiles()
         # If we are not in the upper quantile, we pause:
         trial_id = trial.trial_id
         if trial_id in lower_quantile:
             # sample random trial from upper quantile
             trial_id_to_clone = int(self._random_state.choice(upper_quantile))
-            assert trial_id is not trial_id_to_clone
+            assert trial_id != trial_id_to_clone
             logger.debug(
                 f"Trial {trial_id} is in lower quantile, replaced by {trial_id_to_clone}"
             )
             return trial_id_to_clone
         else:
             return trial_id
 
     def on_trial_result(self, trial: Trial, result: Dict[str, Any]) -> str:
-        if self._resource_attr not in result:
-            time_missing_msg = (
-                f"Cannot find resource_attr {self._resource_attr} "
-                f"in trial result {result}. Make sure that this "
-                "attribute is returned in the "
-                "results of your Trainable."
-            )
-            raise RuntimeError(time_missing_msg)
-        if self.metric not in result:
-            metric_missing_msg = (
-                f"Cannot find metric {self.metric} in trial result {result}. "
-                "Make sure that this attribute is returned "
-                "in the "
-                "results of your Trainable."
-            )
-            raise RuntimeError(metric_missing_msg)
+        for name, value in [
+            ("resource_attr", self._resource_attr),
+            ("metric", self.metric),
+        ]:
+            if value not in result:
+                err_msg = (
+                    f"Cannot find {name} {value} in result {result}. Make sure "
+                    "this attribute is reported by your training function"
+                )
+                raise RuntimeError(err_msg)
 
+        trial_id = trial.trial_id
         cost = result[self._resource_attr]
-        state = self._trial_state[trial.trial_id]
+        state = self._trial_state[trial_id]
 
         # Stop if we reached the maximum budget of this configuration
         if cost >= self.max_t:
             state.stopped = True
             return SchedulerDecision.STOP
 
         # Continue training if perturbation interval has not been reached yet.
@@ -237,29 +232,33 @@
 
         state.last_perturbation_time = cost
 
         trial_id_to_continue = self._get_trial_id_to_continue(trial)
 
         # bookkeeping for debugging reasons
         self._checkpointing_history.append(
-            (trial.trial_id, trial_id_to_continue, self._elapsed_time())
+            (trial_id, trial_id_to_continue, self._elapsed_time())
         )
 
-        if trial_id_to_continue == trial.trial_id:
+        if trial_id_to_continue == trial_id:
             # continue current trial
             return SchedulerDecision.CONTINUE
         else:
+            # Note: At this point, the trial ``trial`` is marked as stopped, so it
+            # cannot be proposed anymore in :meth:`_get_trial_id_to_continue` as
+            # trial to continue from. This means we can just stop the trial, and
+            # its checkpoint can be removed
             state.stopped = True
             # exploit step
             trial_to_clone = self._trial_state[trial_id_to_continue].trial
 
             # explore step
             config = self._explore(trial_to_clone.config)
             self._trial_decisions_stack.append((trial_id_to_continue, config))
-            return SchedulerDecision.PAUSE
+            return SchedulerDecision.STOP
 
     def _save_trial_state(
         self, state: PBTTrialState, time: int, result: Dict[str, Any]
     ) -> float:
         """Saves necessary trial information when result is received.
 
         :param state: State object for trial.
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/random_seeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 
 class RandomSeedGenerator:
     def __init__(self, master_seed: int):
         self._random_state = np.random.RandomState(master_seed)
 
     def __call__(self) -> int:
-        return self._random_state.randint(0, 2**32)
+        return self._random_state.randint(0, 2**31 - 1)
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/density.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/duplicate_detector.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,23 @@
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
     ExclusionList,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import (
     Configuration,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.common import (
+    CandidateGenerator,
+)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
+    BaseSurrogateModel,
+)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
+    TuningJobState,
+)
 
 # DEBUG:
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc_impl import (
     EIAcquisitionFunction,
 )
 
 logger = logging.getLogger(__name__)
@@ -88,17 +97,72 @@
         # the initial phase and return the config.
         # This trick is needed in order to make ``debug_log`` work. Otherwise, the
         # rest of ``get_config`` tries to output a block for this dummy return.
         self._debug_log_copy = self._debug_log
         self._debug_log = None  # No more debug logging for rest of ``get_config``
         return {INTERNAL_KEY: "dummy"}
 
+    def _extended_configs_from_paused(
+        self, paused_trials: List[Tuple[str, int, int]], state: TuningJobState
+    ) -> List[Dict[str, Any]]:
+        return [
+            self.config_space_ext.get(state.config_for_trial[trial_id], resource)
+            for trial_id, _, resource in paused_trials
+        ]
+
+    def _extended_configs_new(
+        self,
+        num_new: int,
+        min_resource: int,
+        exclusion_candidates: ExclusionList,
+        random_generator: CandidateGenerator,
+    ) -> List[Dict[str, Any]]:
+        return [
+            self.config_space_ext.get(config, min_resource)
+            for config in random_generator.generate_candidates_en_bulk(
+                num_new, exclusion_list=exclusion_candidates
+            )
+        ]
+
+    def _scores_for_resource(
+        self,
+        resource: int,
+        start: int,
+        end: int,
+        model: BaseSurrogateModel,
+        sorted_ind: np.ndarray,
+        configs_all: List[Dict[str, Any]],
+    ) -> (List[float], np.ndarray):
+        def my_filter_observed_data(config: Configuration) -> bool:
+            return self.config_space_ext.get_resource(config) == resource
+
+        # If there is data at level ``resource``, the incumbent in EI
+        # should only be computed over this. If there is no data at level
+        # ``resource``, the incumbent is computed over all data
+        state = model.state
+        if state.num_observed_cases(resource=resource) > 0:
+            filter_observed_data = my_filter_observed_data
+        else:
+            filter_observed_data = None
+        model.set_filter_observed_data(filter_observed_data)
+        candidates_scorer = create_initial_candidates_scorer(
+            initial_scoring="acq_func",
+            model=model,
+            acquisition_class=self.acquisition_class,
+            random_state=self.random_state,
+        )
+        ind_for_resource = sorted_ind[start:end]
+        scores_for_resource = candidates_scorer.score(
+            [configs_all[pos] for pos in ind_for_resource]
+        )
+        return scores_for_resource, ind_for_resource
+
     def score_paused_trials_and_new_configs(
         self,
-        paused_trials: List[Tuple[str, int]],
+        paused_trials: List[Tuple[str, int, int]],
         min_resource: int,
         new_trial_id: str,
         skip_optimization: bool,
     ) -> Dict[str, Any]:
         """
         See :meth:`DynamicHPOSearcher.score_paused_trials_and_new_configs`.
         If ``skip_optimization == True``, this is passed to the posterior state
@@ -113,40 +177,32 @@
         if config is None or INTERNAL_KEY not in config:
             return {"config": config}
         # Restore ``debug_log`` (see :meth:``_get_config_modelbased``)
         self._debug_log = self._debug_log_copy
         self._debug_log_copy = None
         # Note that at this point, if debug logging is active, ``get_config``
         # has called ``debug_log.start_get_config("BO", new_trial_id)``
+        exclusion_candidates = self._get_exclusion_candidates(
+            skip_observed=self._allow_duplicates,
+        )
+        random_generator = self._create_random_generator()
 
         # Collect all extended configs to be scored
         state = self.state_transformer.state
         assert (
             not state.hp_ranges.is_attribute_fixed()
         ), "Internal error: state.hp_ranges.is_attribute_fixed() must not be True"
-        configs_paused = [
-            self.config_space_ext.get(state.config_for_trial[trial_id], resource)
-            for trial_id, resource in paused_trials
-        ]
-        resources_all = [x[1] for x in paused_trials]
+        configs_paused = self._extended_configs_from_paused(paused_trials, state)
         num_new = max(self.num_initial_candidates, len(paused_trials))
-        exclusion_candidates = self._get_exclusion_candidates(
-            skip_observed=self._allow_duplicates,
+        configs_new = self._extended_configs_new(
+            num_new, min_resource, exclusion_candidates, random_generator
         )
-        random_generator = self._create_random_generator()
-        # New configurations are scored at level ``min_resource``
-        configs_new = [
-            self.config_space_ext.get(config, min_resource)
-            for config in random_generator.generate_candidates_en_bulk(
-                num_new, exclusion_list=exclusion_candidates
-            )
-        ]
         num_new = len(configs_new)  # Can be less than before
         configs_all = configs_paused + configs_new
-        resources_all.extend([min_resource] * num_new)
+        resources_all = [x[2] for x in paused_trials] + ([min_resource] * num_new)
         num_all = len(resources_all)
         if num_all == 0:
             # Very unlikely, but can happen (if config space is exhausted)
             logger.warning(
                 "Cannot score any configurations (no paused trials, no new "
                 "configurations)."
             )
@@ -162,49 +218,34 @@
         else:
             kwargs = dict()
         # Note: Asking for the model triggers the posterior computation
         model = self.state_transformer.model(**kwargs)
         # Note: ``model.state`` can have fewer observations than
         # ``self.state_transformer.state`` used above, because the former can
         # be filtered down
-        state = model.state
         resources_all = np.array(resources_all)
         sorted_ind = np.argsort(resources_all)
         resources_all = resources_all[sorted_ind]
         # Find positions where resource value changes
         change_pos = (
             [0]
             + list(np.flatnonzero(resources_all[:-1] != resources_all[1:]) + 1)
             + [num_all]
         )
         scores = np.empty((num_all,))
         for start, end in zip(change_pos[:-1], change_pos[1:]):
             resource = resources_all[start]
             assert resources_all[end - 1] == resource
-
-            def my_filter_observed_data(config: Configuration) -> bool:
-                return self.config_space_ext.get_resource(config) == resource
-
-            # If there is data at level ``resource``, the incumbent in EI
-            # should only be computed over this. If there is no data at level
-            # ``resource``, the incumbent is computed over all data
-            if state.num_observed_cases(resource=resource) > 0:
-                filter_observed_data = my_filter_observed_data
-            else:
-                filter_observed_data = None
-            model.set_filter_observed_data(filter_observed_data)
-            candidates_scorer = create_initial_candidates_scorer(
-                initial_scoring="acq_func",
+            scores_for_resource, ind_for_resource = self._scores_for_resource(
+                resource=resource,
+                start=start,
+                end=end,
                 model=model,
-                acquisition_class=self.acquisition_class,
-                random_state=self.random_state,
-            )
-            ind_for_resource = sorted_ind[start:end]
-            scores_for_resource = candidates_scorer.score(
-                [configs_all[pos] for pos in ind_for_resource]
+                sorted_ind=sorted_ind,
+                configs_all=configs_all,
             )
             scores[ind_for_resource] = scores_for_resource
             # DEBUG:
             # _debug_print_info(resource, scores_for_resource, candidates_scorer)
 
         # Pick the winner
         best_ind = np.argmin(scores)
@@ -215,17 +256,17 @@
                 self.debug_log.write_block()
         else:
             config = None
         msg = (
             f"*** Scored {len(paused_trials)} paused and {num_new} new configurations. "
         )
         if best_ind < len(paused_trials):
-            trial_id = paused_trials[best_ind][0]
+            trial_id, pos, _ = paused_trials[best_ind]
             logger.debug(msg + f"Winner is paused, trial_id = {trial_id}")
-            return {"trial_id": paused_trials[best_ind][0]}
+            return {"trial_id": trial_id, "pos": pos}
         else:
             logger.debug(msg + f"Winner is new, trial_id = {new_trial_id}")
             return {"config": config}
 
 
 class DynamicHPOSearcher(BaseSearcher):
     """
@@ -344,15 +385,15 @@
         return self._searcher_int.dataset_size()
 
     def model_parameters(self):
         return self._searcher_int.model_parameters()
 
     def score_paused_trials_and_new_configs(
         self,
-        paused_trials: List[Tuple[str, int]],
+        paused_trials: List[Tuple[str, int, int]],
         min_resource: int,
         new_trial_id: str,
     ) -> Dict[str, Any]:
         """
         This method computes acquisition scores for a number of extended
         configs :math:`(x, r)`. The acquisition score :math:`EI(x | r)` is
         expected improvement (EI) at resource level :math:`r`. Here, the
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,228 +6,250 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import List, Dict, Any, Tuple
-from numpy.random import RandomState
-import logging
-from collections import Counter
-
-from syne_tune.optimizer.schedulers.hyperband_promotion import (
-    PromotionRungSystem,
-)
-from syne_tune.optimizer.schedulers.searchers.dyhpo.dyhpo_searcher import (
-    DynamicHPOSearcher,
-    KEY_NEW_CONFIGURATION,
-)
-
-logger = logging.getLogger(__name__)
-
-
-DEFAULT_SH_PROBABILITY = 0.25
-
-
-class ScheduleDecision:
-    PROMOTE_SH = 0
-    PROMOTE_DYHPO = 1
-    START_DYHPO = 2
-
-
-class DyHPORungSystem(PromotionRungSystem):
-    """
-    Implements the logic which decides which paused trial to promote to the
-    next resource level, or alternatively which configuration to start as a
-    new trial, proposed in:
-
-        | Wistuba, M. and Kadra, A. and Grabocka, J.
-        | Dynamic and Efficient Gray-Box Hyperparameter Optimization for Deep Learning
-        | https://arxiv.org/abs/2202.09774
-
-    We do promotion-based scheduling, as in
-    :class:`~syne_tune.optimizer.schedulers.hyperband_promotion.PromotionRungSystem`.
-    In fact, we run the successive halving rule in :meth:`on_task_schedule` with
-    probability ``probability_sh``, and the DyHPO logic otherwise, or if the SH
-    rule does not promote a trial. This mechanism (not contained in the paper)
-    ensures that trials are promoted eventually, even if DyHPO only starts new
-    trials.
-
-    Since :class:`~syne_tune.optimizer.schedulers.HyperbandScheduler` was designed
-    for promotion decisions to be separate from decisions about new configs, the
-    overall workflow is a bit tricky:
-
-    * In :meth:`FIFOScheduler._suggest`, we first call
-      :code:`promote_trial_id, extra_kwargs = self._promote_trial()`. If
-      ``promote_trial_id != None``, this trial is promoted. Otherwise, we call
-      :code:`config = self.searcher.get_config(**extra_kwargs, trial_id=trial_id)`
-      and start a new trial with this config. In most cases, :meth:`_promote_trial`
-      makes a promotion decision without using the searcher.
-    * Here, we use the fact that information can be passed from
-      :meth:`_promote_trial` to ``self.searcher.get_config`` via ``extra_kwargs``.
-      Namely, :meth:``HyperbandScheduler._promote_trial` calls
-      :meth:`on_task_schedule` here, which calls
-      :meth:`~syne_tune.optimizer.schedulers.searchers.dyhpo.DynamicHPOSearcher.score_paused_trials_and_new_configs`,
-      where everything happens.
-    * First, all paused trials are scored w.r.t. the value of running them for one
-      more unit of resource. Also, a number of random configs are scored w.r.t.
-      the value of running them to the minimum resource.
-    * If the winning config is from a paused trial, this is resumed. If the
-      winning config is a new one, :meth:`on_task_schedule` returns this
-      config using a special key :const:`KEY_NEW_CONFIGURATION`. This dict
-      becomes part of ``extra_kwargs`` and is passed to ``self.searcher.get_config``
-    * :meth:`~syne_tune.optimizer.schedulers.searchers.dyhpo.DynamicHPOSearcher.get_config`
-      is trivial. It obtains an argument of name :const:`KEY_NEW_CONFIGURATION`
-      returns its value, which is the winning config to be started as new trial
-
-    We can ignore ``rung_levels`` and ``promote_quantiles``, they are not used.
-    For each trial, we only need to maintain the resource level at which it is
-    paused.
+from typing import Optional, List, Tuple
+from operator import itemgetter
+import numpy as np
+from dataclasses import dataclass
+
+from syne_tune.util import is_increasing, is_positive_integer
+
+
+@dataclass
+class SlotInRung:
+    """
+    Used to communicate slot positions and content for them.
+    """
+
+    rung_index: int  # 0 is lowest rung
+    level: int  # Resource level of rung
+    slot_index: int  # index of slot in rung
+    trial_id: Optional[int]  # None as long as no trial_id assigned
+    metric_val: Optional[float]  # Metric value (None if not yet occupied)
+
+
+class SynchronousBracket:
+    """
+    Base class for a single bracket in synchronous Hyperband algorithms.
+
+    A bracket consists of a list of rungs. Each rung consists of a number of
+    slots and a resource level (called rung level). The larger the rung level,
+    the smaller the number of slots.
+
+    A slot is occupied (by a metric value), free, or pending. A pending slot
+    has already been returned by :meth:`next_free_slot`. Slots
+    in the lowest rung (smallest rung level, largest size) are filled first.
+    At any point in time, only slots in the lowest not fully occupied rung
+    can be filled. If there are no free slots in the current rung, but there
+    are pending ones, the bracket is blocked, and another bracket needs to
+    be worked on.
     """
 
-    def __init__(
+    def __init__(self, mode: str):
+        assert mode in {"min", "max"}
+        self._mode = mode
+        self._first_free_pos = 0
+        self.current_rung = 0
+
+    @staticmethod
+    def assert_check_rungs(rungs: List[Tuple[int, int]]):
+        assert len(rungs) > 0, "There must be at least one rung"
+        sizes, levels = zip(*rungs)
+        assert is_positive_integer(
+            levels
+        ), f"Rung levels {levels} are not positive integers"
+        assert is_increasing(levels), f"Rung levels {levels} are not increasing"
+        assert is_positive_integer(
+            sizes
+        ), f"Rung sizes {sizes} are not positive integers"
+        assert is_increasing(
+            [-x for x in sizes]
+        ), f"Rung sizes {sizes} are not decreasing"
+
+    @property
+    def num_rungs(self) -> int:
+        raise NotImplementedError
+
+    def is_bracket_complete(self) -> bool:
+        return self.current_rung >= self.num_rungs
+
+    def _current_rung_and_level(
         self,
-        rung_levels: List[int],
-        promote_quantiles: List[float],
-        metric: str,
-        mode: str,
-        resource_attr: str,
-        max_t: int,
-        searcher: DynamicHPOSearcher,
-        probability_sh: bool,
-        random_state: RandomState,
-    ):
-        assert len(rung_levels) > 0, "rung_levels must not be empty"
-        assert isinstance(
-            searcher, DynamicHPOSearcher
-        ), "searcher must be of type DynamicHPOSearcher. Use searcher='dyhpo'"
-        assert (
-            0 <= probability_sh < 1
-        ), f"probability_sh = {probability_sh}, must be in [0, 1)"
-        super().__init__(
-            rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
+    ) -> (List[Tuple[Optional[int], Optional[float]]], int):
+        raise NotImplementedError
+
+    def num_pending_slots(self) -> int:
+        """
+        :return: Number of pending slots (have been returned by
+            ``next_free_slot``, but not yet occupied
+        """
+        if self.is_bracket_complete():
+            return 0
+        rung, _ = self._current_rung_and_level()
+        return sum(x[1] is None for x in rung[: self._first_free_pos])
+
+    def next_free_slot(self) -> Optional[SlotInRung]:
+        if self.is_bracket_complete():
+            return None
+        rung, milestone = self._current_rung_and_level()
+        pos = self._first_free_pos
+        if pos >= len(rung):
+            return None
+        trial_id = rung[pos][0]
+        self._first_free_pos += 1
+        return SlotInRung(
+            rung_index=self.current_rung,
+            level=milestone,
+            slot_index=pos,
+            trial_id=trial_id,
+            metric_val=None,
         )
-        self._check_rung_levels(rung_levels)
-        self._searcher = searcher
-        self._min_resource = rung_levels[0]
-        self._probability_sh = probability_sh
-        self._random_state = random_state
-        # Maps rung level to the one below
-        self._previous_rung_level = dict(zip(rung_levels[1:] + [max_t], rung_levels))
-        # Keeps a record of outcomes of :meth:`on_task_schedule` calls. Entries
-        # are ``(trial_id, decision, milestone)``, where ``decision`` is
-        # constant from :class:`ScheduleDecision`, and ``milestone`` is the
-        # rung level which the trial reaches next
-        self._schedule_records = []
 
-    @staticmethod
-    def _check_rung_levels(rung_levels: List[int]):
-        if len(rung_levels) > 1:
-            rmin = rung_levels[0]
-            step = rung_levels[1] - rmin
-            should_be = list(range(rmin, rung_levels[-1] + 1, step))
-            if rmin != step or rung_levels != should_be:
-                logger.warning(
-                    "DyHPO should be run with linearly spaced rung levels, in "
-                    "that reduction_factor is not used, and grace_period == "
-                    "rung_increment, bracket == 1. Running with rung_levels = "
-                    f"{rung_levels} is not recommended"
-                )
-
-    def _paused_trials_and_milestones(self) -> List[Tuple[str, int]]:
-        """
-        Return list of all trials which are paused. Entries are
-        ``(trial_id, resource)``, where ``resource`` is the next rung level the
-        trial reaches after being resumed.
+    def on_result(self, result: SlotInRung) -> Optional[List[int]]:
+        """
+        Provides result for slot previously requested by ``next_free_slot``.
+        Here, ``result.metric`` is written to the slot in order to make it
+        occupied. Also, ``result.trial_id`` is written there.
+
+        We normally return ``None``. But if the result passed completes the
+        current rung, this triggers the creation of a child run which consists
+        of promoted trials from the current rung. In this case, we return the
+        IDs of trials which have not been promoted. This is used in for early
+        removal of checkpoints, see
+        :meth:`~syne_tune.optimizer.schedulers.synchronous.SynchronousHyperbandScheduler.trials_checkpoints_can_be_removed`.
 
+        :param result: See above
         :return: See above
         """
-        paused_trials = []
-        next_level = self._max_t
-        for rung in self._rungs:
-            paused_trials.extend(
-                (trial_id, next_level)
-                for trial_id, (_, was_promoted) in rung.data.items()
-                if not was_promoted
-            )
-            next_level = rung.level
-        return paused_trials
-
-    def on_task_schedule(self, new_trial_id: str) -> Dict[str, Any]:
-        """
-        The main decision making happens here. We collect ``(trial_id, resource)``
-        for all paused trials and call ``searcher``. The searcher scores all
-        these trials along with a certain number of randomly drawn new
-        configurations.
-
-        If one of the paused trials has the best score, we return its ``trial_id``
-        along with extra information, so it gets promoted.
-        If one of the new configurations has the best score, we return this
-        configuration. In this case, a new trial is started with this configuration.
-
-        Note: For this scheduler type, ``kwargs`` must contain the trial ID of
-        the new trial to be started, in case none can be promoted.
-        """
-        if self._random_state.rand() <= self._probability_sh:
-            # Try to promote trial based on successive halving logic
-            result = super().on_task_schedule(new_trial_id)
-            if result.get("trial_id") is not None:
-                self._schedule_records.append(
-                    (
-                        result["trial_id"],
-                        ScheduleDecision.PROMOTE_SH,
-                        result["milestone"],
-                    )
-                )
-                return result
-        # Follow DyHPO logic
-        paused_trials = self._paused_trials_and_milestones()
-        assert new_trial_id is not None, (
-            "Internal error: kwargs must contain 'trial_id', the ID for a new "
-            "trial to be started if no paused one is resumed. Make sure to "
-            "pass this to the _promote_trial method when calling it in "
-            "_suggest"
+        assert (
+            result.rung_index == self.current_rung
+        ), f"Only accept result for rung index {self.current_rung}:\n" + str(result)
+        pos = result.slot_index
+        assert (
+            0 <= pos < self._first_free_pos
+        ), f"slot_index must be in [0, {self._first_free_pos}):\n" + str(result)
+        rung, milestone = self._current_rung_and_level()
+        assert result.level == milestone, (result, milestone)
+        trial_id, metric_val = rung[pos]
+        self._assert_on_result_trial_id(result, trial_id)
+        assert (
+            metric_val is None
+        ), f"Slot at {pos} already has metric_val = {metric_val}:\n" + str(result)
+        assert result.metric_val is not None, "result.metric_val is missing:\n" + str(
+            result
         )
-        result = self._searcher.score_paused_trials_and_new_configs(
-            paused_trials,
-            min_resource=self._min_resource,
-            new_trial_id=new_trial_id,
+        rung[pos] = (result.trial_id, result.metric_val)
+        # Check whether rung is complete. If so, move to next one and trigger
+        # promotions (optional)
+        is_complete = (
+            self._first_free_pos >= len(rung) and self.num_pending_slots() == 0
         )
-        trial_id = result.get("trial_id")
-        if trial_id is not None:
-            # Trial is to be promoted
-            milestone = next(r for i, r in paused_trials if i == trial_id)
-            resume_from = self._previous_rung_level[milestone]
-            recorded = next(
-                rung.data for rung in self._rungs if rung.level == resume_from
-            )
-            self._mark_as_promoted(recorded, trial_id)
-            ret_dict = {
-                "trial_id": trial_id,
-                "resume_from": resume_from,
-                "milestone": milestone,
-            }
-            self._schedule_records.append(
-                (trial_id, ScheduleDecision.PROMOTE_DYHPO, milestone)
-            )
-        else:
-            # New trial is to be started
-            ret_dict = {KEY_NEW_CONFIGURATION: result["config"]}
-            self._schedule_records.append(
-                (new_trial_id, ScheduleDecision.START_DYHPO, self._min_resource)
-            )
-        return ret_dict
+        trials_not_promoted = None
+        if is_complete:
+            self.current_rung += 1
+            self._first_free_pos = 0
+            if not self.is_bracket_complete():
+                trials_not_promoted = self._promote_trials_at_rung_complete()
+        return trials_not_promoted
+
+    def _assert_on_result_trial_id(self, result: SlotInRung, trial_id: int):
+        pass
+
+    def _promote_trials_at_rung_complete(self) -> List[int]:
+        """
+        This is called when a rung has just been filled in :meth:`on_result`,
+        and this is not the final rung of the bracket. It opens a new rung
+        by promoting top performing trials from the current one.
+
+        :return: List of trials which are not promoted
+        """
+        raise NotImplementedError
+
+
+class SynchronousHyperbandBracket(SynchronousBracket):
+    """
+    Represents a bracket in standard synchronous Hyperband.
+
+    When a rung is fully occupied, slots for the next rung are assigned with
+    the trial_id's having the best metric values. At any point in time, only
+    slots in the lowest not fully occupied rung can be filled.
+    """
+
+    def __init__(self, rungs: List[Tuple[int, int]], mode: str):
+        """
+        :param rungs: List of ``(rung_size, level)``, where ``level`` is rung
+            (resource) level, ``rung_size`` is rung size (number of slots).
+            All entries must be positive int's. The list must be increasing
+            in the first and decreasing in the second component
+        :param mode: Criterion is minimized ('min') or maximized ('max')
+        """
+        self.assert_check_rungs(rungs)
+        super().__init__(mode)
+        # Represents rung levels by (rung, level), where rung is a list of
+        # (trial_id, metric_val) tuples for rungs <= self._current_rung.
+        # For rungs > self._current_rung, the tuple is (rung_size, level).
+        size, level = rungs[0]
+        self._rungs = [([(None, None)] * size, level)] + rungs[1:]
 
     @property
-    def schedule_records(self) -> List[Tuple[str, int, int]]:
-        return self._schedule_records
+    def num_rungs(self) -> int:
+        return len(self._rungs)
+
+    def _current_rung_and_level(
+        self,
+    ) -> (List[Tuple[Optional[int], Optional[float]]], int):
+        return self._rungs[self.current_rung]
+
+    def _assert_on_result_trial_id(self, result: SlotInRung, trial_id: int):
+        if trial_id is not None:
+            assert result.trial_id == trial_id, (result, trial_id)
+
+    def _promote_trials_at_rung_complete(self) -> List[int]:
+        pos = self.current_rung
+        new_len, milestone = self._rungs[pos]
+        previous_rung, _ = self._rungs[pos - 1]
+        top_list, remaining_list = get_top_list(
+            rung=previous_rung, new_len=new_len, mode=self._mode
+        )
+        # Set metric_val entries to None, since this distinguishes
+        # between a pending and occupied slot
+        top_list = [(trial_id, None) for trial_id in top_list]
+        self._rungs[pos] = (top_list, milestone)
+        return remaining_list
 
-    def summary_schedule_records(self) -> str:
-        histogram = Counter([x[1] for x in self._schedule_records])
-        msg_parts = [
-            "Summary of DyHPO on_task_schedule decisions:",
-            f"  Promoted by SH:    {histogram[ScheduleDecision.PROMOTE_SH]}",
-            f"  Promoted by DyHPO: {histogram[ScheduleDecision.PROMOTE_DYHPO]}",
-            f"  Started by DyHPO:  {histogram[ScheduleDecision.START_DYHPO]}",
+
+def get_top_list(
+    rung: List[Tuple[int, float]], new_len: int, mode: str
+) -> (List[int], List[int]):
+    """
+    Returns list of IDs of trials of len ``new_len`` which should be promoted,
+    because they performed best. We also return the list of IDs of the remaining
+    trials, which are not to be promoted.
+
+    :param rung: Current rung which has just been completed
+    :param new_len: Size of new rung
+    :param mode: "min" or "max"
+    :return: ``(top_list, remaining_list)``
+    """
+    # Failed trials insert NaN's
+    rung_valid = [x for x in rung if not np.isnan(x[1])]
+    num_valid = len(rung_valid)
+    if num_valid >= new_len:
+        top_list = [
+            x[0]
+            for x in sorted(rung_valid, key=itemgetter(1), reverse=mode == "max")[
+                :new_len
+            ]
         ]
-        return "\n".join(msg_parts)
+    else:
+        # Not enough valid entries to fill the new rung (this is
+        # very unlikely to happen). In this case, some failed trials
+        # are still promoted to the next rung.
+        invalid_list = [x[0] for x in rung if np.isnan(x[1])]
+        top_list = [x[0] for x in rung_valid] + invalid_list[: (new_len - num_valid)]
+    top_set = set(top_list)
+    remaining_list = [x[0] for x in rung if x[0] not in top_set]
+    return top_list, remaining_list
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,30 @@
     :param opt_warmstart: Parameter for surrogate model fitting. If ``True``,
         each fitting is started from the previous optimum. Not recommended
         in general. Defaults to ``False``
     :type opt_warmstart: bool, optional
     :param opt_verbose: Parameter for surrogate model fitting. If ``True``,
         lots of output. Defaults to ``False``
     :type opt_verbose: bool, optional
+    :param max_size_data_for_model: If this is set, we limit the number of
+        observations the surrogate model is fitted on this value. If there are
+        more observations, they are down sampled, see
+        :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state.SubsampleSingleFidelityStateConverter`
+        for details. This down sampling is repeated every time the model is
+        fit. The ``opt_skip_*`` predicates are evaluated before the state is
+        downsampled. Pass ``None`` not to apply such a threshold. The default is
+        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults.DEFAULT_MAX_SIZE_DATA_FOR_MODEL`.
+    :type max_size_data_for_model: int, optional
+    :param max_size_top_fraction: Only used if ``max_size_data_for_model`` is
+        set. This fraction of the down sampled set is filled with the top entries
+        in the full set, the remaining ones are sampled at random from the full
+        set, see
+        :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state.SubsampleSingleFidelityStateConverter`
+        for details. Defaults to 0.25.
+    :type max_size_top_fraction: float, optional
     :param opt_skip_init_length: Parameter for surrogate model fitting,
         skip predicate. Fitting is never skipped as long as number of
         observations below this threshold. Defaults to 150
     :type opt_skip_init_length: int, optional
     :param opt_skip_period: Parameter for surrogate model fitting, skip
         predicate. If ``>1``, and number of observations above
         ``opt_skip_init_length``, fitting is done only K-th call, and skipped
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,21 @@
     INTERNAL_METRIC_NAME,
     INTERNAL_CONSTRAINT_NAME,
     INTERNAL_COST_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state import (
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state_multi_fidelity import (
     SubsampleMultiFidelityStateConverter,
     SubsampleMFDenseDataStateConverter,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.subsample_state_single_fidelity import (
+    SubsampleSingleFidelityStateConverter,
+)
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
     StateForModelConverter,
 )
 from syne_tune.optimizer.schedulers.utils.simple_profiler import SimpleProfiler
 from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
     Integer,
     Categorical,
@@ -375,16 +378,17 @@
     )
     return {
         "model_factory": model_factory,
         "filter_observed_data": filter_observed_data,
     }
 
 
-def _create_multifidelity_state_converter(
+def _create_state_converter(
     model: str,
+    is_hyperband: bool,
     **kwargs,
 ) -> Optional[StateForModelConverter]:
     """
     For model-based multi-fidelity methods, if ``max_size_data_for_model`` is given,
     we use a state converter which reduces the number of observed datapoints to
     ``max_size_data_for_model``. There are different such converters, depending on
     which method is being used.
@@ -394,35 +398,41 @@
 
     :param kwargs: Arguments
     :return: State converter; or ``None`` if ``max_size_data_for_model`` not given
     """
     max_size = kwargs.get("max_size_data_for_model")
     if max_size is None:
         return None
-    # Note:
-    if model not in ("gp_multitask", "gp_independent"):
-        logger.warning(
-            f"Cannot use max_size_data_for_model together with model={model}"
-        )
-        return None
-    if kwargs.get("searcher_data") == "all":
-        logger.warning(
-            f"You are using max_size_data_for_model={max_size} together with "
-            f"model={model} and searcher_data='all'. This may lead to poor "
-            "results. Use searcher_data='rungs' to limit the size of the data, "
-            "which you can combine with max_size_data_for_model"
-        )
-    if kwargs["scheduler"] == "hyperband_dyhpo":
-        # In DyHPO, there is too much data for some trials, so we need to limit the
-        # data differently
-        # Note: We use the defaults for ``grace_period`` and ``reduction_factor``
-        # here, could make them configurable as well.
-        return SubsampleMFDenseDataStateConverter(max_size=max_size)
+    if is_hyperband:
+        if model not in ("gp_multitask", "gp_independent"):
+            logger.warning(
+                f"Cannot use max_size_data_for_model together with model={model}"
+            )
+            return None
+        if kwargs.get("searcher_data") == "all":
+            logger.warning(
+                f"You are using max_size_data_for_model={max_size} together with "
+                f"model={model} and searcher_data='all'. This may lead to poor "
+                "results. Use searcher_data='rungs' to limit the size of the data, "
+                "which you can combine with max_size_data_for_model"
+            )
+        if kwargs["scheduler"] == "hyperband_dyhpo":
+            # In DyHPO, there is too much data for some trials, so we need to limit the
+            # data differently
+            # Note: We use the defaults for ``grace_period`` and ``reduction_factor``
+            # here, could make them configurable as well.
+            return SubsampleMFDenseDataStateConverter(max_size=max_size)
+        else:
+            return SubsampleMultiFidelityStateConverter(max_size=max_size)
     else:
-        return SubsampleMultiFidelityStateConverter(max_size=max_size)
+        scheduler_mode = kwargs.get("mode", "min")
+        top_fraction = kwargs["max_size_top_fraction"]
+        return SubsampleSingleFidelityStateConverter(
+            max_size=max_size, mode=scheduler_mode, top_fraction=top_fraction
+        )
 
 
 def _create_common_objects(model=None, is_hypertune=False, **kwargs):
     scheduler = kwargs["scheduler"]
     is_hyperband = scheduler.startswith("hyperband")
     if model is None:
         model = "gp_multitask"
@@ -485,18 +495,18 @@
         # Extended config space
         epoch_range = (1, kwargs["max_epochs"])
         result["config_space_ext"] = ExtendedConfiguration(
             hp_ranges,
             resource_attr_key=kwargs["resource_attr"],
             resource_attr_range=epoch_range,
         )
-        # State converter to down sample data
-        state_converter = _create_multifidelity_state_converter(model, **kwargs)
-        if state_converter is not None:
-            result["state_converter"] = state_converter
+    # State converter to down sample data
+    state_converter = _create_state_converter(model, is_hyperband, **kwargs)
+    if state_converter is not None:
+        result["state_converter"] = state_converter
 
     # Create model factory
     if model == "gp_multitask":
         result.update(
             _create_gp_standard_model(
                 hp_ranges=hp_ranges,
                 active_metric=INTERNAL_METRIC_NAME,
@@ -895,14 +905,15 @@
         "debug_log": True,
         "cost_attr": "elapsed_time",
         "normalize_targets": True,
         "no_fantasizing": False,
         "allow_duplicates": False,
         "input_warping": False,
         "boxcox_transform": False,
+        "max_size_top_fraction": 0.25,
     }
     if is_restrict_configs:
         default_options["initial_scoring"] = "acq_func"
         default_options["skip_local_optimization"] = True
     if is_hyperband:
         if is_hypertune:
             default_options["model"] = "gp_independent"
@@ -914,19 +925,19 @@
         default_options["resource_acq_bohb_threshold"] = 3
         default_options["num_init_random"] = 6
         default_options["issm_gamma_one"] = False
         default_options["expdecay_normalize_inputs"] = False
         default_options["separate_noise_variances"] = False
         default_options["hypertune_distribution_num_samples"] = 50
         default_options["hypertune_distribution_num_brackets"] = 1
-        if (
-            kwargs.get("model") in (None, "gp_multitask", "gp_independent")
-            and kwargs.get("searcher_data") != "all"
-        ):
-            default_options["max_size_data_for_model"] = DEFAULT_MAX_SIZE_DATA_FOR_MODEL
+    if (not is_hyperband) or (
+        kwargs.get("model") in (None, "gp_multitask", "gp_independent")
+        and kwargs.get("searcher_data") != "all"
+    ):
+        default_options["max_size_data_for_model"] = DEFAULT_MAX_SIZE_DATA_FOR_MODEL
     if is_multi_output:
         default_options["initial_scoring"] = "acq_func"
         default_options["exponent_cost"] = 1.0
 
     constraints = {
         "random_seed": Integer(0, 2**32 - 1),
         "opt_skip_init_length": Integer(0, None),
@@ -944,14 +955,16 @@
         "skip_local_optimization": Boolean(),
         "debug_log": Boolean(),
         "normalize_targets": Boolean(),
         "no_fantasizing": Boolean(),
         "allow_duplicates": Boolean(),
         "input_warping": Boolean(),
         "boxcox_transform": Boolean(),
+        "max_size_data_for_model": IntegerOrNone(1, None),
+        "max_size_top_fraction": Float(0.0, 1.0),
     }
 
     if is_hyperband:
         model_choices = ("gp_multitask", "gp_independent")
         if not is_hypertune:
             model_choices = model_choices + ("gp_issm", "gp_expdecay")
         constraints["model"] = Categorical(choices=model_choices)
@@ -963,15 +976,14 @@
             choices=tuple(SUPPORTED_RESOURCE_FOR_ACQUISITION)
         )
         constraints["issm_gamma_one"] = Boolean()
         constraints["expdecay_normalize_inputs"] = Boolean()
         constraints["separate_noise_variances"] = Boolean()
         constraints["hypertune_distribution_num_samples"] = Integer(1, None)
         constraints["hypertune_distribution_num_brackets"] = Integer(1, None)
-        constraints["max_size_data_for_model"] = IntegerOrNone(1, None)
     if is_multi_output:
         constraints["initial_scoring"] = Categorical(choices=tuple({"acq_func"}))
         constraints["exponent_cost"] = Float(0.0, 1.0)
 
     return mandatory, default_options, constraints
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/multi_objective_regularized_evolution.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, Any
 import logging
 
 from syne_tune.backend.trial_status import Trial
-from syne_tune.tuner_callback import StoreResultsCallback
+from syne_tune.results_callback import StoreResultsCallback
 from syne_tune.backend.simulator_backend.simulator_callback import SimulatorCallback
 from syne_tune.optimizer.schedulers.fifo import FIFOScheduler
 from syne_tune.optimizer.schedulers.searchers import ModelBasedSearcher
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
     ModelStateTransformer,
 )
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 class DifferentialEvolutionHyperbandBracket(SynchronousBracket):
     """
     Represents a bracket in Differential Evolution Hyperband (DEHB).
 
     There are a number of differences to brackets in standard synchronous
-    Hyperband (:class:`SynchronousHyperbandBracket`):
+    Hyperband (:class:`~syne_tune.optimizer.schedulers.synchronous.hyperband_bracket.SynchronousHyperbandBracket`):
 
-    * ``on_result``: ``result.trial_id`` overwrites ``trial_id`` in rung even if
-      latter is not None.
+    * :meth:`on_result`: ``result.trial_id`` overwrites ``trial_id`` in rung
+      even if latter is not ``None``.
     * Promotions are not triggered automatically when a rung is complete
     * Some additional methods
     """
 
     def __init__(
         self,
         rungs: List[Tuple[int, int]],
@@ -64,11 +64,11 @@
         in rung below the currently active one (which must not be the base
         rung). The list is of the size of the current rung.
         """
         assert self.current_rung > 0, "Current rung is base rung"
         previous_rung, _ = self._rungs[self.current_rung - 1]
         return get_top_list(
             rung=previous_rung, new_len=self.size_of_current_rung(), mode=self._mode
-        )
+        )[0]
 
-    def _promote_trials_at_rung_complete(self):
-        pass
+    def _promote_trials_at_rung_complete(self) -> List[int]:
+        return []
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional, List, Set, Dict, Any
+from typing import Optional, List, Set, Dict, Any, Tuple
 import logging
 import numpy as np
 
+from syne_tune.callbacks.remove_checkpoints_callback import (
+    DefaultRemoveCheckpointsSchedulerMixin,
+)
 from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket_manager import (
     SynchronousHyperbandBracketManager,
 )
 from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket import SlotInRung
 from syne_tune.optimizer.schedulers.synchronous.hyperband_rung_system import (
     RungSystemsPerBracket,
 )
@@ -152,15 +155,17 @@
         return self._max_resource_level
 
     @property
     def searcher_data(self) -> str:
         return self._searcher_data
 
 
-class SynchronousHyperbandScheduler(SynchronousHyperbandCommon):
+class SynchronousHyperbandScheduler(
+    SynchronousHyperbandCommon, DefaultRemoveCheckpointsSchedulerMixin
+):
     """
     Synchronous Hyperband. Compared to
     :class:`~syne_tune.optimizer.schedulers.HyperbandScheduler`, this is also
     scheduling jobs asynchronously, but decision-making is synchronized,
     in that trials are only promoted to the next milestone once the rung they
     are currently paused at, is completely occupied.
 
@@ -258,14 +263,15 @@
         # ``bracket_manager.on_result``. Entries are removed once passed to
         # ``on_result``. Note that a trial_id can be associated with different
         # job descriptions in its lifetime
         self._trial_to_pending_slot = dict()
         # Maps trial_id (active) to config
         self._trial_to_config = dict()
         self._rung_levels = [level for _, level in bracket_rungs[0]]
+        self._trials_checkpoints_can_be_removed = []
 
     @property
     def rung_levels(self) -> List[int]:
         return self._rung_levels
 
     @property
     def num_brackets(self) -> int:
@@ -331,23 +337,28 @@
             logger.warning(
                 "Searcher failed to suggest a configuration for new trial "
                 f"{trial_id}. The corresponding rung slot is marked as failed."
             )
             self._report_as_failed(bracket_id, slot_in_rung)
         return suggestion
 
+    def _on_result(self, result: Tuple[int, SlotInRung]):
+        trials_not_promoted = self.bracket_manager.on_result(result)
+        if trials_not_promoted is not None:
+            self._trials_checkpoints_can_be_removed.extend(trials_not_promoted)
+
     def _report_as_failed(self, bracket_id: int, slot_in_rung: SlotInRung):
         result_failed = SlotInRung(
             rung_index=slot_in_rung.rung_index,
             level=slot_in_rung.level,
             slot_index=slot_in_rung.slot_index,
             trial_id=slot_in_rung.trial_id,
             metric_val=np.NAN,
         )
-        self.bracket_manager.on_result((bracket_id, result_failed))
+        self._on_result((bracket_id, result_failed))
 
     def on_trial_result(self, trial: Trial, result: Dict[str, Any]) -> str:
         trial_id = trial.trial_id
         if trial_id in self._trial_to_pending_slot:
             bracket_id, slot_in_rung = self._trial_to_pending_slot[trial_id]
             assert slot_in_rung.trial_id == trial_id  # Sanity check
             assert self.metric in result, (
@@ -366,15 +377,15 @@
                 assert resource == milestone, (
                     f"Trial trial_id {trial_id}: Obtained result for "
                     + f"resource = {resource}, but not for {milestone}. "
                     + "Training script must not skip rung levels!"
                 )
                 # Reached rung level: Pass result to bracket manager
                 slot_in_rung.metric_val = metric_val
-                self.bracket_manager.on_result((bracket_id, slot_in_rung))
+                self._on_result((bracket_id, slot_in_rung))
                 # Remove it from pending slots
                 del self._trial_to_pending_slot[trial_id]
                 # Trial should be paused
                 trial_decision = SchedulerDecision.PAUSE
             prev_level = self.bracket_manager.level_to_prev_level(bracket_id, milestone)
             if resource > prev_level:
                 # If the training script does not implement checkpointing, each
@@ -418,7 +429,12 @@
             )
 
     def metric_names(self) -> List[str]:
         return [self.metric]
 
     def metric_mode(self) -> str:
         return self.mode
+
+    def trials_checkpoints_can_be_removed(self) -> List[int]:
+        result = self._trials_checkpoints_can_be_removed
+        self._trials_checkpoints_can_be_removed = []
+        return result
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Tuple
+from typing import Tuple, Optional, List
 import copy
 
 from syne_tune.optimizer.schedulers.synchronous.hyperband_bracket import (
     SynchronousHyperbandBracket,
     SlotInRung,
 )
 from syne_tune.optimizer.schedulers.synchronous.hyperband_rung_system import (
@@ -25,26 +25,25 @@
 class SynchronousHyperbandBracketManager:
     """
     Maintains all brackets, relays requests for another job and report of
     result to one of the brackets.
 
     Each bracket contains a number of rungs, the largest one ``max_num_rungs``.
     A bracket with k rungs has offset ``max_num_rungs - k``. Hyperband cycles
-    through brackets with offset 0, ..., ``num_brackets - 1``, where
+    through brackets with offset ``0, ..., num_brackets - 1``, where
     ``num_brackets <= max_num_rungs``.
 
     At any given time, one bracket is primary, all other active brackets are
     secondary. Jobs are preferentially assigned to the primary bracket, but
     if its current rung has no free slots (all are pending), secondary
     brackets are considered.
 
-    Each bracket has a bracket_id (nonnegative int), which is used as key for
-    the dicts in ``next_jobs``, ``on_results``. The primary bracket always has
-    the lowest id of all active ones. For job assignment, we iterate over
-    active brackets starting from the primary, and assign the job to the
+    Each bracket has a ``bracket_id`` (nonnegative int). The primary bracket
+    always has the lowest id of all active ones. For job assignment, we iterate
+    over active brackets starting from the primary, and assign the job to the
     first bracket which has a free slot. If none of the active brackets have
     a free slot, a new bracket is created.
 
     :param bracket_rungs: Rungs for successive brackets, from largest to
         smallest
     :param mode: Criterion is minimized ('min') or maximized ('max')
     """
@@ -120,43 +119,44 @@
         ``slot_in_rung`` is :class:`SlotInRung`, containing the info of what
         is to be done (``trial_id``, ``level`` fields). It is this entry which
         has to be returned in 'on_result``, which the ``metric_val`` field set.
         If the job returned here has ``trial_id == None``, it comes from the
         lowest rung of its bracket, and the ``trial_id`` has to be set as well
         when returning the record in ``on_result``.
 
-        :return: Tuple (bracket_id, slot_in_rung)
+        :return: Tuple ``(bracket_id, slot_in_rung)``
         """
         # Try to assign job to active bracket. There must be at least one,
         # the primary one
         bracket_ids = range(self._primary_bracket_id, self._next_bracket_id)
         for bracket_id in bracket_ids:
             slot_in_rung = self._brackets[bracket_id].next_free_slot()
             if slot_in_rung is not None:
                 return bracket_id, slot_in_rung
         # None of the existing brackets accept jobs. Create a new one
         bracket_id = self._create_new_bracket()
         slot_in_rung = self._brackets[bracket_id].next_free_slot()
         assert slot_in_rung is not None, "Newly created bracket has to have a free slot"
         return bracket_id, slot_in_rung
 
-    def on_result(self, result: Tuple[int, SlotInRung]):
+    def on_result(self, result: Tuple[int, SlotInRung]) -> Optional[List[int]]:
         """
         Called by scheduler to provide result for previously requested job.
-        See ``next_job``.
+        See :meth:`next_job`.
 
-        :param result: Tuple (bracket_id, slot_in_rung)
+        :param result: Tuple ``(bracket_id, slot_in_rung)``
+        :return: See :meth:`~syne_tune.optimizer.schedulers.synchronous.hyperband_bracket.SynchronousBracket.on_result`
         """
         bracket_id, slot_in_rung = result
         assert self._primary_bracket_id <= bracket_id < self._next_bracket_id, (
             f"Invalid bracket_id = {bracket_id}, must be in "
             + f"[{self._primary_bracket_id}, {self._next_bracket_id})"
         )
         bracket = self._brackets[bracket_id]
-        bracket.on_result(slot_in_rung)
+        trials_not_promoted = bracket.on_result(slot_in_rung)
         for_primary = bracket_id == self._primary_bracket_id
         if for_primary:
             # Primary bracket is complete: Move to next one. While very
             # unlikely, brackets after the primary one could be complete
             # as well
             last_bracket = self._next_bracket_id - 1
             while (
@@ -164,7 +164,8 @@
                 and self._primary_bracket_id < last_bracket
             ):
                 self._primary_bracket_id += 1
                 bracket = self._brackets[self._primary_bracket_id]
             # May have to create a new bracket
             if bracket.is_bracket_complete():
                 self._primary_bracket_id = self._create_new_bracket()
+        return trials_not_promoted
```

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.5.0/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/remote/__init__.py` & `syne_tune-0.5.0/syne_tune/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/remote/estimators.py` & `syne_tune-0.5.0/syne_tune/remote/estimators.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/remote/remote_launcher.py` & `syne_tune-0.5.0/syne_tune/remote/remote_launcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/remote/remote_main.py` & `syne_tune-0.5.0/syne_tune/remote/remote_main.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.5.0/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/report.py` & `syne_tune-0.5.0/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/stopping_criterion.py` & `syne_tune-0.5.0/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/try_import.py` & `syne_tune-0.5.0/syne_tune/try_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
 def try_import_backends_message() -> str:
     return _try_import_message(
         "LocalBackend / PythonBackend are not imported", tag=None
     )
 
 
+def try_import_moo_message() -> str:
+    return _try_import_message(
+        "Multi Objective Optimization dependencies are not imported", tag="moo"
+    )
+
+
 def _try_import_message(message_text: str, tag: Optional[str]) -> str:
     if tag is None:
         insert = ""
     else:
         insert = "[" + tag + "]"
     return (
         message_text
```

### Comparing `syne_tune-0.4.1/syne_tune/tuner.py` & `syne_tune-0.5.0/syne_tune/tuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,38 @@
 
 from syne_tune.backend.trial_backend import (
     TrialBackend,
     TrialAndStatusInformation,
     TrialIdAndResultList,
 )
 from syne_tune.backend.trial_status import Status, Trial, TrialResult
-from syne_tune.config_space import config_space_to_json_dict
-from syne_tune.constants import ST_TUNER_CREATION_TIMESTAMP, ST_TUNER_START_TIMESTAMP
+from syne_tune.constants import (
+    ST_TUNER_CREATION_TIMESTAMP,
+    ST_TUNER_START_TIMESTAMP,
+    ST_METADATA_FILENAME,
+    ST_TUNER_DILL_FILENAME,
+    TUNER_DEFAULT_SLEEP_TIME,
+)
 from syne_tune.optimizer.scheduler import SchedulerDecision, TrialScheduler
-from syne_tune.tuner_callback import StoreResultsCallback, TunerCallback
+from syne_tune.optimizer.schedulers.remove_checkpoints import (
+    RemoveCheckpointsSchedulerMixin,
+)
+from syne_tune.tuner_callback import TunerCallback
+from syne_tune.results_callback import StoreResultsCallback
 from syne_tune.tuning_status import TuningStatus, print_best_metric_found
 from syne_tune.util import (
     RegularCallback,
     check_valid_sagemaker_name,
     experiment_path,
     name_from_base,
     dump_json_with_numpy,
 )
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_SLEEP_TIME = 5.0
-
 
 class Tuner:
     """
     Controller of tuning loop, manages interplay between scheduler and
     trial backend. Also, stopping criterion and number of workers are
     maintained here.
 
@@ -54,15 +61,15 @@
     :param stop_criterion: Tuning stops when this predicates returns ``True``.
         Called in each iteration with the current tuning status. It is
         recommended to use :class:`StoppingCriterion`.
     :param n_workers: Number of workers used here. Note that the backend
         needs to support (at least) this number of workers to be run
         in parallel
     :param sleep_time: Time to sleep when all workers are busy. Defaults to
-        :const:`DEFAULT_SLEEP_TIME`
+        :const:`~syne_tune.constants.DEFAULT_SLEEP_TIME`
     :param results_update_interval: Frequency at which results are updated and
         stored (in seconds). Defaults to 10.
     :param print_update_interval: Frequency at which result table is printed.
         Defaults to 30.
     :param max_failures: This many trial execution failures are allowed before
         the tuning loop is aborted. Defaults to 1
     :param tuner_name: Name associated with the tuning experiment, default to
@@ -78,15 +85,15 @@
         trials when stopping criterion is met. If ``True``, the tuner waits
         until all trials are finished. If ``False``, all trials are terminated.
         Defaults to ``False``.
     :param callbacks: Called at certain times in the tuning loop, for example
         when a result is seen. The default callback stores results every
         ``results_update_interval``.
     :param metadata: Dictionary of user-metadata that will be persisted in
-        ``{tuner_path}/metadata.json``, in addition to metadata provided by
+        ``{tuner_path}/{ST_METADATA_FILENAME}``, in addition to metadata provided by
         the user. ``SMT_TUNER_CREATION_TIMESTAMP`` is always included which
         measures the time-stamp when the tuner started to run.
     :param suffix_tuner_name: If ``True``, a timestamp is appended to the
         provided ``tuner_name`` that ensures uniqueness, otherwise the name is
         left unchanged and is expected to be unique. Defaults to ``True``.
     :param save_tuner: If ``True``, the :class:`Tuner` object is serialized at
         the end of tuning, including its dependencies (e.g., scheduler). This
@@ -125,15 +132,15 @@
 
     def __init__(
         self,
         trial_backend: TrialBackend,
         scheduler: TrialScheduler,
         stop_criterion: Callable[[TuningStatus], bool],
         n_workers: int,
-        sleep_time: float = DEFAULT_SLEEP_TIME,
+        sleep_time: float = TUNER_DEFAULT_SLEEP_TIME,
         results_update_interval: float = 10.0,
         print_update_interval: float = 30.0,
         max_failures: int = 1,
         tuner_name: Optional[str] = None,
         asynchronous_scheduling: bool = True,
         wait_trial_completion_when_stopping: bool = False,
         callbacks: Optional[List[TunerCallback]] = None,
@@ -178,21 +185,46 @@
         # to store the logs and tuner results in the same folder.
         self.trial_backend.set_path(
             results_root=str(self.tuner_path)
             if trial_backend_path is None
             else trial_backend_path,
             tuner_name=self.name,
         )
-        self.callbacks = (
-            callbacks if callbacks is not None else [self._default_callback()]
-        )
-
+        self._init_callbacks(callbacks)
         self.tuning_status = None
         self.tuner_saver = None
         self.status_printer = None
+        self._initialize_early_checkpoint_removal()
+
+    def _init_callbacks(self, callbacks: Optional[List[TunerCallback]]):
+        if callbacks is None:
+            callbacks = [self._default_callback()]
+        else:
+            if not any(
+                isinstance(callback, StoreResultsCallback) for callback in callbacks
+            ):
+                logger.warning(
+                    "None of the callbacks provided are of type StoreResultsCallback. "
+                    "This means no tuning results will be written."
+                )
+        self.callbacks: List[TunerCallback] = callbacks
+
+    def _initialize_early_checkpoint_removal(self):
+        """
+        If the scheduler supports early checkpoint removal, the specific callback
+        for this is created here and appended to ``self.callbacks``.
+        """
+        if self.trial_backend.delete_checkpoints:
+            callback = (
+                self.scheduler.callback_for_checkpoint_removal(self.stop_criterion)
+                if isinstance(self.scheduler, RemoveCheckpointsSchedulerMixin)
+                else None
+            )
+            if callback is not None:
+                self.callbacks.append(callback)
 
     def run(self):
         """Launches the tuning."""
         done_trials_statuses = OrderedDict()
         try:
             logger.info(f"results of trials will be saved on {self.tuner_path}")
 
@@ -358,30 +390,22 @@
     def _enrich_metadata(self, metadata: Dict[str, Any]) -> Dict[str, Any]:
         """
         :param metadata: Original metadata
         :return: ``metadata`` enriched by default entries
         """
         res = metadata if metadata is not None else dict()
         self._set_metadata(res, ST_TUNER_CREATION_TIMESTAMP, time.time())
-        self._set_metadata(res, "metric_names", self.scheduler.metric_names())
-        self._set_metadata(res, "metric_mode", self.scheduler.metric_mode())
         self._set_metadata(res, "entrypoint", self.trial_backend.entrypoint_path().stem)
         self._set_metadata(res, "backend", str(type(self.trial_backend).__name__))
-
-        self._set_metadata(
-            res, "scheduler_name", str(self.scheduler.__class__.__name__)
-        )
-        config_space_json = dump_json_with_numpy(
-            config_space_to_json_dict(self.scheduler.config_space)
-        )
-        self._set_metadata(res, "config_space", config_space_json)
+        for key, value in self.scheduler.metadata().items():
+            self._set_metadata(res, key, value)
         return res
 
     def _save_metadata(self):
-        dump_json_with_numpy(self.metadata, self.tuner_path / "metadata.json")
+        dump_json_with_numpy(self.metadata, self.tuner_path / ST_METADATA_FILENAME)
 
     def _stop_condition(self) -> bool:
         return (
             self.stop_criterion(self.tuning_status)
             or self.tuning_status.num_trials_failed > self.max_failures
         )
 
@@ -415,15 +439,15 @@
         # The trials can be finished for different reasons:
         # - they completed,
         # - they were stopped independently of the scheduler, e.g. due to a
         #   timeout argument or a manual interruption
         # - scheduler decided to interrupt them.
         # Note: ``done_trials`` includes trials which are paused.
         done_trials_statuses = self._update_running_trials(
-            trial_status_dict, new_results, callbacks=self.callbacks
+            trial_status_dict, new_results
         )
         trial_status_dict.update(done_trials_statuses)
 
         # update status with new results and all done trials
         self.tuning_status.update(
             trial_status_dict=trial_status_dict, new_results=new_results
         )
@@ -491,25 +515,29 @@
             # we schedule a new trial, possibly using the checkpoint of ``checkpoint_trial_id``
             # if given.
             trial = self.trial_backend.start_trial(
                 config=suggestion.config.copy(),
                 checkpoint_trial_id=suggestion.checkpoint_trial_id,
             )
             self.scheduler.on_trial_add(trial=trial)
+            for callback in self.callbacks:
+                callback.on_start_trial(trial)
             logger.info(f"(trial {trial.trial_id}) - scheduled {suggestion}")
             return trial
         else:
             # suggestion is a trial_id to resume, with possibly a new configuration
             log_msg = f"Resuming trial {suggestion.checkpoint_trial_id}"
             if suggestion.config is not None:
                 log_msg += f" with new_config = {suggestion.config}"
             logger.info(log_msg)
             trial = self.trial_backend.resume_trial(
                 trial_id=suggestion.checkpoint_trial_id, new_config=suggestion.config
             )
+            for callback in self.callbacks:
+                callback.on_resume_trial(trial)
             return trial
 
     def _handle_failure(self, done_trials_statuses: Dict[int, Tuple[Trial, str]]):
         logger.error(f"Stopped as {self.max_failures} failures were reached")
         for trial_id, (_, status) in done_trials_statuses.items():
             if status == Status.failed:
                 logger.error(f"showing log of first failure")
@@ -517,63 +545,61 @@
                 stderr = "".join(self.trial_backend.stderr(trial_id))
                 logger.error(stdout)
                 logger.error(stderr)
                 raise ValueError(f"Trial - {trial_id} failed")
 
     def save(self, folder: Optional[str] = None):
         if folder is None:
-            tuner_serialized_path = self.tuner_path / "tuner.dill"
+            tuner_serialized_path = self.tuner_path / ST_TUNER_DILL_FILENAME
         else:
-            tuner_serialized_path = Path(folder) / "tuner.dill"
+            tuner_serialized_path = Path(folder) / ST_TUNER_DILL_FILENAME
         with open(tuner_serialized_path, "wb") as f:
             logger.debug(f"saving tuner in {tuner_serialized_path}")
             dill.dump(self, f)
             self.trial_backend.on_tuner_save()  # callback
 
     @staticmethod
     def load(tuner_path: Optional[str]):
-        with open(Path(tuner_path) / "tuner.dill", "rb") as f:
+        with open(Path(tuner_path) / ST_TUNER_DILL_FILENAME, "rb") as f:
             tuner = dill.load(f)
             tuner.tuner_path = Path(experiment_path(tuner_name=tuner.name))
             return tuner
 
     def _update_running_trials(
         self,
         trial_status_dict: TrialAndStatusInformation,
         new_results: TrialIdAndResultList,
-        callbacks: List[TunerCallback],
     ) -> TrialAndStatusInformation:
         """
         Updates schedulers with new results and sends decision to stop/pause
         trials to the backend. Trials can be finished because:
 
         * the scheduler decided to stop or pause.
         * the trial failed.
         * the trial was stopped independently of the scheduler, e.g. due to a
           timeout argument or a manual interruption.
         * the trial completed.
 
         :param trial_status_dict: Information on trials from
             ``trial_backend.fetch_status_results``
         :param new_results: New results from ``trial_backend.fetch_status_results``
-        :param callbacks: ``on_trial_result`` for these callbacks is called here
         :return: Dictionary mapping trial-ids that are finished to status
         """
         # gets the list of jobs from running_jobs that are done
         done_trials = dict()
 
         for trial_id, result in new_results:
             if trial_id not in done_trials:
                 trial, status = trial_status_dict[trial_id]
 
                 # communicate new result to the searcher and the scheduler
                 self.last_seen_result_per_trial[trial_id] = result
                 decision = self.scheduler.on_trial_result(trial=trial, result=result)
 
-                for callback in callbacks:
+                for callback in self.callbacks:
                     callback.on_trial_result(
                         trial=trial,
                         status=status,
                         result=result,
                         decision=decision,
                     )
 
@@ -624,15 +650,15 @@
                         f"trial {trial_id} completed and no metrics got observed"
                     )
 
                 last_result = self.last_seen_result_per_trial[trial_id]
                 if trial_id not in done_trials:
                     self.scheduler.on_trial_complete(trial, last_result)
                 if status == Status.completed:
-                    for callback in callbacks:
+                    for callback in self.callbacks:
                         callback.on_trial_complete(trial, last_result)
                 done_trials[trial_id] = (trial, status)
 
             if status == Status.failed:
                 logger.info(f"Trial trial_id {trial_id} failed.")
                 self.scheduler.on_trial_error(trial)
                 done_trials[trial_id] = (trial, status)
```

### Comparing `syne_tune-0.4.1/syne_tune/tuner_callback.py` & `syne_tune-0.5.0/syne_tune/results_callback.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,140 +6,103 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Dict, Any
+from typing import Dict, Any, Optional, List
 from time import perf_counter
 import copy
 import pandas as pd
 
 from syne_tune.backend.trial_status import Trial
-from syne_tune.backend.trial_backend import (
-    TrialAndStatusInformation,
-    TrialIdAndResultList,
+from syne_tune.constants import (
+    ST_DECISION,
+    ST_TRIAL_ID,
+    ST_STATUS,
+    ST_TUNER_TIME,
+    ST_RESULTS_DATAFRAME_FILENAME,
 )
-from syne_tune.constants import ST_DECISION, ST_TRIAL_ID, ST_STATUS, ST_TUNER_TIME
+from syne_tune.tuner_callback import TunerCallback
 from syne_tune.util import RegularCallback
 
 
-class TunerCallback:
+class ExtraResultsComposer:
     """
-    Allows user of :class:`~syne_tune.Tuner` to monitor progress, store
-    additional results, etc.
+    Base class for ``extra_results_composer`` argument in
+    :class:`StoreResultsCallback`. Extracts extra results in
+    :meth:`StoreResultsCallback.on_trial_result` and returns them as
+    dictionary to be appended to the results dataframe.
+
+    Why don't we use a lambda function instead? We would like the tuner,
+    with all its dependent objects, to be dill serializable, and lambda
+    functions are not.
     """
 
-    def on_tuning_start(self, tuner):
-        """Called at start of tuning loop
-
-        :param tuner: :class:`~syne_tune.Tuner` object
-        """
-        pass
-
-    def on_tuning_end(self):
-        """Called once the tuning loop terminates
-
-        This is called before :class:`~syne_tune.Tuner` object is serialized
-        (optionally), and also before running jobs are stopped.
-        """
-        pass
-
-    def on_loop_start(self):
-        """Called at start of each tuning loop iteration
-
-        Every iteration starts with fetching new results from the backend.
-        This is called before this is done.
-        """
-        pass
-
-    def on_loop_end(self):
-        """Called at end of each tuning loop iteration
-
-        This is done before the loop stopping condition is checked and acted
-        upon.
-        """
-        pass
-
-    def on_fetch_status_results(
-        self,
-        trial_status_dict: TrialAndStatusInformation,
-        new_results: TrialIdAndResultList,
-    ):
-        """Called just after ``trial_backend.fetch_status_results``
-
-        :param trial_status_dict: Result of ``fetch_status_results``
-        :param new_results: Result of ``fetch_status_results``
+    def __call__(self, tuner) -> Optional[Dict[str, Any]]:
         """
-        pass
-
-    def on_trial_complete(self, trial: Trial, result: Dict[str, Any]):
-        """Called when a trial completes (``Status.completed``)
+        Called in :meth:`StoreResultsCallback.on_trial_result`. The dictionary
+        returned is appended (as extra columns) to the results dataframe.
 
-        The arguments here also have been passed to ``scheduler.on_trial_complete``,
-        before this call here.
-
-        :param trial: Trial that just completed.
-        :param result: Last result obtained.
+        :param tuner: :class:`~syne_tune.Tuner` object from which extra results
+            are extracted
+        :return: Dictionary (JSON-serializable) to be appended, or ``None`` if
+            nothing should be appended
         """
-        pass
-
-    def on_trial_result(
-        self, trial: Trial, status: str, result: Dict[str, Any], decision: str
-    ):
-        """Called when a new result (reported by a trial) is observed
+        raise NotImplementedError
 
-        The arguments here are inputs or outputs of ``scheduler.on_trial_result``
-        (called just before).
-
-        :param trial: Trial whose report has been received
-        :param status: Status of trial before ``scheduler.on_trial_result`` has
-            been called
-        :param result: Result dict received
-        :param decision: Decision returned by ``scheduler.on_trial_result``
+    def keys(self) -> List[str]:
         """
-        pass
-
-    def on_tuning_sleep(self, sleep_time: float):
-        """Called just after tuner has slept, because no worker was available
-
-        :param sleep_time: Time (in secs) for which tuner has just slept
+        :return: Key names of dictionaries returned in :meth:`__call__`, or
+            ``[]`` if nothing is returned
         """
-        pass
+        return []
 
 
 class StoreResultsCallback(TunerCallback):
     """
     Default implementation of :class:`~TunerCallback` which records all
     reported results, and allows to store them as CSV file.
 
-    :param add_wallclock_time: If True, wallclock time since call of
+    :param add_wallclock_time: If ``True``, wallclock time since call of
         ``on_tuning_start`` is stored as
         :const:`~syne_tune.constants.ST_TUNER_TIME`.
+    :param extra_results_composer: Optional. If given, this is called in
+        :meth:`on_trial_result`, and the resulting dictionary is appended as
+        extra columns to the results dataframe
     """
 
     def __init__(
         self,
         add_wallclock_time: bool = True,
+        extra_results_composer: Optional[ExtraResultsComposer] = None,
     ):
         self.results = []
         self.csv_file = None
         self.save_results_at_frequency = None
         self.add_wallclock_time = add_wallclock_time
+        self._extra_results_composer = extra_results_composer
         self._start_time_stamp = None
+        self._tuner = None
 
     def _set_time_fields(self, result: Dict[str, Any]):
         """
         Note that we only add wallclock time to the result if this has not
         already been done (by the backend)
         """
         if self._start_time_stamp is not None and ST_TUNER_TIME not in result:
             result[ST_TUNER_TIME] = perf_counter() - self._start_time_stamp
 
+    def _append_extra_results(self, result: Dict[str, Any]):
+        if self._extra_results_composer is not None:
+            extra_results = self._extra_results_composer(self._tuner)
+            if extra_results is not None:
+                result.update(extra_results)
+
     def on_trial_result(
         self, trial: Trial, status: str, result: Dict[str, Any], decision: str
     ):
         assert (
             self.save_results_at_frequency is not None
         ), "on_tuning_start must always be called before on_trial_result."
         result = copy.copy(result)
@@ -147,42 +110,45 @@
         result[ST_STATUS] = status
         result[ST_TRIAL_ID] = trial.trial_id
 
         for key in trial.config:
             result[f"config_{key}"] = trial.config[key]
 
         self._set_time_fields(result)
+        self._append_extra_results(result)
 
         self.results.append(result)
 
         if self.csv_file is not None:
             self.save_results_at_frequency()
 
     def store_results(self):
         """
         Store current results into CSV file, of name
-        ``{tuner.tuner_path}/results.csv.zip``.
+        ``{tuner.tuner_path}/{ST_RESULTS_DATAFRAME_FILENAME}``.
         """
         if self.csv_file is not None:
             self.dataframe().to_csv(self.csv_file, index=False)
 
     def dataframe(self) -> pd.DataFrame:
         return pd.DataFrame(self.results)
 
     def on_tuning_start(self, tuner):
-        # we set the path of the csv file once the tuner is created since the path may change when the tuner is stop
-        # and resumed again on a different machine.
-        self.csv_file = str(tuner.tuner_path / "results.csv.zip")
-
-        # we only save results every ``results_update_frequency`` seconds as this operation
-        # may be expensive on remote storage.
+        # We set the path of the csv file once the tuner is created, since the
+        # path may change when the tuner is stopped and resumed again on a
+        # different machine.
+        self.csv_file = str(tuner.tuner_path / ST_RESULTS_DATAFRAME_FILENAME)
+        # We only save results every ``results_update_frequency`` seconds as
+        # this operation may be expensive on remote storage.
         self.save_results_at_frequency = RegularCallback(
             lambda: self.store_results(),
             call_seconds_frequency=tuner.results_update_interval,
         )
         if self.add_wallclock_time:
             self._start_time_stamp = perf_counter()
+        if self._extra_results_composer is not None:
+            self._tuner = tuner
 
     def on_tuning_end(self):
-        # store the results in case some results were not committed yet (since they are saved every
-        # ``results_update_interval`` seconds)
+        # Store the results in case some results were not committed yet (since
+        # they are saved every ``results_update_interval`` seconds)
         self.store_results()
```

### Comparing `syne_tune-0.4.1/syne_tune/tuning_status.py` & `syne_tune-0.5.0/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.4.1/syne_tune/util.py` & `syne_tune-0.5.0/syne_tune/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import re
 import string
 import random
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, List, Union, Dict, Any
+from typing import Optional, List, Union, Dict, Any, Iterable
 from time import perf_counter
 from contextlib import contextmanager
 
 import numpy as np
 
 from syne_tune.constants import SYNE_TUNE_DEFAULT_FOLDER, SYNE_TUNE_ENV_FOLDER
 from syne_tune.try_import import try_import_aws_message
@@ -297,7 +297,14 @@
                     result[k] = vb
             else:
                 result[k] = va
         result.update({k: b[k] for k in keys_b})
         return result
     else:
         return a
+
+
+def find_first_of_type(a: Iterable[Any], typ) -> Optional[Any]:
+    try:
+        return next(x for x in a if isinstance(x, typ))
+    except StopIteration:
+        return None
```

### Comparing `syne_tune-0.4.1/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.5.0/syne_tune.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne-tune
-Version: 0.4.1
+Version: 0.5.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Provides-Extra: kde
 Provides-Extra: gpsearchers
 Provides-Extra: benchmarks
 Provides-Extra: blackbox-repository
 Provides-Extra: aws
 Provides-Extra: yahpo
 Provides-Extra: dev
+Provides-Extra: moo
 Provides-Extra: extra
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
@@ -49,21 +50,22 @@
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to get the latest version from git: 
+or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
+pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -73,62 +75,63 @@
 
 ## Getting started
 
 To enable tuning, you have to report metrics from a training script so that they can be communicated later to Syne Tune,
 this can be accomplished by just calling `report(epoch=epoch, loss=loss)` as shown in the example below:
 
 ```python
-# train_height.py
+# train_height_simple.py
 import logging
 import time
 
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
-
     parser = ArgumentParser()
     parser.add_argument('--steps', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
-
     args, _ = parser.parse_known_args()
     report = Reporter()
-
     for step in range(args.steps):
-        dummy_score = (0.1 + args.width * step / 100) ** (-1) + args.height * 0.1
-        # Feed the score back to Syne Tune.
-        report(step=step, mean_loss=dummy_score, epoch=step + 1)
         time.sleep(0.1)
+        dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
+        # Feed the score back to Syne Tune.
+        report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
 
 ```python
+# launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
 
 # hyperparameter search space to consider
 config_space = {
-    'steps': 100,
     'width': randint(1, 20),
     'height': randint(1, 20),
+    'epochs': 100,
 }
 
 tuner = Tuner(
     trial_backend=LocalBackend(entry_point='train_height.py'),
     scheduler=ASHA(
-        config_space, metric='mean_loss', resource_attr='epoch', max_t=100,
+        config_space,
+        metric='mean_loss',
+        resource_attr='epoch',
+        max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
-    stop_criterion=StoppingCriterion(max_wallclock_time=15),
+    stop_criterion=StoppingCriterion(max_wallclock_time=30),
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
@@ -146,15 +149,16 @@
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
-HyperTune | Li, et al. (2022) | model-based | yes | yes | no 
+HyperTune | Li, et al. (2022) | model-based | yes | yes | no
+DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
@@ -172,87 +176,101 @@
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
-You will find the following examples in [examples/](examples/) folder illustrating different functionalities provided
-by Syne Tune:
+You will find many examples in the [examples/](examples/) folder illustrating
+different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
   [train_height_example.py](examples/training_scripts/height_example/train_height.py) for several baselines  
-* [launch_height_ray.py](examples/launch_height_ray.py):
-  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
-  scheduler
 * [launch_height_moasha.py](examples/launch_height_moasha.py):
   shows how to tune a script reporting multiple-objectives with multiobjective Asynchronous Hyperband (MOASHA)
 * [launch_height_standalone_scheduler.py](examples/launch_height_standalone_scheduler.py):
   launches HPO locally with a custom scheduler that cuts any trial that is not
   in the top 80%
 * [launch_height_sagemaker_remotely.py](examples/launch_height_sagemaker_remotely.py):
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
+* [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
+  launches Bayesian contrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
   launches HPO on SageMaker to tune a entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
+* [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
+  shows how results can be visualized on the fly with TensorBoard
+* [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
+  demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
-launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
-employs an easy-to-use benchmark convention
+  launches HPO locally tuning a multi-layer perceptron on Fashion MNIST. This
+  employs an easy-to-use benchmark convention
 * [launch_huggingface_classification.py](examples/launch_huggingface_classification.py):
   launches HPO on SageMaker to tune a SageMaker Hugging Face estimator for sentiment classification
 * [launch_tuning_gluonts.py](examples/launch_tuning_gluonts.py):
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
+* [launch_height_ray.py](examples/launch_height_ray.py):
+  launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
+  scheduler
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
 * [How can I run on AWS and SageMaker?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-on-aws-and-sagemaker)
 * [What are the metrics reported by default when calling the `Reporter`?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-metrics-reported-by-default-when-calling-the-reporter)
 * [How can I utilize multiple GPUs?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-utilize-multiple-gpus)
 * [What is the default mode when performing optimization?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-is-the-default-mode-when-performing-optimization)
 * [How are trials evaluated on a local machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-are-trials-evaluated-on-a-local-machine)
-* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [Where can I find the output of the tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-the-tuning)
+* [How can I change the default output folder where tuning results are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-change-the-default-output-folder-where-tuning-results-are-stored)
+* [What does the output of the tuning contain?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-does-the-output-of-the-tuning-contain)
 * [How can I enable trial checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-enable-trial-checkpointing)
+* [How can I retrieve the best checkpoint obtained after tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-retrieve-the-best-checkpoint-obtained-after-tuning)
 * [Which schedulers make use of checkpointing?](https://syne-tune.readthedocs.io/en/latest/faq.html#which-schedulers-make-use-of-checkpointing)
 * [Is the tuner checkpointed?](https://syne-tune.readthedocs.io/en/latest/faq.html#is-the-tuner-checkpointed)
 * [Where can I find the output of my trials?](https://syne-tune.readthedocs.io/en/latest/faq.html#where-can-i-find-the-output-of-my-trials)
 * [How can I plot the results of a tuning?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-plot-the-results-of-a-tuning)
 * [How can I specify additional tuning metadata?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-additional-tuning-metadata)
 * [How do I append additional information to the results which are stored?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-append-additional-information-to-the-results-which-are-stored) 
 * [I don’t want to wait, how can I launch the tuning on a remote machine?](https://syne-tune.readthedocs.io/en/latest/faq.html#i-dont-want-to-wait-how-can-i-launch-the-tuning-on-a-remote-machine)
 * [How can I run many experiments in parallel?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-run-many-experiments-in-parallel)
 * [How can I access results after tuning remotely?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-access-results-after-tuning-remotely)
 * [How can I specify dependencies to remote launcher or when using the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-specify-dependencies-to-remote-launcher-or-when-using-the-sagemaker-backend)
 * [How can I benchmark different methods?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-benchmark-different-methods)
 * [What different schedulers do you support? What are the main differences between them?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-different-schedulers-do-you-support-what-are-the-main-differences-between-them)
 * [How do I define the search space?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-define-the-search-space) 
+* [How do I set arguments of multi-fidelity schedulers?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-do-i-set-arguments-of-multi-fidelity-schedulers)
 * [How can I visualize the progress of my tuning experiment with Tensorboard?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-visualize-the-progress-of-my-tuning-experiment-with-tensorboard)
 * [How can I add a new scheduler?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-scheduler)
 * [How can I add a new tabular or surrogate benchmark?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-add-a-new-tabular-or-surrogate-benchmark)
+* [How can I reduce delays in starting trials with the SageMaker backend?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-reduce-delays-in-starting-trials-with-the-sageMaker-backend)
+* [How can I pass lists or dictionaries to the training script?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-pass-lists-or-dictionaries-to-the-training-script)
+* [How can I write extra results for an experiment?](https://syne-tune.readthedocs.io/en/latest/faq.html#how-can-i-write-extra-results-for-an-experiment)
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
-* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
-* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
-* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
+* [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
+* [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
+* [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
+* [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.4.1/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.5.0/syne_tune.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 syne_tune/__init__.py
 syne_tune/config_space.py
 syne_tune/constants.py
 syne_tune/experiments.py
 syne_tune/num_gpu.py
 syne_tune/report.py
+syne_tune/results_callback.py
 syne_tune/stopping_criterion.py
 syne_tune/try_import.py
 syne_tune/tuner.py
 syne_tune/tuner_callback.py
 syne_tune/tuning_status.py
 syne_tune/util.py
 syne_tune/version
@@ -60,48 +61,55 @@
 syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
 syne_tune/callbacks/__init__.py
+syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+syne_tune/callbacks/remove_checkpoints_callback.py
 syne_tune/callbacks/tensorboard_callback.py
 syne_tune/optimizer/__init__.py
 syne_tune/optimizer/baselines.py
 syne_tune/optimizer/scheduler.py
 syne_tune/optimizer/schedulers/__init__.py
 syne_tune/optimizer/schedulers/fifo.py
 syne_tune/optimizer/schedulers/hyperband.py
+syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
 syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
 syne_tune/optimizer/schedulers/hyperband_pasha.py
 syne_tune/optimizer/schedulers/hyperband_promotion.py
 syne_tune/optimizer/schedulers/hyperband_rush.py
 syne_tune/optimizer/schedulers/hyperband_stopping.py
 syne_tune/optimizer/schedulers/median_stopping_rule.py
 syne_tune/optimizer/schedulers/multi_fidelity.py
 syne_tune/optimizer/schedulers/pbt.py
 syne_tune/optimizer/schedulers/random_seeds.py
 syne_tune/optimizer/schedulers/ray_scheduler.py
+syne_tune/optimizer/schedulers/remove_checkpoints.py
 syne_tune/optimizer/schedulers/scheduler_searcher.py
 syne_tune/optimizer/schedulers/multiobjective/__init__.py
+syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
 syne_tune/optimizer/schedulers/multiobjective/moasha.py
+syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
 syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
 syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+syne_tune/optimizer/schedulers/multiobjective/utils.py
 syne_tune/optimizer/schedulers/neuralbands/__init__.py
 syne_tune/optimizer/schedulers/neuralbands/networks.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
 syne_tune/optimizer/schedulers/searchers/__init__.py
 syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
 syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
 syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
 syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
 syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
 syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
-syne_tune/optimizer/schedulers/searchers/multi_objective_regularized_evolution.py
 syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
 syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
 syne_tune/optimizer/schedulers/searchers/searcher.py
 syne_tune/optimizer/schedulers/searchers/searcher_base.py
 syne_tune/optimizer/schedulers/searchers/searcher_callback.py
 syne_tune/optimizer/schedulers/searchers/searcher_factory.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
@@ -157,15 +165,16 @@
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
@@ -227,8 +236,12 @@
 syne_tune/optimizer/schedulers/utils/__init__.py
 syne_tune/optimizer/schedulers/utils/simple_profiler.py
 syne_tune/optimizer/schedulers/utils/successive_halving.py
 syne_tune/remote/__init__.py
 syne_tune/remote/estimators.py
 syne_tune/remote/remote_launcher.py
 syne_tune/remote/remote_main.py
-syne_tune/remote/remote_metrics_callback.py
+syne_tune/remote/remote_metrics_callback.py
+syne_tune/utils/__init__.py
+syne_tune/utils/checkpoint.py
+syne_tune/utils/config_as_json.py
+syne_tune/utils/parse_bool.py
```

### Comparing `syne_tune-0.4.1/syne_tune.egg-info/requires.txt` & `syne_tune-0.5.0/syne_tune.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 numpy<1.24.0,>=1.16.0
 dill>=0.3.6
 pandas
 typing_extensions
+sortedcontainers
 
 [aws]
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 
 [benchmarks]
+torchvision
+filelock
 tqdm
 torch
-filelock
-torchvision
 
 [blackbox-repository]
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet
 s3fs
 scikit-learn
@@ -47,18 +48,18 @@
 
 [extra]
 ray[tune]>=2.0.0
 scikit-learn
 scikit-optimize
 scipy>=1.3.3
 autograd>=1.3
+torchvision
+filelock
 tqdm
 torch
-filelock
-torchvision
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet
 s3fs
 xgboost
 h5py
 statsmodels
@@ -77,23 +78,27 @@
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 onnxruntime>=1.10.0
 configspace
 yahpo-gym
+pymoo>=0.6.0
 botorch>=0.7.2
 
 [gpsearchers]
 scipy>=1.3.3
 autograd>=1.3
 
 [kde]
 statsmodels
 
+[moo]
+pymoo>=0.6.0
+
 [raytune]
 ray[tune]>=2.0.0
 scikit-learn
 scikit-optimize
 
 [yahpo]
 onnxruntime>=1.10.0
```

