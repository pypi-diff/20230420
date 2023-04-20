# Comparing `tmp/flipper-client-1.3.1.tar.gz` & `tmp/flipper-client-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flipper-client-1.3.1.tar", last modified: Wed Sep 28 16:56:33 2022, max compression
+gzip compressed data, was "dist/flipper-client-1.3.2.tar", last modified: Thu Apr 20 17:43:51 2023, max compression
```

## Comparing `flipper-client-1.3.1.tar` & `flipper-client-1.3.2.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      571 2019-03-27 16:48:33.000000 flipper-client-1.3.1/LICENSE.txt
--rw-r--r--   0 adamsavitzky   (501) staff       (20)       47 2019-07-18 21:23:41.000000 flipper-client-1.3.1/MANIFEST.in
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    38156 2022-09-28 16:56:33.000000 flipper-client-1.3.1/PKG-INFO
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    30638 2022-05-24 16:15:07.000000 flipper-client-1.3.1/README.md
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1341 2022-05-24 16:14:27.000000 flipper-client-1.3.1/flipper/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/bucketing/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1075 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1082 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/base.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2789 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/consistent_hash_percentage_bucketer.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1474 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/factory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1015 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/noop_bucketer.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      873 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1967 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage/base.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1321 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage/factory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2469 2020-11-19 17:57:11.000000 flipper-client-1.3.1/flipper/bucketing/percentage/linear_ramp_percentage.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1168 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage/percentage.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1698 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/bucketing/percentage_bucketer.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     6036 2020-02-06 16:47:28.000000 flipper-client-1.3.1/flipper/client.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/conditions/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      651 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2305 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/check.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2258 2019-07-18 21:23:41.000000 flipper-client-1.3.1/flipper/conditions/condition.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/conditions/operators/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      648 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      813 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/equality_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      815 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/greater_than_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      826 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/greater_than_or_equal_to_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      890 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/interface.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      812 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/less_than_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      823 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/less_than_or_equal_to_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      848 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/negated_set_membership_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      813 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/negation_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1989 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      833 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/conditions/operators/set_membership_operator.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/contrib/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1207 2022-05-24 16:14:27.000000 flipper-client-1.3.1/flipper/contrib/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2512 2020-06-04 20:03:28.000000 flipper-client-1.3.1/flipper/contrib/cached.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     3956 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/consul.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1539 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/interface.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2700 2019-07-15 22:51:31.000000 flipper-client-1.3.1/flipper/contrib/memory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     5650 2022-08-01 16:03:31.000000 flipper-client-1.3.1/flipper/contrib/postgresql.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4065 2020-02-06 16:47:28.000000 flipper-client-1.3.1/flipper/contrib/redis.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     3828 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/replicated.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     3817 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/s3.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/contrib/storage/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      731 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/storage/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2370 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/storage/item.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2647 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/storage/meta.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     5702 2019-11-14 20:07:15.000000 flipper-client-1.3.1/flipper/contrib/thrift.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/contrib/util/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      592 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/util/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      686 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper/contrib/util/date.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      877 2019-10-28 17:10:57.000000 flipper-client-1.3.1/flipper/contrib/util/iter.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1074 2019-11-06 17:39:41.000000 flipper-client-1.3.1/flipper/decorators.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper/events/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      835 2019-11-14 20:07:15.000000 flipper-client-1.3.1/flipper/events/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1919 2019-11-14 20:07:15.000000 flipper-client-1.3.1/flipper/events/emitter.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2098 2020-02-06 16:47:28.000000 flipper-client-1.3.1/flipper/events/subscriber.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1266 2020-02-06 16:47:28.000000 flipper-client-1.3.1/flipper/events/types.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      643 2019-11-14 20:07:15.000000 flipper-client-1.3.1/flipper/exceptions.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1967 2020-02-06 16:47:28.000000 flipper-client-1.3.1/flipper/flag.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    38156 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/PKG-INFO
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     3919 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/SOURCES.txt
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        1 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/dependency_links.txt
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      279 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/requires.txt
--rw-r--r--   0 adamsavitzky   (501) staff       (20)       29 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_client.egg-info/top_level.txt
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_thrift/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper_thrift/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1984 2019-07-18 21:23:41.000000 flipper-client-1.3.1/flipper_thrift/feature_flag_store.thrift
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_thrift/python/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:33.000000 flipper-client-1.3.1/flipper_thrift/python/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    44379 2019-07-18 21:23:41.000000 flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/FeatureFlagStore.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      647 2019-07-18 21:09:04.000000 flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      959 2019-07-18 21:09:04.000000 flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/constants.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    17431 2019-07-18 21:23:41.000000 flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/ttypes.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      195 2019-03-27 16:48:32.000000 flipper-client-1.3.1/pyproject.toml
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      115 2022-09-28 16:56:33.000000 flipper-client-1.3.1/setup.cfg
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1030 2022-09-28 16:56:19.000000 flipper-client-1.3.1/setup.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-02-08 00:36:53.000000 flipper-client-1.3.1/tests/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/bucketing/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/bucketing/percentage/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/percentage/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      575 2020-11-19 17:57:11.000000 flipper-client-1.3.1/tests/bucketing/percentage/test_base.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1012 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/percentage/test_factory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4233 2020-11-19 17:57:11.000000 flipper-client-1.3.1/tests/bucketing/percentage/test_linear_ramp_percentage.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1077 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/percentage/test_percentage.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4176 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/bucketing/test_consistent_hash_percentage_bucketer.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1382 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/test_factory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      985 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/test_noop_bucketer.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2536 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/bucketing/test_percentage_bucketer.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/conditions/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/conditions/operators/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      424 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/test_equality_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      608 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/test_greater_than_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      738 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/conditions/operators/test_greater_than_or_equal_to_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/test_less_than_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      723 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/conditions/operators/test_less_than_or_equal_to_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      584 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/conditions/operators/test_negated_set_membership_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      420 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/test_negation_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)      471 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/conditions/operators/test_set_membership_operator.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4206 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/conditions/test_check.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     6566 2019-08-12 20:12:15.000000 flipper-client-1.3.1/tests/conditions/test_condition.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/contrib/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-02-08 00:36:53.000000 flipper-client-1.3.1/tests/contrib/__init__.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/contrib/storage/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:31.000000 flipper-client-1.3.1/tests/contrib/storage/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     7828 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/contrib/storage/test_item.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4377 2019-03-27 16:48:33.000000 flipper-client-1.3.1/tests/contrib/storage/test_meta.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     8523 2020-06-04 20:03:28.000000 flipper-client-1.3.1/tests/contrib/test_cached.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     5355 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/contrib/test_memory.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     4137 2022-05-24 16:15:07.000000 flipper-client-1.3.1/tests/contrib/test_postgresql.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     7907 2022-05-24 16:09:56.000000 flipper-client-1.3.1/tests/contrib/test_redis.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     6428 2019-03-27 16:48:33.000000 flipper-client-1.3.1/tests/contrib/test_replicated.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     8416 2019-03-27 16:48:33.000000 flipper-client-1.3.1/tests/contrib/test_s3.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     7390 2019-08-12 20:18:53.000000 flipper-client-1.3.1/tests/contrib/test_thrift.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/contrib/util/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-10-28 17:10:57.000000 flipper-client-1.3.1/tests/contrib/util/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1087 2019-10-28 17:10:57.000000 flipper-client-1.3.1/tests/contrib/util/test_iter.py
-drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2022-09-28 16:56:33.000000 flipper-client-1.3.1/tests/events/
--rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-11-14 20:07:15.000000 flipper-client-1.3.1/tests/events/__init__.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     2803 2020-11-19 17:57:05.000000 flipper-client-1.3.1/tests/events/test_emitter.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    22425 2021-09-30 18:05:41.000000 flipper-client-1.3.1/tests/test_client.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)     1869 2019-03-27 16:48:32.000000 flipper-client-1.3.1/tests/test_decorators.py
--rw-r--r--   0 adamsavitzky   (501) staff       (20)    10950 2020-02-06 16:47:28.000000 flipper-client-1.3.1/tests/test_flag.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      571 2019-03-27 16:48:33.000000 flipper-client-1.3.2/LICENSE.txt
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)       47 2019-07-18 21:23:41.000000 flipper-client-1.3.2/MANIFEST.in
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    38156 2023-04-20 17:43:51.000000 flipper-client-1.3.2/PKG-INFO
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    30638 2022-05-24 16:15:07.000000 flipper-client-1.3.2/README.md
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1341 2022-05-24 16:14:27.000000 flipper-client-1.3.2/flipper/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/bucketing/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1075 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1082 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/base.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2789 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/consistent_hash_percentage_bucketer.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1474 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/factory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1015 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/noop_bucketer.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/bucketing/percentage/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      873 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/percentage/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1967 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/percentage/base.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1321 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/percentage/factory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2469 2020-11-19 17:57:11.000000 flipper-client-1.3.2/flipper/bucketing/percentage/linear_ramp_percentage.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1168 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/percentage/percentage.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1698 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/bucketing/percentage_bucketer.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     6036 2020-02-06 16:47:28.000000 flipper-client-1.3.2/flipper/client.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/conditions/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      651 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2305 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/check.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2258 2019-07-18 21:23:41.000000 flipper-client-1.3.2/flipper/conditions/condition.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/conditions/operators/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      648 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      813 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/equality_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      815 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/greater_than_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      826 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/greater_than_or_equal_to_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      890 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/interface.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      812 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/less_than_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      823 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/less_than_or_equal_to_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      848 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/negated_set_membership_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      813 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/negation_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1989 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      833 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/conditions/operators/set_membership_operator.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/contrib/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1207 2022-05-24 16:14:27.000000 flipper-client-1.3.2/flipper/contrib/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2512 2020-06-04 20:03:28.000000 flipper-client-1.3.2/flipper/contrib/cached.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     3956 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/consul.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1539 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/interface.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2700 2019-07-15 22:51:31.000000 flipper-client-1.3.2/flipper/contrib/memory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     5650 2022-08-01 16:03:31.000000 flipper-client-1.3.2/flipper/contrib/postgresql.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4065 2020-02-06 16:47:28.000000 flipper-client-1.3.2/flipper/contrib/redis.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     3828 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/replicated.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     3817 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/s3.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/contrib/storage/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      731 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/storage/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2370 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/storage/item.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2647 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/storage/meta.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     5702 2019-11-14 20:07:15.000000 flipper-client-1.3.2/flipper/contrib/thrift.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/contrib/util/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      592 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/util/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      686 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper/contrib/util/date.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      877 2019-10-28 17:10:57.000000 flipper-client-1.3.2/flipper/contrib/util/iter.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1074 2019-11-06 17:39:41.000000 flipper-client-1.3.2/flipper/decorators.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper/events/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      835 2019-11-14 20:07:15.000000 flipper-client-1.3.2/flipper/events/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1919 2019-11-14 20:07:15.000000 flipper-client-1.3.2/flipper/events/emitter.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2098 2020-02-06 16:47:28.000000 flipper-client-1.3.2/flipper/events/subscriber.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1266 2020-02-06 16:47:28.000000 flipper-client-1.3.2/flipper/events/types.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      643 2019-11-14 20:07:15.000000 flipper-client-1.3.2/flipper/exceptions.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1967 2020-02-06 16:47:28.000000 flipper-client-1.3.2/flipper/flag.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    38156 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/PKG-INFO
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     3919 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        1 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      282 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/requires.txt
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)       29 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_client.egg-info/top_level.txt
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_thrift/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper_thrift/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1984 2019-07-18 21:23:41.000000 flipper-client-1.3.2/flipper_thrift/feature_flag_store.thrift
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_thrift/python/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:33.000000 flipper-client-1.3.2/flipper_thrift/python/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    44379 2019-07-18 21:23:41.000000 flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/FeatureFlagStore.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      647 2019-07-18 21:09:04.000000 flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      959 2019-07-18 21:09:04.000000 flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/constants.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    17431 2019-07-18 21:23:41.000000 flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/ttypes.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      195 2019-03-27 16:48:32.000000 flipper-client-1.3.2/pyproject.toml
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      115 2023-04-20 17:43:51.000000 flipper-client-1.3.2/setup.cfg
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1033 2023-04-20 17:27:29.000000 flipper-client-1.3.2/setup.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-02-08 00:36:53.000000 flipper-client-1.3.2/tests/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/bucketing/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/bucketing/percentage/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/percentage/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      575 2020-11-19 17:57:11.000000 flipper-client-1.3.2/tests/bucketing/percentage/test_base.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1012 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/percentage/test_factory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4233 2020-11-19 17:57:11.000000 flipper-client-1.3.2/tests/bucketing/percentage/test_linear_ramp_percentage.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1077 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/percentage/test_percentage.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4176 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/bucketing/test_consistent_hash_percentage_bucketer.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1382 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/test_factory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      985 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/test_noop_bucketer.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2536 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/bucketing/test_percentage_bucketer.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/conditions/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/conditions/operators/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      424 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/test_equality_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      608 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/test_greater_than_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      738 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/conditions/operators/test_greater_than_or_equal_to_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      593 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/test_less_than_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      723 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/conditions/operators/test_less_than_or_equal_to_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      584 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/conditions/operators/test_negated_set_membership_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      420 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/test_negation_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)      471 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/conditions/operators/test_set_membership_operator.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4206 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/conditions/test_check.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     6566 2019-08-12 20:12:15.000000 flipper-client-1.3.2/tests/conditions/test_condition.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/contrib/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-02-08 00:36:53.000000 flipper-client-1.3.2/tests/contrib/__init__.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/contrib/storage/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-03-27 16:48:31.000000 flipper-client-1.3.2/tests/contrib/storage/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     7828 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/contrib/storage/test_item.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4377 2019-03-27 16:48:33.000000 flipper-client-1.3.2/tests/contrib/storage/test_meta.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     8523 2020-06-04 20:03:28.000000 flipper-client-1.3.2/tests/contrib/test_cached.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     5355 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/contrib/test_memory.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     4137 2022-05-24 16:15:07.000000 flipper-client-1.3.2/tests/contrib/test_postgresql.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     7907 2022-05-24 16:09:56.000000 flipper-client-1.3.2/tests/contrib/test_redis.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     6428 2019-03-27 16:48:33.000000 flipper-client-1.3.2/tests/contrib/test_replicated.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     8416 2019-03-27 16:48:33.000000 flipper-client-1.3.2/tests/contrib/test_s3.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     7390 2019-08-12 20:18:53.000000 flipper-client-1.3.2/tests/contrib/test_thrift.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/contrib/util/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-10-28 17:10:57.000000 flipper-client-1.3.2/tests/contrib/util/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1087 2019-10-28 17:10:57.000000 flipper-client-1.3.2/tests/contrib/util/test_iter.py
+drwxr-xr-x   0 adamsavitzky   (501) staff       (20)        0 2023-04-20 17:43:51.000000 flipper-client-1.3.2/tests/events/
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)        0 2019-11-14 20:07:15.000000 flipper-client-1.3.2/tests/events/__init__.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     2803 2020-11-19 17:57:05.000000 flipper-client-1.3.2/tests/events/test_emitter.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    22425 2021-09-30 18:05:41.000000 flipper-client-1.3.2/tests/test_client.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)     1869 2019-03-27 16:48:32.000000 flipper-client-1.3.2/tests/test_decorators.py
+-rw-r--r--   0 adamsavitzky   (501) staff       (20)    10950 2020-02-06 16:47:28.000000 flipper-client-1.3.2/tests/test_flag.py
```

### Comparing `flipper-client-1.3.1/LICENSE.txt` & `flipper-client-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/PKG-INFO` & `flipper-client-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipper-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Description: Flipper
         =======
         ![Circle CI Status](https://circleci.com/gh/carta/flipper-client/tree/master.svg?style=shield&circle-token=e401445db3e99e8fac7555bd9ba5040e6a2eb4bd)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `flipper-client-1.3.1/README.md` & `flipper-client-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/__init__.py` & `flipper-client-1.3.2/flipper/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/__init__.py` & `flipper-client-1.3.2/flipper/bucketing/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/base.py` & `flipper-client-1.3.2/flipper/bucketing/base.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/consistent_hash_percentage_bucketer.py` & `flipper-client-1.3.2/flipper/bucketing/consistent_hash_percentage_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/factory.py` & `flipper-client-1.3.2/flipper/bucketing/factory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/noop_bucketer.py` & `flipper-client-1.3.2/flipper/bucketing/noop_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage/__init__.py` & `flipper-client-1.3.2/flipper/bucketing/percentage/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage/base.py` & `flipper-client-1.3.2/flipper/bucketing/percentage/base.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage/factory.py` & `flipper-client-1.3.2/flipper/bucketing/percentage/factory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage/linear_ramp_percentage.py` & `flipper-client-1.3.2/flipper/bucketing/percentage/linear_ramp_percentage.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage/percentage.py` & `flipper-client-1.3.2/flipper/bucketing/percentage/percentage.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/bucketing/percentage_bucketer.py` & `flipper-client-1.3.2/flipper/bucketing/percentage_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/client.py` & `flipper-client-1.3.2/flipper/client.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/__init__.py` & `flipper-client-1.3.2/flipper/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/check.py` & `flipper-client-1.3.2/flipper/conditions/check.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/condition.py` & `flipper-client-1.3.2/flipper/conditions/condition.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/__init__.py` & `flipper-client-1.3.2/flipper/conditions/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/equality_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/equality_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/greater_than_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/greater_than_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/greater_than_or_equal_to_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/greater_than_or_equal_to_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/interface.py` & `flipper-client-1.3.2/flipper/conditions/operators/interface.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/less_than_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/less_than_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/less_than_or_equal_to_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/less_than_or_equal_to_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/negated_set_membership_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/negated_set_membership_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/negation_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/negation_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/conditions/operators/set_membership_operator.py` & `flipper-client-1.3.2/flipper/conditions/operators/set_membership_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/__init__.py` & `flipper-client-1.3.2/flipper/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/cached.py` & `flipper-client-1.3.2/flipper/contrib/cached.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/consul.py` & `flipper-client-1.3.2/flipper/contrib/consul.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/interface.py` & `flipper-client-1.3.2/flipper/contrib/interface.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/memory.py` & `flipper-client-1.3.2/flipper/contrib/memory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/postgresql.py` & `flipper-client-1.3.2/flipper/contrib/postgresql.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/redis.py` & `flipper-client-1.3.2/flipper/contrib/redis.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/replicated.py` & `flipper-client-1.3.2/flipper/contrib/replicated.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/s3.py` & `flipper-client-1.3.2/flipper/contrib/s3.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/storage/__init__.py` & `flipper-client-1.3.2/flipper/contrib/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/storage/item.py` & `flipper-client-1.3.2/flipper/contrib/storage/item.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/storage/meta.py` & `flipper-client-1.3.2/flipper/contrib/storage/meta.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/thrift.py` & `flipper-client-1.3.2/flipper/contrib/thrift.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/util/__init__.py` & `flipper-client-1.3.2/flipper/contrib/util/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/util/date.py` & `flipper-client-1.3.2/flipper/contrib/util/date.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/contrib/util/iter.py` & `flipper-client-1.3.2/flipper/contrib/util/iter.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/decorators.py` & `flipper-client-1.3.2/flipper/decorators.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/events/__init__.py` & `flipper-client-1.3.2/flipper/events/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/events/emitter.py` & `flipper-client-1.3.2/flipper/events/emitter.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/events/subscriber.py` & `flipper-client-1.3.2/flipper/events/subscriber.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/events/types.py` & `flipper-client-1.3.2/flipper/events/types.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/exceptions.py` & `flipper-client-1.3.2/flipper/exceptions.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper/flag.py` & `flipper-client-1.3.2/flipper/flag.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_client.egg-info/PKG-INFO` & `flipper-client-1.3.2/flipper_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipper-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Description: Flipper
         =======
         ![Circle CI Status](https://circleci.com/gh/carta/flipper-client/tree/master.svg?style=shield&circle-token=e401445db3e99e8fac7555bd9ba5040e6a2eb4bd)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `flipper-client-1.3.1/flipper_client.egg-info/SOURCES.txt` & `flipper-client-1.3.2/flipper_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/__init__.py` & `flipper-client-1.3.2/flipper_thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/feature_flag_store.thrift` & `flipper-client-1.3.2/flipper_thrift/feature_flag_store.thrift`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/python/__init__.py` & `flipper-client-1.3.2/flipper_thrift/python/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/FeatureFlagStore.py` & `flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/FeatureFlagStore.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/__init__.py` & `flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/__init__.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/constants.py` & `flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/constants.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/flipper_thrift/python/feature_flag_store/ttypes.py` & `flipper-client-1.3.2/flipper_thrift/python/feature_flag_store/ttypes.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/setup.py` & `flipper-client-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 requirements = [
-    "cachetools~=4.2.1",
+    "cachetools>=4.2.1,<6",
     "python-consul~=1.0",
     "redis>=2.10.6,<5",
     "thrift~=0.13",
     "boto3~=1.9",
     "pyee~=6.0",
 ]
 
 
 setup(
     name="flipper-client",
-    version="1.3.1",
+    version="1.3.2",
     packages=find_packages(),
     license="Apache License 2.0",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require={
         "postgres": ["psycopg~=3.0.10"],
```

### Comparing `flipper-client-1.3.1/tests/bucketing/percentage/test_base.py` & `flipper-client-1.3.2/tests/bucketing/percentage/test_base.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/percentage/test_factory.py` & `flipper-client-1.3.2/tests/bucketing/percentage/test_factory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/percentage/test_linear_ramp_percentage.py` & `flipper-client-1.3.2/tests/bucketing/percentage/test_linear_ramp_percentage.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/percentage/test_percentage.py` & `flipper-client-1.3.2/tests/bucketing/percentage/test_percentage.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/test_consistent_hash_percentage_bucketer.py` & `flipper-client-1.3.2/tests/bucketing/test_consistent_hash_percentage_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/test_factory.py` & `flipper-client-1.3.2/tests/bucketing/test_factory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/test_noop_bucketer.py` & `flipper-client-1.3.2/tests/bucketing/test_noop_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/bucketing/test_percentage_bucketer.py` & `flipper-client-1.3.2/tests/bucketing/test_percentage_bucketer.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/operators/test_greater_than_operator.py` & `flipper-client-1.3.2/tests/conditions/operators/test_greater_than_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/operators/test_greater_than_or_equal_to_operator.py` & `flipper-client-1.3.2/tests/conditions/operators/test_greater_than_or_equal_to_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/operators/test_less_than_operator.py` & `flipper-client-1.3.2/tests/conditions/operators/test_less_than_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/operators/test_less_than_or_equal_to_operator.py` & `flipper-client-1.3.2/tests/conditions/operators/test_less_than_or_equal_to_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/operators/test_negated_set_membership_operator.py` & `flipper-client-1.3.2/tests/conditions/operators/test_negated_set_membership_operator.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/test_check.py` & `flipper-client-1.3.2/tests/conditions/test_check.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/conditions/test_condition.py` & `flipper-client-1.3.2/tests/conditions/test_condition.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/storage/test_item.py` & `flipper-client-1.3.2/tests/contrib/storage/test_item.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/storage/test_meta.py` & `flipper-client-1.3.2/tests/contrib/storage/test_meta.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_cached.py` & `flipper-client-1.3.2/tests/contrib/test_cached.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_memory.py` & `flipper-client-1.3.2/tests/contrib/test_memory.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_postgresql.py` & `flipper-client-1.3.2/tests/contrib/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_redis.py` & `flipper-client-1.3.2/tests/contrib/test_redis.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_replicated.py` & `flipper-client-1.3.2/tests/contrib/test_replicated.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_s3.py` & `flipper-client-1.3.2/tests/contrib/test_s3.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/test_thrift.py` & `flipper-client-1.3.2/tests/contrib/test_thrift.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/contrib/util/test_iter.py` & `flipper-client-1.3.2/tests/contrib/util/test_iter.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/events/test_emitter.py` & `flipper-client-1.3.2/tests/events/test_emitter.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/test_client.py` & `flipper-client-1.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/test_decorators.py` & `flipper-client-1.3.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `flipper-client-1.3.1/tests/test_flag.py` & `flipper-client-1.3.2/tests/test_flag.py`

 * *Files identical despite different names*

