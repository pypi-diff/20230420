# Comparing `tmp/pubtools-pulp-1.9.2.tar.gz` & `tmp/pubtools-pulp-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubtools-pulp-1.9.2.tar", last modified: Tue Mar 15 05:22:22 2022, max compression
+gzip compressed data, was "pubtools-pulp-1.9.3.tar", last modified: Wed Mar 16 20:25:56 2022, max compression
```

## Comparing `pubtools-pulp-1.9.2.tar` & `pubtools-pulp-1.9.3.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.079190 pubtools-pulp-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     4531 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-03-15 05:22:22.079190 pubtools-pulp-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.043190 pubtools-pulp-1.9.2/pubtools/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.043190 pubtools-pulp-1.9.2/pubtools/_pulp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.043190 pubtools-pulp-1.9.2/pubtools/_pulp/services/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/cachingpulp.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/fakepulp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/fastpurge_.py
--rw-r--r--   0 runner    (1001) docker     (121)     3786 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/pulp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/services/udcache.py
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/step.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.043190 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9754 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/clear_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/fix_cves.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (121)     4587 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.047190 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/contextlib_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/copy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.051190 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19325 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/comps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/direct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/erratum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3452 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/erratum_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/modulemd.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/productid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/rpm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.059190 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/associate.py
--rw-r--r--   0 runner    (1001) docker     (121)    16585 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)     9229 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/end_pre_push.py
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/load_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/load_sums.py
--rw-r--r--   0 runner    (1001) docker     (121)     3707 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/query_pulp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/update.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.063190 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/set_maintenance_off.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/set_maintenance_on.py
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/pubtools/_pulp/ud.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.063190 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-15 05:22:21.000000 pubtools-pulp-1.9.2/pubtools_pulp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 05:22:22.079190 pubtools-pulp-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.039190 pubtools-pulp-1.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:22.079190 pubtools-pulp-1.9.2/tests/push/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_associate_item_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_collect_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     7502 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_context_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_item_state_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5793 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_load_sums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_phase_batching.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_phase_error_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_phase_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_pulperratumpushitem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_pulppushitem.py
--rw-r--r--   0 runner    (1001) docker     (121)    12044 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_push.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_push_copy_fails.py
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_push_prepush.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/test_rpm_bad_filename.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-15 05:22:11.000000 pubtools-pulp-1.9.2/tests/push/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.078527 pubtools-pulp-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-03-16 20:25:56.074528 pubtools-pulp-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.062530 pubtools-pulp-1.9.3/pubtools/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.062530 pubtools-pulp-1.9.3/pubtools/_pulp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.066529 pubtools-pulp-1.9.3/pubtools/_pulp/services/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/cachingpulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/fakepulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3444 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/fastpurge_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3786 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/pulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/services/udcache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.066529 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9754 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/clear_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/fix_cves.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4587 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.066529 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/contextlib_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/copy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.070529 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20514 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/comps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/direct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/erratum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3452 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/erratum_conv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/modulemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/productid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/rpm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.070529 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/associate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16585 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/collect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9229 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/end_pre_push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/load_items.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/load_sums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3707 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/query_pulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.070529 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/set_maintenance_off.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/set_maintenance_on.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/pubtools/_pulp/ud.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.074528 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-16 20:25:55.000000 pubtools-pulp-1.9.3/pubtools_pulp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 20:25:56.078527 pubtools-pulp-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.062530 pubtools-pulp-1.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:56.074528 pubtools-pulp-1.9.3/tests/push/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_associate_item_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_collect_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7502 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_context_counts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_item_state_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5793 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_load_sums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_phase_batching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_phase_error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_phase_limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_pulperratumpushitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_pulppushitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_push_copy_fails.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_push_prepush.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_rpm_bad_filename.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/test_upload_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-16 20:25:47.000000 pubtools-pulp-1.9.3/tests/push/util.py
```

### Comparing `pubtools-pulp-1.9.2/CHANGELOG.md` & `pubtools-pulp-1.9.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 - n/a
 
