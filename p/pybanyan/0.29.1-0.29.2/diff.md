# Comparing `tmp/pybanyan-0.29.1.tar.gz` & `tmp/pybanyan-0.29.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybanyan-0.29.1.tar", last modified: Wed Apr 19 20:45:41 2023, max compression
+gzip compressed data, was "pybanyan-0.29.2.tar", last modified: Thu Apr 20 18:30:56 2023, max compression
```

## Comparing `pybanyan-0.29.1.tar` & `pybanyan-0.29.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.559155 pybanyan-0.29.1/
--rw-r--r--   0 tarun      (501) staff       (20)     3304 2023-04-19 20:44:30.000000 pybanyan-0.29.1/CHANGELOG.md
--rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.29.1/LICENSE.md
--rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.29.1/MANIFEST.in
--rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 20:45:41.559230 pybanyan-0.29.1/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     7756 2023-04-19 18:32:42.000000 pybanyan-0.29.1/README.md
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.543570 pybanyan-0.29.1/banyan/
--rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.547887 pybanyan-0.29.1/banyan/api/
--rw-r--r--   0 tarun      (501) staff       (20)    17853 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/api/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)      397 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)      453 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/api/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     1746 2022-04-07 19:03:43.000000 pybanyan-0.29.1/banyan/api/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     6173 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)      382 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     6392 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/api/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     6069 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/api/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)      851 2022-11-29 19:34:37.000000 pybanyan-0.29.1/banyan/api/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     2215 2023-04-19 20:35:30.000000 pybanyan-0.29.1/banyan/api/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/role.py
--rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)      427 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     1467 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/api/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     1520 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551462 pybanyan-0.29.1/banyan/controllers/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2442 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/admin.py
--rw-r--r--   0 tarun      (501) staff       (20)     2504 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     6045 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/controllers/base.py
--rw-r--r--   0 tarun      (501) staff       (20)    21999 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     2574 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     6024 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/controllers/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/event.py
--rw-r--r--   0 tarun      (501) staff       (20)     3216 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/export.py
--rw-r--r--   0 tarun      (501) staff       (20)     2329 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     6198 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     3850 2022-11-29 19:34:37.000000 pybanyan-0.29.1/banyan/controllers/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10519 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     8869 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     2136 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     9763 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     3966 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     4281 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551845 pybanyan-0.29.1/banyan/core/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/core/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/core/exc.py
--rw-r--r--   0 tarun      (501) staff       (20)      177 2023-04-19 20:43:56.000000 pybanyan-0.29.1/banyan/core/version.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551974 pybanyan-0.29.1/banyan/ext/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/ext/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.553135 pybanyan-0.29.1/banyan/ext/iaas/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/azure_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/gcp.py
--rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/oracle_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/vmware.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.553719 pybanyan-0.29.1/banyan/ext/idp/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/azure_ad.py
--rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/okta.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.554147 pybanyan-0.29.1/banyan/lib/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/certs.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.554483 pybanyan-0.29.1/banyan/lib/cloud/
--rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/cloud/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/cloud/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     4281 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/main.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.557860 pybanyan-0.29.1/banyan/model/
--rw-r--r--   0 tarun      (501) staff       (20)     5990 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2409 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)     1137 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)     1471 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     3887 2022-04-07 19:03:43.000000 pybanyan-0.29.1/banyan/model/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     2095 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/model/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.29.1/banyan/model/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     4591 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     2351 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/service.py
--rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.29.1/banyan/model/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     1953 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.29.1/banyan/model/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     2914 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/model/trustscore.py
--rw-r--r--   0 tarun      (501) staff       (20)     7580 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/model/user_device.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.558081 pybanyan-0.29.1/banyan/plugins/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/plugins/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.558187 pybanyan-0.29.1/banyan/templates/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/templates/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.559031 pybanyan-0.29.1/pybanyan.egg-info/
--rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     2401 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/SOURCES.txt
--rw-r--r--   0 tarun      (501) staff       (20)        1 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/dependency_links.txt
--rw-r--r--   0 tarun      (501) staff       (20)       44 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/entry_points.txt
--rw-r--r--   0 tarun      (501) staff       (20)      389 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/requires.txt
--rw-r--r--   0 tarun      (501) staff       (20)        7 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/top_level.txt
--rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.29.1/requirements-dev.txt
--rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.29.1/requirements.txt
--rw-r--r--   0 tarun      (501) staff       (20)       38 2023-04-19 20:45:41.559451 pybanyan-0.29.1/setup.cfg
--rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.29.1/setup.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.856507 pybanyan-0.29.2/
+-rw-r--r--   0 tarun      (501) staff       (20)     3408 2023-04-20 18:05:27.000000 pybanyan-0.29.2/CHANGELOG.md
+-rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.29.2/LICENSE.md
+-rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.29.2/MANIFEST.in
+-rw-r--r--   0 tarun      (501) staff       (20)     8370 2023-04-20 18:30:56.856590 pybanyan-0.29.2/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     7889 2023-04-20 17:58:41.000000 pybanyan-0.29.2/README.md
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.836530 pybanyan-0.29.2/banyan/
+-rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.841086 pybanyan-0.29.2/banyan/api/
+-rw-r--r--   0 tarun      (501) staff       (20)    17853 2023-04-17 18:19:15.000000 pybanyan-0.29.2/banyan/api/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)      397 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/api/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)      453 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/api/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/api/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1746 2022-04-07 19:03:43.000000 pybanyan-0.29.2/banyan/api/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6173 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/api/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.29.2/banyan/api/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)      382 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/api/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7035 2023-04-20 16:26:01.000000 pybanyan-0.29.2/banyan/api/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6069 2023-04-17 18:19:15.000000 pybanyan-0.29.2/banyan/api/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)      851 2022-11-29 19:34:37.000000 pybanyan-0.29.2/banyan/api/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2023-04-19 20:35:30.000000 pybanyan-0.29.2/banyan/api/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.29.2/banyan/api/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.29.2/banyan/api/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.29.2/banyan/api/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)      427 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/api/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.29.2/banyan/api/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1467 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/api/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1532 2023-04-20 00:20:40.000000 pybanyan-0.29.2/banyan/api/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.845374 pybanyan-0.29.2/banyan/controllers/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/controllers/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2442 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/controllers/admin.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2504 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/controllers/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6112 2023-04-20 17:59:57.000000 pybanyan-0.29.2/banyan/controllers/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)    21999 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2574 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6036 2023-04-20 16:07:31.000000 pybanyan-0.29.2/banyan/controllers/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/controllers/event.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3229 2023-04-20 18:01:33.000000 pybanyan-0.29.2/banyan/controllers/export.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2329 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6189 2023-04-20 00:53:08.000000 pybanyan-0.29.2/banyan/controllers/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3867 2023-04-20 00:53:25.000000 pybanyan-0.29.2/banyan/controllers/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10519 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     8869 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/controllers/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2136 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     9763 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/controllers/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3966 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/controllers/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3761 2023-04-20 00:25:44.000000 pybanyan-0.29.2/banyan/controllers/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.845970 pybanyan-0.29.2/banyan/core/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/core/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/core/exc.py
+-rw-r--r--   0 tarun      (501) staff       (20)      177 2023-04-20 18:04:59.000000 pybanyan-0.29.2/banyan/core/version.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.846113 pybanyan-0.29.2/banyan/ext/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/ext/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.847369 pybanyan-0.29.2/banyan/ext/iaas/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/azure_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/gcp.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/oracle_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/iaas/vmware.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.849359 pybanyan-0.29.2/banyan/ext/idp/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/idp/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/idp/azure_ad.py
+-rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/idp/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.29.2/banyan/ext/idp/okta.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.850908 pybanyan-0.29.2/banyan/lib/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/lib/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/lib/certs.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.851350 pybanyan-0.29.2/banyan/lib/cloud/
+-rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/lib/cloud/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/lib/cloud/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/lib/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4281 2023-04-20 18:02:34.000000 pybanyan-0.29.2/banyan/main.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.855088 pybanyan-0.29.2/banyan/model/
+-rw-r--r--   0 tarun      (501) staff       (20)     5990 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2409 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1137 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1471 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/model/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3887 2022-04-07 19:03:43.000000 pybanyan-0.29.2/banyan/model/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2095 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/model/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.29.2/banyan/model/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4591 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/model/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2351 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.29.2/banyan/model/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1953 2022-12-01 04:15:52.000000 pybanyan-0.29.2/banyan/model/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.29.2/banyan/model/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2914 2023-04-19 20:43:31.000000 pybanyan-0.29.2/banyan/model/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/model/trustscore.py
+-rw-r--r--   0 tarun      (501) staff       (20)     8258 2023-04-20 00:21:02.000000 pybanyan-0.29.2/banyan/model/user_device.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.855384 pybanyan-0.29.2/banyan/plugins/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/plugins/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.855492 pybanyan-0.29.2/banyan/templates/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.2/banyan/templates/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-20 18:30:56.856377 pybanyan-0.29.2/pybanyan.egg-info/
+-rw-r--r--   0 tarun      (501) staff       (20)     8370 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     2401 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/SOURCES.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        1 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/dependency_links.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       44 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/entry_points.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      389 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/requires.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        7 2023-04-20 18:30:56.000000 pybanyan-0.29.2/pybanyan.egg-info/top_level.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.29.2/requirements-dev.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.29.2/requirements.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       38 2023-04-20 18:30:56.856842 pybanyan-0.29.2/setup.cfg
+-rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.29.2/setup.py
```

### Comparing `pybanyan-0.29.1/CHANGELOG.md` & `pybanyan-0.29.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # PyBanyan Change History
 
