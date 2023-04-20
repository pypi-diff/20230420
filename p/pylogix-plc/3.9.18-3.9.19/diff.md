# Comparing `tmp/pylogix-plc-3.9.18.tar.gz` & `tmp/pylogix-plc-3.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogix-plc-3.9.18.tar", last modified: Wed Apr 19 18:09:37 2023, max compression
+gzip compressed data, was "pylogix-plc-3.9.19.tar", last modified: Thu Apr 20 18:43:23 2023, max compression
```

## Comparing `pylogix-plc-3.9.18.tar` & `pylogix-plc-3.9.19.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.145827 pylogix-plc-3.9.18/
--rw-rw-rw-   0        0        0    11357 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/LICENSE.txt
--rw-rw-rw-   0        0        0     5436 2023-04-19 18:09:37.143829 pylogix-plc-3.9.18/PKG-INFO
--rw-rw-rw-   0        0        0     4573 2023-04-19 17:44:52.000000 pylogix-plc-3.9.18/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.090829 pylogix-plc-3.9.18/pylogix/
--rw-rw-rw-   0        0        0      108 2023-04-19 18:09:29.000000 pylogix-plc-3.9.18/pylogix/__init__.py
--rw-rw-rw-   0        0        0    60430 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/eip.py
--rw-rw-rw-   0        0        0    26181 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_comm.py
--rw-rw-rw-   0        0        0    66691 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_device.py
--rw-rw-rw-   0        0        0     4153 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_response.py
--rw-rw-rw-   0        0        0     4026 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_tag.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.137826 pylogix-plc-3.9.18/pylogix_plc.egg-info/
--rw-rw-rw-   0        0        0     5436 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:09:37.146828 pylogix-plc-3.9.18/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-04-19 18:09:20.000000 pylogix-plc-3.9.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.604359 pylogix-plc-3.9.19/
+-rw-rw-rw-   0        0        0      351 2023-04-20 18:43:23.602362 pylogix-plc-3.9.19/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 18:39:38.000000 pylogix-plc-3.9.19/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.535357 pylogix-plc-3.9.19/empty/
+-rw-rw-rw-   0        0        0       45 2023-03-07 06:02:06.000000 pylogix-plc-3.9.19/empty/__init__.py
+-rw-rw-rw-   0        0        0     2007 2023-04-20 18:36:09.000000 pylogix-plc-3.9.19/empty/blank.py
+-rw-rw-rw-   0        0        0       93 2023-04-20 18:34:57.000000 pylogix-plc-3.9.19/empty/empty.py
+-rw-rw-rw-   0        0        0        3 2023-04-20 18:41:56.000000 pylogix-plc-3.9.19/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 18:43:23.594364 pylogix-plc-3.9.19/pylogix_plc.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 18:43:23.000000 pylogix-plc-3.9.19/pylogix_plc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 18:43:23.604359 pylogix-plc-3.9.19/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-04-20 18:43:17.000000 pylogix-plc-3.9.19/setup.py
```

