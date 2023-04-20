# Comparing `tmp/dbt-vertica-1.3.0.tar.gz` & `tmp/dbt-vertica-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-vertica-1.3.0.tar", last modified: Fri Jan 13 15:27:38 2023, max compression
+gzip compressed data, was "dbt-vertica-1.4.4.tar", last modified: Thu Apr 20 06:17:28 2023, max compression
```

## Comparing `dbt-vertica-1.3.0.tar` & `dbt-vertica-1.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/adapters/vertica/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/adapters/vertica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/adapters/vertica/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/adapters/vertica/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/adapters/vertica/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/include/vertica/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/include/vertica/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.353850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/helper.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/dbt/include/vertica/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/dbt_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-01-13 15:27:38.000000 dbt-vertica-1.3.0/dbt_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-01-13 15:27:38.000000 dbt-vertica-1.3.0/dbt_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 15:27:38.000000 dbt-vertica-1.3.0/dbt_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-13 15:27:38.000000 dbt-vertica-1.3.0/dbt_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-13 15:27:38.000000 dbt-vertica-1.3.0/dbt_vertica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 15:27:38.357850 dbt-vertica-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-01-13 15:27:26.000000 dbt-vertica-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.348854 dbt-vertica-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-20 06:17:28.348854 dbt-vertica-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/adapters/vertica/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/adapters/vertica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/adapters/vertica/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/adapters/vertica/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/adapters/vertica/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.340854 dbt-vertica-1.4.4/dbt/include/vertica/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.340854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.344854 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/helper.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/dbt/include/vertica/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:17:28.348854 dbt-vertica-1.4.4/dbt_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-20 06:17:28.000000 dbt-vertica-1.4.4/dbt_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-20 06:17:28.000000 dbt-vertica-1.4.4/dbt_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:17:28.000000 dbt-vertica-1.4.4/dbt_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 06:17:28.000000 dbt-vertica-1.4.4/dbt_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 06:17:28.000000 dbt-vertica-1.4.4/dbt_vertica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:17:28.348854 dbt-vertica-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-20 06:17:14.000000 dbt-vertica-1.4.4/setup.py
```

### Comparing `dbt-vertica-1.3.0/LICENSE` & `dbt-vertica-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/PKG-INFO` & `dbt-vertica-1.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 Metadata-Version: 2.1
 Name: dbt-vertica