+## [1.9.3] - 2022-03-17
+
+- `pubtools-pulp-push`: when the same file exists multiple times in a push, it will no
+  longer be uploaded to Pulp more than once.
+
 ## [1.9.2] - 2022-03-15
 
 - `pubtools-pulp-push`: improved pipelining behavior for larger pushes
 - `pubtools-pulp-push`: fixed duplicate push item metadata
 
 ## [1.9.1] - 2022-03-09
 
@@ -99,15 +104,16 @@
 
 - Publish and maintenance-on/off commands accept comma seperated repo-ids
 
 ## 0.1.0 - 2019-10-09
 
 - Initial release to PyPI
 
-[Unreleased]: https://github.com/release-engineering/pubtools-pulp/compare/v1.9.2...HEAD
+[Unreleased]: https://github.com/release-engineering/pubtools-pulp/compare/v1.9.3...HEAD
+[1.9.3]: https://github.com/release-engineering/pubtools-pulp/compare/v1.9.2...v1.9.3
 [1.9.2]: https://github.com/release-engineering/pubtools-pulp/compare/v1.9.1...v1.9.2
 [1.9.1]: https://github.com/release-engineering/pubtools-pulp/compare/v1.9.0...v1.9.1
 [1.9.0]: https://github.com/release-engineering/pubtools-pulp/compare/v1.8.2...v1.9.0
 [1.8.2]: https://github.com/release-engineering/pubtools-pulp/compare/v1.8.1...v1.8.2
 [1.8.1]: https://github.com/release-engineering/pubtools-pulp/compare/v1.8.0...v1.8.1
 [1.8.0]: https://github.com/release-engineering/pubtools-pulp/compare/v1.7.1...v1.8.0
 [1.7.1]: https://github.com/release-engineering/pubtools-pulp/compare/v1.7.0...v1.7.1
```

### Comparing `pubtools-pulp-1.9.2/LICENSE` & `pubtools-pulp-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/PKG-INFO` & `pubtools-pulp-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-pulp
-Version: 1.9.2
+Version: 1.9.3
 Summary: Publishing tools for Pulp
 Home-page: https://github.com/release-engineering/pubtools-pulp
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-pulp/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-pulp/blob/master/CHANGELOG.md
 Description:
```

### Comparing `pubtools-pulp-1.9.2/README.md` & `pubtools-pulp-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/arguments.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/arguments.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/base.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/base.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/cachingpulp.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/cachingpulp.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/collector.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/collector.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/fakepulp.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/fakepulp.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/fastpurge_.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/fastpurge_.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/pulp.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/pulp.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/services/udcache.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/services/udcache.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/step.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/step.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/task.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/task.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/clear_repo.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/clear_repo.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/common.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/common.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/fix_cves.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/fix_cves.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/garbage_collect.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/garbage_collect.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/publish.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/publish.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/command.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/command.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/contextlib_compat.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/contextlib_compat.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/copy.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/copy.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/base.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     IN_REPOS = "IN_REPOS"
 
 
 @attr.s(frozen=True, slots=True)
 class UploadContext(object):
     client = attr.ib(default=None)
     random = attr.ib(default=None)
