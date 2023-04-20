# Comparing `tmp/half_orm-0.8.0rc8.tar.gz` & `tmp/half_orm-0.8.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "half_orm-0.8.0rc8.tar", last modified: Fri Feb 24 15:49:43 2023, max compression
+gzip compressed data, was "half_orm-0.8.0rc9.tar", last modified: Mon Mar  6 08:19:21 2023, max compression
```

## Comparing `half_orm-0.8.0rc8.tar` & `half_orm-0.8.0rc9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.623988 half_orm-0.8.0rc8/
--rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/AUTHORS
--rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)    26127 2023-02-24 15:49:43.623988 half_orm-0.8.0rc8/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)    25183 2023-02-24 13:50:14.000000 half_orm-0.8.0rc8/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.583986 half_orm-0.8.0rc8/half_orm/
--rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5922 2023-02-24 15:00:53.000000 half_orm-0.8.0rc8/half_orm/field.py
--rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/field_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5786 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/fkey.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3673 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/hotest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    19152 2023-02-24 14:57:15.000000 half_orm-0.8.0rc8/half_orm/model.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1370 2023-02-14 08:50:13.000000 half_orm-0.8.0rc8/half_orm/model_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-02-07 15:08:24.000000 half_orm-0.8.0rc8/half_orm/null.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.607987 half_orm-0.8.0rc8/half_orm/packager/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3780 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/changelog.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4470 2023-02-07 15:08:24.000000 half_orm-0.8.0rc8/half_orm/packager/database.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4545 2023-02-15 15:58:43.000000 half_orm-0.8.0rc8/half_orm/packager/db_conn.py
--rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/hgit.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     5479 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/hop.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/manifest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/modules.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    13429 2023-02-15 16:14:49.000000 half_orm-0.8.0rc8/half_orm/packager/patch.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.607987 half_orm-0.8.0rc8/half_orm/packager/patches/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.559985 half_orm-0.8.0rc8/half_orm/packager/patches/0/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.559985 half_orm-0.8.0rc8/half_orm/packager/patches/0/1/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.611987 half_orm-0.8.0rc8/half_orm/packager/patches/0/1/0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/patches/log
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.611987 half_orm-0.8.0rc8/half_orm/packager/patches/sql/
--rw-r--r--   0 joel      (1000) joel      (1000)     4197 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/patches/sql/half_orm_meta.sql
--rw-r--r--   0 joel      (1000) joel      (1000)     8297 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/repo.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.623988 half_orm-0.8.0rc8/half_orm/packager/templates/
--rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/.gitignore
--rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/MANIFEST.in
--rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/Pipfile
--rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/README
--rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/base_test
--rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/db_connector.py
--rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/module_template_1
--rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/module_template_2
--rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/module_template_3
--rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/relation_test
--rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/setup.py
--rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/templates/warning
--rw-r--r--   0 joel      (1000) joel      (1000)     1733 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/utils.py
--rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/packager/version.txt
--rw-r--r--   0 joel      (1000) joel      (1000)    12382 2023-02-08 08:30:41.000000 half_orm-0.8.0rc8/half_orm/pg_meta.py
--rw-r--r--   0 joel      (1000) joel      (1000)    39997 2023-02-17 08:43:11.000000 half_orm-0.8.0rc8/half_orm/relation.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1521 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/relation_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2302 2023-02-02 08:59:25.000000 half_orm-0.8.0rc8/half_orm/transaction.py
--rw-r--r--   0 joel      (1000) joel      (1000)        9 2023-02-24 15:45:09.000000 half_orm-0.8.0rc8/half_orm/version.txt
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-02-24 15:49:43.587986 half_orm-0.8.0rc8/half_orm.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)    26127 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1553 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-02-24 15:49:43.000000 half_orm-0.8.0rc8/half_orm.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.8.0rc8/pyproject.toml
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-02-24 15:49:43.623988 half_orm-0.8.0rc8/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-02-07 15:08:24.000000 half_orm-0.8.0rc8/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/
+-rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/AUTHORS
+-rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)    27243 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)    26299 2023-03-06 08:08:09.000000 half_orm-0.8.0rc9/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.897335 half_orm-0.8.0rc9/half_orm/
+-rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/half_orm/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5929 2023-03-02 13:06:39.000000 half_orm-0.8.0rc9/half_orm/field.py
+-rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/half_orm/field_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5794 2023-03-02 13:12:11.000000 half_orm-0.8.0rc9/half_orm/fkey.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3673 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/hotest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    18902 2023-03-03 09:24:59.000000 half_orm-0.8.0rc9/half_orm/model.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1370 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/model_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-02-28 09:49:19.000000 half_orm-0.8.0rc9/half_orm/null.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3780 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/changelog.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4472 2023-03-02 13:10:29.000000 half_orm-0.8.0rc9/half_orm/packager/database.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4545 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/db_conn.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/hgit.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     5335 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/hop.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/manifest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/modules.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    13413 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patch.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.885335 half_orm-0.8.0rc9/half_orm/packager/patches/0/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.885335 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/log
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/sql/
+-rw-r--r--   0 joel      (1000) joel      (1000)     4197 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/sql/half_orm_meta.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)     8297 2023-03-02 12:49:19.000000 half_orm-0.8.0rc9/half_orm/packager/repo.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/half_orm/packager/templates/
+-rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/.gitignore
+-rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/MANIFEST.in
+-rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/Pipfile
+-rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/README
+-rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/base_test
+-rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/db_connector.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_1
+-rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_2
+-rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_3
+-rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/relation_test
+-rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/setup.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/warning
+-rw-r--r--   0 joel      (1000) joel      (1000)     1733 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/utils.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/version.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)    12382 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/pg_meta.py
+-rw-r--r--   0 joel      (1000) joel      (1000)    40090 2023-03-02 13:22:03.000000 half_orm-0.8.0rc9/half_orm/relation.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1521 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/relation_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2276 2023-02-28 09:49:19.000000 half_orm-0.8.0rc9/half_orm/transaction.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        9 2023-03-06 08:08:04.000000 half_orm-0.8.0rc9/half_orm/version.txt
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.897335 half_orm-0.8.0rc9/half_orm.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)    27243 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1553 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.8.0rc9/pyproject.toml
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.8.0rc9/setup.py
```

### Comparing `half_orm-0.8.0rc8/LICENSE` & `half_orm-0.8.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/PKG-INFO` & `half_orm-0.8.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper.
+# A simple PostgreSQL to Python mapper [0.8.0rc8]
+
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python; `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -56,44 +57,49 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content).ho_insert()
+        return self.posts_rfk(title=title, content=content)._ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston.ho_delete()
-    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston.ho_insert()
+    gaston._ho_delete()
+    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston._ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post.ho_update(title='Super easy')
-    gaston.ho_delete()
+    post._ho_update(title='Super easy')
+    gaston._ho_delete()
 ```
 
 
-# Learn `half_orm` in half an hour
+# Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-### Set your HALFORM_CONF_DIR
+## Install `half_orm` pre-release
 
-Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`:
+`pip install half_orm==0.8.0rc9`
+
+### Set your HALFORM_CONF_DIR
 
+Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
+(by default, `half_orm` looks in the /etc/half_orm directory):
+ 
 ```sh
 % mkdir ~/.half_orm
 % export HALFORM_CONF_DIR=~/.half_orm
 ```
 
 > Set your HALFORM_CONF_DIR for windows users:
 > - select settings in the menu
@@ -107,15 +113,15 @@
 name = db_name
 user = username
 password = password
 host = localhost
 port = 5432
 ```
 
-Your ready to go!
+You are ready to go!
 ## Connect to the database
 
 ```py
 >>> from half_orm.model import Model
 >>> my_db = Model('my_database')
 ```
 
@@ -228,18 +234,18 @@
 * description: the comment on the relationship if there is one,
 * fields: the list of columns, their types and contraints
 * foreign keys: the list of FKs if any. A `_reverse_*` FK is a FK made on the current relation.
 
 
 ## Constraining a relation
 
-When you instantiate an object with no arguments, its intention corresponds to all the data present in the corresponding relation.
-`Person()` represents the set of people contained in the `actor.person` table (ie. there is no constraint on the set). You can get the number of elements in a relation whith the `len` function as in `len(Person())`.
+When you instantiate an object with no arguments, its intent corresponds to all the data present in the corresponding relation.
+`Person()` represents the set of persons contained in the `actor.person` table (i.e., there is no constraint on the set). You can get the number of elements in a relation with the `len` function, as in `len(Person())`.
 