-Version: 1.3.0
-Summary: The vertica adapter plugin for dbt (data build tool)
-Home-page: https://github.com/vertica/dbt-vertica/
-Author: Vertica (Former authors:- Matthew Carter, Andy Regan, Andrew Hedengren)
-Author-email: arosychuk@gmail.com, andy@andyreagan.com
-License: Apache License
+Version: 1.4.4
+Summary: Official vertica adapter plugin for dbt (data build tool)
+Home-page: https://github.com/ajay.abrol2/dbt-vertica/
+Author: Vertica (Former authors: Matthew Carter, Andy Regan, Andrew Hedengren)
+Author-email: os_dbt_vertica@microfocus.com
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-vertica
-[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database. The adapter is forward compatible with newer versions of dbt-core but it is not backward compatible with dbt-core versions earlier than v1.3.0.
+
+[![PyPI version](https://badge.fury.io/py/dbt-vertica.svg)](https://badge.fury.io/py/dbt-vertica)
+[![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+
+[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database.
 
 For more information on using dbt with Vertica, consult the [Vertica-Setup](https://docs.getdbt.com/reference/warehouse-setups/vertica-setup) and [Configuration](https://docs.getdbt.com/reference/resource-configs/vertica-configs) pages.
 
+
+## dbt-vertica Versions Tested 
+dbt-vertica has been developed using the following software and versions: 
+* Vertica Server 12.0.3-0
+* Python 3.11
+* vertica-python client 1.3.1
+* dbt-core 1.4.4
+* dbt-tests-adapter 1.4.4
+
 ## Supported Features
 ### dbt Core Features
 Below is a table for what features the current Vertica adapter supports for dbt. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves. This list is based upon dbt 1.3.0
 |                dbt Core Features                  | Supported   |
 | ------------------------------------------------- | ----------- |
 | Table Materializations                            | Yes         |
 | Ephemeral Materializations                        | Yes         |
@@ -32,24 +55,14 @@
 | Tests                                             | Yes         |
 | Documentation                                     | Yes         |
 | External Tables                                   | Untested    |
 * **Yes** - Supported, and tests pass.
 * **No** - Not supported or implemented.
 * **Untested** - May support out of the box, though hasn't been tested.
 * **Passes Test** -The testes have passed, though haven't tested in a production like environment
-### Vertica Features
-Below is a table for what features the current Vertica adapter supports for Vertica. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves.
-|   Vertica Features    | Supported |    
-| --------------------- | --------- |
-| Created/Drop Schema   | Yes       |
-| Analyze Statistics    | No        |
-| Purge Delete Vectors  | No        |
-| Projection Management | No        |
-| Primary/Unique Keys   | No        |
-| Other DDLs            | No        |
 
 ## Installation
 ```
 $ pip install dbt-vertica
 ```
 You don't need to install dbt separately. Installing `dbt-vertica` will also install `dbt-core` and `vertica-python`.
 ## Sample Profile Configuration
@@ -92,19 +105,20 @@
 For more information on Vertica’s connection properties please refer to [Vertica-Python](https://github.com/vertica/vertica-python#create-a-connection) Connection Properties.
 
 
 
 
 ## Changelog
 
-See the [changelog](https://github.com/vertica/dbt-vertica/Changelog.md)
+See the [changelog](https://github.com/vertica/dbt-vertica/blob/master/CHANGELOG.md)
 
 
 ## Contributing guidelines
-Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/CONTRIBUTING.md) for details
+
+Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/blob/master/CONTRIBUTING.md) for details
 
 ## Develop
 
 Run a local Vertica instance like:
 
     docker run -p 5433:5433 \
                -p 5444:5444 \
@@ -116,15 +130,15 @@
 Access the local Vertica instance like:
 
     docker exec -it <docker_image_name> /opt/vertica/bin/vsql
 
 
 You need the pytest dbt adapter:
 
-    pip3 install  dbt-tests-adapter==1.3.0
+    pip3 install  dbt-tests-adapter==1.4.4
 
 Run tests via:
   
     pytest tests/functional/adapter/
     # run an individual test 
     pytest tests/functional/adapter/test_basic.py
```

### Comparing `dbt-vertica-1.3.0/README.md` & `dbt-vertica-1.4.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # dbt-vertica
-[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database. The adapter is forward compatible with newer versions of dbt-core but it is not backward compatible with dbt-core versions earlier than v1.3.0.
+
+[![PyPI version](https://badge.fury.io/py/dbt-vertica.svg)](https://badge.fury.io/py/dbt-vertica)
+[![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+
+[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database.
 
 For more information on using dbt with Vertica, consult the [Vertica-Setup](https://docs.getdbt.com/reference/warehouse-setups/vertica-setup) and [Configuration](https://docs.getdbt.com/reference/resource-configs/vertica-configs) pages.
 
+
+## dbt-vertica Versions Tested 
+dbt-vertica has been developed using the following software and versions: 
+* Vertica Server 12.0.3-0
+* Python 3.11
+* vertica-python client 1.3.1
+* dbt-core 1.4.4
+* dbt-tests-adapter 1.4.4
+
 ## Supported Features
 ### dbt Core Features
 Below is a table for what features the current Vertica adapter supports for dbt. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves. This list is based upon dbt 1.3.0
 |                dbt Core Features                  | Supported   |
 | ------------------------------------------------- | ----------- |
 | Table Materializations                            | Yes         |
 | Ephemeral Materializations                        | Yes         |
@@ -21,24 +34,14 @@
 | Tests                                             | Yes         |
 | Documentation                                     | Yes         |
 | External Tables                                   | Untested    |
 * **Yes** - Supported, and tests pass.
 * **No** - Not supported or implemented.
 * **Untested** - May support out of the box, though hasn't been tested.
 * **Passes Test** -The testes have passed, though haven't tested in a production like environment
-### Vertica Features
-Below is a table for what features the current Vertica adapter supports for Vertica. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves.
-|   Vertica Features    | Supported |    
-| --------------------- | --------- |
-| Created/Drop Schema   | Yes       |
-| Analyze Statistics    | No        |
-| Purge Delete Vectors  | No        |
-| Projection Management | No        |
-| Primary/Unique Keys   | No        |
-| Other DDLs            | No        |
 
 ## Installation
 ```
 $ pip install dbt-vertica
 ```
 You don't need to install dbt separately. Installing `dbt-vertica` will also install `dbt-core` and `vertica-python`.
 ## Sample Profile Configuration
@@ -81,19 +84,20 @@
 For more information on Vertica’s connection properties please refer to [Vertica-Python](https://github.com/vertica/vertica-python#create-a-connection) Connection Properties.
 
 
 
 
 ## Changelog
 
-See the [changelog](https://github.com/vertica/dbt-vertica/Changelog.md)
+See the [changelog](https://github.com/vertica/dbt-vertica/blob/master/CHANGELOG.md)
 
 
 ## Contributing guidelines
-Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/CONTRIBUTING.md) for details
+
+Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/blob/master/CONTRIBUTING.md) for details
 
 ## Develop
 
 Run a local Vertica instance like:
 
     docker run -p 5433:5433 \
                -p 5444:5444 \
@@ -105,16 +109,16 @@
 Access the local Vertica instance like:
 
     docker exec -it <docker_image_name> /opt/vertica/bin/vsql
 
 
 You need the pytest dbt adapter:
 
-    pip3 install  dbt-tests-adapter==1.3.0
+    pip3 install  dbt-tests-adapter==1.4.4
 
 Run tests via:
   
     pytest tests/functional/adapter/
     # run an individual test 
     pytest tests/functional/adapter/test_basic.py
 
-    
+
```

### Comparing `dbt-vertica-1.3.0/dbt/__init__.py` & `dbt-vertica-1.4.4/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/adapters/__init__.py` & `dbt-vertica-1.4.4/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/adapters/vertica/__init__.py` & `dbt-vertica-1.4.4/dbt/adapters/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/adapters/vertica/__version__.py` & `dbt-vertica-1.4.4/dbt/adapters/vertica/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 
-version = "1.3.0"
+version = "1.4.4"
```

### Comparing `dbt-vertica-1.3.0/dbt/adapters/vertica/connections.py` & `dbt-vertica-1.4.4/dbt/adapters/vertica/connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                
 
 
         except Exception as exc:
             logger.debug(f':P Error connecting to database: {exc}')
             connection.state = 'fail'
             connection.handle = None
-            raise dbt.exceptions.FailedToConnectException(str(exc))
+            raise dbt.exceptions.DbtFailedToConnectErroe(str(exc))
 
         # This is here mainly to support dbt-integration-tests.
         # It globally enables WITH materialization for every connection dbt
         # makes to Vertica. (Defaults to False)
         # Normal usage would be to use query HINT or declare session parameter in model or hook,
         # but tests do not support hooks and cannot change tests from dbt_utils
         # used in dbt-integration-tests
@@ -152,15 +152,15 @@
 
             except Exception as exc:
                 logger.debug(f':P Could not EnableWithClauseMaterialization: {exc}')
                 pass
 
         retryable_exceptions = [
         Exception,
-        dbt.exceptions.FailedToConnectException
+        dbt.exceptions.FailedToConnectError
         ]
 
         return cls.retry_connection(
         connection,
         connect=connect,
         logger=logger,
         retry_limit=credentials.retries,
@@ -180,21 +180,59 @@
             code=str(code)
         )
 
     def cancel(self, connection):
         logger.debug(':P Cancel query')
         connection.handle.cancel()
 
+    @classmethod
+    def get_result_from_cursor(cls, cursor: Any) -> agate.Table:
+        data: List[Any] = []
+        column_names: List[str] = []
+
+        if cursor.description is not None:
+            column_names = [col[0] for col in cursor.description]
+            rows = cursor.fetchall()
+
+            # check result for every query if there are some queries with ; separator
+            while cursor.nextset():
+                check = cursor._message
+                if isinstance(check, ErrorResponse):
+                    logger.debug(f'Cursor message is: {check}')
+                    self.release()
+                    raise dbt.exceptions.DbtDatabaseError(str(check))
+
+            data = cls.process_results(column_names, rows)
+
+        return dbt.clients.agate_helper.table_from_data_flat(data, column_names)
+
+    def execute(
+        self, sql: str, auto_begin: bool = False, fetch: bool = False
+    ) -> Tuple[AdapterResponse, agate.Table]:
+        sql = self._add_query_comment(sql)
+        _, cursor = self.add_query(sql, auto_begin)
+        response = self.get_response(cursor)
+        if fetch:
+            table = self.get_result_from_cursor(cursor)
+        else:
+            table = dbt.clients.agate_helper.empty_table()
+            while cursor.nextset():
+                check = cursor._message
+                if isinstance(check, vertica_python.vertica.messages.ErrorResponse):
+                    logger.debug(f'Cursor message is: {check}')
+                    self.release()
+                    raise dbt.exceptions.DbtDatabaseError(str(check))
+        return response, table
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
         except vertica_python.DatabaseError as exc:
             logger.debug(f':P Database error: {exc}')
             self.release()
-            raise dbt.exceptions.DatabaseException(str(exc))
+            raise dbt.exceptions.DbtDatabaseError(str(exc))
         except Exception as exc:
             logger.debug(f':P Error: {exc}')
             self.release()
-            raise dbt.exceptions.RuntimeException(str(exc))
+            raise dbt.exceptions.DbtRuntimeError(str(exc))
```

### Comparing `dbt-vertica-1.3.0/dbt/adapters/vertica/impl.py` & `dbt-vertica-1.4.4/dbt/adapters/vertica/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.vertica import verticaConnectionManager
 from typing import Mapping, Any, Optional, List, Union, Dict
 from dbt.adapters.base import available
 from dbt.exceptions import (
 
-    RuntimeException
+    DbtRuntimeError
 )
 
 import agate
 from dataclasses import dataclass
 from dbt.adapters.base.meta import available
 from dbt.adapters.sql import SQLAdapter  # type: ignore
 from dbt.adapters.sql.impl import (
@@ -124,23 +124,23 @@
             strategy = "default"
 
         # validate strategies for this adapter
         valid_strategies = self.valid_incremental_strategies()
         valid_strategies.append("default")
         builtin_strategies = self.builtin_incremental_strategies()
         if strategy in builtin_strategies and strategy not in valid_strategies:
-            raise RuntimeException(
+            raise DbtRuntimeError(
                 f"The incremental strategy '{strategy}' is not valid for this adapter"
             )
 
         strategy = strategy.replace("+", "_")
         macro_name = f"get_incremental_{strategy}_sql"
         # The model_context should have MacroGenerator callable objects for all macros
         if macro_name not in model_context:
-            raise RuntimeException(
+            raise DbtRuntimeError(
                 'dbt could not find an incremental strategy macro with the name "{}" in {}'.format(
                     macro_name, self.config.project_name
                 )
             )
 
         # This returns a callable macro
         return model_context[macro_name]
```

### Comparing `dbt-vertica-1.3.0/dbt/include/__init__.py` & `dbt-vertica-1.4.4/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/__init__.py` & `dbt-vertica-1.4.4/dbt/include/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/apply_grants.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/columns.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/metadata.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/adapters/relation.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/helpers.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/incremental.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,19 @@
   {% elif full_refresh_mode %}
       -- {#-- Make sure the backup doesn't exist so we don't encounter issues with the rename below #}
       {% set tmp_identifier = model['name'] + '__dbt_tmp' %}
       {% set backup_identifier = model['name'] + '__dbt_backup' %}
       {% set intermediate_relation = existing_relation.incorporate(path={"identifier": tmp_identifier}) %}
       {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
       
-      {% set build_sql = vertica__create_table_as(False, target_relation, sql) %}
+      {% set build_sql = vertica__create_table_as(False, intermediate_relation, sql) %}
       
       {% set need_swap = true %}
       {% do to_drop.append(backup_relation) %}
+      {% do to_drop.append(intermediate_relation) %}
   {% else %}
       {% do run_query(vertica__create_table_as(True, tmp_relation, sql)) %}
       {% do adapter.expand_target_column_types(
              from_relation=tmp_relation,
              to_relation=target_relation) %}
       -- {#-- Process schema changes. Returns dict of changes if successful. Use source columns for upserting/merging --#}
          {% set msg %}
```

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/merge.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/merge.sql`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 {% macro vertica__get_merge_sql(target_relation, tmp_relation, unique_key, dest_columns) %}
   {%- set dest_columns_csv =  get_quoted_csv(dest_columns | map(attribute="name")) -%}
   {%- set merge_columns = config.get("unique_key", default=None)%}
-  {%- set merge_update_columns = config.get("merge_update_columns", default=dest_columns)-%}
-  {% if merge_update_columns %}
-    {%- set merge_update_columns = dest_columns -%}
-  {% endif %}
-
+  {%- set merge_update_columns = config.get("merge_update_columns")-%}
+ 
   merge into {{ target_relation }} as DBT_INTERNAL_DEST
   using {{ tmp_relation }} as DBT_INTERNAL_SOURCE
 
   {#-- Test 1, find the provided merge columns #}
   {% if merge_columns %}
     on 
     {% for column in [merge_columns] %}
@@ -22,18 +19,28 @@
     {% for column in dest_columns -%}
       DBT_INTERNAL_DEST.{{ adapter.quote(column.name) }} = DBT_INTERNAL_SOURCE.{{ adapter.quote(column.name) }} 
       {%- if not loop.last %} AND {% endif %}
     {%- endfor %}
   {% endif %}
 
   when matched then update set
-  {% for column in merge_update_columns -%}
-    {{ adapter.quote(column.name) }} = DBT_INTERNAL_SOURCE.{{ adapter.quote(column.name) }}
-    {%- if not loop.last %}, {% endif %}
-  {%- endfor %}
+  {% if merge_update_columns %}
+    
+    {% for column in merge_update_columns -%}
+      {{ adapter.quote(column) }} = DBT_INTERNAL_SOURCE.{{ adapter.quote(column) }}
+      {%- if not loop.last %}, {% endif %}
+    {%- endfor %}
+  {% else %}
+    
+    {% for column in dest_columns -%}
+      {%- set merge_update_columns = dest_columns -%}
+      {{ adapter.quote(column.name) }} = DBT_INTERNAL_SOURCE.{{ adapter.quote(column.name) }}
+      {%- if not loop.last %}, {% endif %}
+    {%- endfor %}
+  {% endif %}
 
   when not matched then insert
     ({{ dest_columns_csv }})
   values
   (
     {% for column in dest_columns -%}
        DBT_INTERNAL_SOURCE.{{ adapter.quote(column.name) }}
```

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/incremental/strategies.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/table/create_table_as.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/table/create_table_as.sql`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,27 @@
   {%- set segmented_by_all_nodes = config.get('segmented_by_all_nodes', default=True) -%}
   {%- set no_segmentation = config.get('no_segmentation', default=False) -%}
   {%- set ksafe = config.get('ksafe', default=none) -%}
   {%- set partition_by_string = config.get('partition_by_string', default=none) -%}
   {%- set partition_by_group_by_string = config.get('partition_by_group_by_string', default=none) -%}
   {%- set partition_by_active_count = config.get('partition_by_active_count', default=none) -%}
   
+  
   create {% if temporary: -%}local temporary{%- endif %} table
     {{ relation.include(database=(not temporary), schema=(not temporary)) }}
     {% if temporary: -%}on commit preserve rows{%- endif %}
     INCLUDE SCHEMA PRIVILEGES as (
     {{ sql }}
   )
+ {% if not temporary: %}
 
   {% if order_by is not none  -%}
       order by {{ order_by }} 
   {% endif -%}
-
+  
   {% if segmented_by_string is not none -%}
               segmented  BY  {{ segmented_by_string }} {% if segmented_by_all_nodes %} ALL NODES {% endif %}
   {% endif %}
 
   {% if no_segmentation =='True' or no_segmentation=='true'  -%} 
     UNSEGMENTED ALL NODES 
   {% endif -%}
@@ -38,10 +40,11 @@
     {% if partition_by_string is not none and partition_by_group_by_string is not none -%}
       group by {{ partition_by_group_by_string }}
     {% endif %}
     {% if partition_by_string is not none and partition_by_active_count is not none %}
       SET ACTIVEPARTITIONCOUNT {{ partition_by_active_count }}
     {% endif %}
   {% endif %}  
+ {% endif %}
   ;
 {% endmacro %}
```

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/table/table.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/models/view/view.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/seeds/helpers.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/seeds/seed.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/snapshot.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/macros/materializations/snapshots/strategies.sql` & `dbt-vertica-1.4.4/dbt/include/vertica/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/profile_template.yml` & `dbt-vertica-1.4.4/dbt/include/vertica/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt/include/vertica/sample_profiles.yml` & `dbt-vertica-1.4.4/dbt/include/vertica/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/dbt_vertica.egg-info/PKG-INFO` & `dbt-vertica-1.4.4/dbt_vertica.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 Metadata-Version: 2.1
 Name: dbt-vertica
-Version: 1.3.0
-Summary: The vertica adapter plugin for dbt (data build tool)
-Home-page: https://github.com/vertica/dbt-vertica/
-Author: Vertica (Former authors:- Matthew Carter, Andy Regan, Andrew Hedengren)
-Author-email: arosychuk@gmail.com, andy@andyreagan.com
-License: Apache License
+Version: 1.4.4
+Summary: Official vertica adapter plugin for dbt (data build tool)
+Home-page: https://github.com/ajay.abrol2/dbt-vertica/
+Author: Vertica (Former authors: Matthew Carter, Andy Regan, Andrew Hedengren)
+Author-email: os_dbt_vertica@microfocus.com
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-vertica
-[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database. The adapter is forward compatible with newer versions of dbt-core but it is not backward compatible with dbt-core versions earlier than v1.3.0.
+
+[![PyPI version](https://badge.fury.io/py/dbt-vertica.svg)](https://badge.fury.io/py/dbt-vertica)
+[![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+
+[dbt](https://www.getdbt.com/) adapter for [Vertica](https://www.vertica.com/). The adapter uses [vertica-python](https://github.com/vertica/vertica-python) to connect to your Vertica database.
 
 For more information on using dbt with Vertica, consult the [Vertica-Setup](https://docs.getdbt.com/reference/warehouse-setups/vertica-setup) and [Configuration](https://docs.getdbt.com/reference/resource-configs/vertica-configs) pages.
 
+
+## dbt-vertica Versions Tested 
+dbt-vertica has been developed using the following software and versions: 
+* Vertica Server 12.0.3-0
+* Python 3.11
+* vertica-python client 1.3.1
+* dbt-core 1.4.4
+* dbt-tests-adapter 1.4.4
+
 ## Supported Features
 ### dbt Core Features
 Below is a table for what features the current Vertica adapter supports for dbt. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves. This list is based upon dbt 1.3.0
 |                dbt Core Features                  | Supported   |
 | ------------------------------------------------- | ----------- |
 | Table Materializations                            | Yes         |
 | Ephemeral Materializations                        | Yes         |
@@ -32,24 +55,14 @@
 | Tests                                             | Yes         |
 | Documentation                                     | Yes         |
 | External Tables                                   | Untested    |
 * **Yes** - Supported, and tests pass.
 * **No** - Not supported or implemented.
 * **Untested** - May support out of the box, though hasn't been tested.
 * **Passes Test** -The testes have passed, though haven't tested in a production like environment
-### Vertica Features
-Below is a table for what features the current Vertica adapter supports for Vertica. This is constantly improving and changing as both dbt adds new functionality, as well as the dbt-vertica driver improves.
-|   Vertica Features    | Supported |    
-| --------------------- | --------- |
-| Created/Drop Schema   | Yes       |
-| Analyze Statistics    | No        |
-| Purge Delete Vectors  | No        |
-| Projection Management | No        |
-| Primary/Unique Keys   | No        |
-| Other DDLs            | No        |
 
 ## Installation
 ```
 $ pip install dbt-vertica
 ```
 You don't need to install dbt separately. Installing `dbt-vertica` will also install `dbt-core` and `vertica-python`.
 ## Sample Profile Configuration
@@ -92,19 +105,20 @@
 For more information on Vertica’s connection properties please refer to [Vertica-Python](https://github.com/vertica/vertica-python#create-a-connection) Connection Properties.
 
 
 
 
 ## Changelog
 
-See the [changelog](https://github.com/vertica/dbt-vertica/Changelog.md)
+See the [changelog](https://github.com/vertica/dbt-vertica/blob/master/CHANGELOG.md)
 
 
 ## Contributing guidelines
-Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/CONTRIBUTING.md) for details
+
+Have a bug or an idea? Please see [CONTRIBUTING.md](https://github.com/vertica/dbt-vertica/blob/master/CONTRIBUTING.md) for details
 
 ## Develop
 
 Run a local Vertica instance like:
 
     docker run -p 5433:5433 \
                -p 5444:5444 \
@@ -116,15 +130,15 @@
 Access the local Vertica instance like:
 
     docker exec -it <docker_image_name> /opt/vertica/bin/vsql
 
 
 You need the pytest dbt adapter:
 
-    pip3 install  dbt-tests-adapter==1.3.0
+    pip3 install  dbt-tests-adapter==1.4.4
 
 Run tests via:
   
     pytest tests/functional/adapter/
     # run an individual test 
     pytest tests/functional/adapter/test_basic.py
```

### Comparing `dbt-vertica-1.3.0/dbt_vertica.egg-info/SOURCES.txt` & `dbt-vertica-1.4.4/dbt_vertica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-vertica-1.3.0/setup.py` & `dbt-vertica-1.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,28 +74,28 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-vertica"
-package_version = "1.3.0"
-description = """The vertica adapter plugin for dbt (data build tool)"""
+package_version = "1.4.4"
+description = """Official vertica adapter plugin for dbt (data build tool)"""
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=README,
     long_description_content_type='text/markdown',
-    license='Apache License', 
-    author='Vertica (Former authors:- Matthew Carter, Andy Regan, Andrew Hedengren)',
-    author_email='arosychuk@gmail.com, andy@andyreagan.com',
-    url='https://github.com/vertica/dbt-vertica/',
+    license='Apache License 2.0', 
+    author='Vertica (Former authors: Matthew Carter, Andy Regan, Andrew Hedengren)',
+    author_email='os_dbt_vertica@microfocus.com',
+    url='https://github.com/ajay.abrol2/dbt-vertica/',
     packages=find_packages(include=["dbt","dbt.*"]),
     
     package_data={
         'dbt': [
             'include/vertica/dbt_project.yml',
             'include/vertica/profile_template.yml',
             'include/vertica/sample_profiles.yml',
@@ -106,14 +106,26 @@
             'include/vertica/macros/materializations/models/table/*.sql',
             'include/vertica/macros/materializations/models/view/*.sql',
             'include/vertica/macros/materializations/seeds/*.sql',
             'include/vertica/macros/materializations/snapshots/*.sql',
         ]
     },
     install_requires=[
-        'dbt-core==1.3.0',
+        'dbt-core==1.4.4',
         # "dbt-core~={}".format(dbt_core_version),
         'vertica-python>=1.1.0',
-        'dbt-tests-adapter==1.3.0',
-        'python-dotenv==0.21.0',
+        'dbt-tests-adapter==1.4.4',
+        'python-dotenv==0.21.1',
     ],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Database",
+        "Topic :: Database :: Database Engines/Servers",
+        "Topic :: Database :: Front-Ends",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Operating System :: OS Independent"
+    ],
+    python_requires=">=3.7.2",
 )
```

