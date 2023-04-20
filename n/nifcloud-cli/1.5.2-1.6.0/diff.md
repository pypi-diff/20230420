# Comparing `tmp/nifcloud-cli-1.5.2.tar.gz` & `tmp/nifcloud-cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifcloud-cli-1.5.2.tar", last modified: Tue Apr  4 05:14:08 2023, max compression
+gzip compressed data, was "nifcloud-cli-1.6.0.tar", last modified: Thu Apr 20 07:41:54 2023, max compression
```

## Comparing `nifcloud-cli-1.5.2.tar` & `nifcloud-cli-1.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/bin/nifcloud
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-04 05:14:08.000000 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-04 05:14:08.000000 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 05:14:08.000000 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 05:14:08.000000 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 05:14:08.000000 nifcloud-cli-1.5.2/nifcloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/clidriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/customizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/addmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/customizations/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/_retry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/cli.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/computing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/computing/3.0/
--rw-r--r--   0 runner    (1001) docker     (123)   706208 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/computing/3.0/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/computing/3.0/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/dns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/dns/2012-12-12N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/endpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/ess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/ess/2010-12-01N2014-05-28/
--rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/v1/
--rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/v1/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/v1/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/nas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/nas/N2016-02-24/
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/nas/N2016-02-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)   137372 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.857668 nifcloud-cli-1.5.2/nifcloudcli/data/script/2015-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/script/2015-09-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/service-activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/nifcloudcli/data/service-activity/2020-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/service-activity/2020-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.853668 nifcloud-cli-1.5.2/nifcloudcli/data/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/nifcloudcli/data/storage/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    90532 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/data/storage/2006-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/nifcloudcli/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/nifcloudcli/topics/topic-tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-04 05:14:08.861668 nifcloud-cli-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-04 05:13:53.000000 nifcloud-cli-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/bin/nifcloud
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/clidriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/customizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/addmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/_retry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/cli.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.496480 nifcloud-cli-1.6.0/nifcloudcli/data/computing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   753203 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.496480 nifcloud-cli-1.6.0/nifcloudcli/data/dns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/endpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/ess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/nas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/topics/topic-tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/setup.py
```

### Comparing `nifcloud-cli-1.5.2/LICENSE` & `nifcloud-cli-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/PKG-INFO` & `nifcloud-cli-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.5.2
+Version: 1.6.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nifcloud-cli-1.5.2/README.md` & `nifcloud-cli-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloud_cli.egg-info/PKG-INFO` & `nifcloud-cli-1.6.0/nifcloud_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.5.2
+Version: 1.6.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nifcloud-cli-1.5.2/nifcloud_cli.egg-info/SOURCES.txt` & `nifcloud-cli-1.6.0/nifcloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/clidriver.py` & `nifcloud-cli-1.6.0/nifcloudcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/commands.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/commands.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/addmodel.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/addmodel.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/configure.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/configure.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/get.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/get.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/list.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/list.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/configure/set.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/set.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/customizations/waiters.py` & `nifcloud-cli-1.6.0/nifcloudcli/customizations/waiters.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/_retry.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/cli.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/computing/3.0/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849738172857252%*

 * *Differences: {"'operations'": "{'CreateRemoteAccessVpnGateway': OrderedDict([('http', OrderedDict([('method', "*

 * *                 "'POST'), ('requestUri', '/api/')])), ('input', OrderedDict([('shape', "*

 * *                 "'CreateRemoteAccessVpnGatewayRequest')])), ('name', "*

 * *                 "'CreateRemoteAccessVpnGateway'), ('output', OrderedDict([('shape', "*

 * *                 "'CreateRemoteAccessVpnGatewayResult')]))]), 'CreateRemoteAccessVpnGatewayUsers': "*

 * *                 "OrderedDict([('http', OrderedDict([('method', […]*

```diff
@@ -319,14 +319,40 @@
                 "shape": "CreateNetworkInterfaceRequest"
             },
             "name": "CreateNetworkInterface",
             "output": {
                 "shape": "CreateNetworkInterfaceResult"
             }
         },
+        "CreateRemoteAccessVpnGateway": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "CreateRemoteAccessVpnGatewayRequest"
+            },
+            "name": "CreateRemoteAccessVpnGateway",
+            "output": {
+                "shape": "CreateRemoteAccessVpnGatewayResult"
+            }
+        },
+        "CreateRemoteAccessVpnGatewayUsers": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "CreateRemoteAccessVpnGatewayUsersRequest"
+            },
+            "name": "CreateRemoteAccessVpnGatewayUsers",
+            "output": {
+                "shape": "CreateRemoteAccessVpnGatewayUsersResult"
+            }
+        },
         "CreateRoute": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateRouteRequest"
@@ -527,14 +553,53 @@
                 "shape": "DeleteNetworkInterfaceRequest"
             },
             "name": "DeleteNetworkInterface",
             "output": {
                 "shape": "DeleteNetworkInterfaceResult"
             }
         },
+        "DeleteRemoteAccessVpnGateway": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DeleteRemoteAccessVpnGatewayRequest"
+            },
+            "name": "DeleteRemoteAccessVpnGateway",
+            "output": {
+                "shape": "DeleteRemoteAccessVpnGatewayResult"
+            }
+        },
+        "DeleteRemoteAccessVpnGatewayConnections": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DeleteRemoteAccessVpnGatewayConnectionsRequest"
+            },
+            "name": "DeleteRemoteAccessVpnGatewayConnections",
+            "output": {
+                "shape": "DeleteRemoteAccessVpnGatewayConnectionsResult"
+            }
+        },
+        "DeleteRemoteAccessVpnGatewayUsers": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DeleteRemoteAccessVpnGatewayUsersRequest"
+            },
+            "name": "DeleteRemoteAccessVpnGatewayUsers",
+            "output": {
+                "shape": "DeleteRemoteAccessVpnGatewayUsersResult"
+            }
+        },
         "DeleteRoute": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRouteRequest"
@@ -865,14 +930,66 @@
                 "shape": "DescribeRegionsRequest"
             },
             "name": "DescribeRegions",
             "output": {
                 "shape": "DescribeRegionsResult"
             }
         },
+        "DescribeRemoteAccessVpnGatewayActivities": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DescribeRemoteAccessVpnGatewayActivitiesRequest"
+            },
+            "name": "DescribeRemoteAccessVpnGatewayActivities",
+            "output": {
+                "shape": "DescribeRemoteAccessVpnGatewayActivitiesResult"
+            }
+        },
+        "DescribeRemoteAccessVpnGatewayClientConfig": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DescribeRemoteAccessVpnGatewayClientConfigRequest"
+            },
+            "name": "DescribeRemoteAccessVpnGatewayClientConfig",
+            "output": {
+                "shape": "DescribeRemoteAccessVpnGatewayClientConfigResult"
+            }
+        },
+        "DescribeRemoteAccessVpnGatewayConnections": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DescribeRemoteAccessVpnGatewayConnectionsRequest"
+            },
+            "name": "DescribeRemoteAccessVpnGatewayConnections",
+            "output": {
+                "shape": "DescribeRemoteAccessVpnGatewayConnectionsResult"
+            }
+        },
+        "DescribeRemoteAccessVpnGateways": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "DescribeRemoteAccessVpnGatewaysRequest"
+            },
+            "name": "DescribeRemoteAccessVpnGateways",
+            "output": {
+                "shape": "DescribeRemoteAccessVpnGatewaysResult"
+            }
+        },
         "DescribeResources": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeResourcesRequest"
@@ -1255,14 +1372,40 @@
                 "shape": "ModifyNetworkInterfaceAttributeRequest"
             },
             "name": "ModifyNetworkInterfaceAttribute",
             "output": {
                 "shape": "ModifyNetworkInterfaceAttributeResult"
             }
         },
+        "ModifyRemoteAccessVpnGatewayAttribute": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "ModifyRemoteAccessVpnGatewayAttributeRequest"
+            },
+            "name": "ModifyRemoteAccessVpnGatewayAttribute",
+            "output": {
+                "shape": "ModifyRemoteAccessVpnGatewayAttributeResult"
+            }
+        },
+        "ModifyRemoteAccessVpnGatewayUserAttribute": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "ModifyRemoteAccessVpnGatewayUserAttributeRequest"
+            },
+            "name": "ModifyRemoteAccessVpnGatewayUserAttribute",
+            "output": {
+                "shape": "ModifyRemoteAccessVpnGatewayUserAttributeResult"
+            }
+        },
         "ModifySslCertificateAttribute": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifySslCertificateAttributeRequest"
@@ -2607,14 +2750,27 @@
                 "shape": "RebootInstancesRequest"
             },
             "name": "RebootInstances",
             "output": {
                 "shape": "RebootInstancesResult"
             }
         },
+        "RebootRemoteAccessVpnGateway": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "RebootRemoteAccessVpnGatewayRequest"
+            },
+            "name": "RebootRemoteAccessVpnGateway",
+            "output": {
+                "shape": "RebootRemoteAccessVpnGatewayResult"
+            }
+        },
         "RefreshInstanceBackupRule": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RefreshInstanceBackupRuleRequest"
@@ -2698,14 +2854,27 @@
                 "shape": "ReleaseMultiIpAddressesRequest"
             },
             "name": "ReleaseMultiIpAddresses",
             "output": {
                 "shape": "ReleaseMultiIpAddressesResult"
             }
         },
+        "ReplaceRemoteAccessVpnGatewayLatestVersion": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "ReplaceRemoteAccessVpnGatewayLatestVersionRequest"
+            },
+            "name": "ReplaceRemoteAccessVpnGatewayLatestVersion",
+            "output": {
+                "shape": "ReplaceRemoteAccessVpnGatewayLatestVersionResult"
+            }
+        },
         "ReplaceRoute": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReplaceRouteRequest"
@@ -2776,14 +2945,40 @@
                 "shape": "SetLoadBalancerListenerSSLCertificateRequest"
             },
             "name": "SetLoadBalancerListenerSSLCertificate",
             "output": {
                 "shape": "SetLoadBalancerListenerSSLCertificateResultWrapper"
             }
         },
+        "SetRemoteAccessVpnGatewayCACertificate": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "SetRemoteAccessVpnGatewayCACertificateRequest"
+            },
+            "name": "SetRemoteAccessVpnGatewayCACertificate",
+            "output": {
+                "shape": "SetRemoteAccessVpnGatewayCACertificateResult"
+            }
+        },
+        "SetRemoteAccessVpnGatewaySSLCertificate": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "SetRemoteAccessVpnGatewaySSLCertificateRequest"
+            },
+            "name": "SetRemoteAccessVpnGatewaySSLCertificate",
+            "output": {
+                "shape": "SetRemoteAccessVpnGatewaySSLCertificateResult"
+            }
+        },
         "StartInstances": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "StartInstancesRequest"
@@ -2828,14 +3023,40 @@
                 "shape": "UnsetLoadBalancerListenerSSLCertificateRequest"
             },
             "name": "UnsetLoadBalancerListenerSSLCertificate",
             "output": {
                 "shape": "UnsetLoadBalancerListenerSSLCertificateResultWrapper"
             }
         },
+        "UnsetRemoteAccessVpnGatewayCACertificate": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "UnsetRemoteAccessVpnGatewayCACertificateRequest"
+            },
+            "name": "UnsetRemoteAccessVpnGatewayCACertificate",
+            "output": {
+                "shape": "UnsetRemoteAccessVpnGatewayCACertificateResult"
+            }
+        },
+        "UnsetRemoteAccessVpnGatewaySSLCertificate": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/api/"
+            },
+            "input": {
+                "shape": "UnsetRemoteAccessVpnGatewaySSLCertificateRequest"
+            },
+            "name": "UnsetRemoteAccessVpnGatewaySSLCertificate",
+            "output": {
+                "shape": "UnsetRemoteAccessVpnGatewaySSLCertificateResult"
+            }
+        },
         "UpdateLoadBalancer": {
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UpdateLoadBalancerRequest"
@@ -2953,14 +3174,22 @@
             "enum": [
                 "1",
                 "2"
             ],
             "name": "AccountingTypeOfImportInstanceRequest",
             "type": "string"
         },
+        "AccountingTypeOfModifyRemoteAccessVpnGatewayAttributeRequest": {
+            "enum": [
+                "1",
+                "2"
+            ],
+            "name": "AccountingTypeOfModifyRemoteAccessVpnGatewayAttributeRequest",
+            "type": "string"
+        },
         "AccountingTypeOfNiftyCreateElasticLoadBalancerRequest": {
             "enum": [
                 "1",
                 "2"
             ],
             "name": "AccountingTypeOfNiftyCreateElasticLoadBalancerRequest",
             "type": "string"
@@ -3493,14 +3722,44 @@
                     "locationName": "publicIpV6",
                     "shape": "String"
                 }
             },
             "name": "AssociationOfCreateNetworkInterface",
             "type": "structure"
         },
+        "AssociationOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "AllocationId": {
+                    "locationName": "allocationId",
+                    "shape": "String"
+                },
+                "AssociationId": {
+                    "locationName": "associationId",
+                    "shape": "String"
+                },
+                "IpOwnerId": {
+                    "locationName": "ipOwnerId",
+                    "shape": "String"
+                },
+                "PublicDnsName": {
+                    "locationName": "publicDnsName",
+                    "shape": "String"
+                },
+                "PublicIp": {
+                    "locationName": "publicIp",
+                    "shape": "String"
+                },
+                "PublicIpV6": {
+                    "locationName": "publicIpV6",
+                    "shape": "String"
+                }
+            },
+            "name": "AssociationOfCreateRemoteAccessVpnGateway",
+            "type": "structure"
+        },
         "AssociationOfDescribeNetworkInterfaces": {
             "members": {
                 "AllocationId": {
                     "locationName": "allocationId",
                     "shape": "String"
                 },
                 "AssociationId": {
@@ -3523,14 +3782,44 @@
                     "locationName": "publicIpV6",
                     "shape": "String"
                 }
             },
             "name": "AssociationOfDescribeNetworkInterfaces",
             "type": "structure"
         },
+        "AssociationOfDescribeRemoteAccessVpnGateways": {
+            "members": {
+                "AllocationId": {
+                    "locationName": "allocationId",
+                    "shape": "String"
+                },
+                "AssociationId": {
+                    "locationName": "associationId",
+                    "shape": "String"
+                },
+                "IpOwnerId": {
+                    "locationName": "ipOwnerId",
+                    "shape": "String"
+                },
+                "PublicDnsName": {
+                    "locationName": "publicDnsName",
+                    "shape": "String"
+                },
+                "PublicIp": {
+                    "locationName": "publicIp",
+                    "shape": "String"
+                },
+                "PublicIpV6": {
+                    "locationName": "publicIpV6",
+                    "shape": "String"
+                }
+            },
+            "name": "AssociationOfDescribeRemoteAccessVpnGateways",
+            "type": "structure"
+        },
         "AssociationOfImportInstance": {
             "members": {
                 "IpOwnerId": {
                     "locationName": "ipOwnerId",
                     "shape": "String"
                 },
                 "PublicDnsName": {
@@ -3832,14 +4121,48 @@
                     "locationName": "status",
                     "shape": "String"
                 }
             },
             "name": "AttachmentOfCreateNetworkInterface",
             "type": "structure"
         },
+        "AttachmentOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "AttachTime": {
+                    "locationName": "attachTime",
+                    "shape": "String"
+                },
+                "AttachmentId": {
+                    "locationName": "attachmentId",
+                    "shape": "String"
+                },
+                "DeleteOnTermination": {
+                    "locationName": "deleteOnTermination",
+                    "shape": "String"
+                },
+                "DeviceIndex": {
+                    "locationName": "deviceIndex",
+                    "shape": "String"
+                },
+                "InstanceId": {
+                    "locationName": "instanceId",
+                    "shape": "String"
+                },
+                "InstanceOwnerId": {
+                    "locationName": "instanceOwnerId",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                }
+            },
+            "name": "AttachmentOfCreateRemoteAccessVpnGateway",
+            "type": "structure"
+        },
         "AttachmentOfDescribeNetworkInterfaces": {
             "members": {
                 "AttachTime": {
                     "locationName": "attachTime",
                     "shape": "String"
                 },
                 "AttachmentId": {
@@ -3866,14 +4189,48 @@
                     "locationName": "status",
                     "shape": "String"
                 }
             },
             "name": "AttachmentOfDescribeNetworkInterfaces",
             "type": "structure"
         },
+        "AttachmentOfDescribeRemoteAccessVpnGateways": {
+            "members": {
+                "AttachTime": {
+                    "locationName": "attachTime",
+                    "shape": "String"
+                },
+                "AttachmentId": {
+                    "locationName": "attachmentId",
+                    "shape": "String"
+                },
+                "DeleteOnTermination": {
+                    "locationName": "deleteOnTermination",
+                    "shape": "String"
+                },
+                "DeviceIndex": {
+                    "locationName": "deviceIndex",
+                    "shape": "String"
+                },
+                "InstanceId": {
+                    "locationName": "instanceId",
+                    "shape": "String"
+                },
+                "InstanceOwnerId": {
+                    "locationName": "instanceOwnerId",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                }
+            },
+            "name": "AttachmentOfDescribeRemoteAccessVpnGateways",
+            "type": "structure"
+        },
         "AttachmentOfImportInstance": {
             "members": {
                 "AttachTime": {
                     "locationName": "attachTime",
                     "shape": "String"
                 },
                 "AttachmentID": {
@@ -4098,14 +4455,24 @@
                 "bypassInterface.NetworkName",
                 "option-nameServer",
                 "description"
             ],
             "name": "AttributeOfNiftyModifyWebProxyAttributeRequest",
             "type": "string"
         },
+        "AuthTypeSet": {
+            "members": {
+                "AuthType": {
+                    "locationName": "authType",
+                    "shape": "String"
+                }
+            },
+            "name": "AuthTypeSet",
+            "type": "structure"
+        },
         "AuthorizeSecurityGroupIngressRequest": {
             "members": {
                 "GroupName": {
                     "locationName": "GroupName",
                     "shape": "String"
                 },
                 "IpPermissions": {
@@ -4611,14 +4978,24 @@
                     "locationName": "chargeDetail",
                     "shape": "ChargeDetail"
                 }
             },
             "name": "ChargeDetailInfo",
             "type": "structure"
         },
+        "CipherSuiteSet": {
+            "members": {
+                "CipherSuite": {
+                    "locationName": "cipherSuite",
+                    "shape": "String"
+                }
+            },
+            "name": "CipherSuiteSet",
+            "type": "structure"
+        },
         "ClearLoadBalancerSessionRequest": {
             "members": {
                 "InstancePort": {
                     "locationName": "InstancePort",
                     "shape": "Integer"
                 },
                 "LoadBalancerName": {
@@ -4648,14 +5025,22 @@
                     "locationName": "ResponseMetadata",
                     "shape": "ResponseMetadata"
                 }
             },
             "name": "ClearLoadBalancerSessionResultWrapper",
             "type": "structure"
         },
+        "ClientTunnelModeOfModifyRemoteAccessVpnGatewayAttributeRequest": {
+            "enum": [
+                "split",
+                "full"
+            ],
+            "name": "ClientTunnelModeOfModifyRemoteAccessVpnGatewayAttributeRequest",
+            "type": "string"
+        },
         "ConfigureHealthCheckRequest": {
             "members": {
                 "HealthCheck": {
                     "locationName": "HealthCheck",
                     "shape": "RequestHealthCheck"
                 },
                 "InstancePort": {
@@ -4700,14 +5085,40 @@
                     "locationName": "ResponseMetadata",
                     "shape": "ResponseMetadata"
                 }
             },
             "name": "ConfigureHealthCheckResultWrapper",
             "type": "structure"
         },
+        "ConnectionSet": {
+            "members": {
+                "AssignedIpAddress": {
+                    "locationName": "assignedIpAddress",
+                    "shape": "String"
+                },
+                "ClientIpAddress": {
+                    "locationName": "clientIpAddress",
+                    "shape": "String"
+                },
+                "ConnectionId": {
+                    "locationName": "connectionId",
+                    "shape": "String"
+                },
+                "RemoteUserName": {
+                    "locationName": "remoteUserName",
+                    "shape": "String"
+                },
+                "StartTime": {
+                    "locationName": "startTime",
+                    "shape": "String"
+                }
+            },
+            "name": "ConnectionSet",
+            "type": "structure"
+        },
         "ConversionTask": {
             "members": {
                 "ConversionTaskId": {
                     "locationName": "conversionTaskId",
                     "shape": "String"
                 },
                 "ExpirationTime": {
@@ -5314,14 +5725,128 @@
                     "locationName": "return",
                     "shape": "Boolean"
                 }
             },
             "name": "CreateNetworkInterfaceResult",
             "type": "structure"
         },
+        "CreateRemoteAccessVpnGatewayRequest": {
+            "members": {
+                "AccountingType": {
+                    "locationName": "AccountingType",
+                    "shape": "Integer"
+                },
+                "CACertificateId": {
+                    "locationName": "CACertificateId",
+                    "shape": "String"
+                },
+                "CipherSuite": {
+                    "locationName": "CipherSuite",
+                    "shape": "ListOfRequestCipherSuite"
+                },
+                "Description": {
+                    "locationName": "Description",
+                    "shape": "String"
+                },
+                "NetworkInterface": {
+                    "locationName": "NetworkInterface",
+                    "shape": "ListOfRequestNetworkInterfaceOfCreateRemoteAccessVpnGateway"
+                },
+                "Placement": {
+                    "locationName": "Placement",
+                    "shape": "RequestPlacementOfCreateRemoteAccessVpnGateway"
+                },
+                "PoolNetworkCidr": {
+                    "locationName": "PoolNetworkCidr",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "RemoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayType": {
+                    "locationName": "RemoteAccessVpnGatewayType",
+                    "shape": "RemoteAccessVpnGatewayTypeOfCreateRemoteAccessVpnGatewayRequest"
+                },
+                "SSLCertificateId": {
+                    "locationName": "SSLCertificateId",
+                    "shape": "String"
+                }
+            },
+            "name": "CreateRemoteAccessVpnGatewayRequest",
+            "required": [
+                "CipherSuite",
+                "NetworkInterface",
+                "PoolNetworkCidr",
+                "SSLCertificateId"
+            ],
+            "type": "structure"
+        },
+        "CreateRemoteAccessVpnGatewayResult": {
+            "members": {
+                "RemoteAccessVpnGateway": {
+                    "locationName": "remoteAccessVpnGateway",
+                    "shape": "RemoteAccessVpnGateway"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "CreateRemoteAccessVpnGatewayResult",
+            "type": "structure"
+        },
+        "CreateRemoteAccessVpnGatewayUsersRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteUser": {
+                    "locationName": "RemoteUser",
+                    "shape": "ListOfRequestRemoteUser"
+                }
+            },
+            "name": "CreateRemoteAccessVpnGatewayUsersRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId",
+                "RemoteUser"
+            ],
+            "type": "structure"
+        },
+        "CreateRemoteAccessVpnGatewayUsersResult": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "remoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "remoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RemoteUserSet": {
+                    "locationName": "remoteUserSet",
+                    "shape": "ListOfRemoteUserSet"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "CreateRemoteAccessVpnGatewayUsersResult",
+            "type": "structure"
+        },
         "CreateRouteRequest": {
             "members": {
                 "DestinationCidrBlock": {
                     "locationName": "DestinationCidrBlock",
                     "shape": "String"
                 },
                 "GatewayId": {
@@ -6143,14 +6668,105 @@
                     "locationName": "return",
                     "shape": "Boolean"
                 }
             },
             "name": "DeleteNetworkInterfaceResult",
             "type": "structure"
         },
+        "DeleteRemoteAccessVpnGatewayConnectionsRequest": {
+            "members": {
+                "Connection": {
+                    "locationName": "Connection",
+                    "shape": "ListOfRequestConnection"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayConnectionsRequest",
+            "required": [
+                "Connection",
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "DeleteRemoteAccessVpnGatewayConnectionsResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayConnectionsResult",
+            "type": "structure"
+        },
+        "DeleteRemoteAccessVpnGatewayRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "DeleteRemoteAccessVpnGatewayResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayResult",
+            "type": "structure"
+        },
+        "DeleteRemoteAccessVpnGatewayUsersRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteUser": {
+                    "locationName": "RemoteUser",
+                    "shape": "ListOfRequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayUsersRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId",
+                "RemoteUser"
+            ],
+            "type": "structure"
+        },
+        "DeleteRemoteAccessVpnGatewayUsersResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "DeleteRemoteAccessVpnGatewayUsersResult",
+            "type": "structure"
+        },
         "DeleteRouteRequest": {
             "members": {
                 "DestinationCidrBlock": {
                     "locationName": "DestinationCidrBlock",
                     "shape": "String"
                 },
                 "RouteTableId": {
@@ -7030,14 +7646,139 @@
                     "locationName": "requestId",
                     "shape": "String"
                 }
             },
             "name": "DescribeRegionsResult",
             "type": "structure"
         },
+        "DescribeRemoteAccessVpnGatewayActivitiesRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayActivitiesRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewayActivitiesResult": {
+            "members": {
+                "Log": {
+                    "locationName": "log",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "remoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "remoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayActivitiesResult",
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewayClientConfigRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayClientConfigRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewayClientConfigResult": {
+            "members": {
+                "Encoding": {
+                    "locationName": "encoding",
+                    "shape": "String"
+                },
+                "FileData": {
+                    "locationName": "fileData",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayClientConfigResult",
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewayConnectionsRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayConnectionsRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewayConnectionsResult": {
+            "members": {
+                "RemoteAccessVpnGatewayConnection": {
+                    "locationName": "remoteAccessVpnGatewayConnection",
+                    "shape": "RemoteAccessVpnGatewayConnection"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "remoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "remoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewayConnectionsResult",
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewaysRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "ListOfRequestRemoteAccessVpnGatewayId"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewaysRequest",
+            "type": "structure"
+        },
+        "DescribeRemoteAccessVpnGatewaysResult": {
+            "members": {
+                "RemoteAccessVpnGatewaySet": {
+                    "locationName": "remoteAccessVpnGatewaySet",
+                    "shape": "ListOfRemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways"
+                },
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                }
+            },
+            "name": "DescribeRemoteAccessVpnGatewaysResult",
+            "type": "structure"
+        },
         "DescribeResourcesRequest": {
             "members": {},
             "name": "DescribeResourcesRequest",
             "type": "structure"
         },
         "DescribeResourcesResult": {
             "members": {
@@ -11614,14 +12355,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "AttachmentSet"
             },
             "name": "ListOfAttachmentSet",
             "type": "list"
         },
+        "ListOfAuthTypeSet": {
+            "member": {
+                "locationName": "item",
+                "shape": "AuthTypeSet"
+            },
+            "name": "ListOfAuthTypeSet",
+            "type": "list"
+        },
         "ListOfAutoScalingReservationSet": {
             "member": {
                 "locationName": "item",
                 "shape": "AutoScalingReservationSet"
             },
             "name": "ListOfAutoScalingReservationSet",
             "type": "list"
@@ -11678,14 +12427,30 @@
             "member": {
                 "locationName": "item",
                 "shape": "CertsSet"
             },
             "name": "ListOfCertsSet",
             "type": "list"
         },
+        "ListOfCipherSuiteSet": {
+            "member": {
+                "locationName": "item",
+                "shape": "CipherSuiteSet"
+            },
+            "name": "ListOfCipherSuiteSet",
+            "type": "list"
+        },
+        "ListOfConnectionSet": {
+            "member": {
+                "locationName": "item",
+                "shape": "ConnectionSet"
+            },
+            "name": "ListOfConnectionSet",
+            "type": "list"
+        },
         "ListOfCopyInstanceSet": {
             "member": {
                 "locationName": "item",
                 "shape": "CopyInstanceSet"
             },
             "name": "ListOfCopyInstanceSet",
             "type": "list"
@@ -12366,14 +13131,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "NetworkInterfaceSetOfCopyFromBackupInstance"
             },
             "name": "ListOfNetworkInterfaceSetOfCopyFromBackupInstance",
             "type": "list"
         },
+        "ListOfNetworkInterfaceSetOfCreateRemoteAccessVpnGateway": {
+            "member": {
+                "locationName": "item",
+                "shape": "NetworkInterfaceSetOfCreateRemoteAccessVpnGateway"
+            },
+            "name": "ListOfNetworkInterfaceSetOfCreateRemoteAccessVpnGateway",
+            "type": "list"
+        },
         "ListOfNetworkInterfaceSetOfCreateVpnGateway": {
             "member": {
                 "locationName": "item",
                 "shape": "NetworkInterfaceSetOfCreateVpnGateway"
             },
             "name": "ListOfNetworkInterfaceSetOfCreateVpnGateway",
             "type": "list"
@@ -12390,14 +13163,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "NetworkInterfaceSetOfDescribeNetworkInterfaces"
             },
             "name": "ListOfNetworkInterfaceSetOfDescribeNetworkInterfaces",
             "type": "list"
         },
+        "ListOfNetworkInterfaceSetOfDescribeRemoteAccessVpnGateways": {
+            "member": {
+                "locationName": "item",
+                "shape": "NetworkInterfaceSetOfDescribeRemoteAccessVpnGateways"
+            },
+            "name": "ListOfNetworkInterfaceSetOfDescribeRemoteAccessVpnGateways",
+            "type": "list"
+        },
         "ListOfNetworkInterfaceSetOfDescribeVpnGateways": {
             "member": {
                 "locationName": "item",
                 "shape": "NetworkInterfaceSetOfDescribeVpnGateways"
             },
             "name": "ListOfNetworkInterfaceSetOfDescribeVpnGateways",
             "type": "list"
@@ -12662,14 +13443,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "RemoteAccessVpnGatewaySet"
             },
             "name": "ListOfRemoteAccessVpnGatewaySet",
             "type": "list"
         },
+        "ListOfRemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways": {
+            "member": {
+                "locationName": "item",
+                "shape": "RemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways"
+            },
+            "name": "ListOfRemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways",
+            "type": "list"
+        },
         "ListOfRemoteAccessVpnGatewaySetOfNiftyCreatePrivateLan": {
             "member": {
                 "locationName": "item",
                 "shape": "RemoteAccessVpnGatewaySetOfNiftyCreatePrivateLan"
             },
             "name": "ListOfRemoteAccessVpnGatewaySetOfNiftyCreatePrivateLan",
             "type": "list"
@@ -12678,14 +13467,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "RemoteAccessVpnGatewaySetOfNiftyDescribePrivateLans"
             },
             "name": "ListOfRemoteAccessVpnGatewaySetOfNiftyDescribePrivateLans",
             "type": "list"
         },
+        "ListOfRemoteUserSet": {
+            "member": {
+                "locationName": "item",
+                "shape": "RemoteUserSet"
+            },
+            "name": "ListOfRemoteUserSet",
+            "type": "list"
+        },
         "ListOfRequestAccountingType": {
             "member": {
                 "shape": "String"
             },
             "name": "ListOfRequestAccountingType",
             "type": "list"
         },
@@ -12729,14 +13526,28 @@
         "ListOfRequestBlockDeviceMapping": {
             "member": {
                 "shape": "RequestBlockDeviceMapping"
             },
             "name": "ListOfRequestBlockDeviceMapping",
             "type": "list"
         },
+        "ListOfRequestCipherSuite": {
+            "member": {
+                "shape": "String"
+            },
+            "name": "ListOfRequestCipherSuite",
+            "type": "list"
+        },
+        "ListOfRequestConnection": {
+            "member": {
+                "shape": "RequestConnection"
+            },
+            "name": "ListOfRequestConnection",
+            "type": "list"
+        },
         "ListOfRequestConversionTaskId": {
             "member": {
                 "shape": "String"
             },
             "name": "ListOfRequestConversionTaskId",
             "type": "list"
         },
@@ -13253,14 +14064,21 @@
         "ListOfRequestNetworkInterfaceOfCopyFromBackupInstance": {
             "member": {
                 "shape": "RequestNetworkInterfaceOfCopyFromBackupInstance"
             },
             "name": "ListOfRequestNetworkInterfaceOfCopyFromBackupInstance",
             "type": "list"
         },
+        "ListOfRequestNetworkInterfaceOfCreateRemoteAccessVpnGateway": {
+            "member": {
+                "shape": "RequestNetworkInterfaceOfCreateRemoteAccessVpnGateway"
+            },
+            "name": "ListOfRequestNetworkInterfaceOfCreateRemoteAccessVpnGateway",
+            "type": "list"
+        },
         "ListOfRequestNetworkInterfaceOfNiftyCreateElasticLoadBalancer": {
             "member": {
                 "shape": "RequestNetworkInterfaceOfNiftyCreateElasticLoadBalancer"
             },
             "name": "ListOfRequestNetworkInterfaceOfNiftyCreateElasticLoadBalancer",
             "type": "list"
         },
@@ -13344,14 +14162,35 @@
         "ListOfRequestRegionName": {
             "member": {
                 "shape": "String"
             },
             "name": "ListOfRequestRegionName",
             "type": "list"
         },
+        "ListOfRequestRemoteAccessVpnGatewayId": {
+            "member": {
+                "shape": "String"
+            },
+            "name": "ListOfRequestRemoteAccessVpnGatewayId",
+            "type": "list"
+        },
+        "ListOfRequestRemoteUser": {
+            "member": {
+                "shape": "RequestRemoteUser"
+            },
+            "name": "ListOfRequestRemoteUser",
+            "type": "list"
+        },
+        "ListOfRequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers": {
+            "member": {
+                "shape": "RequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers"
+            },
+            "name": "ListOfRequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers",
+            "type": "list"
+        },
         "ListOfRequestRemove": {
             "member": {
                 "shape": "RequestRemove"
             },
             "name": "ListOfRequestRemove",
             "type": "list"
         },
@@ -14573,14 +15412,101 @@
                     "locationName": "return",
                     "shape": "Boolean"
                 }
             },
             "name": "ModifyNetworkInterfaceAttributeResult",
             "type": "structure"
         },
+        "ModifyRemoteAccessVpnGatewayAttributeRequest": {
+            "members": {
+                "AccountingType": {
+                    "locationName": "AccountingType",
+                    "shape": "AccountingTypeOfModifyRemoteAccessVpnGatewayAttributeRequest"
+                },
+                "ClientTunnelMode": {
+                    "locationName": "ClientTunnelMode",
+                    "shape": "ClientTunnelModeOfModifyRemoteAccessVpnGatewayAttributeRequest"
+                },
+                "Description": {
+                    "locationName": "Description",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "RemoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayType": {
+                    "locationName": "RemoteAccessVpnGatewayType",
+                    "shape": "RemoteAccessVpnGatewayTypeOfModifyRemoteAccessVpnGatewayAttributeRequest"
+                }
+            },
+            "name": "ModifyRemoteAccessVpnGatewayAttributeRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "ModifyRemoteAccessVpnGatewayAttributeResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "ModifyRemoteAccessVpnGatewayAttributeResult",
+            "type": "structure"
+        },
+        "ModifyRemoteAccessVpnGatewayUserAttributeRequest": {
+            "members": {
+                "Description": {
+                    "locationName": "Description",
+                    "shape": "String"
+                },
+                "Password": {
+                    "locationName": "Password",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "UserName": {
+                    "locationName": "UserName",
+                    "shape": "String"
+                }
+            },
+            "name": "ModifyRemoteAccessVpnGatewayUserAttributeRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId",
+                "UserName"
+            ],
+            "type": "structure"
+        },
+        "ModifyRemoteAccessVpnGatewayUserAttributeResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "ModifyRemoteAccessVpnGatewayUserAttributeResult",
+            "type": "structure"
+        },
         "ModifySslCertificateAttributeRequest": {
             "members": {
                 "Description": {
                     "locationName": "Description",
                     "shape": "RequestDescription"
                 },
                 "FqdnId": {
@@ -15572,14 +16498,112 @@
                     "locationName": "vpcId",
                     "shape": "String"
                 }
             },
             "name": "NetworkInterfaceSetOfCopyFromBackupInstance",
             "type": "structure"
         },
+        "NetworkInterfaceSetOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "Association": {
+                    "locationName": "association",
+                    "shape": "AssociationOfCreateRemoteAccessVpnGateway"
+                },
+                "Attachment": {
+                    "locationName": "attachment",
+                    "shape": "AttachmentOfCreateRemoteAccessVpnGateway"
+                },
+                "AvailabilityZone": {
+                    "locationName": "availabilityZone",
+                    "shape": "String"
+                },
+                "Description": {
+                    "locationName": "description",
+                    "shape": "String"
+                },
+                "GroupSet": {
+                    "locationName": "groupSet",
+                    "shape": "String"
+                },
+                "InterfaceType": {
+                    "locationName": "interfaceType",
+                    "shape": "String"
+                },
+                "Ipv6AddressesSet": {
+                    "locationName": "ipv6AddressesSet",
+                    "shape": "String"
+                },
+                "MacAddress": {
+                    "locationName": "macAddress",
+                    "shape": "String"
+                },
+                "NetworkInterfaceId": {
+                    "locationName": "networkInterfaceId",
+                    "shape": "String"
+                },
+                "NiftyNetworkId": {
+                    "locationName": "niftyNetworkId",
+                    "shape": "String"
+                },
+                "NiftyNetworkName": {
+                    "locationName": "niftyNetworkName",
+                    "shape": "String"
+                },
+                "OwnerId": {
+                    "locationName": "ownerId",
+                    "shape": "String"
+                },
+                "PrivateDnsName": {
+                    "locationName": "privateDnsName",
+                    "shape": "String"
+                },
+                "PrivateIpAddress": {
+                    "locationName": "privateIpAddress",
+                    "shape": "String"
+                },
+                "PrivateIpAddressV6": {
+                    "locationName": "privateIpAddressV6",
+                    "shape": "String"
+                },
+                "PrivateIpAddressesSet": {
+                    "locationName": "privateIpAddressesSet",
+                    "shape": "String"
+                },
+                "RequesterId": {
+                    "locationName": "requesterId",
+                    "shape": "String"
+                },
+                "RequesterManaged": {
+                    "locationName": "requesterManaged",
+                    "shape": "String"
+                },
+                "SourceDestCheck": {
+                    "locationName": "sourceDestCheck",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                },
+                "SubnetId": {
+                    "locationName": "subnetId",
+                    "shape": "String"
+                },
+                "TagSet": {
+                    "locationName": "tagSet",
+                    "shape": "String"
+                },
+                "VpcId": {
+                    "locationName": "vpcId",
+                    "shape": "String"
+                }
+            },
+            "name": "NetworkInterfaceSetOfCreateRemoteAccessVpnGateway",
+            "type": "structure"
+        },
         "NetworkInterfaceSetOfCreateVpnGateway": {
             "members": {
                 "IpAddress": {
                     "locationName": "ipAddress",
                     "shape": "String"
                 },
                 "NetworkId": {
@@ -15766,14 +16790,112 @@
                     "locationName": "vpcId",
                     "shape": "String"
                 }
             },
             "name": "NetworkInterfaceSetOfDescribeNetworkInterfaces",
             "type": "structure"
         },
+        "NetworkInterfaceSetOfDescribeRemoteAccessVpnGateways": {
+            "members": {
+                "Association": {
+                    "locationName": "association",
+                    "shape": "AssociationOfDescribeRemoteAccessVpnGateways"
+                },
+                "Attachment": {
+                    "locationName": "attachment",
+                    "shape": "AttachmentOfDescribeRemoteAccessVpnGateways"
+                },
+                "AvailabilityZone": {
+                    "locationName": "availabilityZone",
+                    "shape": "String"
+                },
+                "Description": {
+                    "locationName": "description",
+                    "shape": "String"
+                },
+                "GroupSet": {
+                    "locationName": "groupSet",
+                    "shape": "String"
+                },
+                "InterfaceType": {
+                    "locationName": "interfaceType",
+                    "shape": "String"
+                },
+                "Ipv6AddressesSet": {
+                    "locationName": "ipv6AddressesSet",
+                    "shape": "String"
+                },
+                "MacAddress": {
+                    "locationName": "macAddress",
+                    "shape": "String"
+                },
+                "NetworkInterfaceId": {
+                    "locationName": "networkInterfaceId",
+                    "shape": "String"
+                },
+                "NiftyNetworkId": {
+                    "locationName": "niftyNetworkId",
+                    "shape": "String"
+                },
+                "NiftyNetworkName": {
+                    "locationName": "niftyNetworkName",
+                    "shape": "String"
+                },
+                "OwnerId": {
+                    "locationName": "ownerId",
+                    "shape": "String"
+                },
+                "PrivateDnsName": {
+                    "locationName": "privateDnsName",
+                    "shape": "String"
+                },
+                "PrivateIpAddress": {
+                    "locationName": "privateIpAddress",
+                    "shape": "String"
+                },
+                "PrivateIpAddressV6": {
+                    "locationName": "privateIpAddressV6",
+                    "shape": "String"
+                },
+                "PrivateIpAddressesSet": {
+                    "locationName": "privateIpAddressesSet",
+                    "shape": "String"
+                },
+                "RequesterId": {
+                    "locationName": "requesterId",
+                    "shape": "String"
+                },
+                "RequesterManaged": {
+                    "locationName": "requesterManaged",
+                    "shape": "String"
+                },
+                "SourceDestCheck": {
+                    "locationName": "sourceDestCheck",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                },
+                "SubnetId": {
+                    "locationName": "subnetId",
+                    "shape": "String"
+                },
+                "TagSet": {
+                    "locationName": "tagSet",
+                    "shape": "String"
+                },
+                "VpcId": {
+                    "locationName": "vpcId",
+                    "shape": "String"
+                }
+            },
+            "name": "NetworkInterfaceSetOfDescribeRemoteAccessVpnGateways",
+            "type": "structure"
+        },
         "NetworkInterfaceSetOfDescribeVpnGateways": {
             "members": {
                 "CidrBlock": {
                     "locationName": "cidrBlock",
                     "shape": "String"
                 },
                 "Descriprion": {
@@ -18947,14 +20069,22 @@
             "enum": [
                 "force",
                 "true"
             ],
             "name": "NiftyRebootOfNiftyUpdateVpnGatewayNetworkInterfacesRequest",
             "type": "string"
         },
+        "NiftyRebootOfRebootRemoteAccessVpnGatewayRequest": {
+            "enum": [
+                "force",
+                "true"
+            ],
+            "name": "NiftyRebootOfRebootRemoteAccessVpnGatewayRequest",
+            "type": "string"
+        },
         "NiftyRebootOfRouterForNiftyRebootRouters": {
             "enum": [
                 "force",
                 "true"
             ],
             "name": "NiftyRebootOfRouterForNiftyRebootRouters",
             "type": "string"
@@ -21189,14 +22319,45 @@
                     "locationName": "return",
                     "shape": "Boolean"
                 }
             },
             "name": "RebootInstancesResult",
             "type": "structure"
         },
+        "RebootRemoteAccessVpnGatewayRequest": {
+            "members": {
+                "NiftyReboot": {
+                    "locationName": "NiftyReboot",
+                    "shape": "NiftyRebootOfRebootRemoteAccessVpnGatewayRequest"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "RebootRemoteAccessVpnGatewayRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "RebootRemoteAccessVpnGatewayResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "RebootRemoteAccessVpnGatewayResult",
+            "type": "structure"
+        },
         "RefreshInstanceBackupRuleRequest": {
             "members": {
                 "InstanceBackupRuleId": {
                     "locationName": "InstanceBackupRuleId",
                     "shape": "String"
                 }
             },
@@ -21620,14 +22781,130 @@
                     "locationName": "return",
                     "shape": "Boolean"
                 }
             },
             "name": "ReleaseMultiIpAddressesResult",
             "type": "structure"
         },
+        "RemoteAccessVpnGateway": {
+            "members": {
+                "AccountingType": {
+                    "locationName": "accountingType",
+                    "shape": "String"
+                },
+                "AuthTypeSet": {
+                    "locationName": "authTypeSet",
+                    "shape": "ListOfAuthTypeSet"
+                },
+                "AvailabilityZone": {
+                    "locationName": "availabilityZone",
+                    "shape": "String"
+                },
+                "CaCertificateId": {
+                    "locationName": "caCertificateId",
+                    "shape": "String"
+                },
+                "CipherSuiteSet": {
+                    "locationName": "cipherSuiteSet",
+                    "shape": "ListOfCipherSuiteSet"
+                },
+                "ClientDownloadEndpoint": {
+                    "locationName": "clientDownloadEndpoint",
+                    "shape": "String"
+                },
+                "ClientTunnelMode": {
+                    "locationName": "clientTunnelMode",
+                    "shape": "String"
+                },
+                "CreatedTime": {
+                    "locationName": "createdTime",
+                    "shape": "String"
+                },
+                "Description": {
+                    "locationName": "description",
+                    "shape": "String"
+                },
+                "GroupSet": {
+                    "locationName": "groupSet",
+                    "shape": "String"
+                },
+                "IsConfiguredNat": {
+                    "locationName": "isConfiguredNat",
+                    "shape": "String"
+                },
+                "NetworkInterfaceSet": {
+                    "locationName": "networkInterfaceSet",
+                    "shape": "ListOfNetworkInterfaceSetOfCreateRemoteAccessVpnGateway"
+                },
+                "NextMonthAccountingType": {
+                    "locationName": "nextMonthAccountingType",
+                    "shape": "String"
+                },
+                "PoolNetworkCidr": {
+                    "locationName": "poolNetworkCidr",
+                    "shape": "String"
+                },
+                "PoolNetworkGatewayIpAddress": {
+                    "locationName": "poolNetworkGatewayIpAddress",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "remoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "remoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayType": {
+                    "locationName": "remoteAccessVpnGatewayType",
+                    "shape": "String"
+                },
+                "RemoteUserSet": {
+                    "locationName": "remoteUserSet",
+                    "shape": "String"
+                },
+                "RouteTableAssociationId": {
+                    "locationName": "routeTableAssociationId",
+                    "shape": "String"
+                },
+                "RouteTableId": {
+                    "locationName": "routeTableId",
+                    "shape": "String"
+                },
+                "SslCertificateId": {
+                    "locationName": "sslCertificateId",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                },
+                "VersionInformation": {
+                    "locationName": "versionInformation",
+                    "shape": "VersionInformationOfCreateRemoteAccessVpnGateway"
+                }
+            },
+            "name": "RemoteAccessVpnGateway",
+            "type": "structure"
+        },
+        "RemoteAccessVpnGatewayConnection": {
+            "members": {
+                "ConnectionCount": {
+                    "locationName": "connectionCount",
+                    "shape": "Integer"
+                },
+                "ConnectionSet": {
+                    "locationName": "connectionSet",
+                    "shape": "ListOfConnectionSet"
+                }
+            },
+            "name": "RemoteAccessVpnGatewayConnection",
+            "type": "structure"
+        },
         "RemoteAccessVpnGatewayInfo": {
             "members": {
                 "RemoteAccessVpnGatewayMeasuredRateSet": {
                     "locationName": "remoteAccessVpnGatewayMeasuredRateSet",
                     "shape": "ListOfRemoteAccessVpnGatewayMeasuredRateSet"
                 },
                 "RemoteAccessVpnGatewayMonthlyRateSet": {
@@ -21692,14 +22969,116 @@
                     "locationName": "type",
                     "shape": "String"
                 }
             },
             "name": "RemoteAccessVpnGatewaySet",
             "type": "structure"
         },
+        "RemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways": {
+            "members": {
+                "AccountingType": {
+                    "locationName": "accountingType",
+                    "shape": "String"
+                },
+                "AuthTypeSet": {
+                    "locationName": "authTypeSet",
+                    "shape": "ListOfAuthTypeSet"
+                },
+                "AvailabilityZone": {
+                    "locationName": "availabilityZone",
+                    "shape": "String"
+                },
+                "CaCertificateId": {
+                    "locationName": "caCertificateId",
+                    "shape": "String"
+                },
+                "CipherSuiteSet": {
+                    "locationName": "cipherSuiteSet",
+                    "shape": "ListOfCipherSuiteSet"
+                },
+                "ClientDownloadEndpoint": {
+                    "locationName": "clientDownloadEndpoint",
+                    "shape": "String"
+                },
+                "ClientTunnelMode": {
+                    "locationName": "clientTunnelMode",
+                    "shape": "String"
+                },
+                "CreatedTime": {
+                    "locationName": "createdTime",
+                    "shape": "String"
+                },
+                "Description": {
+                    "locationName": "description",
+                    "shape": "String"
+                },
+                "GroupSet": {
+                    "locationName": "groupSet",
+                    "shape": "String"
+                },
+                "IsConfiguredNat": {
+                    "locationName": "isConfiguredNat",
+                    "shape": "String"
+                },
+                "NetworkInterfaceSet": {
+                    "locationName": "networkInterfaceSet",
+                    "shape": "ListOfNetworkInterfaceSetOfDescribeRemoteAccessVpnGateways"
+                },
+                "NextMonthAccountingType": {
+                    "locationName": "nextMonthAccountingType",
+                    "shape": "String"
+                },
+                "PoolNetworkCidr": {
+                    "locationName": "poolNetworkCidr",
+                    "shape": "String"
+                },
+                "PoolNetworkGatewayIpAddress": {
+                    "locationName": "poolNetworkGatewayIpAddress",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "remoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayName": {
+                    "locationName": "remoteAccessVpnGatewayName",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayType": {
+                    "locationName": "remoteAccessVpnGatewayType",
+                    "shape": "String"
+                },
+                "RemoteUserSet": {
+                    "locationName": "remoteUserSet",
+                    "shape": "ListOfRemoteUserSet"
+                },
+                "RouteTableAssociationId": {
+                    "locationName": "routeTableAssociationId",
+                    "shape": "String"
+                },
+                "RouteTableId": {
+                    "locationName": "routeTableId",
+                    "shape": "String"
+                },
+                "SslCertificateId": {
+                    "locationName": "sslCertificateId",
+                    "shape": "String"
+                },
+                "Status": {
+                    "locationName": "status",
+                    "shape": "String"
+                },
+                "VersionInformation": {
+                    "locationName": "versionInformation",
+                    "shape": "VersionInformationOfDescribeRemoteAccessVpnGateways"
+                }
+            },
+            "name": "RemoteAccessVpnGatewaySetOfDescribeRemoteAccessVpnGateways",
+            "type": "structure"
+        },
         "RemoteAccessVpnGatewaySetOfNiftyCreatePrivateLan": {
             "members": {
                 "DeviceIndex": {
                     "locationName": "deviceIndex",
                     "shape": "String"
                 },
                 "IpAddress": {
@@ -21736,14 +23115,73 @@
                     "locationName": "remoteAccessVpnGatewayName",
                     "shape": "String"
                 }
             },
             "name": "RemoteAccessVpnGatewaySetOfNiftyDescribePrivateLans",
             "type": "structure"
         },
+        "RemoteAccessVpnGatewayTypeOfCreateRemoteAccessVpnGatewayRequest": {
+            "enum": [
+                "small",
+                "medium",
+                "large"
+            ],
+            "name": "RemoteAccessVpnGatewayTypeOfCreateRemoteAccessVpnGatewayRequest",
+            "type": "string"
+        },
+        "RemoteAccessVpnGatewayTypeOfModifyRemoteAccessVpnGatewayAttributeRequest": {
+            "enum": [
+                "small",
+                "medium",
+                "large"
+            ],
+            "name": "RemoteAccessVpnGatewayTypeOfModifyRemoteAccessVpnGatewayAttributeRequest",
+            "type": "string"
+        },
+        "RemoteUserSet": {
+            "members": {
+                "Description": {
+                    "locationName": "description",
+                    "shape": "String"
+                },
+                "UserName": {
+                    "locationName": "userName",
+                    "shape": "String"
+                }
+            },
+            "name": "RemoteUserSet",
+            "type": "structure"
+        },
+        "ReplaceRemoteAccessVpnGatewayLatestVersionRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "ReplaceRemoteAccessVpnGatewayLatestVersionRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "ReplaceRemoteAccessVpnGatewayLatestVersionResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "ReplaceRemoteAccessVpnGatewayLatestVersionResult",
+            "type": "structure"
+        },
         "ReplaceRouteRequest": {
             "members": {
                 "DestinationCidrBlock": {
                     "locationName": "DestinationCidrBlock",
                     "shape": "String"
                 },
                 "GatewayId": {
@@ -21922,14 +23360,27 @@
                     "locationName": "StateName",
                     "shape": "String"
                 }
             },
             "name": "RequestCertInfo",
             "type": "structure"
         },
+        "RequestConnection": {
+            "members": {
+                "ConnectionId": {
+                    "locationName": "ConnectionId",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestConnection",
+            "required": [
+                "ConnectionId"
+            ],
+            "type": "structure"
+        },
         "RequestCopyInstance": {
             "members": {
                 "AccountingType": {
                     "locationName": "AccountingType",
                     "shape": "AccountingTypeOfCopyInstanceForCopyInstances"
                 },
                 "InstanceName": {
@@ -23073,14 +24524,32 @@
                     "locationName": "NetworkName",
                     "shape": "String"
                 }
             },
             "name": "RequestNetworkInterfaceOfCopyFromBackupInstance",
             "type": "structure"
         },
+        "RequestNetworkInterfaceOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "IpAddress": {
+                    "locationName": "IpAddress",
+                    "shape": "String"
+                },
+                "NetworkId": {
+                    "locationName": "NetworkId",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestNetworkInterfaceOfCreateRemoteAccessVpnGateway",
+            "required": [
+                "IpAddress",
+                "NetworkId"
+            ],
+            "type": "structure"
+        },
         "RequestNetworkInterfaceOfNiftyCreateElasticLoadBalancer": {
             "members": {
                 "IpAddress": {
                     "locationName": "IpAddress",
                     "shape": "String"
                 },
                 "IsVipNetwork": {
@@ -23374,14 +24843,24 @@
                     "locationName": "AvailabilityZone",
                     "shape": "String"
                 }
             },
             "name": "RequestPlacementOfCreateNetworkInterface",
             "type": "structure"
         },
+        "RequestPlacementOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "AvailabilityZone": {
+                    "locationName": "AvailabilityZone",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestPlacementOfCreateRemoteAccessVpnGateway",
+            "type": "structure"
+        },
         "RequestPlacementOfCreateSecurityGroup": {
             "members": {
                 "AvailabilityZone": {
                     "locationName": "AvailabilityZone",
                     "shape": "String"
                 }
             },
@@ -23449,14 +24928,49 @@
                     "locationName": "StartNumber",
                     "shape": "Integer"
                 }
             },
             "name": "RequestRangeOfDescribeUserActivities",
             "type": "structure"
         },
+        "RequestRemoteUser": {
+            "members": {
+                "Description": {
+                    "locationName": "Description",
+                    "shape": "String"
+                },
+                "Password": {
+                    "locationName": "Password",
+                    "shape": "String"
+                },
+                "UserName": {
+                    "locationName": "UserName",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestRemoteUser",
+            "required": [
+                "Password",
+                "UserName"
+            ],
+            "type": "structure"
+        },
+        "RequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers": {
+            "members": {
+                "UserName": {
+                    "locationName": "UserName",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestRemoteUserOfDeleteRemoteAccessVpnGatewayUsers",
+            "required": [
+                "UserName"
+            ],
+            "type": "structure"
+        },
         "RequestRemove": {
             "members": {
                 "Group": {
                     "locationName": "Group",
                     "shape": "String"
                 },
                 "UserId": {
@@ -25164,14 +26678,78 @@
             "enum": [
                 "0",
                 "1"
             ],
             "name": "SetMondayOfScalingScheduleForNiftyUpdateAutoScalingGroup",
             "type": "string"
         },
+        "SetRemoteAccessVpnGatewayCACertificateRequest": {
+            "members": {
+                "CACertificateId": {
+                    "locationName": "CACertificateId",
+                    "shape": "String"
+                },
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "SetRemoteAccessVpnGatewayCACertificateRequest",
+            "required": [
+                "CACertificateId",
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "SetRemoteAccessVpnGatewayCACertificateResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "SetRemoteAccessVpnGatewayCACertificateResult",
+            "type": "structure"
+        },
+        "SetRemoteAccessVpnGatewaySSLCertificateRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                },
+                "SSLCertificateId": {
+                    "locationName": "SSLCertificateId",
+                    "shape": "String"
+                }
+            },
+            "name": "SetRemoteAccessVpnGatewaySSLCertificateRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId",
+                "SSLCertificateId"
+            ],
+            "type": "structure"
+        },
+        "SetRemoteAccessVpnGatewaySSLCertificateResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "SetRemoteAccessVpnGatewaySSLCertificateResult",
+            "type": "structure"
+        },
         "SetSaturdayOfScalingScheduleForNiftyCreateAutoScalingGroup": {
             "enum": [
                 "0",
                 "1"
             ],
             "name": "SetSaturdayOfScalingScheduleForNiftyCreateAutoScalingGroup",
             "type": "string"
@@ -25760,14 +27338,68 @@
                     "locationName": "UnsetLoadBalancerListenerSSLCertificateResult",
                     "shape": "String"
                 }
             },
             "name": "UnsetLoadBalancerListenerSSLCertificateResultWrapper",
             "type": "structure"
         },
+        "UnsetRemoteAccessVpnGatewayCACertificateRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "UnsetRemoteAccessVpnGatewayCACertificateRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "UnsetRemoteAccessVpnGatewayCACertificateResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "UnsetRemoteAccessVpnGatewayCACertificateResult",
+            "type": "structure"
+        },
+        "UnsetRemoteAccessVpnGatewaySSLCertificateRequest": {
+            "members": {
+                "RemoteAccessVpnGatewayId": {
+                    "locationName": "RemoteAccessVpnGatewayId",
+                    "shape": "String"
+                }
+            },
+            "name": "UnsetRemoteAccessVpnGatewaySSLCertificateRequest",
+            "required": [
+                "RemoteAccessVpnGatewayId"
+            ],
+            "type": "structure"
+        },
+        "UnsetRemoteAccessVpnGatewaySSLCertificateResult": {
+            "members": {
+                "RequestId": {
+                    "locationName": "requestId",
+                    "shape": "String"
+                },
+                "Return": {
+                    "locationName": "return",
+                    "shape": "Boolean"
+                }
+            },
+            "name": "UnsetRemoteAccessVpnGatewaySSLCertificateResult",
+            "type": "structure"
+        },
         "UpdateLoadBalancerOptionRequest": {
             "members": {
                 "InstancePort": {
                     "locationName": "InstancePort",
                     "shape": "Integer"
                 },
                 "LoadBalancerName": {
@@ -26098,28 +27730,56 @@
                     "locationName": "Version",
                     "shape": "String"
                 }
             },
             "name": "VersionInformation",
             "type": "structure"
         },
+        "VersionInformationOfCreateRemoteAccessVpnGateway": {
+            "members": {
+                "IsLatest": {
+                    "locationName": "isLatest",
+                    "shape": "String"
+                },
+                "Version": {
+                    "locationName": "version",
+                    "shape": "String"
+                }
+            },
+            "name": "VersionInformationOfCreateRemoteAccessVpnGateway",
+            "type": "structure"
+        },
         "VersionInformationOfCreateVpnGateway": {
             "members": {
                 "IsLatest": {
                     "locationName": "isLatest",
                     "shape": "Boolean"
                 },
                 "Version": {
                     "locationName": "version",
                     "shape": "String"
                 }
             },
             "name": "VersionInformationOfCreateVpnGateway",
             "type": "structure"
         },
+        "VersionInformationOfDescribeRemoteAccessVpnGateways": {
+            "members": {
+                "IsLatest": {
+                    "locationName": "isLatest",
+                    "shape": "String"
+                },
+                "Version": {
+                    "locationName": "version",
+                    "shape": "String"
+                }
+            },
+            "name": "VersionInformationOfDescribeRemoteAccessVpnGateways",
+            "type": "structure"
+        },
         "VersionInformationOfDescribeVpnGateways": {
             "members": {
                 "IsLatest": {
                     "locationName": "isLatest",
                     "shape": "Boolean"
                 },
                 "Version": {
```

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/computing/3.0/waiters-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/waiters-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'waiters'": "{'RemoteAccessVpnGatewayExists': OrderedDict([('delay', 20), ('maxAttempts', 40), "*

 * *              "('operation', 'DescribeRemoteAccessVpnGateways'), ('acceptors', "*

 * *              "[OrderedDict([('matcher', 'path'), ('expected', True), ('argument', "*

 * *              "'length(RemoteAccessVpnGatewaySet[]) > `0`'), ('state', 'success')]), "*

 * *              "OrderedDict([('matcher', 'error'), ('expected', "*

 * *              "'Client.InvalidParameterNotFound.RemoteAccessVpnGatewayId'), ('state', "*

 * *        […]*

```diff
@@ -345,14 +345,63 @@
                     "state": "retry"
                 }
             ],
             "delay": 20,
             "maxAttempts": 40,
             "operation": "NiftyDescribePrivateLans"
         },
+        "RemoteAccessVpnGatewayAvailable": {
+            "acceptors": [
+                {
+                    "argument": "RemoteAccessVpnGatewaySet[].Status",
+                    "expected": "available",
+                    "matcher": "pathAll",
+                    "state": "success"
+                }
+            ],
+            "delay": 20,
+            "maxAttempts": 40,
+            "operation": "DescribeRemoteAccessVpnGateways"
+        },
+        "RemoteAccessVpnGatewayDeleted": {
+            "acceptors": [
+                {
+                    "expected": "Client.InvalidParameterNotFound.RemoteAccessVpnGatewayId",
+                    "matcher": "error",
+                    "state": "success"
+                },
+                {
+                    "argument": "length(RemoteAccessVpnGatewaySet[]) == `0`",
+                    "expected": true,
+                    "matcher": "path",
+                    "state": "success"
+                }
+            ],
+            "delay": 20,
+            "maxAttempts": 40,
+            "operation": "DescribeRemoteAccessVpnGateways"
+        },
+        "RemoteAccessVpnGatewayExists": {
+            "acceptors": [
+                {
+                    "argument": "length(RemoteAccessVpnGatewaySet[]) > `0`",
+                    "expected": true,
+                    "matcher": "path",
+                    "state": "success"
+                },
+                {
+                    "expected": "Client.InvalidParameterNotFound.RemoteAccessVpnGatewayId",
+                    "matcher": "error",
+                    "state": "retry"
+                }
+            ],
+            "delay": 20,
+            "maxAttempts": 40,
+            "operation": "DescribeRemoteAccessVpnGateways"
+        },
         "RouterAvailable": {
             "acceptors": [
                 {
                     "argument": "RouterSet[].State",
                     "expected": "available",
                     "matcher": "pathAll",
                     "state": "success"
```

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999062894570707%*

 * *Differences: {"'shapes'": "{'RequestResourceRecordSet': {'members': {delete: ['XniftyDefaultHost']}}, "*

 * *             "'ResourceRecordSets': {'members': {delete: ['XniftyDefaultHost']}}, "*

 * *             "'TypeOfChangeResourceRecordSetsRequestForChangeResourceRecordSets': {'enum': "*

 * *             "{delete: [7]}}, 'TypeOfListResourceRecordSetsRequest': {'enum': {delete: [7]}}}"}*

```diff
@@ -649,18 +649,14 @@
                 "Weight": {
                     "locationName": "Weight",
                     "shape": "Integer"
                 },
                 "XniftyComment": {
                     "locationName": "XniftyComment",
                     "shape": "String"
-                },
-                "XniftyDefaultHost": {
-                    "locationName": "XniftyDefaultHost",
-                    "shape": "String"
                 }
             },
             "name": "RequestResourceRecordSet",
             "type": "structure"
         },
         "RequestResourceRecords": {
             "members": {
@@ -732,18 +728,14 @@
                     "locationName": "Weight",
                     "shape": "Integer"
                 },
                 "XniftyComment": {
                     "locationName": "XniftyComment",
                     "shape": "String"
                 },
-                "XniftyDefaultHost": {
-                    "locationName": "XniftyDefaultHost",
-                    "shape": "String"
-                },
                 "XniftyHealthCheckConfig": {
                     "locationName": "XniftyHealthCheckConfig",
                     "shape": "XniftyHealthCheckConfig"
                 }
             },
             "name": "ResourceRecordSets",
             "type": "structure"
@@ -770,30 +762,28 @@
             "enum": [
                 "NS",
                 "A",
                 "AAAA",
                 "CNAME",
                 "MX",
                 "TXT",
-                "PTR",
-                "LBR"
+                "PTR"
             ],
             "name": "TypeOfChangeResourceRecordSetsRequestForChangeResourceRecordSets",
             "type": "string"
         },
         "TypeOfListResourceRecordSetsRequest": {
             "enum": [
                 "NS",
                 "A",
                 "AAAA",
                 "CNAME",
                 "MX",
                 "TXT",
-                "PTR",
-                "LBR"
+                "PTR"
             ],
             "name": "TypeOfListResourceRecordSetsRequest",
             "type": "string"
         },
         "XniftyHealthCheckConfig": {
             "members": {
                 "FullyQualifiedDomainName": {
```

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/endpoints.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/v1/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/hatoba/v1/waiters-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/nas/N2016-02-24/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/nas/N2016-02-24/waiters-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975158425887638%*

 * *Differences: {"'shapes'": "{'CreateDBInstanceRequest': {'members': {delete: "*

 * *             "['NiftyReadReplicaDBInstanceIdentifier', 'NiftyReadReplicaPrivateAddress', "*

 * *             "'ReadReplicaAccountingType']}}, 'EngineOfCreateDBInstanceRequest': {'enum': {delete: "*

 * *             "[2]}}, 'ModifyDBInstanceRequest': {'members': {delete: "*

 * *             "['NiftyReadReplicaDBInstanceIdentifier', 'NiftyReadReplicaPrivateAddress', "*

 * *             "'ReadReplicaAccountingType']}}, 'RestoreDBInstanceFromDBSnapshotRequest': "*

 * *    […]*

```diff
@@ -1014,22 +1014,14 @@
                     "locationName": "NiftyMultiAZType",
                     "shape": "Integer"
                 },
                 "NiftyNetworkId": {
                     "locationName": "NiftyNetworkId",
                     "shape": "String"
                 },
-                "NiftyReadReplicaDBInstanceIdentifier": {
-                    "locationName": "NiftyReadReplicaDBInstanceIdentifier",
-                    "shape": "String"
-                },
-                "NiftyReadReplicaPrivateAddress": {
-                    "locationName": "NiftyReadReplicaPrivateAddress",
-                    "shape": "String"
-                },
                 "NiftySlavePrivateAddress": {
                     "locationName": "NiftySlavePrivateAddress",
                     "shape": "String"
                 },
                 "NiftyStorageType": {
                     "locationName": "NiftyStorageType",
                     "shape": "Integer"
@@ -1054,18 +1046,14 @@
                     "locationName": "PreferredMaintenanceWindow",
                     "shape": "String"
                 },
                 "PubliclyAccessible": {
                     "locationName": "PubliclyAccessible",
                     "shape": "Boolean"
                 },
-                "ReadReplicaAccountingType": {
-                    "locationName": "ReadReplicaAccountingType",
-                    "shape": "ReadReplicaAccountingTypeOfCreateDBInstanceRequest"
-                },
                 "VpcSecurityGroupIds": {
                     "locationName": "VpcSecurityGroupIds",
                     "shape": "ListOfRequestVpcSecurityGroupIds"
                 }
             },
             "name": "CreateDBInstanceRequest",
             "required": [
@@ -3180,16 +3168,15 @@
             },
             "name": "EngineDefaults",
             "type": "structure"
         },
         "EngineOfCreateDBInstanceRequest": {
             "enum": [
                 "MySQL",
-                "postgres",
-                "MariaDB"
+                "postgres"
             ],
             "name": "EngineOfCreateDBInstanceRequest",
             "type": "string"
         },
         "EngineOfDescribeDBEngineVersionsRequest": {
             "enum": [
                 "MySQL",
@@ -3852,22 +3839,14 @@
                     "locationName": "NewDBInstanceIdentifier",
                     "shape": "String"
                 },
                 "NiftyMultiAZType": {
                     "locationName": "NiftyMultiAZType",
                     "shape": "Integer"
                 },
-                "NiftyReadReplicaDBInstanceIdentifier": {
-                    "locationName": "NiftyReadReplicaDBInstanceIdentifier",
-                    "shape": "String"
-                },
-                "NiftyReadReplicaPrivateAddress": {
-                    "locationName": "NiftyReadReplicaPrivateAddress",
-                    "shape": "String"
-                },
                 "NiftySlavePrivateAddress": {
                     "locationName": "NiftySlavePrivateAddress",
                     "shape": "String"
                 },
                 "OptionGroupName": {
                     "locationName": "OptionGroupName",
                     "shape": "String"
@@ -3876,18 +3855,14 @@
                     "locationName": "PreferredBackupWindow",
                     "shape": "String"
                 },
                 "PreferredMaintenanceWindow": {
                     "locationName": "PreferredMaintenanceWindow",
                     "shape": "String"
                 },
-                "ReadReplicaAccountingType": {
-                    "locationName": "ReadReplicaAccountingType",
-                    "shape": "ReadReplicaAccountingTypeOfModifyDBInstanceRequest"
-                },
                 "VpcSecurityGroupIds": {
                     "locationName": "VpcSecurityGroupIds",
                     "shape": "ListOfRequestVpcSecurityGroupIds"
                 }
             },
             "name": "ModifyDBInstanceRequest",
             "required": [
@@ -4215,46 +4190,14 @@
                     "locationName": "Port",
                     "shape": "Integer"
                 }
             },
             "name": "PendingModifiedValues",
             "type": "structure"
         },
-        "ReadReplicaAccountingTypeOfCreateDBInstanceRequest": {
-            "enum": [
-                "1",
-                "2"
-            ],
-            "name": "ReadReplicaAccountingTypeOfCreateDBInstanceRequest",
-            "type": "string"
-        },
-        "ReadReplicaAccountingTypeOfModifyDBInstanceRequest": {
-            "enum": [
-                "1",
-                "2"
-            ],
-            "name": "ReadReplicaAccountingTypeOfModifyDBInstanceRequest",
-            "type": "string"
-        },
-        "ReadReplicaAccountingTypeOfRestoreDBInstanceFromDBSnapshotRequest": {
-            "enum": [
-                "1",
-                "2"
-            ],
-            "name": "ReadReplicaAccountingTypeOfRestoreDBInstanceFromDBSnapshotRequest",
-            "type": "string"
-        },
-        "ReadReplicaAccountingTypeOfRestoreDBInstanceToPointInTimeRequest": {
-            "enum": [
-                "1",
-                "2"
-            ],
-            "name": "ReadReplicaAccountingTypeOfRestoreDBInstanceToPointInTimeRequest",
-            "type": "string"
-        },
         "RebootDBInstanceRequest": {
             "members": {
                 "DBInstanceIdentifier": {
                     "locationName": "DBInstanceIdentifier",
                     "shape": "String"
                 },
                 "ForceFailover": {
@@ -4535,22 +4478,14 @@
                     "locationName": "NiftyMultiAZType",
                     "shape": "Integer"
                 },
                 "NiftyNetworkId": {
                     "locationName": "NiftyNetworkId",
                     "shape": "String"
                 },
-                "NiftyReadReplicaDBInstanceIdentifier": {
-                    "locationName": "NiftyReadReplicaDBInstanceIdentifier",
-                    "shape": "String"
-                },
-                "NiftyReadReplicaPrivateAddress": {
-                    "locationName": "NiftyReadReplicaPrivateAddress",
-                    "shape": "String"
-                },
                 "NiftySlavePrivateAddress": {
                     "locationName": "NiftySlavePrivateAddress",
                     "shape": "String"
                 },
                 "NiftyStorageType": {
                     "locationName": "NiftyStorageType",
                     "shape": "Integer"
@@ -4566,18 +4501,14 @@
                 "Port": {
                     "locationName": "Port",
                     "shape": "Integer"
                 },
                 "PubliclyAccessible": {
                     "locationName": "PubliclyAccessible",
                     "shape": "Boolean"
-                },
-                "ReadReplicaAccountingType": {
-                    "locationName": "ReadReplicaAccountingType",
-                    "shape": "ReadReplicaAccountingTypeOfRestoreDBInstanceFromDBSnapshotRequest"
                 }
             },
             "name": "RestoreDBInstanceFromDBSnapshotRequest",
             "required": [
                 "DBInstanceClass",
                 "DBInstanceIdentifier",
                 "DBSnapshotIdentifier"
@@ -4656,22 +4587,14 @@
                     "locationName": "NiftyMultiAZType",
                     "shape": "Integer"
                 },
                 "NiftyNetworkId": {
                     "locationName": "NiftyNetworkId",
                     "shape": "String"
                 },
-                "NiftyReadReplicaDBInstanceIdentifier": {
-                    "locationName": "NiftyReadReplicaDBInstanceIdentifier",
-                    "shape": "String"
-                },
-                "NiftyReadReplicaPrivateAddress": {
-                    "locationName": "NiftyReadReplicaPrivateAddress",
-                    "shape": "String"
-                },
                 "NiftySlavePrivateAddress": {
                     "locationName": "NiftySlavePrivateAddress",
                     "shape": "String"
                 },
                 "NiftyStorageType": {
                     "locationName": "NiftyStorageType",
                     "shape": "Integer"
@@ -4688,18 +4611,14 @@
                     "locationName": "Port",
                     "shape": "Integer"
                 },
                 "PubliclyAccessible": {
                     "locationName": "PubliclyAccessible",
                     "shape": "Boolean"
                 },
-                "ReadReplicaAccountingType": {
-                    "locationName": "ReadReplicaAccountingType",
-                    "shape": "ReadReplicaAccountingTypeOfRestoreDBInstanceToPointInTimeRequest"
-                },
                 "RestoreTime": {
                     "locationName": "RestoreTime",
                     "shape": "TStamp"
                 },
                 "SourceDBInstanceIdentifier": {
                     "locationName": "SourceDBInstanceIdentifier",
                     "shape": "String"
```

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/script/2015-09-01/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/service-activity/2020-11-25/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/data/storage/2006-03-01/service-2.json` & `nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983174554827434%*

 * *Differences: {"'shapes'": "{'GetBucketVersion2Result': {'members': {'Contents': {'shape': 'ListOfContents'}}}, "*

 * *             "'GetBucketVersioningResult': {'members': {delete: ['MfaDelete']}}, "*

 * *             "'GetObjectRequest': {'members': {'PartNumber': OrderedDict([('location', "*

 * *             "'querystring'), ('locationName', 'partNumber'), ('shape', 'String')])}}, "*

 * *             "'GetObjectResult': {'members': {'XAmzMpPartsCount': OrderedDict([('location', "*

 * *             "'header'), ('locationName', 'x-amz-mp-parts […]*

```diff
@@ -756,52 +756,14 @@
                     "locationName": "StorageClass",
                     "shape": "String"
                 }
             },
             "name": "Contents",
             "type": "structure"
         },
-        "ContentsOfGetBucketVersion2": {
-            "members": {
-                "DisplayName": {
-                    "locationName": "DisplayName",
-                    "shape": "String"
-                },
-                "ETag": {
-                    "locationName": "ETag",
-                    "shape": "String"
-                },
-                "ID": {
-                    "locationName": "ID",
-                    "shape": "String"
-                },
-                "Key": {
-                    "locationName": "Key",
-                    "shape": "String"
-                },
-                "LastModified": {
-                    "locationName": "LastModified",
-                    "shape": "TStamp"
-                },
-                "Owner": {
-                    "locationName": "Owner",
-                    "shape": "String"
-                },
-                "Size": {
-                    "locationName": "Size",
-                    "shape": "String"
-                },
-                "StorageClass": {
-                    "locationName": "StorageClass",
-                    "shape": "String"
-                }
-            },
-            "name": "ContentsOfGetBucketVersion2",
-            "type": "structure"
-        },
         "DeleteBucketCorsRequest": {
             "members": {
                 "Bucket": {
                     "location": "uri",
                     "locationName": "Bucket",
                     "shape": "String"
                 }
@@ -1440,15 +1402,15 @@
                 "ContentType": {
                     "location": "header",
                     "locationName": "Content-Type",
                     "shape": "String"
                 },
                 "Contents": {
                     "locationName": "Contents",
-                    "shape": "ListOfContentsOfGetBucketVersion2"
+                    "shape": "ListOfContents"
                 },
                 "ContinuationToken": {
                     "locationName": "ContinuationToken",
                     "shape": "String"
                 },
                 "Delimiter": {
                     "locationName": "Delimiter",
@@ -1507,18 +1469,14 @@
         "GetBucketVersioningResult": {
             "members": {
                 "ContentType": {
                     "location": "header",
                     "locationName": "Content-Type",
                     "shape": "String"
                 },
-                "MfaDelete": {
-                    "locationName": "MfaDelete",
-                    "shape": "String"
-                },
                 "Status": {
                     "locationName": "Status",
                     "shape": "String"
                 }
             },
             "name": "GetBucketVersioningResult",
             "type": "structure"
@@ -1575,14 +1533,19 @@
                     "shape": "String"
                 },
                 "Object": {
                     "location": "uri",
                     "locationName": "Object",
                     "shape": "String"
                 },
+                "PartNumber": {
+                    "location": "querystring",
+                    "locationName": "partNumber",
+                    "shape": "String"
+                },
                 "Range": {
                     "location": "header",
                     "locationName": "Range",
                     "shape": "String"
                 },
                 "ResponseContentDisposition": {
                     "location": "querystring",
@@ -1660,14 +1623,19 @@
                     "shape": "String"
                 },
                 "XAmzExpiration": {
                     "location": "header",
                     "locationName": "x-amz-expiration",
                     "shape": "String"
                 },
+                "XAmzMpPartsCount": {
+                    "location": "header",
+                    "locationName": "x-amz-mp-parts-count",
+                    "shape": "String"
+                },
                 "XAmzServerSideEncryption": {
                     "location": "header",
                     "locationName": "x-amz-server-side-encryption",
                     "shape": "String"
                 }
             },
             "name": "GetObjectResult",
@@ -1793,14 +1761,19 @@
                     "shape": "String"
                 },
                 "Object": {
                     "location": "uri",
                     "locationName": "Object",
                     "shape": "String"
                 },
+                "PartNumber": {
+                    "location": "querystring",
+                    "locationName": "partNumber",
+                    "shape": "String"
+                },
                 "VersionId": {
                     "location": "querystring",
                     "locationName": "versionId",
                     "shape": "String"
                 },
                 "XAmzServerSideEncryptionCustomerAlgorithm": {
                     "location": "header",
@@ -1848,14 +1821,19 @@
                     "shape": "String"
                 },
                 "XAmzExpiration": {
                     "location": "header",
                     "locationName": "x-amz-expiration",
                     "shape": "String"
                 },
+                "XAmzMpPartsCount": {
+                    "location": "header",
+                    "locationName": "x-amz-mp-parts-count",
+                    "shape": "String"
+                },
                 "XAmzServerSideEncryption": {
                     "location": "header",
                     "locationName": "x-amz-server-side-encryption",
                     "shape": "String"
                 },
                 "XAmzVersionId": {
                     "location": "header",
@@ -2095,22 +2073,14 @@
             "flattened": true,
             "member": {
                 "shape": "Contents"
             },
             "name": "ListOfContents",
             "type": "list"
         },
-        "ListOfContentsOfGetBucketVersion2": {
-            "flattened": true,
-            "member": {
-                "shape": "ContentsOfGetBucketVersion2"
-            },
-            "name": "ListOfContentsOfGetBucketVersion2",
-            "type": "list"
-        },
         "ListOfDeleted": {
             "flattened": true,
             "member": {
                 "shape": "Deleted"
             },
             "name": "ListOfDeleted",
             "type": "list"
```

### Comparing `nifcloud-cli-1.5.2/nifcloudcli/link.py` & `nifcloud-cli-1.6.0/nifcloudcli/link.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.5.2/setup.py` & `nifcloud-cli-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='FUJITSU CLOUD TECHNOLOGIES',
     url='https://github.com/nifcloud/nifcloud-cli',
     packages=find_packages(exclude=['tests*']),
     package_data={'nifcloudcli': ['data/*.json', 'topics/*.json']},
     include_package_data=True,
-    install_requires=['nifcloud==1.5.0', 'awscli==1.20.43'],
+    install_requires=['nifcloud==1.6.0', 'awscli==1.20.43'],
     license='Apache License 2.0',
     classifiers=(
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
```