-To constrain a set, you must specify one or more values for the fields/columns in the set with a tuple of the form: `(comp, value)`.
+To define a subset, you must specify conditions on the values of the fields (columns) with tuples of the form: `(comp, value)`.
 The `comp` value ('`=`' if ommited) is either a SQL 
 [comparison operator](https://www.postgresql.org/docs/current/static/functions-comparison.html) or a [pattern matching operator (like or POSIX regular expression)](https://www.postgresql.org/docs/current/static/functions-matching.html).
 
 You can constrain a relation object at instanciation:
 
 ```python
 Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
@@ -278,56 +284,56 @@
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
 Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
-my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('ilike', 'A%'))
+my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
-`my_selection` represents the set of people whose second letter of the name is an `a` or whose first letter of the first name is an `a`.
+`my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
+# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
 by half_orm when the DML method is invoked using the _ho_mogrify() method.
 
 ```py
 people._ho_mogrify()
-people.ho_select()
+people._ho_select()
 ```
 
-## ho_insert
-To insert a tuple in the relation, use the `ho_insert` method as shown below:
+## _ho_insert
+To insert a tuple in the relation, use the `_ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
 ```
 
-By default, `ho_insert` returns the inserted row as a dict:
+By default, `_ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe.ho_insert()['id']
+lagaffe_id = lagaffe._ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.HoTransaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self.HoTransaction
+        @self._ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers).ho_insert()
+                self(**d_pers)._ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -340,64 +346,70 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `ho_insert`.
+By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `_ho_insert`.
 
-## ho_select
-The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## _ho_select
+The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people.ho_select()))
+>>> print(list(people._ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people.ho_offset(1).ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so ho_select is optional
+>>> people._ho_offset(1)._ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
 
 ```python
->>> print(list(people.ho_select('last_name')))
+>>> print(list(people._ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `ho_get` method
+### Select one: the `_ho_get` method
 
-The `ho_get` method returns an object whose fields are constrained with the values of the corresponding row in the database.
+The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
 It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe').ho_get(*args)
+gaston = Person(last_name='Lagaffe')._ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe.ho_is_empty() or len(lagaffe) > 1:
+if lagaffe._ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe.ho_select(*args)))
+gaston = Person(**next(lagaffe._ho_select()))
 gaston._ho_is_singleton = True
 ```
 
+You could use `_ho_get` to retreive the `id` of the row:
+
+```py
+gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+```
+
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
@@ -444,107 +456,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self.ho_select():
+        for elt in self._ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## ho_update
+## _ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_update(birth_date='1970-01-01')
+gaston._ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self.HoTransaction
+        @self._ho_transaction
         def update(self):
-            for d_pers in self.ho_select('id', 'last_name'):
+            for d_pers in self._ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers.ho_update(last_name=d_pers['last_name'].upper())
+                pers._ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation.HoTransaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers.ho_select())])
+>>> print([elt.last_name for elt in list(a_pers._ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_update('*', birth_date='1970-01-01')
+>>> gaston._ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person().ho_update(birth_date='1970-01-01', update_all=True)
+Person()._ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## ho_delete
+## _ho_delete
 
-The `ho_delete` method allows you to remove a set of elements from a table:
+The `_ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_delete()
+gaston._ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person().ho_delete(delete_all=True)
-if not Person().ho_is_empty():
+Person()._ho_delete(delete_all=True)
+if not Person()._ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -641,47 +653,63 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments.ho_select())
+print(list(gaston_comments._ho_select())
 ```
+## Chaining foreign keys
+
+**Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
+according to the names of the tables in the package. See the `hop` command.
 
-> TODO. Some documentation about the chaining of FKeys
+You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
+on his own posts:
 
-## The *`ho_join`* method
+```py
+gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
+gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+list(gaston
+    .post_rfk(**gaston)
+    .comment_rfk(author_id=gaston_id))
+```
 
-The *`ho_join`* method allows you to integrate the data associated to a Relation object in the result obtained by the *`select`* method by using foreign keys of the object or referencing the object.
+**Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
+while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
+## The *`_ho_join`* method
 
-It takes a list of tuples each having two or three elements:
+The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-* a remote Relation object which must be reachable using a direct or "reverse" foreign key,
-* the name of the key under which the associated data would be stored,
-* an optional list of columns (str[]) or the name of a column (str) to be extracted from the
+Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+
+It takes a list of tuples each with two or three elements:
+
+* a remote Relation object that must be accessible by a foreign key (direct or "reverse");
+* the name of the key under which the associated data would be stored;
+* an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
 
   If the third argument is omitted, all columns are retreived.
 
-The following code
+For example, the following code would return the list of people named `Lagaffe` with two
+additional attributes (`comments` and `posts`):
+
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe.ho_join(
+res = lagaffe._ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
-would return the list of people named `Lagaffe` with two
-additional attributes : `comments` and `posts`.
 
-The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
-The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
+* The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
+* The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
 
 # PostgreSQL functions and stored procedures
 
 `half_orm.model.Model` class provides two methods to deal with functions and stored procedures:
 `execute_function` and `call_procedure`. You can
 pass parameters as a list or a dictionary (for named parameters). The returned value of
 `execute_function` is a list of `dict` like objects.
```

### Comparing `half_orm-0.8.0rc8/README.md` & `half_orm-0.8.0rc9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# A simple PostgreSQL to Python mapper.
+# A simple PostgreSQL to Python mapper [0.8.0rc8]
+
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python; `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -32,44 +33,49 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content).ho_insert()
+        return self.posts_rfk(title=title, content=content)._ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston.ho_delete()
-    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston.ho_insert()
+    gaston._ho_delete()
+    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston._ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post.ho_update(title='Super easy')
-    gaston.ho_delete()
+    post._ho_update(title='Super easy')
+    gaston._ho_delete()
 ```
 
 
-# Learn `half_orm` in half an hour
+# Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-### Set your HALFORM_CONF_DIR
+## Install `half_orm` pre-release
 
-Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`:
+`pip install half_orm==0.8.0rc9`
+
+### Set your HALFORM_CONF_DIR
 
+Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
+(by default, `half_orm` looks in the /etc/half_orm directory):
+ 
 ```sh
 % mkdir ~/.half_orm
 % export HALFORM_CONF_DIR=~/.half_orm
 ```
 
 > Set your HALFORM_CONF_DIR for windows users:
 > - select settings in the menu
@@ -83,15 +89,15 @@
 name = db_name
 user = username
 password = password
 host = localhost
 port = 5432
 ```
 
-Your ready to go!
+You are ready to go!
 ## Connect to the database
 
 ```py
 >>> from half_orm.model import Model
 >>> my_db = Model('my_database')
 ```
 
@@ -204,18 +210,18 @@
 * description: the comment on the relationship if there is one,
 * fields: the list of columns, their types and contraints
 * foreign keys: the list of FKs if any. A `_reverse_*` FK is a FK made on the current relation.
 
 
 ## Constraining a relation
 
-When you instantiate an object with no arguments, its intention corresponds to all the data present in the corresponding relation.
-`Person()` represents the set of people contained in the `actor.person` table (ie. there is no constraint on the set). You can get the number of elements in a relation whith the `len` function as in `len(Person())`.
+When you instantiate an object with no arguments, its intent corresponds to all the data present in the corresponding relation.
+`Person()` represents the set of persons contained in the `actor.person` table (i.e., there is no constraint on the set). You can get the number of elements in a relation with the `len` function, as in `len(Person())`.
 
-To constrain a set, you must specify one or more values for the fields/columns in the set with a tuple of the form: `(comp, value)`.
+To define a subset, you must specify conditions on the values of the fields (columns) with tuples of the form: `(comp, value)`.
 The `comp` value ('`=`' if ommited) is either a SQL 
 [comparison operator](https://www.postgresql.org/docs/current/static/functions-comparison.html) or a [pattern matching operator (like or POSIX regular expression)](https://www.postgresql.org/docs/current/static/functions-matching.html).
 
 You can constrain a relation object at instanciation:
 
 ```python
 Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
@@ -254,56 +260,56 @@
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
 Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
-my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('ilike', 'A%'))
+my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
-`my_selection` represents the set of people whose second letter of the name is an `a` or whose first letter of the first name is an `a`.
+`my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
+# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
 by half_orm when the DML method is invoked using the _ho_mogrify() method.
 
 ```py
 people._ho_mogrify()
-people.ho_select()
+people._ho_select()
 ```
 
-## ho_insert
-To insert a tuple in the relation, use the `ho_insert` method as shown below:
+## _ho_insert
+To insert a tuple in the relation, use the `_ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
 ```
 
-By default, `ho_insert` returns the inserted row as a dict:
+By default, `_ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe.ho_insert()['id']
+lagaffe_id = lagaffe._ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.HoTransaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self.HoTransaction
+        @self._ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers).ho_insert()
+                self(**d_pers)._ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -316,64 +322,70 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `ho_insert`.
+By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `_ho_insert`.
 
-## ho_select
-The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## _ho_select
+The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people.ho_select()))
+>>> print(list(people._ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people.ho_offset(1).ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so ho_select is optional
+>>> people._ho_offset(1)._ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
 
 ```python
->>> print(list(people.ho_select('last_name')))
+>>> print(list(people._ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `ho_get` method
+### Select one: the `_ho_get` method
 
-The `ho_get` method returns an object whose fields are constrained with the values of the corresponding row in the database.
+The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
 It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe').ho_get(*args)
+gaston = Person(last_name='Lagaffe')._ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe.ho_is_empty() or len(lagaffe) > 1:
+if lagaffe._ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe.ho_select(*args)))
+gaston = Person(**next(lagaffe._ho_select()))
 gaston._ho_is_singleton = True
 ```
 
+You could use `_ho_get` to retreive the `id` of the row:
+
+```py
+gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+```
+
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
@@ -420,107 +432,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self.ho_select():
+        for elt in self._ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## ho_update
+## _ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_update(birth_date='1970-01-01')
+gaston._ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self.HoTransaction
+        @self._ho_transaction
         def update(self):
-            for d_pers in self.ho_select('id', 'last_name'):
+            for d_pers in self._ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers.ho_update(last_name=d_pers['last_name'].upper())
+                pers._ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation.HoTransaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers.ho_select())])
+>>> print([elt.last_name for elt in list(a_pers._ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_update('*', birth_date='1970-01-01')
+>>> gaston._ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person().ho_update(birth_date='1970-01-01', update_all=True)
+Person()._ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## ho_delete
+## _ho_delete
 
-The `ho_delete` method allows you to remove a set of elements from a table:
+The `_ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_delete()
+gaston._ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person().ho_delete(delete_all=True)
-if not Person().ho_is_empty():
+Person()._ho_delete(delete_all=True)
+if not Person()._ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -617,47 +629,63 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments.ho_select())
+print(list(gaston_comments._ho_select())
 ```
+## Chaining foreign keys
+
+**Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
+according to the names of the tables in the package. See the `hop` command.
 
-> TODO. Some documentation about the chaining of FKeys
+You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
+on his own posts:
 
-## The *`ho_join`* method
+```py
+gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
+gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+list(gaston
+    .post_rfk(**gaston)
+    .comment_rfk(author_id=gaston_id))
+```
 
-The *`ho_join`* method allows you to integrate the data associated to a Relation object in the result obtained by the *`select`* method by using foreign keys of the object or referencing the object.
+**Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
+while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
+## The *`_ho_join`* method
 
-It takes a list of tuples each having two or three elements:
+The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-* a remote Relation object which must be reachable using a direct or "reverse" foreign key,
-* the name of the key under which the associated data would be stored,
-* an optional list of columns (str[]) or the name of a column (str) to be extracted from the
+Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+
+It takes a list of tuples each with two or three elements:
+
+* a remote Relation object that must be accessible by a foreign key (direct or "reverse");
+* the name of the key under which the associated data would be stored;
+* an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
 
   If the third argument is omitted, all columns are retreived.
 
-The following code
+For example, the following code would return the list of people named `Lagaffe` with two
+additional attributes (`comments` and `posts`):
+
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe.ho_join(
+res = lagaffe._ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
-would return the list of people named `Lagaffe` with two
-additional attributes : `comments` and `posts`.
 
-The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
-The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
+* The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
+* The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
 
 # PostgreSQL functions and stored procedures
 
 `half_orm.model.Model` class provides two methods to deal with functions and stored procedures:
 `execute_function` and `call_procedure`. You can
 pass parameters as a list or a dictionary (for named parameters). The returned value of
 `execute_function` is a list of `dict` like objects.
```

### Comparing `half_orm-0.8.0rc8/half_orm/field.py` & `half_orm-0.8.0rc9/half_orm/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,40 +44,40 @@
         if self.__is_set:
             repr_ = f"{repr_} ({self.__name} {self.__comp} {self.__value})"
         return repr_.strip()
 
     def __str__(self):
         return str(self.__value)
 
-    def _praf(self, query, ho_id):
+    def _praf(self, query, _ho_id):
         """Returns field_name prefixed with relation alias if the query is
         select. Otherwise, returns the field name quoted with ".
         """
-        ho_id = f'r{ho_id}'
+        _ho_id = f'r{_ho_id}'
         if query == 'select':
-            return f'{ho_id}."{self.__name}"'
+            return f'{_ho_id}."{self.__name}"'
         return f'"{self.__name}"'
 
-    def _where_repr(self, query, ho_id):
+    def _where_repr(self, query, _ho_id):
         """Returns the SQL representation of the field for the where clause
         """
         where_repr = ''
         comp_str = '%s'
         comp = self._comp()
         if comp == '@@':
             comp_str = 'websearch_to_tsquery(%s)'
         if isinstance(self.__value, (list, tuple)):
             if self.__sql_type[0] != '_': # not an array type
                 comp_str = 'any(%s)'
                 if comp == '@@':
                     comp_str = 'any(websearch_to_tsquery(%s))'
         if not self.unaccent:
-            where_repr = f"{self._praf(query, ho_id)} {comp} {comp_str}"
+            where_repr = f"{self._praf(query, _ho_id)} {comp} {comp_str}"
         else:
-            where_repr = f"unaccent({self._praf(query, ho_id)}) {comp} unaccent({comp_str})"
+            where_repr = f"unaccent({self._praf(query, _ho_id)}) {comp} unaccent({comp_str})"
         return where_repr
 
     @property
     def value(self):
         "Returns the value of the field object"
         return self.__value
```

### Comparing `half_orm-0.8.0rc8/half_orm/fkey.py` & `half_orm-0.8.0rc9/half_orm/fkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from half_orm.pg_meta import normalize_fqrn, normalize_qrn
 
 class FKey:
     """Foreign key class
 
     A foreign key is set by assigning to it a Relation object of the
     corresponding type (see FKey.set method).
-    It is then used to construct the join query for Relation.ho_select
+    It is then used to construct the join query for Relation._ho_select
     method.
     """
 
     def __init__(self,
                  fk_name, relation, fk_sfqrn,
                  fk_names=None, fields=None, confupdtype=None, confdeltype=None):
         self.__relation = relation
@@ -35,28 +35,28 @@
         If model._scope is set, instanciate the class from the scoped module.
         Uses the __cast if it is set.
         """
         model = self.__relation._model
         f_cast = None
         get_rel = model._import_class if model._scope is not None else model.get_relation_class
         if self.__name.find('_reverse_fkey_') == 0 and __cast__:
-            self.__relation = get_rel(__cast__)(**self.__relation.ho_dict())
+            self.__relation = get_rel(__cast__)(**self.__relation._ho_dict())
         else:
             f_cast = __cast__
         f_relation = get_rel(f_cast or normalize_qrn(self.__fk_fqrn))(**kwargs)
-        rev_fkey_name = f'_reverse_{f_relation.ho_id}'
+        rev_fkey_name = f'_reverse_{f_relation._ho_id}'
         f_relation._ho_fkeys[rev_fkey_name] = FKey(
             rev_fkey_name,
             f_relation,
             f_relation._t_fqrn, self.__fields, self.__fk_names)
         f_relation._ho_fkeys[rev_fkey_name].set(self.__relation)
         return f_relation
 
     def values(self):
-        return [list(elt.values()) for elt in self.__to_relation.ho_select(*self.__fk_names)]
+        return [list(elt.values()) for elt in self.__to_relation._ho_select(*self.__fk_names)]
 
     def set(self, to_):
         """Sets the relation associated to the foreign key."""
         from half_orm.relation import Relation
 
         self.__to_relation = to_
         from_ = self.__relation
@@ -67,15 +67,15 @@
         common_classes = to_classes.intersection(self_classes)
         if object in common_classes:
             common_classes.remove(object)
         if not common_classes:
             raise Exception(f"Type mismatch:\n{self.__fk_fqrn} != {to_._fqrn}")
         self.__fk_from = from_
         self.__fk_to = to_
-        self.__is_set = to_.ho_is_set()
+        self.__is_set = to_._ho_is_set()
         from_._ho_join_to[self] = to_
 
     @classmethod
     def __set__(cls, *args):
         "Setting an Fkey is prohibited"
         print('XXX', cls, '\n', args)
         raise RuntimeError
@@ -113,17 +113,17 @@
         """Returns the join_query, join_values of a foreign key.
         fkey interface: frel, from_, to_, fields, fk_names
         """
         from_ = self.__fk_from
         to_ = self.to_
         if id(from_) == id(to_):
             raise RuntimeError("You can't join a relation with itself!")
-        orig_rel_id = f'r{orig_rel.ho_id}'
-        to_id = f'r{to_.ho_id}'
-        from_id = f'r{from_.ho_id}'
+        orig_rel_id = f'r{orig_rel._ho_id}'
+        to_id = f'r{to_._ho_id}'
+        from_id = f'r{from_._ho_id}'
         if to_._qrn == orig_rel._qrn:
             to_id = orig_rel_id
         if from_._qrn == orig_rel._qrn:
             from_id = orig_rel_id
         from_fields = (f'{from_id}.{name}' for name in self.__fields)
         to_fields = (f'{to_id}.{name}' for name in self.fk_names)
         bounds = " and ".join(
```

### Comparing `half_orm-0.8.0rc8/half_orm/hotest.py` & `half_orm-0.8.0rc9/half_orm/hotest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/model.py` & `half_orm-0.8.0rc9/half_orm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 psycopg2.extras.register_uuid()
 
 def deprecated(fct):
     @wraps(fct)
     def wrapper(self, *args, **kwargs):
         name = fct.__name__
-        dep_name = fct.__name__[0:3] == 'ho_' and fct.__name__[3:] or f'_{fct.__name__[4:0]}'
+        dep_name = name.replace('_ho_', '')
         callerframerecord = inspect.stack()[1]
         frame = callerframerecord[0]
         info = inspect.getframeinfo(frame)
         context = ''
         warn_msg = (f'HalfORM WARNING! "{utils.Color.bold(dep_name)}" is deprecated. '
             'It will be removed in half_orm 1.0.\n'
             f'Use "{utils.Color.bold(name)}" instead.\n')
@@ -250,22 +250,18 @@
             tbl_attr['_t_fqrn'] = dct['fqrn']
             tbl_attr['_fqrn'] = pg_meta.normalize_fqrn(dct['fqrn'])
             tbl_attr['__kind'] = REL_CLASS_NAMES[metadata['tablekind']]
             tbl_attr['_fkeys'] = []
             for fct_name, fct in REL_INTERFACES[metadata['tablekind']].items():
                 tbl_attr[fct_name] = fct
                 dep_fct_name = None
-                if fct_name[0:3] == 'ho_':
-                    dep_fct_name = fct_name[3:]
-                    # print('XXX', fct_name, dep_fct_name)
                 if fct_name[0:4] == '_ho_':
-                    dep_fct_name = f'_{fct_name[4:]}'
-                    # print('XXX', fct_name, dep_fct_name)
+                    dep_fct_name = fct_name[4:]
                 if dep_fct_name:
-                    tbl_attr[dep_fct_name] = deprecated(fct)
+                    tbl_attr[dep_fct_name] = deprecated(tbl_attr[fct_name])
             class_name = _gen_class_name(REL_CLASS_NAMES[metadata['tablekind']], dct['fqrn'])
             rel_class = type(class_name, tuple(bases), tbl_attr)
             Model._classes_[tbl_attr['_dbname']][dct['fqrn']] = rel_class
             return rel_class
 
         try:
             schema, table = relation_name.replace('"', '').rsplit('.', 1)
```

### Comparing `half_orm-0.8.0rc8/half_orm/model_errors.py` & `half_orm-0.8.0rc9/half_orm/model_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/changelog.py` & `half_orm-0.8.0rc9/half_orm/packager/changelog.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/database.py` & `half_orm-0.8.0rc9/half_orm/packager/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if get_release and self.__repo.devel:
             self.__last_release = self.last_release
 
     @property
     def last_release(self):
         "Returns the last release"
         self.__last_release = next(
-            self.__model.get_relation_class('half_orm_meta.view.hop_last_release')().ho_select())
+            self.__model.get_relation_class('half_orm_meta.view.hop_last_release')()._ho_select())
         return self.__last_release
 
     @property
     def last_release_s(self):
         "Returns the string representation of the last release X.Y.Z"
         return '{major}.{minor}.{patch}'.format(**self.last_release)
 
@@ -118,8 +118,8 @@
         "Helper: execute a postgresql command"
         return self.__connection_params.execute_pg_command
 
     def register_release(self, major, minor, patch, changelog):
         "Register the release into half_orm_meta.hop_release"
         return self.__model.get_relation_class('half_orm_meta.hop_release')(
             major=major, minor=minor, patch=patch, changelog=changelog
-        ).ho_insert()
+        )._ho_insert()
```

### Comparing `half_orm-0.8.0rc8/half_orm/packager/db_conn.py` & `half_orm-0.8.0rc9/half_orm/packager/db_conn.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/hgit.py` & `half_orm-0.8.0rc9/half_orm/packager/hgit.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/hop.py` & `half_orm-0.8.0rc9/half_orm/packager/hop.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,17 +36,17 @@
             Hop.__available_cmds = ['new']
         else:
             if not self.__repo.devel:
                 Hop.__available_cmds = ['sync-package']
             else:
                 if not self.__repo.production and self.__repo:
                     if self.__repo.hgit.branch == 'hop_main':
-                        Hop.__available_cmds = ['prepare-release']
+                        Hop.__available_cmds = ['prepare']
                     elif self.__repo.hgit.is_hop_patch_branch:
-                        Hop.__available_cmds = ['apply-release', 'undo-release', 'commit-release']
+                        Hop.__available_cmds = ['apply', 'undo', 'release']
                 elif self:
                     Hop.__available_cmds = ['upgrade', 'restore']
 
     @property
     def repo_checked(self):
         "Returns wether we are in a repo or not."
         return self.__repo.checked
@@ -77,37 +77,37 @@
             self.__repo.new(package_name, devel)
 
 
         @click.command()
         @click.option(
             '-l', '--level',
             type=click.Choice(['patch', 'minor', 'major']), help="Release level.")
-        @click.option('-m', '--message', type=str, help="The commit message")
-        def prepare_release(level, message=None):
+        @click.option('-m', '--message', type=str, help="The git commit message")
+        def prepare(level, message=None):
             """ Prepares the next release.
             """
-            self.__command = 'prepare-release'
+            self.__command = 'prepare'
             self.__repo.prepare_release(level, message)
             sys.exit()
 
         @click.command()
-        def apply_release():
+        def apply():
             """Apply the current release.
             """
-            self.__command = 'apply-release'
+            self.__command = 'apply'
             self.__repo.apply_release()
 
         @click.command()
         @click.option(
             '-d', '--database-only', is_flag=True,
             help='Restore the database to the previous release.')
-        def undo_release(database_only):
+        def undo(database_only):
             """Undo the last release.
             """
-            self.__command = 'undo-release'
+            self.__command = 'undo'
             self.__repo.undo_release(database_only)
 
         @click.command()
         # @click.option('-d', '--dry-run', is_flag=True, help='Do nothing')
         # @click.option('-l', '--loop', is_flag=True, help='Run every patches to apply')
         def upgrade():
             """Apply one or many patches.
@@ -121,27 +121,27 @@
         @click.argument('release')
         def restore(release):
             "Restore to release"
             self.__repo.restore(release)
 
         @click.command()
         @click.option('-p', '--push', is_flag=True, help='Push git repo to origin')
-        def commit_release(push=False):
+        def release(push=False):
             self.__repo.commit_release(push)
 
         @click.command()
         def sync_package():
             self.__repo.sync_package()
 
         cmds = {
             'new': new,
-            'prepare-release': prepare_release,
-            'apply-release': apply_release,
-            'undo-release': undo_release,
-            'commit-release': commit_release,
+            'prepare': prepare,
+            'apply': apply,
+            'undo': undo,
+            'release': release,
             'sync-package': sync_package,
             'upgrade': upgrade,
             'restore': restore
         }
 
         for cmd in self.__available_cmds:
             click_main.add_command(cmds[cmd])
```

### Comparing `half_orm-0.8.0rc8/half_orm/packager/manifest.py` & `half_orm-0.8.0rc9/half_orm/packager/manifest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/modules.py` & `half_orm-0.8.0rc9/half_orm/packager/modules.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/patch.py` & `half_orm-0.8.0rc9/half_orm/packager/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     @property
     def state(self):
         "The state of a patch"
         if self.__repo.devel:
             if not self.__repo.production:
                 resp = ['[Releases in development]']
                 if len(self.__changelog.releases_in_dev) == 0:
-                    resp.append("No release in development.\nUse `hop prepare-release`.")
+                    resp.append("No release in development.\nUse `hop prepare`.")
                 for release in self.__changelog.releases_in_dev:
                     resp.append(f'- {release} (branch hop_{release})')
             else:
                 resp = ['[Releases to apply]']
                 if len(self.__changelog.releases_to_apply_in_prod) == 0:
                     resp.append("No new release to apply.")
                 for release in self.__changelog.releases_to_apply_in_prod:
@@ -273,15 +273,15 @@
             utils.error(f'Next release is {next_release} Please switch to the branch {next_branch}!\n', 1)
         # Git repo must be clean
         if not self.__repo.hgit.repos_is_clean():
             utils.error(
                 f'Please `git commit` your changes before releasing {next_release}.\n', exit_code=1)
         # The patch must be applied and the last to apply
         if not self.__repo.database.last_release_s == next_release:
-            utils.error(f'Please `hop test-release` before releasing {next_release}.\n', exit_code=1)
+            utils.error(f'Please `hop test` before releasing {next_release}.\n', exit_code=1)
         # If we undo the patch (db only) and re-apply it the repo must still be clear.
         self.undo(database_only=True)
         self.apply(next_release, force=True)
         if not self.__repo.hgit.repos_is_clean():
             utils.error(
                 'Something has changed when re-applying the release. This should not happen.\n',
                 exit_code=1)
```

### Comparing `half_orm-0.8.0rc8/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql` & `half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/patches/sql/half_orm_meta.sql` & `half_orm-0.8.0rc9/half_orm/packager/patches/sql/half_orm_meta.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/repo.py` & `half_orm-0.8.0rc9/half_orm/packager/repo.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/templates/README` & `half_orm-0.8.0rc9/half_orm/packager/templates/README`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/templates/setup.py` & `half_orm-0.8.0rc9/half_orm/packager/templates/setup.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/packager/utils.py` & `half_orm-0.8.0rc9/half_orm/packager/utils.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/pg_meta.py` & `half_orm-0.8.0rc9/half_orm/pg_meta.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/relation.py` & `half_orm-0.8.0rc9/half_orm/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
 """
 Main methods provided by the class Relation:
 - insert: inserts a tuple into the pg table.
 - select: returns a generator of the elements of the set defined by
   the constraint on the Relation object. The elements are dictionaries with the
   keys corresponding to the selected columns names in the relation.
-  The result is affected by the methods: ho_distinct, ho_order_by, ho_limit and ho_offset
+  The result is affected by the methods: _ho_distinct, _ho_order_by, _ho_limit and _ho_offset
   (see below).
 - update: updates the set defined by the constraint on the Relation object
   with the values passed as arguments.
 - delete: deletes from the relation the set of elements defined by the constraint
   on the Relation object.
 - get: returns the unique element defined by the constraint on the Relation object.
   the element returned if of the type of the Relation object.
 - count: returns the number of elements in the set defined by the constraint on the
   Relation object.
 
 The following methods can be chained on the object before a select.
 
-- ho_distinct: ensures that there are no duplicates on the select result.
-- ho_order_by: sets the order of the select result.
-- ho_limit: limits the number of elements returned by the select method.
-- ho_offset: sets the offset for the select method.
+- _ho_distinct: ensures that there are no duplicates on the select result.
+- _ho_order_by: sets the order of the select result.
+- _ho_limit: limits the number of elements returned by the select method.
+- _ho_offset: sets the offset for the select method.
 
 """
 
 from functools import wraps
 from collections import OrderedDict
 from uuid import UUID
 from typing import Generator, List
@@ -50,15 +50,15 @@
 import psycopg2
 from psycopg2.extras import RealDictCursor
 
 
 import yaml
 
 from half_orm import relation_errors
-from half_orm.transaction import HoTransaction
+from half_orm.transaction import Transaction
 from half_orm.field import Field
 
 class _SetOperators:
     """_SetOperators class stores the set operations made on the Relation class objects
 
     - __operator is one of {'or', 'and', 'sub', 'neg'}
     - __right is a Relation object. It can be None if the operator is 'neg'.
@@ -160,22 +160,22 @@
     kwk_ = set(kwargs.keys())
     if kwk_.intersection(self._ho_fields.keys()) != kwk_:
         raise relation_errors.UnknownAttributeError(str(kwk_.difference(self._ho_fields.keys())))
     _ = {self.__dict__[field_name]._set(value)
          for field_name, value in kwargs.items() if value is not None}
     self.__isfrozen = True
 
-def ho_insert(self, *args, data=None) -> '[dict]':
+def _ho_insert(self, *args, data=None) -> '[dict]':
     """Insert a new tuple into the Relation.
 
     Returns:
         [dict]: A singleton containing the data inserted.
 
     Example:
-        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1970-01-01').ho_insert()
+        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1970-01-01')._ho_insert()
         >>> print(gaston)
         {'id': 1772, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1970, 1, 1)}
 
     Note:
         It is not possible to insert more than one row with the insert method
     """
     query_template = "insert into {} ({}) values ({})"
@@ -194,40 +194,40 @@
         query = self.__add_returning(query, *returning)
     self.__execute(query, tuple(values))
     res = [dict(elt) for elt in self.__cursor.fetchall()]
     if (args or not data) and len(res):
         return res[0]
     return {}
 
-def ho_select(self, *args):
+def _ho_select(self, *args):
     """Gets the set of values correponding to the constraint attached to the object.
     This method is a generator.
 
     Arguments:
         *args: the fields names of the returned attributes. If omitted,
             all the fields are returned.
 
     Yields:
         the result of the query as a dictionary.
 
     Example:
-        >>> for person in Person(last_name=('like', 'La%')).ho_select('id'):
+        >>> for person in Person(last_name=('like', 'La%'))._ho_select('id'):
         >>>     print(person)
         {'id': 1772}
     """
     query, values = self._ho_prep_select(*args)
     try:
         self.__execute(query, values)
     except Exception as err:
         sys.stderr.write(f"QUERY: {query}\nVALUES: {values}\n")
         raise err
     for elt in self.__cursor:
         yield dict(elt)
 
-def ho_get(self, *args: List[str]) -> Relation:
+def _ho_get(self, *args: List[str]) -> Relation:
     """The get method allows you to fetch a singleton from the database.
     It garantees that the constraint references one and only one tuple.
 
     Args:
         args (List[str]): list of fields names.\
         If ommitted, all the values of the row retreived from the database\
         are set for the self object.\
@@ -236,39 +236,39 @@
     Returns:
         Relation: the object retreived from the database.
 
     Raises:
         ExpectedOneError: an exception is raised if no or more than one element is found.
 
     Example:
-        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston').ho_get()
+        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston')._ho_get()
         >>> type(gaston) is Person
         True
         >>> gaston.id
         (int4) NOT NULL (id = 1772)
         >>> str(gaston.id)
         '1772'
         >>> gaston.id.value
         1772
     """
     _count = len(self)
     if _count != 1:
         raise relation_errors.ExpectedOneError(self, _count)
     self._ho_is_singleton = True
-    ret = self(**(next(self.ho_select(*args))))
+    ret = self(**(next(self._ho_select(*args))))
     ret._ho_is_singleton = True
     return ret
 
-def ho_update(self, *args, update_all=False, **kwargs):
+def _ho_update(self, *args, update_all=False, **kwargs):
     """
     kwargs represents the values to be updated {[field name:value]}
     The object self must be set unless update_all is True.
     The constraints of the relations are updated with kwargs.
     """
-    if not (self.ho_is_set() or update_all):
+    if not (self._ho_is_set() or update_all):
         raise RuntimeError(
             f'Attempt to update all rows of {self.__class__.__name__}'
             ' without update_all being set to True!')
 
     update_args = dict(kwargs)
     for key, value in kwargs.items():
         # None values are first removed
@@ -289,19 +289,19 @@
         query = self.__add_returning(query, *args)
     self.__execute(query, tuple(values))
     for field_name, value in update_args.items():
         self._ho_fields[field_name]._set(value)
     if args:
         return [dict(elt) for elt in self.__cursor.fetchall()]
 
-def ho_delete(self, *args, delete_all=False):
+def _ho_delete(self, *args, delete_all=False):
     """Removes a set of tuples from the relation.
     To empty the relation, delete_all must be set to True.
     """
-    if not (self.ho_is_set() or delete_all):
+    if not (self._ho_is_set() or delete_all):
         raise RuntimeError(
             f'Attempt to delete all rows from {self.__class__.__name__}'
             ' without delete_all being set to True!')
     query_template = "delete from {} {}"
     _, values = self.__get_query(query_template)
     self.__query_type = 'delete'
     _, where, _ = self.__where_args()
@@ -359,25 +359,25 @@
         return self.__cursor.execute(query, values)
     except (psycopg2.OperationalError, psycopg2.InterfaceError):
         self._model.ping()
         self.__cursor = self._model._connection.cursor(cursor_factory=RealDictCursor)
         return self.__cursor.execute(query, values)
 
 @property
-def ho_id(self):
+def _ho_id(self):
     """Return the __id_cast or the id of the relation.
     """
     return self.__id_cast or id(self)
 
 @property
-def ho_only(self):
+def _ho_only(self):
     "Returns the value of self.__only"
     return self.__only
-@ho_only.setter
-def ho_only(self, value):
+@_ho_only.setter
+def _ho_only(self, value):
     """Set the value of self.__only. Restrict the values of a query to
     the elements of the relation (no inherited values).
     """
     if not value in {True, False}:
         raise ValueError(f'{value} is not a bool!')
     self.__only = value
 
@@ -408,15 +408,15 @@
                 if key != '': # we skip empty keys
                     setattr(self, key, self._ho_fkeys[value])
                     self._ho_fkeys_attr.add(key)
             except KeyError as exp:
                 raise relation_errors.WrongFkeyError(self, value) from exp
     self.__fkeys_properties = True
 
-def ho_group_by(self, yml_directive):
+def _ho_group_by(self, yml_directive):
     """Returns an aggregation of the data according to the yml directive
     description.
     """
     def inner_group_by(data, directive, grouped_data, gdata=None):
         """recursive fonction to actually group the data in grouped_data."""
         deja_vu_key = set()
         if gdata is None:
@@ -479,15 +479,15 @@
 
     grouped_data = {}
     data = list(self)
     directive = yaml.safe_load(yml_directive)
     inner_group_by(data, directive, grouped_data)
     return grouped_data
 
-def ho_json(self, yml_directive=None, res_field_name='elements', **kwargs):
+def _ho_json(self, yml_directive=None, res_field_name='elements', **kwargs):
     """Returns a JSON representation of the set returned by the select query.
     if kwargs, returns {res_field_name: [list of elements]}.update(kwargs)
     """
 
     def handler(obj):
         """Replacement of default handler for json.dumps."""
         if hasattr(obj, 'isoformat'):
@@ -496,23 +496,23 @@
             return str(obj)
         if isinstance(obj, timedelta):
             return obj.total_seconds()
         raise TypeError(
             f'Object of type {type(obj)} with value of {repr(obj)} is not JSON serializable')
 
     if yml_directive:
-        res = self.ho_group_by(yml_directive)
+        res = self._ho_group_by(yml_directive)
     else:
         res = list(self)
     if kwargs:
         res = {res_field_name: res}
         res.update(kwargs)
     return json.dumps(res, default=handler)
 
-def ho_dict(self):
+def _ho_dict(self):
     """Returns a dictionary containing only the values of the fields
     that are set."""
     return {key:field.value for key, field in self._ho_fields.items() if field.is_set()}
 
 def __to_dict_val_comp(self):
     """Returns a dictionary containing the values and comparators of the fields
     that are set."""
@@ -557,22 +557,22 @@
         ret.append('')
         ret.append(fkeys_usage)
         for fkey in self._ho_fkeys:
             ret.append(f"    '': '{fkey}',")
         ret.append('}')
     return '\n'.join(ret)
 
-def ho_is_set(self):
+def _ho_is_set(self):
     """Return True if one field at least is set or if self has been
     constrained by at least one of its foreign keys or self is the
     result of a combination of Relations (using set operators).
     """
     joined_to = False
     for _, jt_ in self._ho_join_to.items():
-        joined_to |= jt_.ho_is_set()
+        joined_to |= jt_._ho_is_set()
     return (joined_to or bool(self.__set_operators.operator) or bool(self.__neg) or
             bool({field for field in self._ho_fields.values() if field.is_set()}))
 
 def __get_set_fields(self):
     """Returns a list containing only the fields that are set."""
     return [field for field in self._ho_fields.values() if field.is_set()]
 
@@ -603,39 +603,39 @@
         _fields_ += self.__get_set_fields()
     return out, _fields_
 
 def __join(self, orig_rel, deja_vu):
     for fkey, fk_rel in self._ho_join_to.items():
         fk_rel.__query_type = orig_rel.__query_type
         fk_rel.__get_from(orig_rel, deja_vu)
-        if fk_rel.ho_id not in deja_vu:
-            deja_vu[fk_rel.ho_id] = []
-        elif (fk_rel, fkey) in deja_vu[fk_rel.ho_id] or fk_rel is orig_rel:
+        if fk_rel._ho_id not in deja_vu:
+            deja_vu[fk_rel._ho_id] = []
+        elif (fk_rel, fkey) in deja_vu[fk_rel._ho_id] or fk_rel is orig_rel:
             #sys.stderr.write(f"déjà vu in from! {fk_rel._fqrn}\n")
             continue
-        deja_vu[fk_rel.ho_id].append((fk_rel, fkey))
+        deja_vu[fk_rel._ho_id].append((fk_rel, fkey))
         if fk_rel.__set_operators.operator:
-            fk_rel.__get_from(self.ho_id)
+            fk_rel.__get_from(self._ho_id)
         _, where, values = fk_rel.__where_args()
         where = f" and\n    {where}"
         orig_rel.__sql_query.insert(1, f'\n  join {__sql_id(fk_rel)} on\n   ')
         orig_rel.__sql_query.insert(2, fkey._join_query(self))
         orig_rel.__sql_query.append(where)
         orig_rel.__sql_values += values
 
 def __sql_id(self):
     """Returns the FQRN as alias for the sql query."""
-    return f"{self._qrn} as r{self.ho_id}"
+    return f"{self._qrn} as r{self._ho_id}"
 
 def __get_from(self, orig_rel=None, deja_vu=None):
     """Constructs the __sql_query and gets the __sql_values for self."""
     if deja_vu is None:
         orig_rel = self
         self.__sql_query = [__sql_id(self)]
-        deja_vu = {self.ho_id:[(self, None)]}
+        deja_vu = {self._ho_id:[(self, None)]}
     self.__join(orig_rel, deja_vu)
 
 def __where_repr(self, rel_id_):
     where_repr = []
     for field in self.__get_set_fields():
         where_repr.append(field._where_repr(self.__query_type, rel_id_))
     where_repr = ' and\n    '.join(where_repr) or '1 = 1'
@@ -643,15 +643,15 @@
     if self.__neg:
         ret = f"not ({ret})"
     return ret
 
 def __where_args(self, *args):
     """Returns the what, where and values needed to construct the queries.
     """
-    rel_id_ = self.ho_id
+    rel_id_ = self._ho_id
     what = f'r{rel_id_}.*'
     if args:
         what = ', '.join([f'r{rel_id_}.{arg}' for arg in args])
     s_where, set_fields = self.__walk_op(rel_id_)
     s_where = ''.join(s_where)
     if s_where == '()':
         s_where = '(1 = 1)'
@@ -695,45 +695,45 @@
         query = f"{query} order by {self.__select_params['order_by']}"
     if 'limit' in self.__select_params.keys():
         query = f"{query} limit {self.__select_params['limit']}"
     if 'offset' in self.__select_params.keys():
         query = f"{query} offset {self.__select_params['offset']}"
     return query, values
 
-def ho_distinct(self):
+def _ho_distinct(self):
     """Set distinct in SQL select request."""
     self.__select_params['distinct'] = 'distinct'
     return self
 
-def ho_unaccent(self, *fields_names):
+def _ho_unaccent(self, *fields_names):
     "Sets unaccent for each field listed in fields_names"
     for field_name in fields_names:
         if not isinstance(self.__dict__[field_name], Field):
             raise ValueError(f'{field_name} is not a Field!')
         self.__dict__[field_name].unaccent = True
     return self
 
-def ho_order_by(self, _order_):
+def _ho_order_by(self, _order_):
     """Set SQL order by according to the "order" string passed
 
     @order string example :
     "field1, field2 desc, field3, field4 desc"
     """
     self.__select_params['order_by'] = _order_
     return self
 
-def ho_limit(self, _limit_):
+def _ho_limit(self, _limit_):
     """Set limit for the next SQL select request."""
     if _limit_:
         self.__select_params['limit'] = _limit_
     elif 'limit' in self.__select_params:
         self.__select_params.pop('limit')
     return self
 
-def ho_offset(self, _offset_):
+def _ho_offset(self, _offset_):
     """Set the offset for the next SQL select request."""
     self.__select_params['offset'] = _offset_
     return self
 
 def _ho_mogrify(self):
     """Prints the select query."""
     self.__mogrify = True
@@ -752,15 +752,15 @@
         self.__execute(query, vars_)
     except Exception as err:
         self._ho_mogrify()
         self.__execute(query, vars_)
         raise Exception from err
     return self.__cursor.fetchone()['count']
 
-def ho_is_empty(self):
+def _ho_is_empty(self):
     """Returns True if the relation is empty, False otherwise.
 
     Same as __len__ but limits the request to 1 element (faster).
     Use it instead of len(relation) == 0.
     """
     self.__query = "select"
     query_template = "select\n  count(distinct {})\nfrom {}\n  {}\n  {} limit 1"
@@ -824,25 +824,25 @@
             fk_queries = ["%s" for _ in range(len(fk_values))]
 
     return fields_names, set_fields, fk_fields, fk_queries, fk_values
 
 def __call__(self, **kwargs):
     return self.__class__(**kwargs)
 
-def ho_cast(self, qrn):
+def _ho_cast(self, qrn):
     """Cast a relation into another relation.
     """
     new = self._model._import_class(qrn)(**self.__to_dict_val_comp())
     new.__id_cast = id(self)
     new._ho_join_to = self._ho_join_to
     new.__set_operators = self.__set_operators
     return new
 
-def ho_join(self, *f_rels):
-    """Joins data to self.ho_select() result. Returns a dict
+def _ho_join(self, *f_rels):
+    """Joins data to self._ho_select() result. Returns a dict
     f_rels is a list of [(obj: Relation(), name: str, fields: Optional(<str|str[]>)), ...].
 
     Each obj in f_rels must have a direct or reverse fkey to self.
     If res is the result, res[name] contains the data associated to the element
     through the fkey or reversed fkey.
     If fields is a str, the data associated with res[name] is returned in a list (only one column).
     Otherwise (str[]), res[name] is a list of dict.
@@ -867,15 +867,15 @@
         TO_PROCESS = {UUID, date, datetime, time, timedelta}
         if value.__class__ in TO_PROCESS:
             return str(value)
         return value
 
     res = list(
         {key: to_str(value) for key, value in elt.items()}
-        for elt in self.ho_distinct()
+        for elt in self._ho_distinct()
     )
     result_as_list = False
     ref = self()
     for f_rel in f_rels:
         if not isinstance(f_rel, tuple):
             raise RuntimeError("f_rels must be a list of tuples.")
         if len(f_rel) == 3:
@@ -904,15 +904,15 @@
                 fkey_found = True
                 f_relation_fk_names = remote_fk.fk_names
                 break
 
         if not fkey_found:
             raise RuntimeError(f"No foreign key between {self._fqrn} and {f_relation._fqrn}!")
         inter = [{key: to_str(val) for key, val in elt.items()}
-            for elt in remote.ho_distinct().ho_select(
+            for elt in remote._ho_distinct()._ho_select(
                 *([f'"{field}"' for field in fields] + f_relation_fk_names))]
         for elt in inter:
             key = tuple(elt[subelt] for subelt in f_relation_fk_names)
             if key not in res_remote:
                 res_remote[key] = []
             if result_as_list:
                 res_remote[key].append(to_str(elt[fields[0]]))
@@ -1002,52 +1002,52 @@
 def __enter__(self):
     """Context management entry
 
     Returns self in a transaction context.
 
     Example usage:
     with relation as rel:
-        rel.ho_update(col=new_val)
+        rel._ho_update(col=new_val)
 
     Equivalent to (in a transaction context):
-    rel = relation.ho_select()
+    rel = relation._ho_select()
     for elt in rel:
         new_elt = relation(**elt)
-        new_elt.ho_update(col=new_val)
+        new_elt._ho_update(col=new_val)
     """
-    @self.HoTransaction
+    @self._ho_transaction
     def context(self):
         return self
     return context(self)
 
 def __exit__(_, *__):
     """Context management exit
 
     Not much to do here.
     """
     return False
 
 def __iter__(self):
-    return self.ho_select()
+    return self._ho_select()
 
 def __next__(self):
-    return next(self.ho_select())
+    return next(self._ho_select())
 
 def singleton(fct):
     """Decorator. Enforces the relation to define a singleton.
 
     _ho_is_singleton is set by Relation.get.
     _ho_is_singleton is unset as soon as a Field is set.
     """
     @wraps(fct)
     def wrapper(self, *args, **kwargs):
         if self._ho_is_singleton:
             return fct(self, *args, **kwargs)
         try:
-            self = self.ho_get()
+            self = self._ho_get()
             return fct(self, *args, **kwargs)
         except relation_errors.ExpectedOneError as err:
             raise relation_errors.NotASingletonError(err)
     return wrapper
 
 #### Deprecated
 
@@ -1096,35 +1096,35 @@
     # protected methods
     '_ho_freeze': _ho_freeze,
     '_ho_unfreeze': _ho_unfreeze,
     '_ho_prep_select': _ho_prep_select,
     '_ho_mogrify': _ho_mogrify,
 
     # public methods
-    'ho_id': ho_id,
-    'ho_order_by': ho_order_by,
-    'ho_limit': ho_limit,
-    'ho_offset': ho_offset,
-    'ho_distinct': ho_distinct,
-    'ho_unaccent': ho_unaccent,
-    'ho_cast': ho_cast,
-    'ho_only': ho_only,
-    'ho_is_empty': ho_is_empty,
-    'ho_group_by':ho_group_by,
-    'ho_json': ho_json,
-    'ho_dict': ho_dict,
-    'ho_is_set': ho_is_set,
-    'ho_get': ho_get,
-    'ho_join': ho_join,
-    'ho_insert': ho_insert,
-    'ho_select': ho_select,
-    'ho_update': ho_update,
-    'ho_delete': ho_delete,
+    '_ho_id': _ho_id,
+    '_ho_order_by': _ho_order_by,
+    '_ho_limit': _ho_limit,
+    '_ho_offset': _ho_offset,
+    '_ho_distinct': _ho_distinct,
+    '_ho_unaccent': _ho_unaccent,
+    '_ho_cast': _ho_cast,
+    '_ho_only': _ho_only,
+    '_ho_is_empty': _ho_is_empty,
+    '_ho_group_by':_ho_group_by,
+    '_ho_json': _ho_json,
+    '_ho_dict': _ho_dict,
+    '_ho_is_set': _ho_is_set,
+    '_ho_get': _ho_get,
+    '_ho_join': _ho_join,
+    '_ho_insert': _ho_insert,
+    '_ho_select': _ho_select,
+    '_ho_update': _ho_update,
+    '_ho_delete': _ho_delete,
 
-    'HoTransaction': HoTransaction,
+    '_ho_transaction': Transaction,
 }
 
 
 TABLE_INTERFACE = COMMON_INTERFACE
 VIEW_INTERFACE = COMMON_INTERFACE
 MVIEW_INTERFACE = COMMON_INTERFACE
 FDATA_INTERFACE = COMMON_INTERFACE
```

### Comparing `half_orm-0.8.0rc8/half_orm/relation_errors.py` & `half_orm-0.8.0rc9/half_orm/relation_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/half_orm/transaction.py` & `half_orm-0.8.0rc9/half_orm/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #-*- coding: utf-8 -*-
 # pylint: disable=too-few-public-methods, protected-access
 
-"""This module provides the HoTransaction class."""
+"""This module provides the Transaction class."""
 
 import sys
 
-class HoTransaction:
-    """The HoTransaction class is intended to be used as a class attribute of
+class Transaction:
+    """The Transaction class is intended to be used as a class attribute of
     relation.Relation class:
 
-    Relation.HoTransaction = HoTransaction
+    Relation.Transaction = Transaction
 
     The Relation.transaction can be used as a decorator of any method of a
     sub class of Relation class or any function receiving a Relation object
     as its first argument.
 
     Example of use:
 
     ```python
     gaston = halftest.relation("actor.person", first_name="Gaston")
-    @gaston.HoTransaction
+    @gaston.Transaction
     def do_something(person):
         #... code to be done
     do_somethin(gaston)
     ```
     Every SQL commands executed in the do_something function will be put in a
     transaction and commited or rolled back at the end of the function.
 
     Functions decorated by a transaction can be nested:
 
     ```python
-    @gaston.HoTransaction
+    @gaston.Transaction
     def second(gaston):
         # ... do something else
-    @gaston.HoTransaction
+    @gaston.Transaction
     def first(gaston):
         # ... do something
         second(gaston)
     first(gaston)
     ```
     Here second is called by first and both function are played in the same
     transaction.
@@ -50,22 +50,22 @@
     def __call__(self, relation, *args, **kwargs):
         """Each time a transaction is hit, the level is increased.
         The transaction is commited when the level is back to 0 after
         the return of the function.
         """
         res = None
         try:
-            HoTransaction.__level += 1
+            Transaction.__level += 1
             if relation._model._connection.autocommit:
                 relation._model._connection.autocommit = False
             res = self.__func(relation, *args, **kwargs)
-            HoTransaction.__level -= 1
-            if HoTransaction.__level == 0:
+            Transaction.__level -= 1
+            if Transaction.__level == 0:
                 relation._model._connection.commit()
                 relation._model._connection.autocommit = True
         except Exception as err:
-            sys.stderr.write(f"HoTransaction error: {err}\nRolling back!\n")
-            HoTransaction.__level = 0
+            sys.stderr.write(f"Transaction error: {err}\nRolling back!\n")
+            Transaction.__level = 0
             relation._model._connection.rollback()
             relation._model._connection.autocommit = True
             raise err
         return res
```

### Comparing `half_orm-0.8.0rc8/half_orm.egg-info/PKG-INFO` & `half_orm-0.8.0rc9/half_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half-orm
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper.
+# A simple PostgreSQL to Python mapper [0.8.0rc8]
+
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python; `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -56,44 +57,49 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content).ho_insert()
+        return self.posts_rfk(title=title, content=content)._ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston.ho_delete()
-    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston.ho_insert()
+    gaston._ho_delete()
+    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston._ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post.ho_update(title='Super easy')
-    gaston.ho_delete()
+    post._ho_update(title='Super easy')
+    gaston._ho_delete()
 ```
 
 
-# Learn `half_orm` in half an hour
+# Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-### Set your HALFORM_CONF_DIR
+## Install `half_orm` pre-release
 
-Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`:
+`pip install half_orm==0.8.0rc9`
+
+### Set your HALFORM_CONF_DIR
 
+Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
+(by default, `half_orm` looks in the /etc/half_orm directory):
+ 
 ```sh
 % mkdir ~/.half_orm
 % export HALFORM_CONF_DIR=~/.half_orm
 ```
 
 > Set your HALFORM_CONF_DIR for windows users:
 > - select settings in the menu
@@ -107,15 +113,15 @@
 name = db_name
 user = username
 password = password
 host = localhost
 port = 5432
 ```
 
-Your ready to go!
+You are ready to go!
 ## Connect to the database
 
 ```py
 >>> from half_orm.model import Model
 >>> my_db = Model('my_database')
 ```
 
@@ -228,18 +234,18 @@
 * description: the comment on the relationship if there is one,
 * fields: the list of columns, their types and contraints
 * foreign keys: the list of FKs if any. A `_reverse_*` FK is a FK made on the current relation.
 
 
 ## Constraining a relation
 
-When you instantiate an object with no arguments, its intention corresponds to all the data present in the corresponding relation.
-`Person()` represents the set of people contained in the `actor.person` table (ie. there is no constraint on the set). You can get the number of elements in a relation whith the `len` function as in `len(Person())`.
+When you instantiate an object with no arguments, its intent corresponds to all the data present in the corresponding relation.
+`Person()` represents the set of persons contained in the `actor.person` table (i.e., there is no constraint on the set). You can get the number of elements in a relation with the `len` function, as in `len(Person())`.
 
-To constrain a set, you must specify one or more values for the fields/columns in the set with a tuple of the form: `(comp, value)`.
+To define a subset, you must specify conditions on the values of the fields (columns) with tuples of the form: `(comp, value)`.
 The `comp` value ('`=`' if ommited) is either a SQL 
 [comparison operator](https://www.postgresql.org/docs/current/static/functions-comparison.html) or a [pattern matching operator (like or POSIX regular expression)](https://www.postgresql.org/docs/current/static/functions-matching.html).
 
 You can constrain a relation object at instanciation:
 
 ```python
 Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
@@ -278,56 +284,56 @@
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
 Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
-my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('ilike', 'A%'))
+my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
-`my_selection` represents the set of people whose second letter of the name is an `a` or whose first letter of the first name is an `a`.
+`my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
+# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
 by half_orm when the DML method is invoked using the _ho_mogrify() method.
 
 ```py
 people._ho_mogrify()
-people.ho_select()
+people._ho_select()
 ```
 
-## ho_insert
-To insert a tuple in the relation, use the `ho_insert` method as shown below:
+## _ho_insert
+To insert a tuple in the relation, use the `_ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
 ```
 
-By default, `ho_insert` returns the inserted row as a dict:
+By default, `_ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe.ho_insert()['id']
+lagaffe_id = lagaffe._ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.HoTransaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self.HoTransaction
+        @self._ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers).ho_insert()
+                self(**d_pers)._ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -340,64 +346,70 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `ho_insert`.
+By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `_ho_insert`.
 
-## ho_select
-The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## _ho_select
+The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people.ho_select()))
+>>> print(list(people._ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people.ho_offset(1).ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so ho_select is optional
+>>> people._ho_offset(1)._ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
 
 ```python
->>> print(list(people.ho_select('last_name')))
+>>> print(list(people._ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `ho_get` method
+### Select one: the `_ho_get` method
 
-The `ho_get` method returns an object whose fields are constrained with the values of the corresponding row in the database.
+The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
 It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe').ho_get(*args)
+gaston = Person(last_name='Lagaffe')._ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe.ho_is_empty() or len(lagaffe) > 1:
+if lagaffe._ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe.ho_select(*args)))
+gaston = Person(**next(lagaffe._ho_select()))
 gaston._ho_is_singleton = True
 ```
 
+You could use `_ho_get` to retreive the `id` of the row:
+
+```py
+gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+```
+
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
@@ -444,107 +456,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self.ho_select():
+        for elt in self._ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## ho_update
+## _ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_update(birth_date='1970-01-01')
+gaston._ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self.HoTransaction
+        @self._ho_transaction
         def update(self):
-            for d_pers in self.ho_select('id', 'last_name'):
+            for d_pers in self._ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers.ho_update(last_name=d_pers['last_name'].upper())
+                pers._ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation.HoTransaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers.ho_select())])
+>>> print([elt.last_name for elt in list(a_pers._ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_update('*', birth_date='1970-01-01')
+>>> gaston._ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person().ho_update(birth_date='1970-01-01', update_all=True)
+Person()._ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## ho_delete
+## _ho_delete
 
-The `ho_delete` method allows you to remove a set of elements from a table:
+The `_ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston.ho_delete()
+gaston._ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person().ho_delete(delete_all=True)
-if not Person().ho_is_empty():
+Person()._ho_delete(delete_all=True)
+if not Person()._ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -641,47 +653,63 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments.ho_select())
+print(list(gaston_comments._ho_select())
 ```
+## Chaining foreign keys
+
+**Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
+according to the names of the tables in the package. See the `hop` command.
 
-> TODO. Some documentation about the chaining of FKeys
+You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
+on his own posts:
 
-## The *`ho_join`* method
+```py
+gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
+gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+list(gaston
+    .post_rfk(**gaston)
+    .comment_rfk(author_id=gaston_id))
+```
 
-The *`ho_join`* method allows you to integrate the data associated to a Relation object in the result obtained by the *`select`* method by using foreign keys of the object or referencing the object.
+**Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
+while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
+## The *`_ho_join`* method
 
-It takes a list of tuples each having two or three elements:
+The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-* a remote Relation object which must be reachable using a direct or "reverse" foreign key,
-* the name of the key under which the associated data would be stored,
-* an optional list of columns (str[]) or the name of a column (str) to be extracted from the
+Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+
+It takes a list of tuples each with two or three elements:
+
+* a remote Relation object that must be accessible by a foreign key (direct or "reverse");
+* the name of the key under which the associated data would be stored;
+* an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
 
   If the third argument is omitted, all columns are retreived.
 
-The following code
+For example, the following code would return the list of people named `Lagaffe` with two
+additional attributes (`comments` and `posts`):
+
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe.ho_join(
+res = lagaffe._ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
-would return the list of people named `Lagaffe` with two
-additional attributes : `comments` and `posts`.
 
-The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
-The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
+* The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
+* The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
 
 # PostgreSQL functions and stored procedures
 
 `half_orm.model.Model` class provides two methods to deal with functions and stored procedures:
 `execute_function` and `call_procedure`. You can
 pass parameters as a list or a dictionary (for named parameters). The returned value of
 `execute_function` is a list of `dict` like objects.
```

### Comparing `half_orm-0.8.0rc8/half_orm.egg-info/SOURCES.txt` & `half_orm-0.8.0rc9/half_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc8/setup.py` & `half_orm-0.8.0rc9/setup.py`

 * *Files identical despite different names*

