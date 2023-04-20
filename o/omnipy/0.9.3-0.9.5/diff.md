# Comparing `tmp/omnipy-0.9.3.tar.gz` & `tmp/omnipy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnipy-0.9.3.tar", max compression
+gzip compressed data, was "omnipy-0.9.5.tar", max compression
```

## Comparing `omnipy-0.9.3.tar` & `omnipy-0.9.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    11357 2022-08-22 11:56:15.427867 omnipy-0.9.3/LICENSE
--rw-r--r--   0        0        0    21170 2023-02-27 17:03:45.555903 omnipy-0.9.3/README.md
--rw-r--r--   0        0        0     2617 2023-03-01 06:03:02.474097 omnipy-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      358 2023-03-01 06:03:02.479022 omnipy-0.9.3/src/omnipy/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.364882 omnipy-0.9.3/src/omnipy/api/__init__.py
--rw-r--r--   0        0        0     1183 2023-02-24 09:55:13.737916 omnipy-0.9.3/src/omnipy/api/enums.py
--rw-r--r--   0        0        0       81 2023-02-03 14:24:42.365857 omnipy-0.9.3/src/omnipy/api/exceptions.py
--rw-r--r--   0        0        0    12773 2023-02-24 09:54:27.822894 omnipy-0.9.3/src/omnipy/api/protocols.py
--rw-r--r--   0        0        0      222 2023-02-14 01:53:17.083940 omnipy-0.9.3/src/omnipy/api/types.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.366814 omnipy-0.9.3/src/omnipy/compute/__init__.py
--rw-r--r--   0        0        0     3723 2023-02-03 14:24:42.366946 omnipy-0.9.3/src/omnipy/compute/flow.py
--rw-r--r--   0        0        0     3074 2023-02-14 01:43:00.003267 omnipy-0.9.3/src/omnipy/compute/func_job.py
--rw-r--r--   0        0        0     8579 2023-02-03 14:24:42.367595 omnipy-0.9.3/src/omnipy/compute/job.py
--rw-r--r--   0        0        0     1999 2023-02-28 19:23:19.637412 omnipy-0.9.3/src/omnipy/compute/job_creator.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.367737 omnipy-0.9.3/src/omnipy/compute/mixins/__init__.py
--rw-r--r--   0        0        0      746 2023-02-03 14:24:42.367847 omnipy-0.9.3/src/omnipy/compute/mixins/flow_context.py
--rw-r--r--   0        0        0     1719 2023-02-03 14:24:42.368162 omnipy-0.9.3/src/omnipy/compute/mixins/func_signature.py
--rw-r--r--   0        0        0     3686 2023-02-03 14:24:42.368371 omnipy-0.9.3/src/omnipy/compute/mixins/iterate.py
--rw-r--r--   0        0        0      744 2023-02-28 19:22:32.370614 omnipy-0.9.3/src/omnipy/compute/mixins/mixin_types.py
--rw-r--r--   0        0        0     1908 2023-02-03 14:24:42.369798 omnipy-0.9.3/src/omnipy/compute/mixins/name.py
--rw-r--r--   0        0        0     2584 2023-02-03 14:24:42.370665 omnipy-0.9.3/src/omnipy/compute/mixins/params.py
--rw-r--r--   0        0        0      636 2023-02-03 14:24:42.371170 omnipy-0.9.3/src/omnipy/compute/mixins/result_key.py
--rw-r--r--   0        0        0     9401 2023-02-03 14:24:42.371492 omnipy-0.9.3/src/omnipy/compute/mixins/serialize.py
--rw-r--r--   0        0        0     2319 2023-02-03 14:24:42.371579 omnipy-0.9.3/src/omnipy/compute/task.py
--rw-r--r--   0        0        0     4422 2023-02-03 14:24:42.371863 omnipy-0.9.3/src/omnipy/compute/tasklist_job.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.371902 omnipy-0.9.3/src/omnipy/config/__init__.py
--rw-r--r--   0        0        0      225 2023-02-03 14:24:42.372017 omnipy-0.9.3/src/omnipy/config/engine.py
--rw-r--r--   0        0        0      633 2023-02-03 14:24:42.372377 omnipy-0.9.3/src/omnipy/config/job.py
--rw-r--r--   0        0        0      695 2023-02-14 04:10:36.533814 omnipy-0.9.3/src/omnipy/config/root_log.py
--rw-r--r--   0        0        0        0 2023-02-28 19:24:13.117949 omnipy-0.9.3/src/omnipy/data/__init__.py
--rw-r--r--   0        0        0    11070 2023-02-28 20:13:38.948231 omnipy-0.9.3/src/omnipy/data/dataset.py
--rw-r--r--   0        0        0    10528 2023-02-28 20:12:58.560155 omnipy-0.9.3/src/omnipy/data/model.py
--rw-r--r--   0        0        0     5331 2023-02-28 19:35:06.758130 omnipy-0.9.3/src/omnipy/data/serializer.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.373952 omnipy-0.9.3/src/omnipy/engine/__init__.py
--rw-r--r--   0        0        0     1683 2023-02-28 22:21:38.250721 omnipy-0.9.3/src/omnipy/engine/base.py
--rw-r--r--   0        0        0     9193 2023-02-28 19:37:12.183392 omnipy-0.9.3/src/omnipy/engine/job_runner.py
--rw-r--r--   0        0        0     1917 2023-02-28 19:37:21.998880 omnipy-0.9.3/src/omnipy/engine/local.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.374736 omnipy-0.9.3/src/omnipy/hub/__init__.py
--rw-r--r--   0        0        0      507 2023-02-14 01:43:00.005895 omnipy-0.9.3/src/omnipy/hub/entry.py
--rw-r--r--   0        0        0     4021 2023-02-14 03:45:00.843707 omnipy-0.9.3/src/omnipy/hub/root_log.py
--rw-r--r--   0        0        0     5188 2023-02-14 01:43:00.007210 omnipy-0.9.3/src/omnipy/hub/runtime.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.375614 omnipy-0.9.3/src/omnipy/log/__init__.py
--rw-r--r--   0        0        0       70 2023-02-14 01:43:00.007305 omnipy-0.9.3/src/omnipy/log/constants.py
--rw-r--r--   0        0        0     1297 2023-02-14 04:10:06.920895 omnipy-0.9.3/src/omnipy/log/mixin.py
--rw-r--r--   0        0        0     3512 2023-02-14 01:43:00.008519 omnipy-0.9.3/src/omnipy/log/registry.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.376336 omnipy-0.9.3/src/omnipy/modules/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.376394 omnipy-0.9.3/src/omnipy/modules/fairtracks/__init__.py
--rw-r--r--   0        0        0     1675 2023-02-03 14:24:42.377256 omnipy-0.9.3/src/omnipy/modules/fairtracks/functions.py
--rw-r--r--   0        0        0      598 2023-02-03 14:24:42.377609 omnipy-0.9.3/src/omnipy/modules/fairtracks/tasks.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.377656 omnipy-0.9.3/src/omnipy/modules/general/__init__.py
--rw-r--r--   0        0        0      234 2023-02-03 14:24:42.378006 omnipy-0.9.3/src/omnipy/modules/general/models.py
--rw-r--r--   0        0        0     2006 2023-02-03 14:24:42.378188 omnipy-0.9.3/src/omnipy/modules/general/tasks.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.378220 omnipy-0.9.3/src/omnipy/modules/json/__init__.py
--rw-r--r--   0        0        0     3238 2023-02-28 19:38:21.073991 omnipy-0.9.3/src/omnipy/modules/json/datasets.py
--rw-r--r--   0        0        0     1144 2023-02-03 14:24:42.378849 omnipy-0.9.3/src/omnipy/modules/json/flows.py
--rw-r--r--   0        0        0     3206 2023-02-03 14:24:42.379348 omnipy-0.9.3/src/omnipy/modules/json/functions.py
--rw-r--r--   0        0        0     2850 2023-02-28 19:39:42.650229 omnipy-0.9.3/src/omnipy/modules/json/models.py
--rw-r--r--   0        0        0     1587 2023-02-28 19:40:02.050693 omnipy-0.9.3/src/omnipy/modules/json/serializers.py
--rw-r--r--   0        0        0     3754 2023-02-03 14:24:42.380417 omnipy-0.9.3/src/omnipy/modules/json/tasks.py
--rw-r--r--   0        0        0     1477 2023-02-28 16:12:04.902506 omnipy-0.9.3/src/omnipy/modules/json/types.py
--rw-r--r--   0        0        0       20 2023-02-03 14:24:42.382453 omnipy-0.9.3/src/omnipy/modules/pandas/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-03 14:24:42.382748 omnipy-0.9.3/src/omnipy/modules/pandas/models.py
--rw-r--r--   0        0        0     1738 2023-02-28 19:41:39.217018 omnipy-0.9.3/src/omnipy/modules/pandas/serializers.py
--rw-r--r--   0        0        0     3150 2023-02-14 01:43:06.002318 omnipy-0.9.3/src/omnipy/modules/pandas/tasks.py
--rw-r--r--   0        0        0      654 2023-02-14 01:43:00.008792 omnipy-0.9.3/src/omnipy/modules/prefect/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.385531 omnipy-0.9.3/src/omnipy/modules/prefect/engine/__init__.py
--rw-r--r--   0        0        0     5832 2023-02-28 19:42:42.334836 omnipy-0.9.3/src/omnipy/modules/prefect/engine/prefect.py
--rw-r--r--   0        0        0     2862 2023-02-14 01:43:00.009050 omnipy-0.9.3/src/omnipy/modules/prefect/settings/logging.yml
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.386331 omnipy-0.9.3/src/omnipy/modules/raw/__init__.py
--rw-r--r--   0        0        0      451 2023-02-28 19:43:13.593695 omnipy-0.9.3/src/omnipy/modules/raw/protocols.py
--rw-r--r--   0        0        0     1545 2023-02-28 19:43:32.037956 omnipy-0.9.3/src/omnipy/modules/raw/serializers.py
--rw-r--r--   0        0        0     1285 2023-02-03 14:24:42.387150 omnipy-0.9.3/src/omnipy/modules/raw/tasks.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.387503 omnipy-0.9.3/src/omnipy/modules/tables/__init__.py
--rw-r--r--   0        0        0      361 2023-02-03 14:24:42.387871 omnipy-0.9.3/src/omnipy/modules/tables/models.py
--rw-r--r--   0        0        0     1246 2023-02-03 14:24:42.388152 omnipy-0.9.3/src/omnipy/modules/tables/tasks.py
--rw-r--r--   0        0        0        0 2023-02-03 14:24:42.388201 omnipy-0.9.3/src/omnipy/util/__init__.py
--rw-r--r--   0        0        0     4704 2023-02-28 19:03:51.702484 omnipy-0.9.3/src/omnipy/util/callable_decorator_cls.py
--rw-r--r--   0        0        0     1748 2023-02-03 14:24:42.388722 omnipy-0.9.3/src/omnipy/util/dataframe.py
--rw-r--r--   0        0        0     1690 2023-02-14 01:43:00.009783 omnipy-0.9.3/src/omnipy/util/helpers.py
--rw-r--r--   0        0        0     8652 2023-02-28 19:44:56.823530 omnipy-0.9.3/src/omnipy/util/mixin.py
--rw-r--r--   0        0        0     1464 2023-02-03 14:24:42.389349 omnipy-0.9.3/src/omnipy/util/param_key_mapper.py
--rw-r--r--   0        0        0     1144 2023-02-14 01:43:00.010064 omnipy-0.9.3/src/omnipy/util/publisher.py
--rw-r--r--   0        0        0    23131 1970-01-01 00:00:00.000000 omnipy-0.9.3/setup.py
--rw-r--r--   0        0        0    22797 1970-01-01 00:00:00.000000 omnipy-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-10 07:53:17.530444 omnipy-0.9.5/LICENSE
+-rw-r--r--   0        0        0    21170 2023-03-01 05:51:15.986569 omnipy-0.9.5/README.md
+-rw-r--r--   0        0        0     2706 2023-03-14 14:06:59.618671 omnipy-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      358 2023-03-14 14:06:59.625549 omnipy-0.9.5/src/omnipy/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 06:43:26.570780 omnipy-0.9.5/src/omnipy/api/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-01 05:51:15.992602 omnipy-0.9.5/src/omnipy/api/enums.py
+-rw-r--r--   0        0        0       81 2023-01-24 06:43:26.571004 omnipy-0.9.5/src/omnipy/api/exceptions.py
+-rw-r--r--   0        0        0    12773 2023-03-01 05:51:15.992741 omnipy-0.9.5/src/omnipy/api/protocols.py
+-rw-r--r--   0        0        0      222 2023-02-14 09:38:18.591478 omnipy-0.9.5/src/omnipy/api/types.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.612010 omnipy-0.9.5/src/omnipy/compute/__init__.py
+-rw-r--r--   0        0        0     3723 2023-01-24 12:52:38.405579 omnipy-0.9.5/src/omnipy/compute/flow.py
+-rw-r--r--   0        0        0     3074 2023-02-14 09:38:18.591778 omnipy-0.9.5/src/omnipy/compute/func_job.py
+-rw-r--r--   0        0        0     8579 2023-02-01 11:41:12.887209 omnipy-0.9.5/src/omnipy/compute/job.py
+-rw-r--r--   0        0        0     1999 2023-03-01 05:51:15.993169 omnipy-0.9.5/src/omnipy/compute/job_creator.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.612257 omnipy-0.9.5/src/omnipy/compute/mixins/__init__.py
+-rw-r--r--   0        0        0      746 2023-01-24 12:47:48.628308 omnipy-0.9.5/src/omnipy/compute/mixins/flow_context.py
+-rw-r--r--   0        0        0     1719 2023-01-24 06:43:26.571665 omnipy-0.9.5/src/omnipy/compute/mixins/func_signature.py
+-rw-r--r--   0        0        0     3686 2023-01-24 06:43:26.571768 omnipy-0.9.5/src/omnipy/compute/mixins/iterate.py
+-rw-r--r--   0        0        0      744 2023-03-01 05:51:15.993299 omnipy-0.9.5/src/omnipy/compute/mixins/mixin_types.py
+-rw-r--r--   0        0        0     1908 2023-01-31 13:38:42.021250 omnipy-0.9.5/src/omnipy/compute/mixins/name.py
+-rw-r--r--   0        0        0     2584 2023-01-24 13:42:06.446734 omnipy-0.9.5/src/omnipy/compute/mixins/params.py
+-rw-r--r--   0        0        0      636 2023-01-24 06:43:26.572084 omnipy-0.9.5/src/omnipy/compute/mixins/result_key.py
+-rw-r--r--   0        0        0     9401 2023-01-31 13:38:42.021434 omnipy-0.9.5/src/omnipy/compute/mixins/serialize.py
+-rw-r--r--   0        0        0     2319 2023-01-24 12:50:59.424967 omnipy-0.9.5/src/omnipy/compute/task.py
+-rw-r--r--   0        0        0     4422 2023-01-24 06:43:26.572615 omnipy-0.9.5/src/omnipy/compute/tasklist_job.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.612862 omnipy-0.9.5/src/omnipy/config/__init__.py
+-rw-r--r--   0        0        0      225 2023-01-12 12:13:31.612913 omnipy-0.9.5/src/omnipy/config/engine.py
+-rw-r--r--   0        0        0      633 2023-01-31 13:38:42.021577 omnipy-0.9.5/src/omnipy/config/job.py
+-rw-r--r--   0        0        0      695 2023-02-14 09:38:18.591860 omnipy-0.9.5/src/omnipy/config/root_log.py
+-rw-r--r--   0        0        0        0 2023-03-01 05:51:15.993494 omnipy-0.9.5/src/omnipy/data/__init__.py
+-rw-r--r--   0        0        0    11368 2023-03-14 14:06:07.572683 omnipy-0.9.5/src/omnipy/data/dataset.py
+-rw-r--r--   0        0        0    10528 2023-03-01 05:51:15.994004 omnipy-0.9.5/src/omnipy/data/model.py
+-rw-r--r--   0        0        0     5331 2023-03-01 05:51:15.994129 omnipy-0.9.5/src/omnipy/data/serializer.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.613659 omnipy-0.9.5/src/omnipy/engine/__init__.py
+-rw-r--r--   0        0        0     1683 2023-03-01 05:51:15.994248 omnipy-0.9.5/src/omnipy/engine/base.py
+-rw-r--r--   0        0        0     9193 2023-03-01 05:51:15.994374 omnipy-0.9.5/src/omnipy/engine/job_runner.py
+-rw-r--r--   0        0        0     1917 2023-03-01 05:51:15.994733 omnipy-0.9.5/src/omnipy/engine/local.py
+-rw-r--r--   0        0        0        0 2023-01-24 06:43:26.573653 omnipy-0.9.5/src/omnipy/hub/__init__.py
+-rw-r--r--   0        0        0      507 2023-02-14 09:38:18.593344 omnipy-0.9.5/src/omnipy/hub/entry.py
+-rw-r--r--   0        0        0     4021 2023-02-14 09:38:18.593455 omnipy-0.9.5/src/omnipy/hub/root_log.py
+-rw-r--r--   0        0        0     5188 2023-02-14 09:38:18.593677 omnipy-0.9.5/src/omnipy/hub/runtime.py
+-rw-r--r--   0        0        0        0 2023-01-24 06:43:26.573853 omnipy-0.9.5/src/omnipy/log/__init__.py
+-rw-r--r--   0        0        0       70 2023-02-14 09:38:18.593799 omnipy-0.9.5/src/omnipy/log/constants.py
+-rw-r--r--   0        0        0     1297 2023-02-14 09:38:18.594129 omnipy-0.9.5/src/omnipy/log/mixin.py
+-rw-r--r--   0        0        0     3512 2023-02-14 09:38:18.594258 omnipy-0.9.5/src/omnipy/log/registry.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.614122 omnipy-0.9.5/src/omnipy/modules/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.614177 omnipy-0.9.5/src/omnipy/modules/fairtracks/__init__.py
+-rw-r--r--   0        0        0     1675 2023-01-12 12:13:31.614431 omnipy-0.9.5/src/omnipy/modules/fairtracks/functions.py
+-rw-r--r--   0        0        0      598 2023-02-14 09:38:18.594730 omnipy-0.9.5/src/omnipy/modules/fairtracks/tasks.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.614556 omnipy-0.9.5/src/omnipy/modules/general/__init__.py
+-rw-r--r--   0        0        0      234 2023-01-31 13:38:42.022490 omnipy-0.9.5/src/omnipy/modules/general/models.py
+-rw-r--r--   0        0        0     2006 2023-02-14 09:38:18.594863 omnipy-0.9.5/src/omnipy/modules/general/tasks.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.614665 omnipy-0.9.5/src/omnipy/modules/json/__init__.py
+-rw-r--r--   0        0        0     3238 2023-03-01 05:51:15.994864 omnipy-0.9.5/src/omnipy/modules/json/datasets.py
+-rw-r--r--   0        0        0     1144 2023-02-14 09:38:18.595026 omnipy-0.9.5/src/omnipy/modules/json/flows.py
+-rw-r--r--   0        0        0     3206 2023-02-14 09:38:18.595298 omnipy-0.9.5/src/omnipy/modules/json/functions.py
+-rw-r--r--   0        0        0     2850 2023-03-01 05:51:15.994970 omnipy-0.9.5/src/omnipy/modules/json/models.py
+-rw-r--r--   0        0        0     1587 2023-03-01 05:51:15.995075 omnipy-0.9.5/src/omnipy/modules/json/serializers.py
+-rw-r--r--   0        0        0     3754 2023-02-14 09:38:18.596155 omnipy-0.9.5/src/omnipy/modules/json/tasks.py
+-rw-r--r--   0        0        0     1477 2023-03-01 05:51:15.995177 omnipy-0.9.5/src/omnipy/modules/json/types.py
+-rw-r--r--   0        0        0       20 2023-01-12 12:13:31.614971 omnipy-0.9.5/src/omnipy/modules/pandas/__init__.py
+-rw-r--r--   0        0        0     1441 2023-03-14 14:06:07.586961 omnipy-0.9.5/src/omnipy/modules/pandas/models.py
+-rw-r--r--   0        0        0     1738 2023-03-01 05:51:15.995299 omnipy-0.9.5/src/omnipy/modules/pandas/serializers.py
+-rw-r--r--   0        0        0     3150 2023-02-14 09:38:18.596677 omnipy-0.9.5/src/omnipy/modules/pandas/tasks.py
+-rw-r--r--   0        0        0      654 2023-02-14 09:38:18.596782 omnipy-0.9.5/src/omnipy/modules/prefect/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-31 13:38:42.023284 omnipy-0.9.5/src/omnipy/modules/prefect/engine/__init__.py
+-rw-r--r--   0        0        0     5832 2023-03-01 05:51:15.995626 omnipy-0.9.5/src/omnipy/modules/prefect/engine/prefect.py
+-rw-r--r--   0        0        0     2862 2023-02-14 09:38:18.596873 omnipy-0.9.5/src/omnipy/modules/prefect/settings/logging.yml
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.615273 omnipy-0.9.5/src/omnipy/modules/raw/__init__.py
+-rw-r--r--   0        0        0      451 2023-03-01 05:51:15.995746 omnipy-0.9.5/src/omnipy/modules/raw/protocols.py
+-rw-r--r--   0        0        0     1545 2023-03-01 05:51:15.995849 omnipy-0.9.5/src/omnipy/modules/raw/serializers.py
+-rw-r--r--   0        0        0     1285 2023-01-17 11:55:06.653611 omnipy-0.9.5/src/omnipy/modules/raw/tasks.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.615477 omnipy-0.9.5/src/omnipy/modules/tables/__init__.py
+-rw-r--r--   0        0        0      361 2023-02-14 09:38:18.597228 omnipy-0.9.5/src/omnipy/modules/tables/models.py
+-rw-r--r--   0        0        0     1246 2023-02-14 09:38:18.597354 omnipy-0.9.5/src/omnipy/modules/tables/tasks.py
+-rw-r--r--   0        0        0        0 2023-01-12 12:13:31.615775 omnipy-0.9.5/src/omnipy/util/__init__.py
+-rw-r--r--   0        0        0     4704 2023-03-01 05:51:15.995989 omnipy-0.9.5/src/omnipy/util/callable_decorator_cls.py
+-rw-r--r--   0        0        0     1748 2023-01-12 12:13:31.615920 omnipy-0.9.5/src/omnipy/util/dataframe.py
+-rw-r--r--   0        0        0     1690 2023-02-14 09:38:18.597476 omnipy-0.9.5/src/omnipy/util/helpers.py
+-rw-r--r--   0        0        0     8652 2023-03-01 05:51:15.996124 omnipy-0.9.5/src/omnipy/util/mixin.py
+-rw-r--r--   0        0        0     1464 2023-01-12 12:13:31.616104 omnipy-0.9.5/src/omnipy/util/param_key_mapper.py
+-rw-r--r--   0        0        0     1144 2023-02-14 09:38:18.598779 omnipy-0.9.5/src/omnipy/util/publisher.py
+-rw-r--r--   0        0        0    23073 1970-01-01 00:00:00.000000 omnipy-0.9.5/setup.py
+-rw-r--r--   0        0        0    22769 1970-01-01 00:00:00.000000 omnipy-0.9.5/PKG-INFO
```

### Comparing `omnipy-0.9.3/LICENSE` & `omnipy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/README.md` & `omnipy-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/pyproject.toml` & `omnipy-0.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 [tool.poetry]
 name = "omnipy"
