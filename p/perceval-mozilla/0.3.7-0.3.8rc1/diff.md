# Comparing `tmp/perceval_mozilla-0.3.7.tar.gz` & `tmp/perceval_mozilla-0.3.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_mozilla-0.3.7.tar", max compression
+gzip compressed data, was "perceval_mozilla-0.3.8rc1.tar", max compression
```

## Comparing `perceval_mozilla-0.3.7.tar` & `perceval_mozilla-0.3.8rc1.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0      180 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/LICENSE
--rw-r--r--   0        0        0     1379 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/NEWS
--rw-r--r--   0        0        0     2373 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/README.md
--rw-r--r--   0        0        0        0 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/_version.py
--rw-r--r--   0        0        0    10890 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/crates.py
--rw-r--r--   0        0        0    10821 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/kitsune.py
--rw-r--r--   0        0        0    11469 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/mozillaclub.py
--rw-r--r--   0        0        0    10907 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/perceval/backends/mozilla/remo.py
--rw-r--r--   0        0        0     1396 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0     1889 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/base.py
--rw-r--r--   0        0        0        0 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/__init__.py
--rw-r--r--   0        0        0     1637 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_example_1
--rw-r--r--   0        0        0     2797 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_example_2
--rw-r--r--   0        0        0     1840 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_example_3
--rw-r--r--   0        0        0     6506 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_example_4
--rw-r--r--   0        0        0       19 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_team_1
--rw-r--r--   0        0        0      312 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_team_2
--rw-r--r--   0        0        0      295 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_team_3
--rw-r--r--   0        0        0      298 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_team_4
--rw-r--r--   0        0        0      324 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_1
--rw-r--r--   0        0        0      555 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_2
--rw-r--r--   0        0        0      555 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_3
--rw-r--r--   0        0        0      823 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_4
--rw-r--r--   0        0        0      369 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_version_downloads_1
--rw-r--r--   0        0        0        2 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_version_downloads_empty
--rw-r--r--   0        0        0      724 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_versions_1
--rw-r--r--   0        0        0     3641 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_versions_2
--rw-r--r--   0        0        0      748 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_versions_3
--rw-r--r--   0        0        0     5010 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crate_versions_4
--rw-r--r--   0        0        0     2181 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crates_page_1
--rw-r--r--   0        0        0     2352 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crates_page_2
--rw-r--r--   0        0        0       59 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crates_page_empty
--rw-r--r--   0        0        0    39923 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/crates/crates_summary
--rw-r--r--   0        0        0        0 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_answers_empty.json
--rw-r--r--   0        0        0     3693 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_question_answers.json
--rw-r--r--   0        0        0       78 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_question_answers_empy.json
--rw-r--r--   0        0        0     5730 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_questions_1_2.json
--rw-r--r--   0        0        0     8148 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_questions_2_2.json
--rw-r--r--   0        0        0       78 2023-02-03 08:15:56.255249 perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_questions_empty.json
--rw-r--r--   0        0        0  2047401 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/mozillaclub/feed.json
--rw-r--r--   0        0        0     1141 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_activities.json
--rw-r--r--   0        0        0     2893 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_activities_page_1_2.json
--rw-r--r--   0        0        0     2888 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_activities_page_2_2.json
--rw-r--r--   0        0        0       78 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_activities_page_empty.json
--rw-r--r--   0        0        0     1263 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events.json
--rw-r--r--   0        0        0     3463 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_1_2.json
--rw-r--r--   0        0        0     3784 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_2_2.json
--rw-r--r--   0        0        0      158 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_empty.json
--rw-r--r--   0        0        0     2904 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_page_1_2.json
--rw-r--r--   0        0        0     2889 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_page_2_2.json
--rw-r--r--   0        0        0       78 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_events_page_empty.json
--rw-r--r--   0        0        0    28055 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_reps.json
--rw-r--r--   0        0        0     2263 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_users.json
--rw-r--r--   0        0        0     4143 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_users_page_1_2.json
--rw-r--r--   0        0        0     4123 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_users_page_2_2.json
--rw-r--r--   0        0        0       78 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/data/remo/remo_users_page_empty.json
--rwxr-xr-x   0        0        0     1017 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/run_tests.py
--rw-r--r--   0        0        0    20404 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/test_crates.py
--rw-r--r--   0        0        0    14955 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/test_kitsune.py
--rw-r--r--   0        0        0    12118 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/test_mozillaclub.py
--rw-r--r--   0        0        0    17239 2023-02-03 08:15:56.263249 perceval_mozilla-0.3.7/tests/test_remo.py
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 perceval_mozilla-0.3.7/setup.py
--rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 perceval_mozilla-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      180 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/LICENSE
+-rw-r--r--   0        0        0     1379 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/NEWS
+-rw-r--r--   0        0        0     2373 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/_version.py
+-rw-r--r--   0        0        0    10890 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/crates.py
+-rw-r--r--   0        0        0    10821 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/kitsune.py
+-rw-r--r--   0        0        0    11469 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/mozillaclub.py
+-rw-r--r--   0        0        0    10907 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/remo.py
+-rw-r--r--   0        0        0     1401 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1889 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/base.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/data/crates/__init__.py
+-rw-r--r--   0        0        0     1637 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_1
+-rw-r--r--   0        0        0     2797 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_2
+-rw-r--r--   0        0        0     1840 2023-04-20 15:35:39.855369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_3
+-rw-r--r--   0        0        0     6506 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_4
+-rw-r--r--   0        0        0       19 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_team_1
+-rw-r--r--   0        0        0      312 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_team_2
+-rw-r--r--   0        0        0      295 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_team_3
+-rw-r--r--   0        0        0      298 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_team_4
+-rw-r--r--   0        0        0      324 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_1
+-rw-r--r--   0        0        0      555 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_2
+-rw-r--r--   0        0        0      555 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_3
+-rw-r--r--   0        0        0      823 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_4
+-rw-r--r--   0        0        0      369 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_version_downloads_1
+-rw-r--r--   0        0        0        2 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_version_downloads_empty
+-rw-r--r--   0        0        0      724 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_1
+-rw-r--r--   0        0        0     3641 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_2
+-rw-r--r--   0        0        0      748 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_3
+-rw-r--r--   0        0        0     5010 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_4
+-rw-r--r--   0        0        0     2181 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crates_page_1
+-rw-r--r--   0        0        0     2352 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crates_page_2
+-rw-r--r--   0        0        0       59 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crates_page_empty
+-rw-r--r--   0        0        0    39923 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/crates/crates_summary
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_answers_empty.json
+-rw-r--r--   0        0        0     3693 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_question_answers.json
+-rw-r--r--   0        0        0       78 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_question_answers_empy.json
+-rw-r--r--   0        0        0     5730 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_questions_1_2.json
+-rw-r--r--   0        0        0     8148 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_questions_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-20 15:35:39.859369 perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_questions_empty.json
+-rw-r--r--   0        0        0  2047401 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/mozillaclub/feed.json
+-rw-r--r--   0        0        0     1141 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities.json
+-rw-r--r--   0        0        0     2893 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities_page_1_2.json
+-rw-r--r--   0        0        0     2888 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities_page_empty.json
+-rw-r--r--   0        0        0     1263 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events.json
+-rw-r--r--   0        0        0     3463 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_1_2.json
+-rw-r--r--   0        0        0     3784 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_2_2.json
+-rw-r--r--   0        0        0      158 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_empty.json
+-rw-r--r--   0        0        0     2904 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_page_1_2.json
+-rw-r--r--   0        0        0     2889 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_page_empty.json
+-rw-r--r--   0        0        0    28055 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_reps.json
+-rw-r--r--   0        0        0     2263 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users.json
+-rw-r--r--   0        0        0     4143 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users_page_1_2.json
+-rw-r--r--   0        0        0     4123 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users_page_empty.json
+-rwxr-xr-x   0        0        0     1017 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    20404 2023-04-20 15:35:39.863369 perceval_mozilla-0.3.8rc1/tests/test_crates.py
+-rw-r--r--   0        0        0    14955 2023-04-20 15:35:39.867370 perceval_mozilla-0.3.8rc1/tests/test_kitsune.py
+-rw-r--r--   0        0        0    12118 2023-04-20 15:35:39.867370 perceval_mozilla-0.3.8rc1/tests/test_mozillaclub.py
+-rw-r--r--   0        0        0    17239 2023-04-20 15:35:39.867370 perceval_mozilla-0.3.8rc1/tests/test_remo.py
+-rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 perceval_mozilla-0.3.8rc1/PKG-INFO
```

### Comparing `perceval_mozilla-0.3.7/LICENSE` & `perceval_mozilla-0.3.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/NEWS` & `perceval_mozilla-0.3.8rc1/NEWS`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/README.md` & `perceval_mozilla-0.3.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/perceval/backends/mozilla/crates.py` & `perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/perceval/backends/mozilla/kitsune.py` & `perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/perceval/backends/mozilla/mozillaclub.py` & `perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/perceval/backends/mozilla/remo.py` & `perceval_mozilla-0.3.8rc1/perceval/backends/mozilla/remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/pyproject.toml` & `perceval_mozilla-0.3.8rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-mozilla"
-version = "0.3.7"
+version = "0.3.8-rc.1"
 description = "Bundle of Perceval backends for Mozilla ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_mozilla-0.3.7/tests/base.py` & `perceval_mozilla-0.3.8rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_example_1` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_example_2` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_example_3` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_example_4` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_example_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_2` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_3` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_owner_user_4` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_owner_user_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_versions_1` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_versions_2` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_versions_3` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crate_versions_4` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crate_versions_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crates_page_1` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crates_page_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crates_page_2` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crates_page_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/crates/crates_summary` & `perceval_mozilla-0.3.8rc1/tests/data/crates/crates_summary`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_question_answers.json` & `perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_question_answers.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_questions_1_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_questions_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/kitsune/kitsune_questions_2_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/kitsune/kitsune_questions_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/mozillaclub/feed.json` & `perceval_mozilla-0.3.8rc1/tests/data/mozillaclub/feed.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_activities.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_activities_page_1_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_activities_page_2_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_activities_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_events.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_events_1_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_events_2_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_events_page_1_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_events_page_2_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_events_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_reps.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_reps.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_users.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_users_page_1_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/data/remo/remo_users_page_2_2.json` & `perceval_mozilla-0.3.8rc1/tests/data/remo/remo_users_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/run_tests.py` & `perceval_mozilla-0.3.8rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/test_crates.py` & `perceval_mozilla-0.3.8rc1/tests/test_crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/test_kitsune.py` & `perceval_mozilla-0.3.8rc1/tests/test_kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/test_mozillaclub.py` & `perceval_mozilla-0.3.8rc1/tests/test_mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/tests/test_remo.py` & `perceval_mozilla-0.3.8rc1/tests/test_remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.7/setup.py` & `perceval_mozilla-0.3.8rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: perceval-mozilla
+Version: 0.3.8rc1
+Summary: Bundle of Perceval backends for Mozilla ecosystem.
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: grimoirelab-toolkit (>=0.3)
+Requires-Dist: perceval (>=0.19)
+Requires-Dist: requests (>=2.7.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-perceval-mozilla/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-perceval-mozilla
+Description-Content-Type: text/markdown
+
+# perceval-mozilla [![Build Status](https://github.com/chaoss/grimoirelab-perceval-mozilla/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-perceval-mozilla/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-perceval-mozilla.svg)](https://coveralls.io/r/chaoss/grimoirelab-perceval-mozilla?branch=master) [![PyPI version](https://badge.fury.io/py/perceval-mozilla.svg)](https://badge.fury.io/py/perceval-mozilla)
+
+Bundle of Perceval backends for Mozilla ecosystem.
+
+## Backends
+
+The backends currently managed by this package support the next repositories:
+
+* Crates
+* Kitsune
+* MozillaClub
+* ReMo
+
+## Requirements
+
+ * Python >= 3.7
+
+You will also need some other libraries for running the tool, you can find the
+whole list of dependencies in [pyproject.toml](pyproject.toml) file.
+
+## Installation
+
+There are several ways to install perceval-mozilla on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI
+
+perceval-mozilla can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install perceval-mozilla
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-perceval-mozilla
+$ cd grimoirelab-perceval-mozilla
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install perceval-mozilla in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install perceval-mozilla and the dependencies in 
+a project isolated environment using:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
+## Examples
+
+### Crates
+
+```
+$ perceval crates
+```
+
+### Kitsune
+
+```
+$ perceval kitsune --offset 373990
+```
+
+### Mozilla Club Events
+
+```
+$ perceval mozillaclub
+```
+
+### ReMo
+```
+$ perceval remo
+```
 
-packages = \
-['perceval', 'perceval.backends.mozilla', 'tests', 'tests.data.crates']
+## License
 
-package_data = \
-{'': ['*'], 'tests': ['data/kitsune/*', 'data/mozillaclub/*', 'data/remo/*']}
+Licensed under GNU General Public License (GPL), version 3 or later.
 
-install_requires = \
-['grimoirelab-toolkit>=0.3', 'perceval>=0.19', 'requests>=2.7.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'perceval-mozilla',
-    'version': '0.3.7',
-    'description': 'Bundle of Perceval backends for Mozilla ecosystem.',
-    'long_description': '# perceval-mozilla [![Build Status](https://github.com/chaoss/grimoirelab-perceval-mozilla/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-perceval-mozilla/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-perceval-mozilla.svg)](https://coveralls.io/r/chaoss/grimoirelab-perceval-mozilla?branch=master) [![PyPI version](https://badge.fury.io/py/perceval-mozilla.svg)](https://badge.fury.io/py/perceval-mozilla)\n\nBundle of Perceval backends for Mozilla ecosystem.\n\n## Backends\n\nThe backends currently managed by this package support the next repositories:\n\n* Crates\n* Kitsune\n* MozillaClub\n* ReMo\n\n## Requirements\n\n * Python >= 3.7\n\nYou will also need some other libraries for running the tool, you can find the\nwhole list of dependencies in [pyproject.toml](pyproject.toml) file.\n\n## Installation\n\nThere are several ways to install perceval-mozilla on your system: packages or source \ncode using Poetry or pip.\n\n### PyPI\n\nperceval-mozilla can be installed using pip, a tool for installing Python packages. \nTo do it, run the next command:\n```\n$ pip install perceval-mozilla\n```\n\n### Source code\n\nTo install from the source code you will need to clone the repository first:\n```\n$ git clone https://github.com/chaoss/grimoirelab-perceval-mozilla\n$ cd grimoirelab-perceval-mozilla\n```\n\nThen use pip or Poetry to install the package along with its dependencies.\n\n#### Pip\nTo install the package from local directory run the following command:\n```\n$ pip install .\n```\nIn case you are a developer, you should install perceval-mozilla in editable mode:\n```\n$ pip install -e .\n```\n\n#### Poetry\nWe use [poetry](https://python-poetry.org/) for dependency management and \npackaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).\nOnce you have installed it, you can install perceval-mozilla and the dependencies in \na project isolated environment using:\n```\n$ poetry install\n```\nTo spaw a new shell within the virtual environment use:\n```\n$ poetry shell\n```\n\n## Examples\n\n### Crates\n\n```\n$ perceval crates\n```\n\n### Kitsune\n\n```\n$ perceval kitsune --offset 373990\n```\n\n### Mozilla Club Events\n\n```\n$ perceval mozillaclub\n```\n\n### ReMo\n```\n$ perceval remo\n```\n\n## License\n\nLicensed under GNU General Public License (GPL), version 3 or later.\n',
-    'author': 'GrimoireLab Developers',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://chaoss.github.io/grimoirelab/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