+## 0.29.2
+
+ * more bugfixes to close Github tickets
+ * improve logic used to update device attributes 
+
 ## 0.29.1
 
  * bugfixes to close Github tickets
 
 ## 0.29.0
 
  * make api_key the primary credential (refresh_token still works)
```

### Comparing `pybanyan-0.29.1/LICENSE.md` & `pybanyan-0.29.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/PKG-INFO` & `pybanyan-0.29.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.29.1
+Version: 0.29.2
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
@@ -40,47 +40,47 @@
 $ pip install -r requirements.txt
 $ python setup.py install --user
 ```
 
 ## Usage
 
 This package contains both an API client and a CLI tool.
-To use either one, you need to [generate] an API token from the Banyan Command Center.
+To use either one, you need to [generate][docs] an API credential from the Banyan Command Center.
 
 ### API library
 
-Here's a sample script that uses the library to print the names of every service registered in Banyan:
+Here's a sample script that uses the library to print the names of every hosted website service registered in Banyan:
 
 ```python
 from banyan.api import BanyanApiClient
 
 c = BanyanApiClient()
-for service in c.services.list():
+for service in c.services_web.list():
     print(service.name)
 ```
 
 Output:
 ```console
 $ python examples/list_services.py
 jira
 jupyter
 kube
 mysql
 rds-mysql
 rds-pgsql
 ```
 
-The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
+The `BanyanApiClient` class accepts optional arguments to specify the API server and API credential. If not provided, 
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY` (you can also use a personal refresh token as your API credential.
 
-Full API documentation will be available soon.
+Full API documentation is available in the [docs].
 
 ### Banyan CLI tool
 
-Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential in the `api_key` field (you can also use a personal refresh token as your API credential):
 
 ```ini
 [banyan]
 api_url = https://net.banyanops.com
 api_key = MY_API_KEY
 ```
 
@@ -96,15 +96,15 @@
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           full application debug mode
   -q, --quiet           suppress all console output
   --version, -v         show program's version number and exit
   --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
-  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY environment
                         variable.
   --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
   --output-format {table,json,yaml}, -o {table,json,yaml}
                         desired output format (table, json, yaml)
 
 Commands:
   {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
@@ -126,16 +126,16 @@
     service-web         manage hosted website services
     user                manage users
 ```
 
 Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
 
 ```console
-$ banyan service
-usage: banyan service [-h]
+$ banyan service-web
+usage: banyan service-web [-h]
                       {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
                       ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 sub-commands:
@@ -152,16 +152,16 @@
     update              update an existing service from a JSON specification
 ```
 
 To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
 For example:
 
 ```console
-$ banyan service attach-policy --help
-usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
+$ banyan service-web attach-policy --help
+usage: banyan service-web attach-policy [-h] [--permissive] [--enforcing]
                                     service_name_or_id policy_name_or_id
 
 positional arguments:
   service_name_or_id  Name or ID of the service to attach a policy to.
   policy_name_or_id   Name or ID of the policy to attach to the service.
 
 optional arguments:
@@ -203,11 +203,11 @@
 issues with the library, please create a new [issue in Github][github-issue].
 
 ## Contributions
 
 We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
 workflow][github-pr].
 
-[generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
+[docs]: https://docs.banyansecurity.io/docs/api-guide/introduction/
 [github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
 [github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
 [devel]: https://pybanyan.readthedocs.io/development.html
```

### Comparing `pybanyan-0.29.1/README.md` & `pybanyan-0.29.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,47 +22,47 @@
 $ pip install -r requirements.txt
 $ python setup.py install --user
 ```
 
 ## Usage
 
 This package contains both an API client and a CLI tool.
-To use either one, you need to [generate] an API token from the Banyan Command Center.
+To use either one, you need to [generate][docs] an API credential from the Banyan Command Center.
 
 ### API library
 
-Here's a sample script that uses the library to print the names of every service registered in Banyan:
+Here's a sample script that uses the library to print the names of every hosted website service registered in Banyan:
 
 ```python
 from banyan.api import BanyanApiClient
 
 c = BanyanApiClient()
-for service in c.services.list():
+for service in c.services_web.list():
     print(service.name)
 ```
 
 Output:
 ```console
 $ python examples/list_services.py
 jira
 jupyter
 kube
 mysql
 rds-mysql
 rds-pgsql
 ```
 
-The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
+The `BanyanApiClient` class accepts optional arguments to specify the API server and API credential. If not provided, 
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY` (you can also use a personal refresh token as your API credential.
 
-Full API documentation will be available soon.
+Full API documentation is available in the [docs].
 
 ### Banyan CLI tool
 
-Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential in the `api_key` field (you can also use a personal refresh token as your API credential):
 
 ```ini
 [banyan]
 api_url = https://net.banyanops.com
 api_key = MY_API_KEY
 ```
 
@@ -78,15 +78,15 @@
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           full application debug mode
   -q, --quiet           suppress all console output
   --version, -v         show program's version number and exit
   --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
-  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY environment
                         variable.
   --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
   --output-format {table,json,yaml}, -o {table,json,yaml}
                         desired output format (table, json, yaml)
 
 Commands:
   {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
@@ -108,16 +108,16 @@
     service-web         manage hosted website services
     user                manage users
 ```
 
 Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
 
 ```console
-$ banyan service
-usage: banyan service [-h]
+$ banyan service-web
+usage: banyan service-web [-h]
                       {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
                       ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 sub-commands:
@@ -134,16 +134,16 @@
     update              update an existing service from a JSON specification
 ```
 
 To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
 For example:
 
 ```console
-$ banyan service attach-policy --help
-usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
+$ banyan service-web attach-policy --help
+usage: banyan service-web attach-policy [-h] [--permissive] [--enforcing]
                                     service_name_or_id policy_name_or_id
 
 positional arguments:
   service_name_or_id  Name or ID of the service to attach a policy to.
   policy_name_or_id   Name or ID of the policy to attach to the service.
 
 optional arguments:
@@ -185,11 +185,11 @@
 issues with the library, please create a new [issue in Github][github-issue].
 
 ## Contributions
 
 We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
 workflow][github-pr].
 
-[generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
+[docs]: https://docs.banyansecurity.io/docs/api-guide/introduction/
 [github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
 [github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
 [devel]: https://pybanyan.readthedocs.io/development.html
```

### Comparing `pybanyan-0.29.1/banyan/api/__init__.py` & `pybanyan-0.29.2/banyan/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/audit.py` & `pybanyan-0.29.2/banyan/api/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/base.py` & `pybanyan-0.29.2/banyan/api/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/cloud_resource.py` & `pybanyan-0.29.2/banyan/api/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/device.py` & `pybanyan-0.29.2/banyan/api/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,46 @@
         """
         :meta private:
         """
         data_class = Device
         info_class = DeviceV2
         arg_type = str
         list_uri = '/v2/devices'
+        uri_param_v2 = 'serial_number'
         delete_uri = '/delete_device'
         insert_uri = '/mdm/update_device'
         uri_param = 'SerialNumber'
         obj_name = 'device'
         supports_paging = True
 
+
+    def get_single(self, serial_number: str) -> DeviceV2:
+        """
+        Bypasses cache because it can be too slow in orgs with >1000 devices
+        """
+        get_single = self._client.api_request('GET',
+                                                 self.Meta.list_uri,
+                                                 params={self.Meta.uri_param_v2: serial_number})
+        
+        devices = get_single['devices']
+        if len(devices) != 1:
+            raise Exception("Couldn't find a single device for this serial_number")
+        obj = DeviceV2.Schema().load(devices[0])
+        return obj
+
     def create(self, obj: Device):
         """
         Raises an exception. Devices cannot be created via API. They must be registered by installing the
         Banyan App on a device.
 
         :param obj: A device which will definitely not be created.
         :type obj: Device
         :raises: :py:exc:`BanyanError`
         """
-        raise BanyanError('devices cannot be created via the API')
+        raise BanyanError('devices cannot be created via the API')    
 
     def update(self, obj: DeviceV2) -> str:
         """
         Updates a limited set of properties belonging to a device. The properties that can be updated are:
 
         * Device hardware data: :py:data:`architecture`, :py:data:`model`, and :py:data:`platform`.
         * Corporate ownership status: :py:data:`ownership`.
@@ -51,25 +67,26 @@
         Changes to any other fields in the :py:class:`Device` object will be ignored.
 
         :param obj: The device to be updated.
         :type obj: Device
         :return: Message from the server indicating success or failure.
         :rtype: str
         """
-        self._ensure_exists(obj.serial_number)
+        
         change_attr = {
             "Model": obj.model,
             "Ownership": obj.ownership,
             "Platform": obj.platform,
             "OS": obj.os,
             "Architecture": obj.architecture,
             "Banned": obj.banned,
             "IsMDMPresent": obj.mdm_present,
             "MDMVendorName": obj.mdm_vendor_name
         }
+        print(change_attr)
         response_json = self._client.api_request('POST',
                                                  self.Meta.insert_uri,
                                                  params={self.Meta.uri_param: obj.serial_number},
                                                  json=change_attr)
         return response_json['Message']
 
     def ban(self, obj: DeviceV2) -> str:
```

### Comparing `pybanyan-0.29.1/banyan/api/event_v2.py` & `pybanyan-0.29.2/banyan/api/event_v2.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/netagent.py` & `pybanyan-0.29.2/banyan/api/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/policy.py` & `pybanyan-0.29.2/banyan/api/policy.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/role.py` & `pybanyan-0.29.2/banyan/api/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/service.py` & `pybanyan-0.29.2/banyan/api/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/service_infra.py` & `pybanyan-0.29.2/banyan/api/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/service_web.py` & `pybanyan-0.29.2/banyan/api/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/shield.py` & `pybanyan-0.29.2/banyan/api/shield.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/api/user.py` & `pybanyan-0.29.2/banyan/api/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List
 
 from banyan.api.base import ApiBase
-from banyan.model.user_device import User, TrustScore
+from banyan.model.user_device import User, UserV2, TrustScore
 
 
 class UserAPI(ApiBase):
     class Meta:
         data_class = User
-        info_class = User
+        info_class = UserV2
         arg_type = str
-        list_uri = '/endusers'
+        list_uri = '/v2/enduser'
         delete_uri = None
         insert_uri = None
         uri_param = 'Email'
         obj_name = 'user'
         supports_paging = True
 
     def set_max_trustlevel(self, obj: User, max_level: str, reason: str, ext_source: str) -> str:
```

### Comparing `pybanyan-0.29.1/banyan/controllers/access_tier.py` & `pybanyan-0.29.2/banyan/controllers/access_tier.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/admin.py` & `pybanyan-0.29.2/banyan/controllers/admin.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/api_key.py` & `pybanyan-0.29.2/banyan/controllers/api_key.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/audit.py` & `pybanyan-0.29.2/banyan/controllers/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/base.py` & `pybanyan-0.29.2/banyan/controllers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,17 @@
             (['--version', '-v'],
              {'action': 'version',
               'version': VERSION_BANNER}),
             (['--api-url'],
              {'help': 'URL for the Banyan API server. Can also be configured via the BANYAN_API_URL '
                       'environment variable.'}),
             (['--api-key'],
-             {'help': 'API credential used for the authentication to the Banyan API server. Can also be '
-                      'configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment variable.'}),
+             {'help': 'API credential used for the authentication to the Banyan API server. You can also '
+                      'use a personal refresh token as your API credential. Can also be '
+                      'configured via the BANYAN_API_KEY environment variable.'}),
             (['--insecure-tls', '-k'],
              {'action': 'store_true',
              'help': 'Allow connections to API servers with invalid TLS certificates.'}),
             (['--output-format', '-o'],
              {'choices': ['table', 'json', 'yaml'],
               'help': 'desired output format (table, json, yaml)'}),
         ]
```

### Comparing `pybanyan-0.29.1/banyan/controllers/cloud_resource.py` & `pybanyan-0.29.2/banyan/controllers/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/connector.py` & `pybanyan-0.29.2/banyan/controllers/connector.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/device.py` & `pybanyan-0.29.2/banyan/controllers/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             (['serial_number'],
              {
                  'help': 'Serial number of the device.'
              }),
         ])
     def get(self):
         serial_number = self.app.pargs.serial_number
-        device = self._client.find(serial_number)
+        device = self._client.get_single(serial_number)
         device_json = DeviceV2.Schema().dump(device)
         # colorized_json = highlight(policy_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(device_json, handler='json', indent=2, sort_keys=True)
 
     @ex(help='update device attributes to set MDM vendor presence',
         arguments=[
             (['serial_number'],
@@ -61,15 +61,15 @@
                  'required': True,        
                  'help': 'Set MDM vendor name.'        
              })
         ])        
     def update(self):
         # get the device first
         serial_number = self.app.pargs.serial_number
-        device = self._client.find(serial_number)
+        device = self._client.get_single(serial_number)
         device.mdm_present = self.app.pargs.mdm_present.lower() == "true"
         device.mdm_vendor_name = self.app.pargs.mdm_vendor_name
         print(self._client.update(device))
         device_json = DeviceV2.Schema().dump(device)
         self.app.render(device_json, handler='json', indent=2, sort_keys=True)
 
     # TODO: implement /delete_device?Email=X&SerialNumber=Y
```

### Comparing `pybanyan-0.29.1/banyan/controllers/event.py` & `pybanyan-0.29.2/banyan/controllers/event.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/export.py` & `pybanyan-0.29.2/banyan/controllers/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class ExportController(Controller):
     class Meta:
         label = 'export'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'export all objects from an organization'
+        help = '(deprecated) export all objects from an organization'
 
     @property
     def _client(self) -> BanyanApiClient:
         return self.app.client
 
     @ex(help='export all objects from an organization',
         arguments=[
```

### Comparing `pybanyan-0.29.1/banyan/controllers/netagent.py` & `pybanyan-0.29.2/banyan/controllers/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/policy.py` & `pybanyan-0.29.2/banyan/controllers/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class PolicyController(Controller):
     class Meta:
         label = 'policy'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'manage authorization policies for users and workloads'
+        help = 'manage policies for access to resources'
 
     @property
     def _client(self) -> PolicyAPI:
         return self.app.client.policies
 
     @ex(help='list policies')
     def list(self):
@@ -37,15 +37,15 @@
              {
                  'metavar': 'policy_name_or_id',
                  'help': 'Name or ID of the policy to display.'
              }),
         ])
     def get(self):
         info: PolicyInfo = self._client[self.app.pargs.policy_name]
-        policy_json = Policy.Schema().dump(info.policy)
+        policy_json = Policy.Schema().dump(info.policy_spec)
         # colorized_json = highlight(policy_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(policy_json, handler='json', indent=2, sort_keys=True)
 
     @ex(help='create a new policy from a JSON specification',
         arguments=[
             (['policy_spec'],
              {
```

### Comparing `pybanyan-0.29.1/banyan/controllers/role.py` & `pybanyan-0.29.2/banyan/controllers/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class RoleController(Controller):
     class Meta:
         label = 'role'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'manage user and workload roles'
+        help = 'manage roles to classify users and devices'
 
     @property
     def _client(self) -> RoleAPI:
         return self.app.client.roles
 
     @ex(help='list roles')
     def list(self):
@@ -37,15 +37,15 @@
              {
                  'metavar': 'role_name_or_id',
                  'help': 'Name or ID of the role to display.'
              }),
         ])
     def get(self):
         info: RoleInfo = self._client[self.app.pargs.role_name]
-        role_json = Role.Schema().dump(info.role)
+        role_json = Role.Schema().dump(info.role_spec)
         # colorized_json = highlight(policy_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(role_json, handler='json', indent=2, sort_keys=True)
 
     @ex(help='create a new role from a JSON specification',
         arguments=[
             (['role_spec'],
              {
```

### Comparing `pybanyan-0.29.1/banyan/controllers/service.py` & `pybanyan-0.29.2/banyan/controllers/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/service_infra.py` & `pybanyan-0.29.2/banyan/controllers/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/service_tunnel.py` & `pybanyan-0.29.2/banyan/controllers/service_tunnel.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/service_web.py` & `pybanyan-0.29.2/banyan/controllers/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/controllers/shield.py` & `pybanyan-0.29.2/banyan/controllers/shield.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/aws.py` & `pybanyan-0.29.2/banyan/ext/iaas/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/azure_cloud.py` & `pybanyan-0.29.2/banyan/ext/iaas/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/base.py` & `pybanyan-0.29.2/banyan/ext/iaas/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/gcp.py` & `pybanyan-0.29.2/banyan/ext/iaas/gcp.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/oracle_cloud.py` & `pybanyan-0.29.2/banyan/ext/iaas/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/iaas/vmware.py` & `pybanyan-0.29.2/banyan/ext/iaas/vmware.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/idp/azure_ad.py` & `pybanyan-0.29.2/banyan/ext/idp/azure_ad.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/idp/base.py` & `pybanyan-0.29.2/banyan/ext/idp/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/ext/idp/okta.py` & `pybanyan-0.29.2/banyan/ext/idp/okta.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/lib/certs.py` & `pybanyan-0.29.2/banyan/lib/certs.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/lib/cloud/__init__.py` & `pybanyan-0.29.2/banyan/lib/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/lib/cloud/aws.py` & `pybanyan-0.29.2/banyan/lib/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/lib/service.py` & `pybanyan-0.29.2/banyan/lib/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/main.py` & `pybanyan-0.29.2/banyan/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,22 +92,22 @@
             Base,
             UserController,
             ServiceWebController,
             ServiceTunnelController,
             ServiceInfraController,
             RoleController,
             PolicyController,
-            ExportController,
             EventV2Controller,
             DeviceController,
             ConnectorController,
             CloudResourceController,
             AuditController,
             ApiKeyController,
             AccessTierController,
+            ExportController,
             ShieldController,
             ServiceController,
             NetagentController,
         ]
 
 
 class MyAppTest(TestApp, MyApp):
```

### Comparing `pybanyan-0.29.1/banyan/model/__init__.py` & `pybanyan-0.29.2/banyan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/access_tier.py` & `pybanyan-0.29.2/banyan/model/access_tier.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/api_key.py` & `pybanyan-0.29.2/banyan/model/api_key.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/attachment.py` & `pybanyan-0.29.2/banyan/model/attachment.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/audit.py` & `pybanyan-0.29.2/banyan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/cloud_resource.py` & `pybanyan-0.29.2/banyan/model/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/connector.py` & `pybanyan-0.29.2/banyan/model/connector.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/event_v2.py` & `pybanyan-0.29.2/banyan/model/event_v2.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/netagent.py` & `pybanyan-0.29.2/banyan/model/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/policy.py` & `pybanyan-0.29.2/banyan/model/policy.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/role.py` & `pybanyan-0.29.2/banyan/model/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/service.py` & `pybanyan-0.29.2/banyan/model/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/service_infra.py` & `pybanyan-0.29.2/banyan/model/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/service_tunnel.py` & `pybanyan-0.29.2/banyan/model/service_tunnel.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/service_web.py` & `pybanyan-0.29.2/banyan/model/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/shield.py` & `pybanyan-0.29.2/banyan/model/shield.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/trustscore.py` & `pybanyan-0.29.2/banyan/model/trustscore.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/banyan/model/user_device.py` & `pybanyan-0.29.2/banyan/model/user_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,36 @@
     timestamp: datetime = field(metadata={"marshmallow_field": NanoTimestampField(data_key='Timestamp')})
     source: str = field(metadata={'data_key': 'Source'})
     compromised_status: str = field(metadata={'data_key': 'CompromisedStatus'})
     compliant_status: str = field(metadata={'data_key': 'CompliantStatus'})
 
 
 @dataclass
+class UserV2(Resource):
+    class Meta:
+        unknown = EXCLUDE
+
+    username: str = field(metadata={'data_key': 'name'})
+    email: str
+    invited_at: datetime = field(metadata={"marshmallow_field": NanoTimestampField()})
+    created_at: datetime = field(metadata={"marshmallow_field": NanoTimestampField()})
+    last_login: datetime = field(metadata={"marshmallow_field": NanoTimestampField()})
+    status: str
+    roles: List[str] = field(default_factory=list, metadata={'data_key': 'security_roles', 'allow_none': True})
+
+    @property
+    def name(self) -> str:
+        return self.username
+
+    @property
+    def id(self) -> str:
+        return self.email
+
+
+@dataclass
 class User(Resource):
     class Meta:
         unknown = EXCLUDE
 
     username: str = field(metadata={'data_key': 'Name'})
     email: str = field(metadata={'data_key': 'Email'})
     groups: str = field(metadata={'data_key': 'Groups'})
```

### Comparing `pybanyan-0.29.1/pybanyan.egg-info/PKG-INFO` & `pybanyan-0.29.2/pybanyan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.29.1
+Version: 0.29.2
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
@@ -40,47 +40,47 @@
 $ pip install -r requirements.txt
 $ python setup.py install --user
 ```
 
 ## Usage
 
 This package contains both an API client and a CLI tool.
-To use either one, you need to [generate] an API token from the Banyan Command Center.
+To use either one, you need to [generate][docs] an API credential from the Banyan Command Center.
 
 ### API library
 
-Here's a sample script that uses the library to print the names of every service registered in Banyan:
+Here's a sample script that uses the library to print the names of every hosted website service registered in Banyan:
 
 ```python
 from banyan.api import BanyanApiClient
 
 c = BanyanApiClient()
-for service in c.services.list():
+for service in c.services_web.list():
     print(service.name)
 ```
 
 Output:
 ```console
 $ python examples/list_services.py
 jira
 jupyter
 kube
 mysql
 rds-mysql
 rds-pgsql
 ```
 
-The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
+The `BanyanApiClient` class accepts optional arguments to specify the API server and API credential. If not provided, 
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY` (you can also use a personal refresh token as your API credential.
 
-Full API documentation will be available soon.
+Full API documentation is available in the [docs].
 
 ### Banyan CLI tool
 
-Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential in the `api_key` field (you can also use a personal refresh token as your API credential):
 
 ```ini
 [banyan]
 api_url = https://net.banyanops.com
 api_key = MY_API_KEY
 ```
 
@@ -96,15 +96,15 @@
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           full application debug mode
   -q, --quiet           suppress all console output
   --version, -v         show program's version number and exit
   --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
-  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY environment
                         variable.
   --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
   --output-format {table,json,yaml}, -o {table,json,yaml}
                         desired output format (table, json, yaml)
 
 Commands:
   {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
@@ -126,16 +126,16 @@
     service-web         manage hosted website services
     user                manage users
 ```
 
 Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
 
 ```console
-$ banyan service
-usage: banyan service [-h]
+$ banyan service-web
+usage: banyan service-web [-h]
                       {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
                       ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 sub-commands:
@@ -152,16 +152,16 @@
     update              update an existing service from a JSON specification
 ```
 
 To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
 For example:
 
 ```console
-$ banyan service attach-policy --help
-usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
+$ banyan service-web attach-policy --help
+usage: banyan service-web attach-policy [-h] [--permissive] [--enforcing]
                                     service_name_or_id policy_name_or_id
 
 positional arguments:
   service_name_or_id  Name or ID of the service to attach a policy to.
   policy_name_or_id   Name or ID of the policy to attach to the service.
 
 optional arguments:
@@ -203,11 +203,11 @@
 issues with the library, please create a new [issue in Github][github-issue].
 
 ## Contributions
 
 We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
 workflow][github-pr].
 
-[generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
+[docs]: https://docs.banyansecurity.io/docs/api-guide/introduction/
 [github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
 [github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
 [devel]: https://pybanyan.readthedocs.io/development.html
```

### Comparing `pybanyan-0.29.1/pybanyan.egg-info/SOURCES.txt` & `pybanyan-0.29.2/pybanyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.1/setup.py` & `pybanyan-0.29.2/setup.py`

 * *Files identical despite different names*