-version = "0.9.3"
+version = "0.9.5"
 description = "Omnipy is a high level Python library for type-driven data wrangling and scalable workflow orchestration (under development)"
 license = "Apache-2.0"
 repository = "http://github.com/fairtracks/omnipy"
 authors = ["Sveinung Gundersen <sveinugu@gmail.com>", "Federico Bianchini <fredebi@uio.no>", "Ahmed Ghanem <ahmedg@uio.no>", "Joshua Baskaran <joshuaba@uio.no>"]
 readme = "README.md"
 homepage = "https://fairtracks.net/fair/#fair-07-transformation"
+documentation = "http://omnipy.readthedocs.io/"
 keywords = ["data wrangling", "metadata", "workflows", "etl", "research data", "prefect", "pydantic", "FAIR", "ontologies", "JSON", "tabular", "type-driven", "orchestration", "data models", "universal"]
 classifiers = ["Development Status :: 2 - Pre-Alpha", "Framework :: Pydantic", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.10", "Topic :: Software Development :: Libraries"]
 packages = [{include = "omnipy", from = "src"}]
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 #python = ">=3.8.1,<4.0"
+aiostream = "^0.4.5"
+greenlet = "^2.0.1"
+inflection = "^0.5.1"
 pandas = "^1.2.4"
-requests = "^2.25.1"
 prefect = "^2.7.3"
 pydantic = "^1.10.2"
 pytest-asyncio = "^0.20.2"
-aiostream = "^0.4.5"
 pytest-cases = "^3.6.13"
-orjson = "^3.8.0"
+requests = "^2.25.1"
+typing-inspect = "^0.8.0"
 
 # Potential dependencies
 #dpath = "^2.1.0"
 #beartype = "^0.11.0"
 #typing-extensions = "^4.4.0"
 #phantom-types = "^1.1.0"
-greenlet = "^2.0.1"
-python-slugify = "^7.0.0"
-inflection = "^0.5.1"
-typing-inspect = "^0.8.0"
+#orjson = "^3.8.0"
+#python-slugify = "^7.0.0"
 
 [tool.poetry.group.dev.dependencies]
+deepdiff = "^6.2.1"
+flake8 = "^6.0.0"
+flake8-quotes = "^3.3.1"
+isort = "^5.10.1"
+mypy = "^1.0.0"
 pytest = "^7.1.0"
 pytest-pycharm = "^0.7.0"
 yapf = "^0.32.0"
-flake8 = "^6.0.0"
-isort = "^5.10.1"
-flake8-quotes = "^3.3.1"
-deepdiff = "^6.2.1"
-sphinx = "^6.1.3"
+
+[tool.poetry.group.docs.dependencies]
 furo = "^2022.12.7"
-sphinx-copybutton = "^0.5.1"
+sphinx = "^6.1.3"
 sphinx-autoapi = "^2.0.1"
-mypy = "^1.0.0"
+sphinx-copybutton = "^0.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.yapf]
 based_on_style = "google"
```

### Comparing `omnipy-0.9.3/src/omnipy/api/enums.py` & `omnipy-0.9.5/src/omnipy/api/enums.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/api/protocols.py` & `omnipy-0.9.5/src/omnipy/api/protocols.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/flow.py` & `omnipy-0.9.5/src/omnipy/compute/flow.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/func_job.py` & `omnipy-0.9.5/src/omnipy/compute/func_job.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/job.py` & `omnipy-0.9.5/src/omnipy/compute/job.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/job_creator.py` & `omnipy-0.9.5/src/omnipy/compute/job_creator.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/flow_context.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/flow_context.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/func_signature.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/func_signature.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/iterate.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/iterate.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/mixin_types.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/mixin_types.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/name.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/name.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/params.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/params.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/result_key.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/result_key.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/mixins/serialize.py` & `omnipy-0.9.5/src/omnipy/compute/mixins/serialize.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/task.py` & `omnipy-0.9.5/src/omnipy/compute/task.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/compute/tasklist_job.py` & `omnipy-0.9.5/src/omnipy/compute/tasklist_job.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/config/job.py` & `omnipy-0.9.5/src/omnipy/config/job.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/config/root_log.py` & `omnipy-0.9.5/src/omnipy/config/root_log.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/data/dataset.py` & `omnipy-0.9.5/src/omnipy/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,20 @@
             self._raise_no_model_exception()
 
         GenericModel.__init__(self, **input_data)
         UserDict.__init__(self, self.data)  # noqa
         if not self.__doc__:
             self._set_standard_field_description()
 
-    # TODO: Add test for get_model_class
-
     def get_model_class(self) -> ModelT:
+        """
+        Returns the concrete Model class used for all data files in the dataset, e.g.:
+        `Model[List[int]]`
+        :return: The concrete Model class used for all data files in the dataset
+        """
         return self.__fields__.get(DATA_KEY).type_
 
     # TODO: Update _raise_no_model_exception() text. Model is now a requirement
 
     @staticmethod
     def _raise_no_model_exception() -> None:
         raise TypeError(
@@ -246,14 +249,17 @@
 
     def as_multi_model_dataset(self) -> MultiModelDataset[ModelT]:
         multi_model_dataset = MultiModelDataset[self.get_model_class()]()
         for obj_type in self:
             multi_model_dataset.data[obj_type] = self.data[obj_type]
         return multi_model_dataset
 
+    def __eq__(self, other: object) -> bool:
+        return self.__class__ == other.__class__ and super().__eq__(other)
+
 
 # TODO: Use json serializer package from the pydantic config instead of 'json'
 
 
 class MultiModelDataset(Dataset[ModelT], Generic[ModelT]):
     """
         Variant of Dataset that allows custom models to be set on individual data files
```

### Comparing `omnipy-0.9.3/src/omnipy/data/model.py` & `omnipy-0.9.5/src/omnipy/data/model.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/data/serializer.py` & `omnipy-0.9.5/src/omnipy/data/serializer.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/engine/base.py` & `omnipy-0.9.5/src/omnipy/engine/base.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/engine/job_runner.py` & `omnipy-0.9.5/src/omnipy/engine/job_runner.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/engine/local.py` & `omnipy-0.9.5/src/omnipy/engine/local.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/hub/root_log.py` & `omnipy-0.9.5/src/omnipy/hub/root_log.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/hub/runtime.py` & `omnipy-0.9.5/src/omnipy/hub/runtime.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/log/mixin.py` & `omnipy-0.9.5/src/omnipy/log/mixin.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/log/registry.py` & `omnipy-0.9.5/src/omnipy/log/registry.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/fairtracks/functions.py` & `omnipy-0.9.5/src/omnipy/modules/fairtracks/functions.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/fairtracks/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/fairtracks/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/general/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/general/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/datasets.py` & `omnipy-0.9.5/src/omnipy/modules/json/datasets.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/flows.py` & `omnipy-0.9.5/src/omnipy/modules/json/flows.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/functions.py` & `omnipy-0.9.5/src/omnipy/modules/json/functions.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/models.py` & `omnipy-0.9.5/src/omnipy/modules/json/models.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/serializers.py` & `omnipy-0.9.5/src/omnipy/modules/json/serializers.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/json/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/json/types.py` & `omnipy-0.9.5/src/omnipy/modules/json/types.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/pandas/models.py` & `omnipy-0.9.5/src/omnipy/modules/pandas/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
-from typing import Any, Dict, Iterable, List
+from collections.abc import Iterable
+from typing import Any, Dict, List
 
 from omnipy.data.dataset import Dataset
 from omnipy.data.model import Model, ROOT_KEY
 
 from . import pd
 
 
@@ -20,31 +20,23 @@
             assert isinstance(column, str)
 
     @staticmethod
     def _data_not_empty_object(data: pd.DataFrame) -> None:
         assert not any(data.isna().all(axis=1))
 
     def dict(self, *args, **kwargs) -> Dict[Any, Any]:
-        return super().dict(*args, **kwargs)[ROOT_KEY].to_dict(orient='records')  # noqa
+        df = super().dict(*args, **kwargs)[ROOT_KEY]
+        df = df.replace({pd.NA: None})
+        return df.to_dict(orient='records')  # noqa
 
     def from_data(self, value: Iterable[Any]) -> None:
-        self.contents = self._convert_ints_to_nullable_ints(pd.DataFrame(value))
+        self.contents = pd.DataFrame(value).convert_dtypes()
 
     def from_json(self, value: str) -> None:
-        self.contents = self._convert_ints_to_nullable_ints(pd.read_json(value))
-
-    @classmethod
-    def _convert_ints_to_nullable_ints(cls, dataframe: pd.DataFrame) -> pd.DataFrame:
-        for key, col in dataframe.items():
-            if col.dtype == 'int64' or (col.dtype == 'float64' and col.isna().any()):
-                try:
-                    dataframe[key] = col.astype(float).astype('Int64')
-                except TypeError:
-                    pass
-        return dataframe
+        self.contents = pd.read_json(value).convert_dtypes()
 
 
 class PandasDataset(Dataset[PandasModel]):
     ...
 
 
 class ListOfPandasDatasetsWithSameNumberOfFiles(Model[List[PandasDataset]]):
```

### Comparing `omnipy-0.9.3/src/omnipy/modules/pandas/serializers.py` & `omnipy-0.9.5/src/omnipy/modules/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/pandas/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/pandas/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/prefect/__init__.py` & `omnipy-0.9.5/src/omnipy/modules/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/prefect/engine/prefect.py` & `omnipy-0.9.5/src/omnipy/modules/prefect/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/prefect/settings/logging.yml` & `omnipy-0.9.5/src/omnipy/modules/prefect/settings/logging.yml`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/raw/serializers.py` & `omnipy-0.9.5/src/omnipy/modules/raw/serializers.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/raw/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/raw/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/modules/tables/tasks.py` & `omnipy-0.9.5/src/omnipy/modules/tables/tasks.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/callable_decorator_cls.py` & `omnipy-0.9.5/src/omnipy/util/callable_decorator_cls.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/dataframe.py` & `omnipy-0.9.5/src/omnipy/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/helpers.py` & `omnipy-0.9.5/src/omnipy/util/helpers.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/mixin.py` & `omnipy-0.9.5/src/omnipy/util/mixin.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/param_key_mapper.py` & `omnipy-0.9.5/src/omnipy/util/param_key_mapper.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/src/omnipy/util/publisher.py` & `omnipy-0.9.5/src/omnipy/util/publisher.py`

 * *Files identical despite different names*

### Comparing `omnipy-0.9.3/setup.py` & `omnipy-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,25 @@
 package_data = \
 {'': ['*'], 'omnipy.modules.prefect': ['settings/*']}
 
 install_requires = \
 ['aiostream>=0.4.5,<0.5.0',
  'greenlet>=2.0.1,<3.0.0',
  'inflection>=0.5.1,<0.6.0',
- 'orjson>=3.8.0,<4.0.0',
  'pandas>=1.2.4,<2.0.0',
  'prefect>=2.7.3,<3.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pytest-asyncio>=0.20.2,<0.21.0',
  'pytest-cases>=3.6.13,<4.0.0',
- 'python-slugify>=7.0.0,<8.0.0',
  'requests>=2.25.1,<3.0.0',
  'typing-inspect>=0.8.0,<0.9.0']
 
 setup_kwargs = {
     'name': 'omnipy',
-    'version': '0.9.3',
+    'version': '0.9.5',
     'description': 'Omnipy is a high level Python library for type-driven data wrangling and scalable workflow orchestration (under development)',
     'long_description': '\n![Omnypy logo](https://fairtracks.net/_nuxt/img/9a84303.webp)\n\nOmnipy is the new name of the Python package formerly known as uniFAIR.\n\nWe are very grateful to Dr. Jamin Chen, who gracefully transferred ownership of the (mostly unused) "omnipy" name in PyPI to us!\n\n--\n\nUpdate Feb 3, 2023: Documentation of the Omnipy API is still sparse. However, for running examples,\nplease check out the [omnipy-examples repo](https://github.com/fairtracks/omnipy_examples) and its\nrelated [PYPI package](https://pypi.org/project/omnipy-examples/)!\n\n(NOTE: Read the section [Transformation on the FAIRtracks.net website](https://fairtracks.net/fair/#fair-07-transformation)\nfor a more detailed and better formatted version of the following description!)\n\n## Generic functionality\n\nOmnipy is designed primarily to simplify development and deployment of (meta)data transformation \nprocesses in the context of FAIRification and data brokering efforts. However, the functionality is \nvery generic and can also be used to support research data (and metadata) transformations in a range \nof fields and contexts beyond life science, including day-to-day research scenarios:\n\n![Conceptual overview of Omnipy](https://fairtracks.net/_nuxt/img/aef0283-1440.png)\n\n**Data wrangling in day-to-day research:** Researchers in life science and other data-centric fields\noften need to extract, manipulate and integrate data and/or metadata from different sources, such as\nrepositories, databases or flat files. Much research time is spent on trivial and not-so-trivial\ndetails of such ["data wrangling"](https://en.wikipedia.org/wiki/Data_wrangling):\n\n- reformat data structures\n- clean up errors\n- remove duplicate data\n- map and integrate dataset fields\n- etc.\n\nGeneral software for data wrangling and analysis, such as [Pandas](https://pandas.pydata.org/),\n[R](https://www.r-project.org/) or [Frictionless](https://frictionlessdata.io/), are useful, but\nresearchers still regularly end up with hard-to-reuse scripts, often with manual steps.\n\n**Step-wise data model transformations:** With the Omnipy\nPython package, researchers can import (meta)data in almost any shape or form: _nested JSON; tabular\n(relational) data; binary streams; or other data structures_. Through a step-by-step process, data\nis continuously parsed and reshaped according to a series of data model transformations.\n\n<ui-quote-text quote=\'Omnipy tasks (single steps) and flows (workflows) are defined as transformations from specific input data models to specific output data models.\'>\n</ui-quote-text>\n\n**"Parse, don\'t validate":** Omnipy follows the principles of "Type-driven design" (read \n_Technical note #2: "Parse, don\'t validate"_ on the \n[FAIRtracks.net website](https://fairtracks.net/fair/#fair-07-transformation) for more info). It \nmakes use of cutting-edge [Python type hints](https://peps.python.org/pep-0484/) and the popular\n[pydantic](https://pydantic-docs.helpmanual.io/) package to "pour" data into precisely defined data\nmodels that can range from very general (e.g. _"any kind of JSON data", "any kind of tabular data"_,\netc.) to very specific (e.g. _"follow the FAIRtracks JSON Schema for track files with the extra\nrestriction of only allowing BigBED files"_).\n\n**Data types as contracts:** Omnipy _tasks_ (single steps) or _flows_ (workflows) are defined as\ntransformations from specific _input_ data models to specific _output_ data models.\n[pydantic](https://pydantic-docs.helpmanual.io/)-based parsing guarantees that the input and output\ndata always follows the data models (i.e. data types). Thus, the data models defines "contracts"\nthat simplifies reuse of tasks and flows in a _mix-and-match_ fashion.\n\n**Catalog of common processing steps:** Omnipy is built from the ground up to be modular. We aim \nto provide a catalog of commonly useful functionality ranging from:\n\n- data import from REST API endpoints, common flat file formats, database dumps, etc.\n- flattening of complex, nested JSON structures\n- standardization of relational tabular data (i.e. removing redundancy)\n- mapping of tabular data between schemas\n- lookup and mapping of ontology terms\n- semi-automatic data cleaning (through e.g. [Open Refine](https://openrefine.org/))\n- support for common data manipulation software and libraries, such as\n  [Pandas](https://pandas.pydata.org/), [R](https://www.r-project.org/),\n  [Frictionless](https://frictionlessdata.io/), etc.\n\nIn particular, we will provide a _FAIRtracks_ module that contains data models and processing steps\nto transform metadata to follow the [FAIRtracks standard](/standards/#standards-01-fairtracks).\n\n![Catalog of commonly useful processing steps, data modules and tool integrations](https://fairtracks.net/_nuxt/img/7101c5f-1280.png)\n\n**Refine and apply templates:** An Omnipy module typically consists of a set of generic _task_ and\n_flow templates_ with related data models, (de)serializers, and utility functions. The user can then\npick task and flow templates from this extensible, modular catalog, further refine them in the\ncontext of a custom, use case-specific flow, and apply them to the desired compute engine to carry\nout the transformations needed to wrangle data into the required shape.\n\n**Rerun only when needed:** When piecing together a custom flow in Omnipy, the user has persistent\naccess to the state of the data at every step of the process. Persistent intermediate data allows\nfor caching of tasks based on the input data and parameters. Hence, if the input data and parameters\nof a task does not change between runs, the task is not rerun. This is particularly useful for\nimporting from REST API endpoints, as a flow can be continuously rerun without taxing the remote\nserver; data import will only carried out in the initial iteration or when the REST API signals that\nthe data has changed.\n\n**Scale up with external compute resources:** In the case of large datasets, the researcher can set\nup a flow based on a representative sample of the full dataset, in a size that is suited for running\nlocally on, say, a laptop. Once the flow has produced the correct output on the sample data, the\noperation can be seamlessly scaled up to the full dataset and sent off in\n[software containers](https://www.docker.com/resources/what-container/) to run on external compute\nresources, using e.g. [Kubernetes](https://kubernetes.io/). Such offloaded flows\ncan be easily monitored using a web GUI.\n\n![Working with Omnipy directly from an Integrated Development Environment (IDE)](https://fairtracks.net/_nuxt/img/f9be071-1440.png)\n\n**Industry-standard ETL backbone:** Offloading of flows to external compute resources is provided by\nthe integration of Omnipy with a workflow engine based on the [Prefect](https://www.prefect.io/)\nPython package. Prefect is an industry-leading platform for dataflow automation and orchestration\nthat brings a [series of powerful features](https://www.prefect.io/opensource/) to Omnipy:\n\n- Predefined integrations with a range of compute infrastructure solutions\n- Predefined integration with various services to support extraction, transformation, and loading\n  (ETL) of data and metadata\n- Code as workflow ("If Python can write it, Prefect can run it")\n- Dynamic workflows: no predefined Direct Acyclic Graphs (DAGs) needed!\n- Command line and web GUI-based visibility and control of jobs\n- Trigger jobs from external events such as GitHub commits, file uploads, etc.\n- Define continuously running workflows that still respond to external events\n- Run tasks concurrently through support for asynchronous tasks\n\n![Overview of the compute and storage infrastructure integrations that comes built-in with Prefect](https://fairtracks.net/_nuxt/img/ccc322a-1440.png)\n\n**Pluggable workflow engines:** It is also possible to integrate Omnipy with other workflow\nbackends by implementing new workflow engine plugins. This is relatively easy to do, as the core\narchitecture of Omnipy allows the user to easily switch the workflow engine at runtime. Omnipy\nsupports both traditional DAG-based and the more _avant garde_ code-based definition of flows. Two\nworkflow engines are currently supported: _local_ and _prefect_.\n\n## Scenarios\nAs initial use cases, we will consider the following two scenarios:\n* Transforming ENCODE metadata into FAIRtracks format\n* Transforming TCGA metadata into FAIRtracks format\n\n## Nomenclature:\n* Omnipy is designed to work with content which could be classified both as data and metadata in their original context. For simplicity, we will refer to all such content as "data".\n\n## Overview of the proposed FAIRification process:\n\n* ### Step 1: Import data from original source:\n  * #### 1A: From API endpoints\n    * _Input:_ API endpoint producing JSON data\n    * _Output:_ JSON files (possibly with embedded JSON objects/lists [as strings])\n    * _Description:_ General interface to support various API endpoints. Import all data by crawling API endpoints providing JSON content\n    * _Generalizable:_ Partly (at least reuse of utility functions)\n    * _Manual/automatic:_ Automatic\n    * _Details:_\n      * GDC/TCGA substeps (implemented as Step objects with file input/output)\n        * 1A. Filtering step:\n          * Input: parameters defining how to filter, e.g.:\n            * For all endpoints (projects, cases, files, annotations), support:\n              * Filter on list of IDs\n              * Specific number of items\n              * All\n            * Example config:\n              * projects: 2 items\n              * cases: 2 items\n              * files: all\n              * annotations: all\n            *  Define standard configurations, e.g.:\n                * Default: limited extraction (3 projects * 3 cases * 5 files? (+ annotations?))\n                * All TCGA\n                * List of projects\n            * Hierarchical for loop through endpoints to create filter definitions\n          * Output: Filter definitions as four files, e.g. as JSON, \n            as they should be input to the filter parameter to the API:\n             ```\n            projects_filter.json:\n            {\n                "op": "in",\n                "content": {\n                    "field": "project_id",\n                    "value": [\'TCGA_ABCD\', \'TCGA_BCDE\']\n                }\n            }\n            \n            cases_filter.json:\n            {\n                "op": "in",\n                "content": {\n                    "field": "case_id",\n                    "value": [\'1234556\', \'234567\', \'3456789\', \'4567890\']\n                }\n            }\n            \n            files_filter.json:\n            {\n                "op": "in",\n                "content": {\n                    "field": "file_id",\n                    "value": [\'1234556\', \'234567\', \'3456789\', \'4567890\']\n                }\n            }\n            \n            annotations.json\n            {\n                "op": "in",\n                "content": {\n                    "field": "annotation_id",\n                    "value": [\'1234556\', \'234567\', \'3456789\', \'4567890\']\n                }\n            }\n            ```\n            \n        * 1B. Fetch and divide all fields step:\n          * Input: None\n          * Output: JSON files specifying all the fields of an endpoint fetched from the `mapping` API. \n              The fields should be divided into chunks of a size that is small enough for the endpoints to \n              handle. The JSON output should also specify the primary_key field, that needs to be added to \n              all the API calls in order for the results to be joinable.\n              \n              Example JSON files:\n             ```\n            projects_fields.json:\n            {\n                "primary_key": "project_id",\n                "fields_divided": [\n                    ["field_a", "field_b"],\n                    ["field_c.subfield_a", "field_c.subfield_b", "field_d"]      \n                ]\n            }\n            \n            (...) # For all endpoints\n            ```\n        * 1C. Download from all endpoints according to the filters and the field divisions.\n              If there is a limitation on the number of hits that the endpoint is able to return, divide into smaller\n              API calls for a certain number of hits and concatenate the results. Make sure that proper waiting time\n              (1 second?) is added between the calls (to not overload the endpoint).\n        * 1D. Extract identifiers from nested objects (when present) and insert into parents objects\n      * ENCODE:\n        * Identify where to start (Cart? Experiment?)\n        * To get all data for a table (double-check this): `https://www.encodeproject.org/experiments/@@listing?format=json&frame=object`\n        * Download all tables directly.\n  * #### 1b: From JSON files\n    * _Input:_ JSON content as files\n    * _Output:_ Pandas DataFrames (possibly with embedded JSON objects/lists)\n    * _Description:_ Import data from files. Requires specific parsers to be implemented.\n    * _Generalizable:_ Fully\n    * _Manual/automatic:_ Automatic\n  * #### 1c: From non-JSON files\n    * _Input:_ File content in some supported format (e.g. GSuite)\n    * _Output:_ Pandas DataFrames (possibly containing lists of identifiers as Pandas Series) + reference metadata\n    * _Description:_ Import data from files. Requires specific parsers to be implemented.\n    * _Generalizable:_ Partly (generating reference metadata might be tricky)\n    * _Manual/automatic:_ Automatic\n  * #### 1d: From database\n    * _Input:_ Direct access to relational database\n    * _Output:_ Pandas DataFrames (possibly containing lists of identifiers as Pandas Series) + reference metadata\n    * _Description:_ Import data from database\n    * _Generalizable:_ Fully\n    * _Manual/automatic:_ Automatic\n* ### Step 2: JSON cleanup\n    * _Input:_ Pandas DataFrames (possibly with embedded JSON objects/lists)\n    * _Output:_ Pandas DataFrames (possibly containing lists of identifiers as Pandas Series) + reference metadata\n    * _Description:_ Replace embedded objects with identifiers (possibly as lists)\n    * _Generalizable:_ Partly (generating reference metadata might be tricky)\n    * _Manual/automatic:_ Depending on original input\n    * _Details:_\n      * If there are embedded objects from other tables:\n        * ENCODE update: \n          * By using the `frame=object` parameter, we will not get any embedded objects from the APIs for the main tables. There is, however, some "auditing" fields that contain JSON objects. We can ignore these in the first iteration.\n        * If the original table of the embedded objects can be retrieved directly from an API, replace such embedded objects with unique identifiers to the object in another table (maintaining a reference to the name of the table, if needed)\n          * Record the reference metadata `(table_from, attr_from) -> (table_to, attr_to)` for joins:\n            * Example: `(table: "experiment", column: "replicates") -> (table: "replicate", column: "@id")`\n        * If the original table of the embedded objects are not directly available from an API, one needs to fill out the other table with the content that is embedded in the current object, creating the table if needed.\n      * For all fields with identifiers that reference other tables:\n        * Record the reference metadata `(table_from, attr_from) -> (table_to, attr_to)` for joins.\n        * If the field contains a list of identifiers\n          * Convert into Pandas Series\n* ### Step 3: Create reference tables to satisfy 1NF\n    * _Input:_ Pandas DataFrames (possibly containing lists of identifiers as Pandas Series) + reference metadata\n    * _Output:_ Pandas DataFrames (original tables without reference column) [1NF] + reference tables + reference metadata\n    * _Description:_ Move references into separate tables, transforming the tables in first normal form ([1NF](https://en.wikipedia.org/wiki/Database_normalization#Satisfying_1NF))\n    * _Generalizable:_ Fully\n    * _Manual/automatic:_ Automatic\n    * _Details:_\n      * For each reference pair: \n        * Create a reference table\n        * For each item in the "from"-reference column:\n          * Add new rows in the reference table for each "to"-identifier, using the same "from"-identifier\n            * Example: Table "experiment-replicate" with columns "experiment.@id", "replicate.@id"\n        * Delete the complete column from the original table\n* ### Step 4: Satisfy 2NF\n    * _Input:_ Pandas DataFrames (original tables without reference column) [1NF] + reference tables\n    * _Output:_ Pandas DataFrames (original tables without reference column) [2NF] + reference tables\n    * _Description:_ Automatic transformation of original tables into second normal form ([2NF](https://en.wikipedia.org/wiki/Database_normalization#Satisfying_2NF)):\n    * _Generalizable:_ Fully (if not, we skip it)\n    * _Manual/automatic:_ Automatic\n    * _Details:_\n      * Use existing library.\n* ### Step 5: Satisfy 3NF\n    * _Input:_ Pandas DataFrames (original tables without reference column) [2NF] + reference tables\n    * _Output:_ Pandas DataFrames (original tables without reference column) [3NF] + reference tables\n    * _Description:_ Automatic transformation of original tables into third normal form ([3NF](https://en.wikipedia.org/wiki/Database_normalization#Satisfying_3NF)):\n    * _Generalizable:_ Fully (if not, we skip it)\n    * _Manual/automatic:_ Automatic\n    * _Details:_\n      * Use existing library.\n* ### Step 6: Create model map\n    * _Input:_ Pandas DataFrames (original tables without reference column) [Any NF] + reference tables + FAIRtracks JSON schemas\n    * _Output:_ Model map [some data structure (to be defined) mapping FAIRtracks objects and attributes to tables/columns in the original data]\n    * _Description:_ Manual mapping of FAIRtracks objects and attributes to corresponding tables and columns in the original data.\n    * _Generalizable:_ Fully\n    * _Manual/automatic:_ Manual\n    * Details:\n      * For each FAIRtracks object:\n        * Define a start table in the original data\n        * For each FAIRtracks attribute:\n          * Manually find the path (or paths) to the original table/column that this maps to\n            * _Example:_ `Experiments:organism (FAIRtracks) -> Experiments.Biosamples.Organism.scientific_name`\n* ### Step 7: Apply model map to generate initial FAIRtracks tables\n  * _Input:_ Pandas DataFrames (original tables without reference column) [Any NF] + reference tables + Model map \n  * _Output:_ Pandas DataFrames (initial FAIRtracks tables, possibly with multimapped attributes)\n    * Example: `Experiment.target_from_origcolumn1` and `Experimentl.target_from_origcolumn2` contain content from two different attributes from the original data that both corresponds to `Experiment.target`\n  * _Description:_ Generate initial FAIRtracks tables by applying the model map, mapping FAIRtracks attributes with one or more attributes (columns) in the original table.\n  * _Generalizable:_ Fully\n  * _Manual/automatic:_ Automatic\n  * _Details:_\n    * For every FAIRtracks object:\n      * Create a new pandas DataFrame\n      * For every FAIRtracks attribute:\n        * From the model map, get the path to the corresponding original table/column, or a list of such paths in case of multimapping\n        * For each path:\n          * Automatically join tables to get primary keys and attribute value in the same table:\n            * _Example:_ `experiment-biosample JOIN biosample-organism JOIN organism` will create mapping table with two columns: `Experiments.local_id` and `Organism.scientific_name`\n          * Add column to FAIRtracks DataFrame\n          * In case of multimodeling, record the relation between FAIRtracks attribute and corresponding multimapped attributes, e.g. by generating unique attribute names for each path, such as `Experiment.target_from_origcolumn1` and `Experiment.target_from_origcolumn2`, which one can derive directly from the model map.\n* ### Step 8: Harmonize multimapped attributes\n  * _Input:_ Pandas DataFrames (initial FAIRtracks tables, possibly with multimapped attributes) + model map\n  * _Output:_ Pandas DataFrames (initial FAIRtracks tables)\n  * _Description:_ Harmonize multimapped attributes manually, or possibly by applying scripts\n  * _Generalizable:_ Limited (mostly by reusing util functions)\n  * _Manual/automatic:_ Mixed (possibly scriptable)\n  * _Details:_\n    * For all multimapped attributes:\n      * Manually review values (in batch mode) and generate a single output value for each combination:\n        * Hopefully Open Refine can be used for this. If so, one needs to implement data input/output mechanisms.\n\n* ### Further steps to be detailed:\n  * For all FAIRtracks attributes with ontology terms: Convert terms using required ontologies\n  * Other FAIRtracks specific value conversion \n  * Manual batch correction of values (possibly with errors), probably using Open Refine\n  * Validation of FAIRtracks document\n\nSuggestion: we will use Pandas DataFrames as the core data structure for tables, given that the library provides the required features (specifically Foreign key and Join capabilities)\n\n\n',
     'author': 'Sveinung Gundersen',
     'author_email': 'sveinugu@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fairtracks.net/fair/#fair-07-transformation',
```

### Comparing `omnipy-0.9.3/PKG-INFO` & `omnipy-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnipy
-Version: 0.9.3
+Version: 0.9.5
 Summary: Omnipy is a high level Python library for type-driven data wrangling and scalable workflow orchestration (under development)
 Home-page: https://fairtracks.net/fair/#fair-07-transformation
 License: Apache-2.0
 Keywords: data wrangling,metadata,workflows,etl,research data,prefect,pydantic,FAIR,ontologies,JSON,tabular,type-driven,orchestration,data models,universal
 Author: Sveinung Gundersen
 Author-email: sveinugu@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -17,23 +17,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiostream (>=0.4.5,<0.5.0)
 Requires-Dist: greenlet (>=2.0.1,<3.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
 Requires-Dist: prefect (>=2.7.3,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.20.2,<0.21.0)
 Requires-Dist: pytest-cases (>=3.6.13,<4.0.0)
-Requires-Dist: python-slugify (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
+Project-URL: Documentation, http://omnipy.readthedocs.io/
 Project-URL: Repository, http://github.com/fairtracks/omnipy
 Description-Content-Type: text/markdown
 
 
 ![Omnypy logo](https://fairtracks.net/_nuxt/img/9a84303.webp)
 
 Omnipy is the new name of the Python package formerly known as uniFAIR.
```

