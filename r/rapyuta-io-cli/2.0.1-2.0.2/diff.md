# Comparing `tmp/rapyuta-io-cli-2.0.1.tar.gz` & `tmp/rapyuta-io-cli-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-2.0.1.tar", last modified: Wed Apr 19 11:05:21 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-2.0.2.tar", last modified: Thu Apr 20 12:39:59 2023, max compression
```

## Comparing `rapyuta-io-cli-2.0.1.tar` & `rapyuta-io-cli-2.0.2.tar`

### file list

```diff
@@ -1,222 +1,200 @@
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)    11357 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/LICENSE
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2736 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/PKG-INFO
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2453 2023-04-04 05:52:38.000000 rapyuta-io-cli-2.0.1/README.md
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2736 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/PKG-INFO
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     5457 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 pallab    (1000) pallab    (1000)        1 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 pallab    (1000) pallab    (1000)       45 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/entry_points.txt
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      438 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/requires.txt
--rw-rw-r--   0 pallab    (1000) pallab    (1000)        7 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/top_level.txt
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/riocli/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      728 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      675 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/__main__.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/riocli/apply/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3798 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1446 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/explain.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/apply/manifests/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      451 2022-12-20 12:13:39.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/04-build-catkin.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      524 2022-12-20 12:13:39.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/05-build-docker.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      348 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/06-build-docker-ros.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      206 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/07-device-preinstalled.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      194 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/08-device-docker.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      895 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/09-cloud-routed-network.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      246 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/10-device-routed-network.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      212 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/11-cloud-native-network.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      246 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/12-device-native-network.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      696 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/13-device-package-with-rosbag.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      910 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/14-cloud-package-with-rosbag.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      530 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/15-device-deployment-no-override-options.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      773 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/16-device-deployment-with-override-options.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      582 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/17-device-deployment-with-on-demand-options.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      915 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/deployment.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      273 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/device-with-both-runtimes.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      121 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/disk.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      171 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/managedservice.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1188 2023-04-10 10:43:41.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/package.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      133 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/project.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      802 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/secret.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      102 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/static-route.yaml
--rw-rw-r--   0 pallab    (1000) pallab    (1000)    15225 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/parse.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     8142 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/apply/resolver.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1697 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/template.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1938 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/auth/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1386 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/auth/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2524 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/login.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1015 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/logout.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1130 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/refresh_token.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2567 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/staging.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      911 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/status.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1320 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/auth/token.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2309 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/util.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2723 2023-04-19 11:03:19.000000 rapyuta-io-cli-2.0.1/riocli/bootstrap.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/build/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1415 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/build/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3513 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1394 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3644 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/import_build.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4889 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1767 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1807 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/logs.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3191 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/build/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1667 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/trigger.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1884 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/build/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/chart/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1295 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2342 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/apply.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3182 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/chart.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2138 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1069 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/info.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1328 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1208 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/search.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2303 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/completion/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1361 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/completion/__init__.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/config/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1100 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/config/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3519 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/config/config.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/deployment/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1544 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/deployment/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1487 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4423 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/deployment/errors.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2820 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2278 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2352 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/logs.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)    14700 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/deployment/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      887 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/run.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2495 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/ssh.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1113 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/status.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     5648 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/util.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1821 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/wait.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/device/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1903 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/device/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4447 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/config.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2824 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1404 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1645 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/device/deployment.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1313 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/execute.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     6340 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/files.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1585 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4083 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/label.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1407 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3301 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/metric.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2739 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/device/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1268 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/device/onboard.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/device/tools/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1313 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2517 2023-04-16 11:13:46.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/device_init.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1626 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/forward.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1461 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/rapyuta_logs.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1735 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/scp.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3281 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/service.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3141 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/ssh.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2669 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/util.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3736 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/topic.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3878 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/disk/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1101 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/disk/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1553 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/disk/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1414 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1414 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3100 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/disk/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2821 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/exceptions/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      892 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/exceptions/__init__.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/managedservice/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1326 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1283 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1398 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1316 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/list_providers.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2037 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3977 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/marketplace/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1172 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1569 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4032 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/install.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1597 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3365 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/model/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)       36 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/model/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     5810 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/model/base.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/network/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1296 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/network/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2086 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1916 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1500 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2430 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1959 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/logs.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4062 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2676 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/native_network.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3184 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/routed_network.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     6168 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/package/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1332 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/package/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1472 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/package/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1554 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1390 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/package/deployment.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2347 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2447 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     9441 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/package/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2204 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/parameter/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1628 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2969 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/parameter/apply.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1483 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3560 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/diff.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2151 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/download.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1187 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2076 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/upload.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2587 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/utils.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/project/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1296 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1642 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1413 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2076 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1806 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1814 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/project/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1231 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/project/select.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3816 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/rosbag/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1019 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     4323 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/blob.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)    11554 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/job.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      162 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/secret/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1298 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/secret/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2436 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1406 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1503 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/docker_secret.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3442 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/import_secret.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1649 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1965 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3023 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/secret/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2779 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/source_secret.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2031 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/secret/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/shell/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2040 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/shell/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      719 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/shell/prompt.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/static_route/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1415 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/static_route/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1148 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/create.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1478 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/delete.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1977 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/inspect.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1028 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/static_route/list.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1889 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/static_route/model.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1158 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/static_route/open.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2418 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/static_route/util.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/usergroup/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)        0 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/usergroup/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)        0 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/usergroup/list.py
-drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/utils/
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     3381 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/__init__.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)      944 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/utils/context.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     2378 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/utils/execute.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1357 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/utils/mermaid.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1607 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/utils/selector.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1602 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/spinner.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1929 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/utils/ssh_tunnel.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1094 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/validate.py
--rw-rw-r--   0 pallab    (1000) pallab    (1000)       38 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/setup.cfg
--rw-rw-r--   0 pallab    (1000) pallab    (1000)     1627 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.572095 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.572095 rapyuta-io-cli-2.0.2/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.576094 rapyuta-io-cli-2.0.2/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15225 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.576094 rapyuta-io-cli-2.0.2/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.584095 rapyuta-io-cli-2.0.2/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14705 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3977 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.600095 rapyuta-io-cli-2.0.2/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.600095 rapyuta-io-cli-2.0.2/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/usergroup/list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3381 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/setup.py
```

### Comparing `rapyuta-io-cli-2.0.1/PKG-INFO` & `rapyuta-io-cli-2.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: rapyuta-io-cli
-Version: 2.0.1
-Summary: Rapyuta.io CLI Python command line application.
-Home-page: http://docs.rapyuta.io
-Author: Rapyuta Robotics
-Author-email: opensource@rapyuta-robotics.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Rapyuta CLI
 
 Rapyuta CLI exposes features of Rapyuta.io platform on the command-line.
 
 The application is written in Python 3 and it is distributed through PyPI for
 Python 3 environments.
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/__main__.py` & `rapyuta-io-cli-2.0.2/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/explain.py` & `rapyuta-io-cli-2.0.2/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/parse.py` & `rapyuta-io-cli-2.0.2/riocli/apply/parse.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/resolver.py` & `rapyuta-io-cli-2.0.2/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/template.py` & `rapyuta-io-cli-2.0.2/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/apply/util.py` & `rapyuta-io-cli-2.0.2/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/login.py` & `rapyuta-io-cli-2.0.2/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/logout.py` & `rapyuta-io-cli-2.0.2/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/refresh_token.py` & `rapyuta-io-cli-2.0.2/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/staging.py` & `rapyuta-io-cli-2.0.2/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/status.py` & `rapyuta-io-cli-2.0.2/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/token.py` & `rapyuta-io-cli-2.0.2/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/auth/util.py` & `rapyuta-io-cli-2.0.2/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/bootstrap.py` & `rapyuta-io-cli-2.0.2/riocli/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/create.py` & `rapyuta-io-cli-2.0.2/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/delete.py` & `rapyuta-io-cli-2.0.2/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/import_build.py` & `rapyuta-io-cli-2.0.2/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/list.py` & `rapyuta-io-cli-2.0.2/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/logs.py` & `rapyuta-io-cli-2.0.2/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/model.py` & `rapyuta-io-cli-2.0.2/riocli/build/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Build as v1Build, Client, BuildOptions, CatkinOption
 
 from riocli.model import Model
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Build(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/trigger.py` & `rapyuta-io-cli-2.0.2/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/build/util.py` & `rapyuta-io-cli-2.0.2/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/apply.py` & `rapyuta-io-cli-2.0.2/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/chart.py` & `rapyuta-io-cli-2.0.2/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/delete.py` & `rapyuta-io-cli-2.0.2/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/info.py` & `rapyuta-io-cli-2.0.2/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/list.py` & `rapyuta-io-cli-2.0.2/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/search.py` & `rapyuta-io-cli-2.0.2/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/chart/util.py` & `rapyuta-io-cli-2.0.2/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/completion/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/config/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/config/config.py` & `rapyuta-io-cli-2.0.2/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/delete.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/errors.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/list.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/logs.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/model.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
 from riocli.deployment.errors import ERRORS
 from riocli.deployment.util import add_mount_volume_provision_config
 from riocli.model import Model
 from riocli.package.util import find_package_guid
 from riocli.static_route.util import find_static_route_guid
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Deployment(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/run.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/run.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/ssh.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/status.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/util.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/deployment/wait.py` & `rapyuta-io-cli-2.0.2/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/config.py` & `rapyuta-io-cli-2.0.2/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/create.py` & `rapyuta-io-cli-2.0.2/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/delete.py` & `rapyuta-io-cli-2.0.2/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/deployment.py` & `rapyuta-io-cli-2.0.2/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/execute.py` & `rapyuta-io-cli-2.0.2/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/files.py` & `rapyuta-io-cli-2.0.2/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/label.py` & `rapyuta-io-cli-2.0.2/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/list.py` & `rapyuta-io-cli-2.0.2/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/metric.py` & `rapyuta-io-cli-2.0.2/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/model.py` & `rapyuta-io-cli-2.0.2/riocli/device/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 import typing
 
 from rapyuta_io import Client
 from rapyuta_io.clients.device import Device as v1Device, DevicePythonVersion
 
 from riocli.model import Model
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Device(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/onboard.py` & `rapyuta-io-cli-2.0.2/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/device_init.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/forward.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/scp.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/service.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/ssh.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/tools/util.py` & `rapyuta-io-cli-2.0.2/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/topic.py` & `rapyuta-io-cli-2.0.2/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/device/util.py` & `rapyuta-io-cli-2.0.2/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/create.py` & `rapyuta-io-cli-2.0.2/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/delete.py` & `rapyuta-io-cli-2.0.2/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/list.py` & `rapyuta-io-cli-2.0.2/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/model.py` & `rapyuta-io-cli-2.0.2/riocli/disk/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import click_spinner
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.utils.rest_client import HttpMethod
 
 from riocli.disk.util import _api_call
 from riocli.model import Model
-from riocli.utils.validate import load_schema, validate_manifest
+from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class Disk(Model):
     def find_object(self, client: Client) -> typing.Any:
         _, disk = self.rc.find_depends({'kind': 'disk', 'nameOrGUID': self.metadata.name})
         if not disk:
             return False
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/disk/util.py` & `rapyuta-io-cli-2.0.2/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/exceptions/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/list.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/model.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import typing
 
 from munch import munchify
 from rapyuta_io import Client
 
 from riocli.managedservice.util import ManagedServicesClient
 from riocli.model import Model
-from riocli.utils.validate import load_schema, validate_manifest
+from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class ManagedService(Model):
     def find_object(self, client: Client) -> typing.Any:
         name = self.metadata.name
         client = ManagedServicesClient()
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/managedservice/util.py` & `rapyuta-io-cli-2.0.2/riocli/managedservice/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/marketplace/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/marketplace/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/marketplace/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/marketplace/install.py` & `rapyuta-io-cli-2.0.2/riocli/marketplace/install.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/marketplace/list.py` & `rapyuta-io-cli-2.0.2/riocli/marketplace/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/marketplace/util.py` & `rapyuta-io-cli-2.0.2/riocli/marketplace/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/model/base.py` & `rapyuta-io-cli-2.0.2/riocli/model/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 from abc import ABC, abstractmethod
 from datetime import datetime
 from shutil import get_terminal_size
-import yaml
-import os
 
 import click
 from munch import Munch, munchify
 from rapyuta_io import Client
-from pathlib import Path
 
 from riocli.project.util import find_project_guid
 
 prompt = ">> {}{}{} [{}]"  # >> msg  spacer  rigth_msg time
 
 DELETE_POLICY_LABEL = 'rapyuta.io/deletionPolicy'
 
-schema_dir = Path('jsonschema')
-
 def message_with_prompt(msg, right_msg="", fg='white', with_time=True):
     columns, _ = get_terminal_size()
     time = datetime.now().isoformat('T')
     spacer = ' ' * (int(columns) - len(msg + right_msg + time) - 12)
     msg = prompt.format(msg, spacer, right_msg, time)
     click.secho(msg, fg=fg)
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/create.py` & `rapyuta-io-cli-2.0.2/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/delete.py` & `rapyuta-io-cli-2.0.2/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/list.py` & `rapyuta-io-cli-2.0.2/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/logs.py` & `rapyuta-io-cli-2.0.2/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/model.py` & `rapyuta-io-cli-2.0.2/riocli/network/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # limitations under the License.
 import typing
 from typing import Union, Any, Dict
 
 from rapyuta_io import Client
 from rapyuta_io.clients.native_network import NativeNetwork, Parameters as NativeNetworkParameters
 from rapyuta_io.clients.routed_network import RoutedNetwork, Parameters as RoutedNetworkParameters
+from rapyuta_io.clients.common_models import Limits
 
 from riocli.model import Model
 from riocli.network.util import find_network_name, NetworkNotFound
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Network(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
@@ -69,14 +70,17 @@
         else:
             device = client.get_device(self.spec.deviceGUID)
             parameters = NativeNetworkParameters(device=device,
                                                  network_interface=self.spec.networkInterface)
 
         return NativeNetwork(self.metadata.name, self.spec.runtime.lower(), self.spec.rosDistro, parameters=parameters)
 
+    def _get_limits(self):
+        return Limits(self.spec.resourceLimits['cpu'], self.spec.resourceLimits['memory'])
+
     def _create_routed_network(self, client: Client) -> RoutedNetwork:
         if self.spec.runtime == 'cloud':
             network = self._create_cloud_routed_network(client)
         else:
             network = self._create_device_routed_network(client)
 
         return network
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/native_network.py` & `rapyuta-io-cli-2.0.2/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/routed_network.py` & `rapyuta-io-cli-2.0.2/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/network/util.py` & `rapyuta-io-cli-2.0.2/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/create.py` & `rapyuta-io-cli-2.0.2/riocli/package/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/delete.py` & `rapyuta-io-cli-2.0.2/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/deployment.py` & `rapyuta-io-cli-2.0.2/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/list.py` & `rapyuta-io-cli-2.0.2/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/model.py` & `rapyuta-io-cli-2.0.2/riocli/package/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import typing
 
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.clients.package import RestartPolicy
 
 from riocli.model import Model
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Package(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/package/util.py` & `rapyuta-io-cli-2.0.2/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/apply.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/delete.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/diff.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/diff.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/download.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/download.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/list.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/upload.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/upload.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/parameter/utils.py` & `rapyuta-io-cli-2.0.2/riocli/parameter/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,17 @@
             continue
 
         if tree_names and each not in tree_names:
             continue
 
         trees.append(each)
 
+    if tree_names and not trees:
+        raise Exception('specified tree names are invalid')
+
     return trees
 
 
 def display_trees(root_dir: str, trees: typing.List[str] = []) -> None:
     for each in trees:
         tree_out = display_tree(os.path.join(root_dir, each), string_rep=True)
         click.secho(tree_out, fg='yellow')
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/create.py` & `rapyuta-io-cli-2.0.2/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/delete.py` & `rapyuta-io-cli-2.0.2/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/list.py` & `rapyuta-io-cli-2.0.2/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/model.py` & `rapyuta-io-cli-2.0.2/riocli/project/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Project as v1Project, Client
 
 from riocli.model import Model
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Project(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/select.py` & `rapyuta-io-cli-2.0.2/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/project/util.py` & `rapyuta-io-cli-2.0.2/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/rosbag/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/rosbag/blob.py` & `rapyuta-io-cli-2.0.2/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/rosbag/job.py` & `rapyuta-io-cli-2.0.2/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/create.py` & `rapyuta-io-cli-2.0.2/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/delete.py` & `rapyuta-io-cli-2.0.2/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/docker_secret.py` & `rapyuta-io-cli-2.0.2/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/import_secret.py` & `rapyuta-io-cli-2.0.2/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/list.py` & `rapyuta-io-cli-2.0.2/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/model.py` & `rapyuta-io-cli-2.0.2/riocli/secret/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import typing
 
 from rapyuta_io import Secret as v1Secret, SecretConfigDocker, \
     SecretConfigSourceBasicAuth, \
     SecretConfigSourceSSHAuth, Client
 
 from riocli.model import Model
-from riocli.utils.validate import load_schema, validate_manifest
+from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class Secret(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/source_secret.py` & `rapyuta-io-cli-2.0.2/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/secret/util.py` & `rapyuta-io-cli-2.0.2/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/shell/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/shell/prompt.py` & `rapyuta-io-cli-2.0.2/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/create.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/delete.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/inspect.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/list.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/model.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 import typing
 
 from rapyuta_io import Client
 from rapyuta_io.clients.static_route import StaticRoute as v1StaticRoute
 
 from riocli.model import Model
-from riocli.utils.validate import validate_manifest, load_schema
+from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class StaticRoute(Model):
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
```

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/open.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/open.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/static_route/util.py` & `rapyuta-io-cli-2.0.2/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/__init__.py` & `rapyuta-io-cli-2.0.2/riocli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/context.py` & `rapyuta-io-cli-2.0.2/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/execute.py` & `rapyuta-io-cli-2.0.2/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/mermaid.py` & `rapyuta-io-cli-2.0.2/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/selector.py` & `rapyuta-io-cli-2.0.2/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/spinner.py` & `rapyuta-io-cli-2.0.2/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-2.0.2/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.1/riocli/utils/validate.py` & `rapyuta-io-cli-2.0.2/riocli/jsonschema/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 @lru_cache(maxsize=None)
 def load_schema(resource: str) -> dict:
     """
     Reads JSON schema yaml and returns a dict.
     """
-    schema_dir = Path('jsonschema')
+    schema_dir = Path(__file__).parent.joinpath('schemas')
     with open(schema_dir.joinpath(resource + "-schema.yaml")) as f:
         return yaml.safe_load(f)
 
 
 def validate_manifest(instance, schema) -> None:
     """
     Validates a manifest against a JSON schema.
```

### Comparing `rapyuta-io-cli-2.0.1/setup.py` & `rapyuta-io-cli-2.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 
 setup(
     name="rapyuta-io-cli",
     packages=find_packages(),
     package_data={
         'riocli': [
-            'apply/manifests/*.yaml'
+            'apply/manifests/*.yaml',
+            'jsonschema/schemas/*.yaml'
         ]
     },
     include_package_data=True,
     entry_points={"console_scripts": ["rio = riocli.bootstrap:cli"]},
     version=version,
     description="Rapyuta.io CLI Python command line application.",
     long_description=long_descr,
```

