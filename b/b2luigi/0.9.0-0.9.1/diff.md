# Comparing `tmp/b2luigi-0.9.0.tar.gz` & `tmp/b2luigi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2luigi-0.9.0.tar", last modified: Mon Mar 20 14:33:58 2023, max compression
+gzip compressed data, was "b2luigi-0.9.1.tar", last modified: Wed Mar 29 22:14:16 2023, max compression
```

## Comparing `b2luigi-0.9.0.tar` & `b2luigi-0.9.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0      136 2023-01-13 18:57:20.852507 b2luigi-0.9.0/.bumpversion.cfg
--rw-r--r--   0        0        0      168 2022-04-05 19:08:00.604171 b2luigi-0.9.0/.github/labeler.yml
--rw-r--r--   0        0        0      606 2021-04-19 15:35:29.820283 b2luigi-0.9.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      229 2022-04-05 19:08:00.604171 b2luigi-0.9.0/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1539 2021-04-19 15:35:29.823616 b2luigi-0.9.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1233 2020-05-12 18:06:28.503934 b2luigi-0.9.0/.gitignore
--rw-r--r--   0        0        0      477 2023-01-13 18:37:12.195881 b2luigi-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       51 2020-02-06 08:03:49.471804 b2luigi-0.9.0/.readthedocs.yml
--rw-r--r--   0        0        0    19057 2023-03-20 14:22:20.354202 b2luigi-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     3358 2020-02-06 08:03:49.471804 b2luigi-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       91 2020-02-06 08:03:49.471804 b2luigi-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    32422 2020-02-06 08:03:49.475137 b2luigi-0.9.0/LICENSE
--rw-r--r--   0        0        0     1858 2021-11-16 14:01:26.170412 b2luigi-0.9.0/README.rst
--rw-r--r--   0        0        0     5860 2023-03-20 14:19:34.255576 b2luigi-0.9.0/b2luigi/__init__.py
--rw-r--r--   0        0        0      242 2021-04-19 15:35:29.823616 b2luigi-0.9.0/b2luigi/basf2_helper/__init__.py
--rw-r--r--   0        0        0     6754 2021-04-19 15:35:29.823616 b2luigi-0.9.0/b2luigi/basf2_helper/data.py
--rw-r--r--   0        0        0      282 2021-04-19 15:35:29.823616 b2luigi-0.9.0/b2luigi/basf2_helper/targets.py
--rw-r--r--   0        0        0     3627 2021-09-15 12:07:31.577226 b2luigi-0.9.0/b2luigi/basf2_helper/tasks.py
--rw-r--r--   0        0        0      377 2021-04-19 15:35:29.826950 b2luigi-0.9.0/b2luigi/basf2_helper/utils.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.0/b2luigi/batch/__init__.py
--rw-r--r--   0        0        0     1110 2022-01-08 01:24:00.082163 b2luigi-0.9.0/b2luigi/batch/cache.py
--rw-r--r--   0        0        0     7470 2021-04-19 15:35:29.826950 b2luigi-0.9.0/b2luigi/batch/processes/__init__.py
--rw-r--r--   0        0        0    64567 2023-03-20 14:18:09.989608 b2luigi-0.9.0/b2luigi/batch/processes/gbasf2.py
--rwxr-xr-x   0        0        0      968 2022-10-07 15:37:00.857191 b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py
--rwxr-xr-x   0        0        0     2593 2022-11-14 11:09:44.556064 b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py
--rwxr-xr-x   0        0        0     1061 2022-10-07 15:37:00.857191 b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py
--rw-r--r--   0        0        0     1431 2022-10-07 15:37:00.857191 b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py
--rw-r--r--   0        0        0    11061 2022-08-25 15:07:10.097728 b2luigi-0.9.0/b2luigi/batch/processes/htcondor.py
--rw-r--r--   0        0        0     3649 2021-04-19 15:35:29.830283 b2luigi-0.9.0/b2luigi/batch/processes/lsf.py
--rwxr-xr-x   0        0        0     1540 2022-10-07 15:37:00.857191 b2luigi-0.9.0/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2
--rw-r--r--   0        0        0     1347 2021-04-19 15:35:29.830283 b2luigi-0.9.0/b2luigi/batch/processes/test.py
--rw-r--r--   0        0        0     1684 2023-03-17 14:41:39.044701 b2luigi-0.9.0/b2luigi/batch/workers.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.0/b2luigi/cli/__init__.py
--rw-r--r--   0        0        0     2515 2021-11-16 14:01:26.173745 b2luigi-0.9.0/b2luigi/cli/arguments.py
--rw-r--r--   0        0        0     4310 2021-04-19 15:35:29.833616 b2luigi-0.9.0/b2luigi/cli/process.py
--rw-r--r--   0        0        0     3888 2021-04-19 15:35:29.833616 b2luigi-0.9.0/b2luigi/cli/runner.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.0/b2luigi/core/__init__.py
--rw-r--r--   0        0        0     3041 2021-11-23 15:40:39.312670 b2luigi-0.9.0/b2luigi/core/dispatchable_task.py
--rw-r--r--   0        0        0     3636 2021-04-19 15:35:29.836950 b2luigi-0.9.0/b2luigi/core/executable.py
--rw-r--r--   0        0        0     1230 2020-12-14 17:27:18.844556 b2luigi-0.9.0/b2luigi/core/parameter.py
--rw-r--r--   0        0        0     5338 2021-04-19 15:35:29.836950 b2luigi-0.9.0/b2luigi/core/settings.py
--rw-r--r--   0        0        0     8924 2021-07-14 19:39:19.067382 b2luigi-0.9.0/b2luigi/core/task.py
--rw-r--r--   0        0        0     3178 2021-11-18 14:40:16.375973 b2luigi-0.9.0/b2luigi/core/temporary_wrapper.py
--rw-r--r--   0        0        0    11487 2023-03-20 13:02:23.915837 b2luigi-0.9.0/b2luigi/core/utils.py
--rw-r--r--   0        0        0      605 2021-04-19 15:35:29.836950 b2luigi-0.9.0/docs/Makefile
--rw-r--r--   0        0        0     5417 2021-08-03 10:35:07.243570 b2luigi-0.9.0/docs/advanced/basf2-examples.rst
--rw-r--r--   0        0        0     4278 2022-11-14 11:16:46.018025 b2luigi-0.9.0/docs/advanced/development.rst
--rw-r--r--   0        0        0     4248 2021-04-19 15:35:29.840283 b2luigi-0.9.0/docs/advanced/faq.rst
--rw-r--r--   0        0        0     5130 2023-03-20 14:20:06.798640 b2luigi-0.9.0/docs/conf.py
--rw-r--r--   0        0        0     2526 2021-04-19 15:35:29.840283 b2luigi-0.9.0/docs/documentation/api.rst
--rw-r--r--   0        0        0      751 2021-03-26 16:18:36.506513 b2luigi-0.9.0/docs/documentation/b2luigi.basf2_helper.rst
--rw-r--r--   0        0        0     3528 2021-07-14 12:29:39.595620 b2luigi-0.9.0/docs/documentation/run_modes.rst
--rw-r--r--   0        0        0     6114 2023-03-20 13:02:23.919170 b2luigi-0.9.0/docs/index.rst
--rw-r--r--   0        0        0     6275 2020-05-27 12:08:37.450453 b2luigi-0.9.0/docs/usage/batch.rst
--rw-r--r--   0        0        0     2114 2021-11-16 14:01:26.173745 b2luigi-0.9.0/docs/usage/installation.rst
--rw-r--r--   0        0        0     7852 2021-11-23 15:40:39.312670 b2luigi-0.9.0/docs/usage/quickstart.rst
--rw-r--r--   0        0        0     4453 2022-10-07 15:37:00.857191 b2luigi-0.9.0/examples/basf2/basf2_chain_example.py
--rw-r--r--   0        0        0     2620 2022-10-07 15:37:00.857191 b2luigi-0.9.0/examples/gbasf2/example_mdst_analysis.py
--rw-r--r--   0        0        0     2193 2022-10-07 15:37:00.857191 b2luigi-0.9.0/examples/gbasf2/gbasf2_example.py
--rw-r--r--   0        0        0      133 2022-10-07 15:37:00.857191 b2luigi-0.9.0/examples/gbasf2/settings.json
--rw-r--r--   0        0        0     1466 2021-11-23 15:40:39.312670 b2luigi-0.9.0/examples/htcondor/htcondor_example.py
--rw-r--r--   0        0        0      182 2021-11-23 16:24:47.181004 b2luigi-0.9.0/examples/htcondor/settings.json
--rw-r--r--   0        0        0       50 2021-11-03 15:23:14.408281 b2luigi-0.9.0/examples/htcondor/setup_script.sh
--rw-r--r--   0        0        0      442 2022-08-25 15:07:10.097728 b2luigi-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      392 2021-04-19 15:35:29.846949 b2luigi-0.9.0/setup.cfg
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.106721 b2luigi-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.110055 b2luigi-0.9.0/tests/batch/__init__.py
--rw-r--r--   0        0        0    17959 2021-10-20 18:18:44.110055 b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json
--rw-r--r--   0        0        0    17971 2021-10-20 18:18:44.110055 b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json
--rw-r--r--   0        0        0     5690 2021-10-20 18:18:44.110055 b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json
--rw-r--r--   0        0        0   164412 2021-10-20 18:18:44.113388 b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json
--rw-r--r--   0        0        0      858 2021-10-20 18:18:44.113388 b2luigi-0.9.0/tests/batch/batch_task_1.py
--rw-r--r--   0        0        0      782 2021-10-20 18:18:44.113388 b2luigi-0.9.0/tests/batch/batch_task_2.py
--rw-r--r--   0        0        0      880 2021-10-20 18:18:44.113388 b2luigi-0.9.0/tests/batch/test_batch_process.py
--rw-r--r--   0        0        0    18499 2023-03-20 14:18:09.989608 b2luigi-0.9.0/tests/batch/test_gbasf2_helper_functions.py
--rw-r--r--   0        0        0    10865 2023-03-20 14:18:09.989608 b2luigi-0.9.0/tests/batch/test_gbasf2_process.py
--rw-r--r--   0        0        0     5689 2022-01-08 01:24:00.085497 b2luigi-0.9.0/tests/batch/test_htcondor_processs.py
--rw-r--r--   0        0        0        0 2021-11-16 14:01:26.173745 b2luigi-0.9.0/tests/cli/__init__.py
--rw-r--r--   0        0        0     1397 2021-11-16 14:01:26.173745 b2luigi-0.9.0/tests/cli/process_with_user_args_ignored_by_b2luigi.py
--rw-r--r--   0        0        0      562 2021-11-16 14:01:26.173745 b2luigi-0.9.0/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py
--rw-r--r--   0        0        0     1003 2021-11-16 14:01:26.173745 b2luigi-0.9.0/tests/cli/test_ignore_additional_command_line_args.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/__init__.py
--rw-r--r--   0        0        0      662 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/dispatch_1.py
--rw-r--r--   0        0        0      668 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/dispatch_2.py
--rw-r--r--   0        0        0      602 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/dispatch_with_env_and_script.py
--rw-r--r--   0        0        0      368 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/folder_structures.py
--rw-r--r--   0        0        0      350 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/temporary_task_1.py
--rw-r--r--   0        0        0      319 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/temporary_task_2.py
--rw-r--r--   0        0        0     1750 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/test_dispatch_task.py
--rw-r--r--   0        0        0      824 2021-10-20 18:18:44.116721 b2luigi-0.9.0/tests/core/test_folder_structures.py
--rw-r--r--   0        0        0     1700 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/core/test_parameter.py
--rw-r--r--   0        0        0     3984 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/core/test_requires.py
--rw-r--r--   0        0        0     3079 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/core/test_settings.py
--rw-r--r--   0        0        0     3493 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/core/test_task.py
--rw-r--r--   0        0        0      930 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/core/test_temporary_files.py
--rw-r--r--   0        0        0     9422 2023-03-20 13:02:23.919170 b2luigi-0.9.0/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/doc_examples/__init__.py
--rw-r--r--   0        0        0     1876 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/doc_examples/dict_requirement_example.py
--rw-r--r--   0        0        0       29 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/doc_examples/settings.json
--rw-r--r--   0        0        0      547 2021-10-20 18:18:44.120055 b2luigi-0.9.0/tests/doc_examples/simple_example.py
--rw-r--r--   0        0        0      547 2021-10-20 18:18:44.123388 b2luigi-0.9.0/tests/doc_examples/simple_example_b2luigi.py
--rw-r--r--   0        0        0     1149 2021-10-20 18:18:44.123388 b2luigi-0.9.0/tests/doc_examples/simple_example_b2luigi_2.py
--rw-r--r--   0        0        0      482 2021-10-20 18:18:44.123388 b2luigi-0.9.0/tests/doc_examples/test_examples.py
--rw-r--r--   0        0        0      906 2021-11-16 14:01:26.173745 b2luigi-0.9.0/tests/helpers.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 b2luigi-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2023-03-29 22:11:46.367240 b2luigi-0.9.1/.bumpversion.cfg
+-rw-r--r--   0        0        0      168 2022-04-05 19:08:00.604171 b2luigi-0.9.1/.github/labeler.yml
+-rw-r--r--   0        0        0      606 2021-04-19 15:35:29.820283 b2luigi-0.9.1/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      229 2022-04-05 19:08:00.604171 b2luigi-0.9.1/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1539 2021-04-19 15:35:29.823616 b2luigi-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1233 2020-05-12 18:06:28.503934 b2luigi-0.9.1/.gitignore
+-rw-r--r--   0        0        0      477 2023-01-13 18:37:12.195881 b2luigi-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       51 2020-02-06 08:03:49.471804 b2luigi-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0    19777 2023-03-29 22:11:46.370573 b2luigi-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3358 2020-02-06 08:03:49.471804 b2luigi-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       91 2020-02-06 08:03:49.471804 b2luigi-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    32422 2020-02-06 08:03:49.475137 b2luigi-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1858 2021-11-16 14:01:26.170412 b2luigi-0.9.1/README.rst
+-rw-r--r--   0        0        0     5859 2023-03-29 22:11:46.370573 b2luigi-0.9.1/b2luigi/__init__.py
+-rw-r--r--   0        0        0      242 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/__init__.py
+-rw-r--r--   0        0        0     6754 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/data.py
+-rw-r--r--   0        0        0      282 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/targets.py
+-rw-r--r--   0        0        0     3627 2021-09-15 12:07:31.577226 b2luigi-0.9.1/b2luigi/basf2_helper/tasks.py
+-rw-r--r--   0        0        0      377 2021-04-19 15:35:29.826950 b2luigi-0.9.1/b2luigi/basf2_helper/utils.py
+-rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/batch/__init__.py
+-rw-r--r--   0        0        0     1110 2022-01-08 01:24:00.082163 b2luigi-0.9.1/b2luigi/batch/cache.py
+-rw-r--r--   0        0        0     7470 2021-04-19 15:35:29.826950 b2luigi-0.9.1/b2luigi/batch/processes/__init__.py
+-rw-r--r--   0        0        0    64579 2023-03-29 17:06:46.273750 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2.py
+-rwxr-xr-x   0        0        0      968 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py
+-rwxr-xr-x   0        0        0     2593 2022-11-14 11:09:44.556064 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py
+-rwxr-xr-x   0        0        0     1061 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py
+-rw-r--r--   0        0        0     1431 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py
+-rw-r--r--   0        0        0    11061 2022-08-25 15:07:10.097728 b2luigi-0.9.1/b2luigi/batch/processes/htcondor.py
+-rw-r--r--   0        0        0     3649 2021-04-19 15:35:29.830283 b2luigi-0.9.1/b2luigi/batch/processes/lsf.py
+-rwxr-xr-x   0        0        0     1540 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2
+-rw-r--r--   0        0        0     1347 2021-04-19 15:35:29.830283 b2luigi-0.9.1/b2luigi/batch/processes/test.py
+-rw-r--r--   0        0        0     1684 2023-03-17 14:41:39.044701 b2luigi-0.9.1/b2luigi/batch/workers.py
+-rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/cli/__init__.py
+-rw-r--r--   0        0        0     2515 2021-11-16 14:01:26.173745 b2luigi-0.9.1/b2luigi/cli/arguments.py
+-rw-r--r--   0        0        0     4310 2021-04-19 15:35:29.833616 b2luigi-0.9.1/b2luigi/cli/process.py
+-rw-r--r--   0        0        0     3888 2021-04-19 15:35:29.833616 b2luigi-0.9.1/b2luigi/cli/runner.py
+-rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/core/__init__.py
+-rw-r--r--   0        0        0     3041 2021-11-23 15:40:39.312670 b2luigi-0.9.1/b2luigi/core/dispatchable_task.py
+-rw-r--r--   0        0        0     3636 2021-04-19 15:35:29.836950 b2luigi-0.9.1/b2luigi/core/executable.py
+-rw-r--r--   0        0        0     1939 2023-03-29 15:56:55.436388 b2luigi-0.9.1/b2luigi/core/parameter.py
+-rw-r--r--   0        0        0     5338 2021-04-19 15:35:29.836950 b2luigi-0.9.1/b2luigi/core/settings.py
+-rw-r--r--   0        0        0     8924 2021-07-14 19:39:19.067382 b2luigi-0.9.1/b2luigi/core/task.py
+-rw-r--r--   0        0        0     3178 2021-11-18 14:40:16.375973 b2luigi-0.9.1/b2luigi/core/temporary_wrapper.py
+-rw-r--r--   0        0        0    11487 2023-03-20 13:02:23.915837 b2luigi-0.9.1/b2luigi/core/utils.py
+-rw-r--r--   0        0        0      605 2021-04-19 15:35:29.836950 b2luigi-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0     5417 2021-08-03 10:35:07.243570 b2luigi-0.9.1/docs/advanced/basf2-examples.rst
+-rw-r--r--   0        0        0     4278 2022-11-14 11:16:46.018025 b2luigi-0.9.1/docs/advanced/development.rst
+-rw-r--r--   0        0        0     4248 2021-04-19 15:35:29.840283 b2luigi-0.9.1/docs/advanced/faq.rst
+-rw-r--r--   0        0        0     5130 2023-03-29 22:11:46.370573 b2luigi-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0     2526 2021-04-19 15:35:29.840283 b2luigi-0.9.1/docs/documentation/api.rst
+-rw-r--r--   0        0        0      751 2021-03-26 16:18:36.506513 b2luigi-0.9.1/docs/documentation/b2luigi.basf2_helper.rst
+-rw-r--r--   0        0        0     3528 2021-07-14 12:29:39.595620 b2luigi-0.9.1/docs/documentation/run_modes.rst
+-rw-r--r--   0        0        0     6114 2023-03-20 13:02:23.919170 b2luigi-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0     6275 2020-05-27 12:08:37.450453 b2luigi-0.9.1/docs/usage/batch.rst
+-rw-r--r--   0        0        0     2114 2021-11-16 14:01:26.173745 b2luigi-0.9.1/docs/usage/installation.rst
+-rw-r--r--   0        0        0     7852 2021-11-23 15:40:39.312670 b2luigi-0.9.1/docs/usage/quickstart.rst
+-rw-r--r--   0        0        0     4453 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/basf2/basf2_chain_example.py
+-rw-r--r--   0        0        0     2620 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/example_mdst_analysis.py
+-rw-r--r--   0        0        0     2193 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/gbasf2_example.py
+-rw-r--r--   0        0        0      133 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/settings.json
+-rw-r--r--   0        0        0     1466 2021-11-23 15:40:39.312670 b2luigi-0.9.1/examples/htcondor/htcondor_example.py
+-rw-r--r--   0        0        0      182 2021-11-23 16:24:47.181004 b2luigi-0.9.1/examples/htcondor/settings.json
+-rw-r--r--   0        0        0       50 2021-11-03 15:23:14.408281 b2luigi-0.9.1/examples/htcondor/setup_script.sh
+-rw-r--r--   0        0        0      442 2022-08-25 15:07:10.097728 b2luigi-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      392 2021-04-19 15:35:29.846949 b2luigi-0.9.1/setup.cfg
+-rw-r--r--   0        0        0        0 2021-10-20 18:18:44.106721 b2luigi-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/__init__.py
+-rw-r--r--   0        0        0    17959 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json
+-rw-r--r--   0        0        0    17971 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json
+-rw-r--r--   0        0        0     5690 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json
+-rw-r--r--   0        0        0   164412 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json
+-rw-r--r--   0        0        0      858 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/batch_task_1.py
+-rw-r--r--   0        0        0      782 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/batch_task_2.py
+-rw-r--r--   0        0        0      880 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/test_batch_process.py
+-rw-r--r--   0        0        0    18499 2023-03-20 14:18:09.989608 b2luigi-0.9.1/tests/batch/test_gbasf2_helper_functions.py
+-rw-r--r--   0        0        0    10865 2023-03-20 14:18:09.989608 b2luigi-0.9.1/tests/batch/test_gbasf2_process.py
+-rw-r--r--   0        0        0     5689 2022-01-08 01:24:00.085497 b2luigi-0.9.1/tests/batch/test_htcondor_processs.py
+-rw-r--r--   0        0        0        0 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     1397 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/process_with_user_args_ignored_by_b2luigi.py
+-rw-r--r--   0        0        0      562 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py
+-rw-r--r--   0        0        0     1003 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/test_ignore_additional_command_line_args.py
+-rw-r--r--   0        0        0        0 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/__init__.py
+-rw-r--r--   0        0        0      662 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_1.py
+-rw-r--r--   0        0        0      668 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_2.py
+-rw-r--r--   0        0        0      602 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_with_env_and_script.py
+-rw-r--r--   0        0        0      368 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/folder_structures.py
+-rw-r--r--   0        0        0      350 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/temporary_task_1.py
+-rw-r--r--   0        0        0      319 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/temporary_task_2.py
+-rw-r--r--   0        0        0     1750 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/test_dispatch_task.py
+-rw-r--r--   0        0        0      824 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/test_folder_structures.py
+-rw-r--r--   0        0        0     2168 2023-03-29 15:56:55.446388 b2luigi-0.9.1/tests/core/test_parameter.py
+-rw-r--r--   0        0        0     3984 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_requires.py
+-rw-r--r--   0        0        0     3079 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_settings.py
+-rw-r--r--   0        0        0     3493 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_task.py
+-rw-r--r--   0        0        0      930 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_temporary_files.py
+-rw-r--r--   0        0        0     9422 2023-03-20 13:02:23.919170 b2luigi-0.9.1/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/__init__.py
+-rw-r--r--   0        0        0     1876 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/dict_requirement_example.py
+-rw-r--r--   0        0        0       29 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/settings.json
+-rw-r--r--   0        0        0      547 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/simple_example.py
+-rw-r--r--   0        0        0      547 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi.py
+-rw-r--r--   0        0        0     1149 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi_2.py
+-rw-r--r--   0        0        0      482 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/test_examples.py
+-rw-r--r--   0        0        0      906 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/helpers.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 b2luigi-0.9.1/PKG-INFO
```

### Comparing `b2luigi-0.9.0/.github/workflows/deploy.yml` & `b2luigi-0.9.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/.github/workflows/test.yml` & `b2luigi-0.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/.gitignore` & `b2luigi-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/CHANGELOG.md` & `b2luigi-0.9.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 Older entries have been generated from github releases.
 New entries aim to adhere to the format proposed by [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## [0.9.1] - 2023-03-20
+
+### Fixed
+
+- Fix circular import [#188](https://github.com/nils-braun/b2luigi/issues/188)
+
+### Added
+
+- Add the ability to pass a custom hashing function to parameters via the `hash_function` keyword argument. The function must take one argument, the value of the parameter. It is up to the user to ensure unique strings are created. [#189](https://github.com/nils-braun/b2luigi/pull/189)
+- **gbasf2**: Switch to the `--new` flag in `gb2_ds_get` which downloads files significantly faster than previously. Gbasf2 release v5r6 (November 2022) is required. [#190](https://github.com/nils-braun/b2luigi/pull/190).
+
+**Full Changelog**: https://github.com/nils-braun/b2luigi/compare/v0.9.1...v0.9.0
+
 ## [0.9.0] - 2023-03-20
 
 ### Fixed
 
 - **gbasf2**: Fix bug introduced in [#181](https://github.com/nils-braun/b2luigi/pull/181) when generating basf2 queries with just a simple `.root` extension, raising a wrong false positive errors. Now moved splitting functionality into separate function and added extensive unit tests. Thanks @schmitca for reporting [#184](https://github.com/nils-braun/b2luigi/pull/184).
 
 ### Added
```

### Comparing `b2luigi-0.9.0/CODE_OF_CONDUCT.md` & `b2luigi-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/LICENSE` & `b2luigi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/README.rst` & `b2luigi-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/__init__.py` & `b2luigi-0.9.1/b2luigi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Task scheduling and batch running for basf2 jobs made simple"""
 from luigi import *
 from luigi.util import copies
 
-from b2luigi.cli.process import process
-from b2luigi.core.dispatchable_task import DispatchableTask, dispatch
-from b2luigi.core.settings import clear_setting, get_setting, set_setting
-from b2luigi.core.task import ExternalTask, Task, WrapperTask
-from b2luigi.core.temporary_wrapper import on_temporary_files
-
 # version must be defined after importing the luigi namespace,
 # otherwise the b2luigi.__version__ gets overwritten by the one from luigi
-__version__ = "0.9.0"
-
-from typing import Collection, Optional, Union
+__version__ = "0.9.1"
 
-from b2luigi.core.parameter import BoolParameter, wrap_parameter
+from b2luigi.core.parameter import wrap_parameter, BoolParameter
+from typing import Optional, Union, Collection
 
 wrap_parameter()
 
+from b2luigi.core.task import Task, ExternalTask, WrapperTask
+from b2luigi.core.temporary_wrapper import on_temporary_files
+from b2luigi.core.dispatchable_task import DispatchableTask, dispatch
+from b2luigi.core.settings import get_setting, set_setting, clear_setting
+from b2luigi.cli.process import process
+
 
 class requires(object):
     """
     This "hack" copies the luigi.requires functionality, except that we allow for
     additional kwarg arguments when called.
 
     It can be used to require a certain task, but with some variables already set,
```

### Comparing `b2luigi-0.9.0/b2luigi/basf2_helper/data.py` & `b2luigi-0.9.1/b2luigi/basf2_helper/data.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/basf2_helper/tasks.py` & `b2luigi-0.9.1/b2luigi/basf2_helper/tasks.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/cache.py` & `b2luigi-0.9.1/b2luigi/batch/cache.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/__init__.py` & `b2luigi-0.9.1/b2luigi/batch/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/gbasf2.py` & `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2.py`

 * *Files 0% similar despite different names*

```diff
@@ -799,15 +799,15 @@
             old_monitoring_failed_downloads_file = (
                 f"{monitoring_download_file_stem}_old{monitoring_downloads_file_ext}"
             )
 
             # In case of first download, the file 'monitoring_failed_downloads_file' does not exist
             if not os.path.isfile(monitoring_failed_downloads_file):
                 ds_get_command = shlex.split(
-                    f"gb2_ds_get --force {dataset_query_string} "
+                    f"gb2_ds_get --new --force {dataset_query_string} "
                     f"--failed_lfns {monitoring_failed_downloads_file}"
                 )
                 print(
                     f"Downloading dataset into\n  {tmp_output_dir_path}\n  with command\n  ",
                     " ".join(ds_get_command),
                 )
 
@@ -815,15 +815,15 @@
             else:
                 # Rename current 'monitoring_failed_downloads_file' to reuse the path in case the download fails again
                 os.rename(
                     monitoring_failed_downloads_file,
                     old_monitoring_failed_downloads_file,
                 )
                 ds_get_command = shlex.split(
-                    f"gb2_ds_get --force {dataset_query_string} "
+                    f"gb2_ds_get --new --force {dataset_query_string} "
                     f"--input_dslist {old_monitoring_failed_downloads_file} "
                     f"--failed_lfns {monitoring_failed_downloads_file}"
                 )
                 print(
                     f"Downloading remaining files into\n  {tmp_output_dir_path}\n  with command\n  ",
                     " ".join(ds_get_command),
                 )
```

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py` & `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py` & `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py` & `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py` & `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/htcondor.py` & `b2luigi-0.9.1/b2luigi/batch/processes/htcondor.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/lsf.py` & `b2luigi-0.9.1/b2luigi/batch/processes/lsf.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2` & `b2luigi-0.9.1/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/processes/test.py` & `b2luigi-0.9.1/b2luigi/batch/processes/test.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/batch/workers.py` & `b2luigi-0.9.1/b2luigi/batch/workers.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/cli/arguments.py` & `b2luigi-0.9.1/b2luigi/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/cli/process.py` & `b2luigi-0.9.1/b2luigi/cli/process.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/cli/runner.py` & `b2luigi-0.9.1/b2luigi/cli/runner.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/dispatchable_task.py` & `b2luigi-0.9.1/b2luigi/core/dispatchable_task.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/executable.py` & `b2luigi-0.9.1/b2luigi/core/executable.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/parameter.py` & `b2luigi-0.9.1/b2luigi/core/parameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 import hashlib
 
 import luigi
 from luigi.parameter import _no_value
+from inspect import signature
 
 
 def wrap_parameter():
     """
     Monkey patch the parameter base class (and with it all other parameters(
-    of luigi to include an additional "hashed" parameter in its constructor.
+    of luigi to include two additional parameters in its constructor:
+    "hashed" and "hash_function".
+
+    Enabling the "hashed" parameter will use a hashed version of the
+    parameter value when creating file paths our of the parameters of a task
+    instead of the value itself. By default an md5 hash is used. A custom
+    hash function can be provided via the "hash_function" parameter. This
+    function should take one input, the value of the parameter. It is up
+    to the user to ensure a unique string is created from the input.
 
-    Enabling this parameter will use a hashed version of the parameter value
-    when creating file paths our of the parameters of a task instead of the
-    value itself.
     This is especially useful when you have list, string or dict parameters,
     where the resulting file path may include "/" or "{}".
     """
     import b2luigi
     parameter_class = b2luigi.Parameter
 
     def serialize_hashed(self, x):
-        return "hashed_" + hashlib.md5(str(x).encode()).hexdigest()
+        if self.hash_function is None:
+            return "hashed_" + hashlib.md5(str(x).encode()).hexdigest()
+        else:
+            return self.hash_function(x)
 
     old_init = parameter_class.__init__
 
-    def __init__(self, hashed=False, *args, **kwargs):
+    def __init__(self, hashed=False, hash_function=None, *args, **kwargs):
         old_init(self, *args, **kwargs)
 
+        if hash_function is not None:
+            n_params = len(signature(hash_function).parameters)
+            assert n_params == 1, "Custom hash function can have only"\
+                f" 1 argument, found {n_params}"
+
+        self.hash_function = hash_function
+
         if hashed:
             self.serialize_hashed = lambda x: serialize_hashed(self, x)
 
     parameter_class.__init__ = __init__
 
 
 class BoolParameter(luigi.BoolParameter):
```

### Comparing `b2luigi-0.9.0/b2luigi/core/settings.py` & `b2luigi-0.9.1/b2luigi/core/settings.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/task.py` & `b2luigi-0.9.1/b2luigi/core/task.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/temporary_wrapper.py` & `b2luigi-0.9.1/b2luigi/core/temporary_wrapper.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/b2luigi/core/utils.py` & `b2luigi-0.9.1/b2luigi/core/utils.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/Makefile` & `b2luigi-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/advanced/basf2-examples.rst` & `b2luigi-0.9.1/docs/advanced/basf2-examples.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/advanced/development.rst` & `b2luigi-0.9.1/docs/advanced/development.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/advanced/faq.rst` & `b2luigi-0.9.1/docs/advanced/faq.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/conf.py` & `b2luigi-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 project = 'b2luigi'
 copyright = '2018, Nils Braun'
 author = 'Nils Braun'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
-release = '0.9.0'
+release = '0.9.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `b2luigi-0.9.0/docs/documentation/api.rst` & `b2luigi-0.9.1/docs/documentation/api.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/documentation/b2luigi.basf2_helper.rst` & `b2luigi-0.9.1/docs/documentation/b2luigi.basf2_helper.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/documentation/run_modes.rst` & `b2luigi-0.9.1/docs/documentation/run_modes.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/index.rst` & `b2luigi-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/usage/batch.rst` & `b2luigi-0.9.1/docs/usage/batch.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/usage/installation.rst` & `b2luigi-0.9.1/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/docs/usage/quickstart.rst` & `b2luigi-0.9.1/docs/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/examples/basf2/basf2_chain_example.py` & `b2luigi-0.9.1/examples/basf2/basf2_chain_example.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/examples/gbasf2/example_mdst_analysis.py` & `b2luigi-0.9.1/examples/gbasf2/example_mdst_analysis.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/examples/gbasf2/gbasf2_example.py` & `b2luigi-0.9.1/examples/gbasf2/gbasf2_example.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/examples/htcondor/htcondor_example.py` & `b2luigi-0.9.1/examples/htcondor/htcondor_example.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json` & `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json` & `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json` & `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json` & `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/batch_task_1.py` & `b2luigi-0.9.1/tests/batch/batch_task_1.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/batch_task_2.py` & `b2luigi-0.9.1/tests/batch/batch_task_2.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/test_batch_process.py` & `b2luigi-0.9.1/tests/batch/test_batch_process.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/test_gbasf2_helper_functions.py` & `b2luigi-0.9.1/tests/batch/test_gbasf2_helper_functions.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/test_gbasf2_process.py` & `b2luigi-0.9.1/tests/batch/test_gbasf2_process.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/batch/test_htcondor_processs.py` & `b2luigi-0.9.1/tests/batch/test_htcondor_processs.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/cli/process_with_user_args_ignored_by_b2luigi.py` & `b2luigi-0.9.1/tests/cli/process_with_user_args_ignored_by_b2luigi.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py` & `b2luigi-0.9.1/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/cli/test_ignore_additional_command_line_args.py` & `b2luigi-0.9.1/tests/cli/test_ignore_additional_command_line_args.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/dispatch_1.py` & `b2luigi-0.9.1/tests/core/dispatch_1.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/dispatch_2.py` & `b2luigi-0.9.1/tests/core/dispatch_2.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/dispatch_with_env_and_script.py` & `b2luigi-0.9.1/tests/core/dispatch_with_env_and_script.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_dispatch_task.py` & `b2luigi-0.9.1/tests/core/test_dispatch_task.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_folder_structures.py` & `b2luigi-0.9.1/tests/core/test_folder_structures.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_parameter.py` & `b2luigi-0.9.1/tests/core/test_parameter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import b2luigi
 
 from ..helpers import B2LuigiTestCase
 
 
+def custom_hash_function(x):
+    return "_".join([str(y) for y in x])
+
+
 class HashedParameterTestCase(B2LuigiTestCase):
     def test_hash_consistency(self):
         first_parameter = b2luigi.DictParameter()
         self.assertFalse(hasattr(first_parameter, "serialize_hashed"))
 
         second_parameter = b2luigi.DictParameter(hashed=True)
         self.assertTrue(hasattr(second_parameter, "serialize_hashed"))
@@ -19,22 +23,27 @@
 
         serialized_first = second_parameter.serialize_hashed([1, "test", 456, {"hello": "bye"}])
         serialized_second = second_parameter.serialize_hashed([1, "test", 457, {"hello": "bye"}])
 
         self.assertNotEqual(serialized_first, serialized_second)
         self.assertEqual(serialized_first, "hashed_7816c14282fd03e3dc4e398f28aa5a30")
 
+        third_parameter = b2luigi.ListParameter(hashed=True, hash_function=custom_hash_function)
+        serialized = third_parameter.serialize_hashed([0, 1, 2])
+        self.assertEqual(serialized, "0_1_2")
+
     def test_with_task(self):
         class MyTask(b2luigi.Task):
             my_parameter = b2luigi.ListParameter(hashed=True)
+            custom_hashed_parameter = b2luigi.ListParameter(hashed=True, hash_function=custom_hash_function)
 
             def run(self):
                 with open(self.get_output_file_name("test.txt"), "w") as f:
                     f.write("test")
 
             def output(self):
                 yield self.add_to_output("test.txt")
 
-        task = MyTask(my_parameter=["Some", "strange", "items", "with", "bad / signs"])
+        task = MyTask(my_parameter=["Some", "strange", "items", "with", "bad / signs"], custom_hashed_parameter=[0, 1, 2])
 
-        self.assertTrue(task.get_output_file_name("test.txt")
-                        .endswith("results/my_parameter=hashed_08928069d368e4a0f8ac02a0193e443b/test.txt"))
+        expected_path = "results/my_parameter=hashed_08928069d368e4a0f8ac02a0193e443b/custom_hashed_parameter=0_1_2/test.txt"
+        self.assertTrue(task.get_output_file_name("test.txt").endswith(expected_path))
```

### Comparing `b2luigi-0.9.0/tests/core/test_requires.py` & `b2luigi-0.9.1/tests/core/test_requires.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_settings.py` & `b2luigi-0.9.1/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_task.py` & `b2luigi-0.9.1/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_temporary_files.py` & `b2luigi-0.9.1/tests/core/test_temporary_files.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/core/test_utils.py` & `b2luigi-0.9.1/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/doc_examples/dict_requirement_example.py` & `b2luigi-0.9.1/tests/doc_examples/dict_requirement_example.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/doc_examples/simple_example.py` & `b2luigi-0.9.1/tests/doc_examples/simple_example.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/doc_examples/simple_example_b2luigi.py` & `b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/doc_examples/simple_example_b2luigi_2.py` & `b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi_2.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/tests/helpers.py` & `b2luigi-0.9.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.0/PKG-INFO` & `b2luigi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2luigi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Task scheduling and batch running for basf2 jobs made simple
 Home-page: https://github.com/nils-braun/b2luigi
 Author: Nils Braun
 Author-email: nils.braun@kit.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: luigi>=3.0.2
 Requires-Dist: parse>=1.8.4
```