+    uploads_by_key = attr.ib(default=attr.Factory(dict))
 
 
 @attr.s(frozen=True, slots=True)
 class PulpPushItem(object):
     """Wraps a pushitem with additional info for Pulp push.
 
     This class must be subclassed for each specific content type supporting push.
@@ -387,56 +388,78 @@
         def handle_result(page):
             items = [self]
             matched = self.match_items_units(items, page.data)
             return next(matched)
 
         return f_map(pulp_client.search_content(crit), handle_result)
 
+    def with_pulp_refreshed_after_upload(self, pulp_client):
+        """Like with_pulp_refreshed, but additionally asserts that the item exists in
+        at least one Pulp repo, as expected after a successful upload.
+        """
+
+        # Helper to verify that we've really got into at least one repo as a result
+        # of the upload.
+        def asserting_uploaded_ok(item):
+            if not item.in_pulp_repos:
+                msg = (
+                    "Fatal error: item supposedly uploaded successfully, "
+                    "but remains missing from Pulp: %s"
+                ) % item.pushsource_item
+                raise RuntimeError(msg)
+            return item
+
+        out = self.with_pulp_refreshed(pulp_client)
+        return f_map(out, asserting_uploaded_ok)
+
     def ensure_uploaded(self, ctx, repo_f=None):
         """Ensure that this item is uploaded into at least one Pulp repo.
 
         Returns a Future with an updated copy of this item, resolved after
         upload succeeds.
 
         Should be called only if the caller has determined that the item needs
         an upload (e.g. because the item is missing).
 
         Subclasses MAY override this to customize upload behavior, however in
         most cases it makes more sense to override only `upload_to_repo`.
         """
-        # In order to get the unit into Pulp, we must first upload it into some
-        # (any) repo from dest.
-        if repo_f is None:
-            # Because uploading to a repo will lock the repo (during import task),
-            # for the most possible concurrency it's best to try to uniformly
-            # distribute the repos used for upload. For example if we receive
-            # 100 items all for repos [a, b, c, d], we will get the best
-            # performance if each repo is used for roughly 25 uploads.
-            #
-            # Hence the random choice of a target repo.
-            repo_id = ctx.random.choice(self.pushsource_item.dest)
-            repo_f = ctx.client.get_repository(repo_id)
 
-        upload_tasks = f_flat_map(repo_f, self.upload_to_repo)
+        upload_f = None
 
-        # Helper to verify that we've really got into at least one repo as a result
-        # of the upload.
-        def asserting_uploaded_ok(item):
-            if not item.in_pulp_repos:
-                msg = (
-                    "Fatal error: item supposedly uploaded successfully, "
-                    "but remains missing from Pulp: %s"
-                ) % item.pushsource_item
-                raise RuntimeError(msg)
-            return item
+        upload_key = self.upload_key
+        if upload_key:
+            # It might be possible to reuse an earlier upload.
+            upload_f = ctx.uploads_by_key.get(upload_key)
 
-        updated_f = f_flat_map(
-            upload_tasks, lambda _: self.with_pulp_refreshed(ctx.client)
+        if upload_f:
+            LOG.info("Upload shared for %s", self.pushsource_item.src)
+        else:
+            # In order to get the unit into Pulp, we must first upload it into some
+            # (any) repo from dest.
+            if repo_f is None:
+                # Because uploading to a repo will lock the repo (during import task),
+                # for the most possible concurrency it's best to try to uniformly
+                # distribute the repos used for upload. For example if we receive
+                # 100 items all for repos [a, b, c, d], we will get the best
+                # performance if each repo is used for roughly 25 uploads.
+                #
+                # Hence the random choice of a target repo.
+                repo_id = ctx.random.choice(self.pushsource_item.dest)
+                repo_f = ctx.client.get_repository(repo_id)
+
+            upload_f = f_flat_map(repo_f, self.upload_to_repo)
+
+            if upload_key:
+                # Cache this for later uploads having the same key
+                ctx.uploads_by_key[upload_key] = upload_f
+
+        return f_flat_map(
+            upload_f, lambda _: self.with_pulp_refreshed_after_upload(ctx.client)
         )
-        return f_map(updated_f, asserting_uploaded_ok)
 
     def ensure_uptodate(self, client):
         """Ensure that this item is up-to-date in Pulp.
 
         In this context, up-to-date means that any mutable fields on the associated
         Pulp unit hold the desired values (e.g. "description" field on FileUnits).
 
@@ -515,7 +538,17 @@
     def upload_to_repo(self, repo):
         """Upload this item to a specific repo.
 
         Subclasses MUST override this method to invoke whichever upload method is
         appropriate for the handled content type.
         """
         raise NotImplementedError()
+
+    @property
+    def upload_key(self):
+        """A key which can be associated with upload of this item to enable the
+        caching and reusing of upload futures.
+
+        Subclasses SHOULD override this to return a non-None hashable value for
+        content types which can safely reuse uploads.
+        """
+        return None
```

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/direct.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/direct.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/erratum.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/erratum.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/erratum_conv.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/erratum_conv.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/file.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,22 @@
             assert isinstance(unit, FileUnit)
             key = (unit.path, unit.sha256sum)
             units_by_key[key] = unit
 
         for item in items:
             yield item.with_unit(units_by_key.get(item.file_key))
 
+    @property
+    def upload_key(self):
+        # We can reuse prior uploads if they use an identical name & content.
+        # (It's a bit weird that you need to upload a file multiple times if you
+        # want it to appear with different names in different repos, but it's
+        # just the way Pulp works.)
+        return (self.pushsource_item.name, self.pushsource_item.sha256sum)
+
     def upload_to_repo(self, repo):
         return repo.upload_file(
             self.pushsource_item.src,
             relative_url=self.pushsource_item.name,
             description=self.pushsource_item.description,
             version=self.pushsource_item.version,
             display_order=self.pushsource_item.display_order,
```

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/items/rpm.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/items/rpm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 
 from pubtools.pulplib import RpmUnit, Criteria
 from pushsource import RpmPushItem
 import attr
 import six
 
-from .base import supports_type, PulpPushItem
+from .base import supports_type, PulpPushItem, UploadContext
 
 
 @attr.s(frozen=True, slots=True)
-class RpmUploader(object):
+class RpmUploadContext(UploadContext):
     """A custom context for RPM uploads.
 
     This context object avoids having to query the all-rpm-content repo repeatedly.
     """
 
     upload_repo = attr.ib(default=None)
-    client = attr.ib(default=None)
 
 
 @supports_type(RpmPushItem)
 @attr.s(frozen=True, slots=True)
 class PulpRpmPushItem(PulpPushItem):
     """Handler for RPMs."""
 
@@ -92,22 +91,28 @@
             units_by_sum[unit.sha256sum] = unit
 
         for item in items:
             yield item.with_unit(units_by_sum.get(item.pushsource_item.sha256sum))
 
     @classmethod
     def upload_context(cls, pulp_client):
-        return RpmUploader(
-            client=pulp_client, upload_repo=pulp_client.get_repository(cls.UPLOAD_REPO)
+        return RpmUploadContext(
+            client=pulp_client,
+            upload_repo=pulp_client.get_repository(cls.UPLOAD_REPO),
         )
 
     @property
     def can_pre_push(self):
         # We support pre-push by uploading to all-rpm-content first.
         return True
 
+    @property
+    def upload_key(self):
+        # Any prior upload of identical content can be reused.
+        return self.pushsource_item.sha256sum
+
     def ensure_uploaded(self, ctx, repo_f=None):
         # Overridden to force our desired upload repo.
         return super(PulpRpmPushItem, self).ensure_uploaded(ctx, ctx.upload_repo)
 
     def upload_to_repo(self, repo):
         return repo.upload_rpm(self.pushsource_item.src, cdn_path=self.cdn_path)
```

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/associate.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/associate.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/base.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/base.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/collect.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/collect.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/context.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/context.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/end_pre_push.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/end_pre_push.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/load_items.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/load_items.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/load_sums.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/load_sums.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/publish.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/publish.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/query_pulp.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/query_pulp.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/update.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/update.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/push/phase/upload.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/push/phase/upload.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/base.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/base.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/set_maintenance_off.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/set_maintenance_off.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/tasks/set_maintenance/set_maintenance_on.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/tasks/set_maintenance/set_maintenance_on.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools/_pulp/ud.py` & `pubtools-pulp-1.9.3/pubtools/_pulp/ud.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/pubtools_pulp.egg-info/PKG-INFO` & `pubtools-pulp-1.9.3/pubtools_pulp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-pulp
-Version: 1.9.2
+Version: 1.9.3
 Summary: Publishing tools for Pulp
 Home-page: https://github.com/release-engineering/pubtools-pulp
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-pulp/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-pulp/blob/master/CHANGELOG.md
 Description:
```

### Comparing `pubtools-pulp-1.9.2/pubtools_pulp.egg-info/SOURCES.txt` & `pubtools-pulp-1.9.3/pubtools_pulp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,8 +73,9 @@
 tests/push/test_phase_limits.py
 tests/push/test_pulperratumpushitem.py
 tests/push/test_pulppushitem.py
 tests/push/test_push.py
 tests/push/test_push_copy_fails.py
 tests/push/test_push_prepush.py
 tests/push/test_rpm_bad_filename.py
+tests/push/test_upload_sharing.py
 tests/push/util.py
```

### Comparing `pubtools-pulp-1.9.2/pubtools_pulp.egg-info/entry_points.txt` & `pubtools-pulp-1.9.3/pubtools_pulp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/setup.py` & `pubtools-pulp-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.in") as f:
         return f.read().splitlines()
 
 
 setup(
     name="pubtools-pulp",
-    version="1.9.2",
+    version="1.9.3",
     packages=find_packages(exclude=["tests"]),
     url="https://github.com/release-engineering/pubtools-pulp",
     license="GNU General Public License",
     description=get_description(),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `pubtools-pulp-1.9.2/tests/push/conftest.py` & `pubtools-pulp-1.9.3/tests/push/conftest.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_associate_item_order.py` & `pubtools-pulp-1.9.3/tests/push/test_associate_item_order.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_collect_duplicates.py` & `pubtools-pulp-1.9.3/tests/push/test_collect_duplicates.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_context_counts.py` & `pubtools-pulp-1.9.3/tests/push/test_context_counts.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_item_state_checks.py` & `pubtools-pulp-1.9.3/tests/push/test_item_state_checks.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_load_sums.py` & `pubtools-pulp-1.9.3/tests/push/test_load_sums.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_phase_batching.py` & `pubtools-pulp-1.9.3/tests/push/test_phase_batching.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_phase_error_logs.py` & `pubtools-pulp-1.9.3/tests/push/test_phase_error_logs.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_phase_limits.py` & `pubtools-pulp-1.9.3/tests/push/test_phase_limits.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_pulperratumpushitem.py` & `pubtools-pulp-1.9.3/tests/push/test_pulperratumpushitem.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_pulppushitem.py` & `pubtools-pulp-1.9.3/tests/push/test_pulppushitem.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_push.py` & `pubtools-pulp-1.9.3/tests/push/test_push.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,24 +121,24 @@
         compare_plaintext=False,
         compare_jsonl=False,
         # This will ensure the Pulp state matches the baseline.
         compare_extra=compare_extra,
     )
 
     # It should have invoked hook(s).
-    assert len(hookspy) == 9
+    assert len(hookspy) == 11
     (hook_name, hook_kwargs) = hookspy[0]
     assert hook_name == "task_start"
     (hook_name, hook_kwargs) = hookspy[1]
     assert hook_name == "pulp_repository_pre_publish"
     (hook_name, hook_kwargs) = hookspy[2]
     assert hook_name == "pulp_repository_published"
-    (hook_name, hook_kwargs) = hookspy[7]
+    (hook_name, hook_kwargs) = hookspy[-2]
     assert hook_name == "task_pulp_flush"
-    (hook_name, hook_kwargs) = hookspy[8]
+    (hook_name, hook_kwargs) = hookspy[-1]
     assert hook_name == "task_stop"
 
     # It should have recorded various push items.
     # We don't try to verify the entire sequence of items here, it's too
     # cumbersome. Instead we pick a single item and trace the expected
     # changes over time:
 
@@ -350,15 +350,15 @@
     # File after push should be as it was before except that description was updated
     # to the desired value.
     assert updated_file == attr.evolve(updated_file, description="My wonderful ISO")
 
     # Orphaned file after push should be as it was before except no longer an orphan.
     assert updated_orphan_file == attr.evolve(
         orphan_file,
-        repository_memberships=["iso-dest1"],
+        repository_memberships=["iso-dest1", "iso-dest2"],
     )
 
     # Erratum after push should be updated. The full update will not be tested here
     # as it's extremely verbose, we'll just sample some fields. But, critically,
     # the 'version' field (which was not an integer in pulp) should have been
     # simply overwritten with the input rather than bumped.
     assert updated_erratum.title == "Important: sudo security update"
```

### Comparing `pubtools-pulp-1.9.2/tests/push/test_push_copy_fails.py` & `pubtools-pulp-1.9.3/tests/push/test_push_copy_fails.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_push_prepush.py` & `pubtools-pulp-1.9.3/tests/push/test_push_prepush.py`

 * *Files identical despite different names*

### Comparing `pubtools-pulp-1.9.2/tests/push/test_rpm_bad_filename.py` & `pubtools-pulp-1.9.3/tests/push/test_rpm_bad_filename.py`

 * *Files identical despite different names*

