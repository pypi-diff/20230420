# Comparing `tmp/eduvpn_client-4.1.0.tar.gz` & `tmp/eduvpn_client-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eduvpn_client-4.1.0.tar", last modified: Tue Apr 18 14:45:24 2023, max compression
+gzip compressed data, was "eduvpn_client-4.1.1.tar", last modified: Thu Apr 20 08:04:04 2023, max compression
```

## Comparing `eduvpn_client-4.1.0.tar` & `eduvpn_client-4.1.1.tar`

### file list

```diff
@@ -1,1000 +1,1000 @@
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/
--rw-r--r--   0 jerry     (1000) users      (100)    35149 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/LICENSE
--rw-r--r--   0 jerry     (1000) users      (100)      936 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/LICENSE.spdx
--rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/MANIFEST.in
--rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)      662 2023-03-23 15:01:02.000000 eduvpn_client-4.1.0/README.md
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.228278 eduvpn_client-4.1.0/doc/
--rw-r--r--   0 jerry     (1000) users      (100)       17 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/.gitignore
--rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/Makefile
--rw-r--r--   0 jerry     (1000) users      (100)     6119 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/conf.py
--rw-r--r--   0 jerry     (1000) users      (100)     2424 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/developer.rst
--rw-r--r--   0 jerry     (1000) users      (100)     3506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/flow.dia
--rw-r--r--   0 jerry     (1000) users      (100)    32141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/flow.png
--rw-r--r--   0 jerry     (1000) users      (100)      787 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/index.rst
--rw-r--r--   0 jerry     (1000) users      (100)     5941 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/installation.rst
--rw-r--r--   0 jerry     (1000) users      (100)      629 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/doc/knownissues.rst
--rw-r--r--   0 jerry     (1000) users      (100)       80 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/requirements.txt
--rw-r--r--   0 jerry     (1000) users      (100)   201590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/screenshot.png
--rw-r--r--   0 jerry     (1000) users      (100)     2814 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/doc/updating.rst
--rw-r--r--   0 jerry     (1000) users      (100)      700 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/usage.rst
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.231278 eduvpn_client-4.1.0/eduvpn/
--rw-r--r--   0 jerry     (1000) users      (100)       22 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)       71 2023-04-18 09:59:58.000000 eduvpn_client-4.1.0/eduvpn/__main__.py
--rw-r--r--   0 jerry     (1000) users      (100)    21618 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/app.py
--rw-r--r--   0 jerry     (1000) users      (100)    25290 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/cli.py
--rw-r--r--   0 jerry     (1000) users      (100)     1972 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/config.py
--rw-r--r--   0 jerry     (1000) users      (100)     2088 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/connection.py
--rw-r--r--   0 jerry     (1000) users      (100)     2321 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/i18n.py
--rw-r--r--   0 jerry     (1000) users      (100)     4284 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/keyring.py
--rw-r--r--   0 jerry     (1000) users      (100)    27203 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/nm.py
--rw-r--r--   0 jerry     (1000) users      (100)     1139 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/notify.py
--rw-r--r--   0 jerry     (1000) users      (100)     2689 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/ovpn.py
--rw-r--r--   0 jerry     (1000) users      (100)     2977 2023-04-18 10:26:25.000000 eduvpn_client-4.1.0/eduvpn/server.py
--rw-r--r--   0 jerry     (1000) users      (100)     1152 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/settings.py
--rw-r--r--   0 jerry     (1000) users      (100)     1993 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/storage.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.232278 eduvpn_client-4.1.0/eduvpn/ui/
--rw-r--r--   0 jerry     (1000) users      (100)        0 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/eduvpn/ui/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)     1370 2023-04-18 10:06:53.000000 eduvpn_client-4.1.0/eduvpn/ui/__main__.py
--rw-r--r--   0 jerry     (1000) users      (100)     5089 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/app.py
--rw-r--r--   0 jerry     (1000) users      (100)     6541 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/search.py
--rw-r--r--   0 jerry     (1000) users      (100)     3392 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/ui/stats.py
--rw-r--r--   0 jerry     (1000) users      (100)    50856 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/ui/ui.py
--rw-r--r--   0 jerry     (1000) users      (100)     3788 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/utils.py
--rw-r--r--   0 jerry     (1000) users      (100)     7301 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/utils.py
--rw-r--r--   0 jerry     (1000) users      (100)     2229 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/variants.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.233278 eduvpn_client-4.1.0/eduvpn_client.egg-info/
--rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)    39118 2023-04-18 14:45:24.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/SOURCES.txt
--rw-r--r--   0 jerry     (1000) users      (100)        1 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/dependency_links.txt
--rw-r--r--   0 jerry     (1000) users      (100)      193 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/entry_points.txt
--rw-r--r--   0 jerry     (1000) users      (100)      129 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/requires.txt
--rw-r--r--   0 jerry     (1000) users      (100)        7 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/top_level.txt
--rw-r--r--   0 jerry     (1000) users      (100)      362 2023-04-18 14:45:24.401279 eduvpn_client-4.1.0/setup.cfg
--rw-r--r--   0 jerry     (1000) users      (100)     3016 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/setup.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.234278 eduvpn_client-4.1.0/share/applications/
--rw-r--r--   0 jerry     (1000) users      (100)      178 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/applications/org.eduvpn.client.desktop
--rw-r--r--   0 jerry     (1000) users      (100)      208 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/applications/org.letsconnect-vpn.client.desktop
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.234278 eduvpn_client-4.1.0/share/eduvpn/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.235278 eduvpn_client-4.1.0/share/eduvpn/builder/
--rw-r--r--   0 jerry     (1000) users      (100)    79500 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui
--rw-r--r--   0 jerry     (1000) users      (100)    79493 2023-04-17 14:01:52.000000 eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui~
--rw-r--r--   0 jerry     (1000) users      (100)    16139 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/country_codes.json
--rw-r--r--   0 jerry     (1000) users      (100)    41091 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/eduvpn.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.247278 eduvpn_client-4.1.0/share/eduvpn/images/
--rw-r--r--   0 jerry     (1000) users      (100)     2491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle.svg
--rw-r--r--   0 jerry     (1000) users      (100)    23956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    43016 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back.png
--rw-r--r--   0 jerry     (1000) users      (100)     1227 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2026 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down.png
--rw-r--r--   0 jerry     (1000) users      (100)      459 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      554 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      226 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      365 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right.png
--rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected.png
--rw-r--r--   0 jerry     (1000) users      (100)     7683 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    12654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2033 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting.png
--rw-r--r--   0 jerry     (1000) users      (100)     4997 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8431 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default.png
--rw-r--r--   0 jerry     (1000) users      (100)     5315 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected.png
--rw-r--r--   0 jerry     (1000) users      (100)     6892 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    11157 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1068 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     2292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3677 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)     2138 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     4355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     9182 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    14079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3648 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo.png
--rw-r--r--   0 jerry     (1000) users      (100)     7525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    11375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/eduvpn/images/flags/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.395279 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/
--rw-r--r--   0 jerry     (1000) users      (100)      367 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      297 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      384 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      230 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      705 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      871 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      702 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      910 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      660 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1066 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      587 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      750 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      816 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      276 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      812 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      423 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      629 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      529 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      342 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      434 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      457 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      633 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      222 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      584 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      829 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      701 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      786 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      885 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1129 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      350 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      476 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      508 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1144 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      520 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      591 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1734 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      813 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1160 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      241 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      275 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      264 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      738 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1095 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1546 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      710 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      843 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1067 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1465 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      864 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      941 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      826 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      489 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      647 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      860 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1172 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      721 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1547 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      925 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      846 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      716 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      671 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1135 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      403 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      606 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      676 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1890 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      576 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      593 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      613 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      808 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      727 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1059 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      438 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      767 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      810 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      511 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      242 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      225 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      210 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      477 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      579 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      249 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      686 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      775 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      651 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      368 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      598 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      659 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      597 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      698 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      932 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      259 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      232 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      517 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      250 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      229 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      909 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1087 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1852 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      473 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      565 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      878 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      268 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      912 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      596 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      814 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      858 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      574 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      859 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      831 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1194 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      614 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      874 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      560 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      396 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      233 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      513 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      373 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1887 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      626 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1137 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      770 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1136 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      381 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      653 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      528 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      266 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      244 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      388 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      548 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      690 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1031 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1076 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1514 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      298 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      401 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      265 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      898 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1238 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1065 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      494 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      636 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      623 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      959 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1030 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1402 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      622 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      803 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      301 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      818 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      561 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      954 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      952 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      468 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      236 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      707 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      825 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      630 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      605 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      307 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      913 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1131 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      774 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      601 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2243 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      851 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      254 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      361 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      391 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      427 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      482 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      572 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      856 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1086 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      478 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      592 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      248 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      857 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1162 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      352 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      625 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      827 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      764 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      828 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      337 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      177 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      186 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      324 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      804 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      523 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      206 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1085 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1755 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      610 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      480 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      616 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      310 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      353 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      540 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      602 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      895 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      850 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      692 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      269 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      245 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      452 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      526 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      820 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1014 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      234 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      797 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      295 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      559 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      530 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      322 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      545 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      970 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      485 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      317 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      472 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      417 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      765 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1180 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      383 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      440 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      832 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      425 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      631 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      632 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      991 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      563 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      673 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      905 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      577 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1019 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      263 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      557 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      334 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      811 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      762 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      962 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      510 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      645 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      208 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      328 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      393 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      253 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      255 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      406 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      687 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      524 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      837 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1372 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1052 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1672 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      674 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      293 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      502 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      965 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      699 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1150 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1000 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      578 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)      942 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute.png
--rw-r--r--   0 jerry     (1000) users      (100)     3790 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     5404 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      644 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2247 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      312 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)      519 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      985 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1029 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      619 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings.png
--rw-r--r--   0 jerry     (1000) users      (100)     1077 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/icons/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/icons/hicolor/128x128/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/
--rw-r--r--   0 jerry     (1000) users      (100)     9421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)     5083 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/256x256/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/
--rw-r--r--   0 jerry     (1000) users      (100)    24039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)    11183 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/48x48/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/
--rw-r--r--   0 jerry     (1000) users      (100)     2714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)     1739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/512x512/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.397279 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/
--rw-r--r--   0 jerry     (1000) users      (100)    67703 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)    26109 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/letsconnect/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/letsconnect/images/
--rw-r--r--   0 jerry     (1000) users      (100)     1638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/app-icon-circle.svg
--rw-r--r--   0 jerry     (1000) users      (100)     2188 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect.png
--rw-r--r--   0 jerry     (1000) users      (100)     4471 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     7163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration.png
--rw-r--r--   0 jerry     (1000) users      (100)     5498 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8037 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/de_DE/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 jerry     (1000) users      (100)     3669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/eduVPN.mo
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/es_LA/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/
--rw-r--r--   0 jerry     (1000) users      (100)     3696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/eduVPN.mo
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/tests/
--rw-r--r--   0 jerry     (1000) users      (100)        0 2022-09-27 12:47:39.000000 eduvpn_client-4.1.0/tests/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)    16825 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/mock_config.py
--rw-r--r--   0 jerry     (1000) users      (100)      847 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/test_nm.py
--rw-r--r--   0 jerry     (1000) users      (100)     2869 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/test_stats.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.352556 eduvpn_client-4.1.1/
+-rw-r--r--   0 jerry     (1000) users      (100)    35149 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/LICENSE
+-rw-r--r--   0 jerry     (1000) users      (100)      936 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/LICENSE.spdx
+-rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/MANIFEST.in
+-rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-20 08:04:04.352556 eduvpn_client-4.1.1/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2023-03-23 15:01:02.000000 eduvpn_client-4.1.1/README.md
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.198553 eduvpn_client-4.1.1/doc/
+-rw-r--r--   0 jerry     (1000) users      (100)       17 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/.gitignore
+-rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/Makefile
+-rw-r--r--   0 jerry     (1000) users      (100)     6119 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/doc/conf.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2424 2023-04-20 07:48:14.000000 eduvpn_client-4.1.1/doc/developer.rst
+-rw-r--r--   0 jerry     (1000) users      (100)     3506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/flow.dia
+-rw-r--r--   0 jerry     (1000) users      (100)    32141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/flow.png
+-rw-r--r--   0 jerry     (1000) users      (100)      787 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/doc/index.rst
+-rw-r--r--   0 jerry     (1000) users      (100)     4951 2023-04-19 09:11:35.000000 eduvpn_client-4.1.1/doc/installation.rst
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2023-04-19 09:10:57.000000 eduvpn_client-4.1.1/doc/knownissues.rst
+-rw-r--r--   0 jerry     (1000) users      (100)       80 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/requirements.txt
+-rw-r--r--   0 jerry     (1000) users      (100)   201590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/doc/screenshot.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3009 2023-04-19 09:10:18.000000 eduvpn_client-4.1.1/doc/updating.rst
+-rw-r--r--   0 jerry     (1000) users      (100)      700 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/doc/usage.rst
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.200554 eduvpn_client-4.1.1/eduvpn/
+-rw-r--r--   0 jerry     (1000) users      (100)       22 2023-04-20 07:48:14.000000 eduvpn_client-4.1.1/eduvpn/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)       71 2023-04-18 09:59:58.000000 eduvpn_client-4.1.1/eduvpn/__main__.py
+-rw-r--r--   0 jerry     (1000) users      (100)    21618 2023-04-20 07:36:28.000000 eduvpn_client-4.1.1/eduvpn/app.py
+-rw-r--r--   0 jerry     (1000) users      (100)    25290 2023-04-18 13:38:11.000000 eduvpn_client-4.1.1/eduvpn/cli.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1972 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/config.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2088 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/connection.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2321 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/i18n.py
+-rw-r--r--   0 jerry     (1000) users      (100)     4284 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/keyring.py
+-rw-r--r--   0 jerry     (1000) users      (100)    27203 2023-04-20 07:36:28.000000 eduvpn_client-4.1.1/eduvpn/nm.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1139 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/notify.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2689 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/ovpn.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2977 2023-04-18 10:26:25.000000 eduvpn_client-4.1.1/eduvpn/server.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1152 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/settings.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1993 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/storage.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.201554 eduvpn_client-4.1.1/eduvpn/ui/
+-rw-r--r--   0 jerry     (1000) users      (100)        0 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/eduvpn/ui/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1370 2023-04-18 10:06:53.000000 eduvpn_client-4.1.1/eduvpn/ui/__main__.py
+-rw-r--r--   0 jerry     (1000) users      (100)     5089 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/ui/app.py
+-rw-r--r--   0 jerry     (1000) users      (100)     6541 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/ui/search.py
+-rw-r--r--   0 jerry     (1000) users      (100)     3392 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/eduvpn/ui/stats.py
+-rw-r--r--   0 jerry     (1000) users      (100)    50925 2023-04-20 07:48:01.000000 eduvpn_client-4.1.1/eduvpn/ui/ui.py
+-rw-r--r--   0 jerry     (1000) users      (100)     3788 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/ui/utils.py
+-rw-r--r--   0 jerry     (1000) users      (100)     7301 2023-04-17 09:57:40.000000 eduvpn_client-4.1.1/eduvpn/utils.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2229 2023-04-18 13:38:11.000000 eduvpn_client-4.1.1/eduvpn/variants.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.202554 eduvpn_client-4.1.1/eduvpn_client.egg-info/
+-rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-20 08:04:03.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)    39118 2023-04-20 08:04:04.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        1 2023-04-20 08:04:03.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      193 2023-04-20 08:04:03.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/entry_points.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      129 2023-04-20 08:04:03.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/requires.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        7 2023-04-20 08:04:03.000000 eduvpn_client-4.1.1/eduvpn_client.egg-info/top_level.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      362 2023-04-20 08:04:04.353556 eduvpn_client-4.1.1/setup.cfg
+-rw-r--r--   0 jerry     (1000) users      (100)     3016 2023-04-20 07:48:14.000000 eduvpn_client-4.1.1/setup.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.202554 eduvpn_client-4.1.1/share/applications/
+-rw-r--r--   0 jerry     (1000) users      (100)      178 2023-04-18 13:38:11.000000 eduvpn_client-4.1.1/share/applications/org.eduvpn.client.desktop
+-rw-r--r--   0 jerry     (1000) users      (100)      208 2023-04-18 13:38:11.000000 eduvpn_client-4.1.1/share/applications/org.letsconnect-vpn.client.desktop
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.202554 eduvpn_client-4.1.1/share/eduvpn/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.203554 eduvpn_client-4.1.1/share/eduvpn/builder/
+-rw-r--r--   0 jerry     (1000) users      (100)    79500 2023-04-18 13:38:11.000000 eduvpn_client-4.1.1/share/eduvpn/builder/mainwindow.ui
+-rw-r--r--   0 jerry     (1000) users      (100)    79493 2023-04-17 14:01:52.000000 eduvpn_client-4.1.1/share/eduvpn/builder/mainwindow.ui~
+-rw-r--r--   0 jerry     (1000) users      (100)    16139 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/country_codes.json
+-rw-r--r--   0 jerry     (1000) users      (100)    41091 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/eduvpn.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.214554 eduvpn_client-4.1.1/share/eduvpn/images/
+-rw-r--r--   0 jerry     (1000) users      (100)     2491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle.svg
+-rw-r--r--   0 jerry     (1000) users      (100)    23956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    43016 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/back.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1227 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/back@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2026 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/back@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-down.png
+-rw-r--r--   0 jerry     (1000) users      (100)      459 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-down@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      554 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-down@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      226 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right-white.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right-white@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      365 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right-white@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right.png
+-rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/chevron-right@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/cross.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/cross@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/cross@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7683 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    12654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2033 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4997 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8431 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-default.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5315 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-default@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-default@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected.png
+-rw-r--r--   0 jerry     (1000) users      (100)     6892 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11157 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1068 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3677 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2138 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/earth-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     9182 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    14079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3648 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.193554 eduvpn_client-4.1.1/share/eduvpn/images/flags/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.349556 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/
+-rw-r--r--   0 jerry     (1000) users      (100)      367 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      297 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      384 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      230 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      705 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      871 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      702 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      910 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      660 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1066 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      587 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      750 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      816 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      276 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      812 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      423 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      629 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Artsakh@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Artsakh@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Artsakh@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      529 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      342 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      434 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      457 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      633 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      222 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      584 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      829 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      701 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      786 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      885 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1129 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      350 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      476 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      508 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-BO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-BO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-BO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1144 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      520 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      591 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1734 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      813 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1160 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      241 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      275 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      264 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      738 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-AB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-AB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-AB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1095 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1546 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      710 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      843 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1067 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1465 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      864 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      941 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      826 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      489 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      647 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      860 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1172 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      721 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1547 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      925 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      846 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-SK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-SK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      716 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-SK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      671 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1135 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      403 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      606 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      676 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1890 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      576 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      593 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      613 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      808 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      727 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1059 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      438 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      767 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      810 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      511 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      242 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Chechnya@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      225 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Chechnya@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Chechnya@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      210 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      477 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      579 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      249 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      686 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      775 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      651 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      368 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      598 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      659 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      597 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      698 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      932 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      259 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      232 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      517 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/England-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/England-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/England-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      250 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      229 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      909 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1087 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1852 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      473 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      565 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      878 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      268 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      912 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      596 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      814 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-TF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-TF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-TF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      858 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/France-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/France-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/France-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-ENG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-ENG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-ENG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      574 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      859 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-WLS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-WLS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-WLS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      831 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1194 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE-AB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      614 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE-AB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      874 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE-AB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      560 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      396 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      233 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      513 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      373 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1887 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      626 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1137 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      770 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1136 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      381 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      653 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      528 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      266 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      244 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ID@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ID@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ID@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      388 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      548 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      690 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1031 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1076 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1514 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      298 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      401 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      265 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      898 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1238 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1065 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      494 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      636 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      623 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      959 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1030 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1402 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      622 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      803 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      301 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      818 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      561 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      954 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Kurdistan@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Kurdistan@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      952 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Kurdistan@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      468 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      236 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      707 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      825 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      630 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      605 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ME@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      307 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ME@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ME@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      913 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1131 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      774 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ML@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ML@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ML@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      601 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2243 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      851 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      254 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      361 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      391 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      427 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      482 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      572 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      856 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1086 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      478 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      592 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      248 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      857 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1162 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      352 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      625 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      827 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      764 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      828 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      337 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Netherlands Antilles@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Netherlands Antilles@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/OM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/OM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/OM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      177 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Overlay@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      186 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Overlay@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Overlay@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      324 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      804 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      523 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      206 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1085 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1755 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      610 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      480 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      616 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      310 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      353 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      540 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/QA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/QA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/QA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      602 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      895 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      850 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      692 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      269 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      245 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      452 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      526 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      820 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1014 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      234 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      797 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      295 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      559 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      530 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      322 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      545 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      970 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      485 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ST@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ST@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ST@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      317 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      472 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      417 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      765 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1180 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      383 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Sealand@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      440 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Sealand@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Sealand@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Serb Republic@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Serb Republic@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Serb Republic@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/South Ossetia@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/South Ossetia@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/South Ossetia@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      832 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      425 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      631 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      632 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      991 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      563 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      673 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      905 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      577 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1019 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      263 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      557 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      334 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      811 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      762 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      962 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Transnistria@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Transnistria@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Transnistria@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      510 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      645 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      208 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/US@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/US@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      328 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/US@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      393 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      253 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      255 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      406 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      687 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      524 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      837 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1372 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1052 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1672 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      674 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/WS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      293 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/WS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/WS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/XK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/XK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      502 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/XK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/YE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/YE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/YE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      965 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      699 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1150 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/group.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/group@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/group@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1000 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      578 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)      942 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3790 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5404 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/institute@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      644 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2247 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/question-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      312 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)      519 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      985 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/server-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1029 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      619 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1077 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/eduvpn/images/settings@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.193554 eduvpn_client-4.1.1/share/icons/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/icons/hicolor/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.193554 eduvpn_client-4.1.1/share/icons/hicolor/128x128/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.349556 eduvpn_client-4.1.1/share/icons/hicolor/128x128/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)     9421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/128x128/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5083 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.193554 eduvpn_client-4.1.1/share/icons/hicolor/256x256/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.349556 eduvpn_client-4.1.1/share/icons/hicolor/256x256/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)    24039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/256x256/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11183 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/icons/hicolor/48x48/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.350556 eduvpn_client-4.1.1/share/icons/hicolor/48x48/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)     2714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/48x48/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/icons/hicolor/512x512/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.350556 eduvpn_client-4.1.1/share/icons/hicolor/512x512/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)    67703 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/512x512/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)    26109 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/letsconnect/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.351556 eduvpn_client-4.1.1/share/letsconnect/images/
+-rw-r--r--   0 jerry     (1000) users      (100)     1638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/app-icon-circle.svg
+-rw-r--r--   0 jerry     (1000) users      (100)     2188 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/letsconnect.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4471 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/letsconnect@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/letsconnect@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/server-illustration.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5498 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/server-illustration@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8037 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/letsconnect/images/server-illustration@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/locale/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/locale/de_DE/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.351556 eduvpn_client-4.1.1/share/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 jerry     (1000) users      (100)     3669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/locale/de_DE/LC_MESSAGES/eduVPN.mo
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.194553 eduvpn_client-4.1.1/share/locale/es_LA/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.352556 eduvpn_client-4.1.1/share/locale/es_LA/LC_MESSAGES/
+-rw-r--r--   0 jerry     (1000) users      (100)     3696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.1/share/locale/es_LA/LC_MESSAGES/eduVPN.mo
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-20 08:04:04.352556 eduvpn_client-4.1.1/tests/
+-rw-r--r--   0 jerry     (1000) users      (100)        0 2022-09-27 12:47:39.000000 eduvpn_client-4.1.1/tests/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)    16825 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/tests/mock_config.py
+-rw-r--r--   0 jerry     (1000) users      (100)      847 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/tests/test_nm.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2869 2023-04-17 08:56:44.000000 eduvpn_client-4.1.1/tests/test_stats.py
```

### Comparing `eduvpn_client-4.1.0/LICENSE` & `eduvpn_client-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/LICENSE.spdx` & `eduvpn_client-4.1.1/LICENSE.spdx`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/PKG-INFO` & `eduvpn_client-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eduvpn_client
-Version: 4.1.0
+Version: 4.1.1
 Summary: eduVPN client
 Home-page: https://github.com/eduvpn/python-eduvpn-client
 Author: Jeroen Wijenbergh
 Author-email: jeroen.wijenbergh@geant.org
 License: GPL3
 Keywords: vpn openvpn networking security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eduvpn_client-4.1.0/README.md` & `eduvpn_client-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/Makefile` & `eduvpn_client-4.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/conf.py` & `eduvpn_client-4.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/developer.rst` & `eduvpn_client-4.1.1/doc/developer.rst`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 How to make a release
 ---------------------
 
 Prepare the code
 ^^^^^^^^^^^^^^^^
 
-* Determine version number (for example 4.1.0)
+* Determine version number (for example 4.1.1)
 
 * Compose a list of changes (check issue tracker)
 
 * Make sure the test suite runs with python3
 
 * Set version number in ``setup.py``, and ``eduvpn.spec`` and ensure eduvpn-common has the targeted version set
```

### Comparing `eduvpn_client-4.1.0/doc/flow.dia` & `eduvpn_client-4.1.1/doc/flow.dia`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/flow.png` & `eduvpn_client-4.1.1/doc/flow.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/index.rst` & `eduvpn_client-4.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/installation.rst` & `eduvpn_client-4.1.1/doc/installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 .. note::
 
     If your target is not supported you can make an issue on the `GitHub <https://github.com/eduvpn/python-eduvpn-client>`_ and we will see if we can provide it. Right now we only provide `x86_64` packages (we use a compiled dependency), if you want an ARM package for a certain target you can also make an issue.
 
 
 Debian (11) and Ubuntu (22.04 & 22.10)
-=================
+======================================
 
 .. code-block:: console
 
     $ sudo apt install apt-transport-https lsb-release wget
     $ wget -O- https://app.eduvpn.org/linux/v4/deb/app+linux@eduvpn.org.asc | gpg --dearmor | sudo tee /usr/share/keyrings/eduvpn-v4.gpg >/dev/null
     $ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/eduvpn-v4.gpg] https://app.eduvpn.org/linux/v4/deb/ $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/eduvpn-v4.list
     $ sudo apt update
     $ sudo apt install eduvpn-client
 
-Fedora (36 & 37)
-=================
+Fedora (36, 37 & 38)
+====================
 
 .. code-block:: console
 
     $ curl -O https://app.eduvpn.org/linux/v4/rpm/app+linux@eduvpn.org.asc
     $ sudo rpm --import app+linux@eduvpn.org.asc
     $ cat << 'EOF' | sudo tee /etc/yum.repos.d/python-eduvpn-client_v4.repo
     [python-eduvpn-client_v4]
@@ -62,103 +62,73 @@
 
 Arch (Unofficial)
 =================
 
 There is an unofficial package in the `Arch User Repository (AUR) <https://aur.archlinux.org/packages/python-eduvpn-client/>`_.
 
 
-Manual source installation
+Pip installation
 ==========================
+We also provide pip packages. These are useful if your distro is not officially supported in our packaging (yet).
 
 Dependencies
 ------------
 
-To manually install the eduVPN package you first need to satisfy the build requirements.
+To manually install the eduVPN package via Pip you first need to satisfy the dependencies.
 
 For Debian or Ubuntu:
 
 .. code-block:: console
 
-    $ sudo apt install build-essential git make
+    $ sudo apt update
+    $ sudo apt install \
+		gir1.2-nm-1.0 \
+		gir1.2-secret-1 \
+		gir1.2-gtk-3.0 \
+		gir1.2-notify-0.7 \
+		libgirepository1.0-dev \
+		libdbus-glib-1-dev \
+		python3-gi \
+		python3-setuptools \
+		python3-pytest \
+		python3-wheel \
+		python3-dbus \
+		network-manager-openvpn-gnome
 
 For Fedora:
 
 .. code-block:: console
 
-    $ sudo dnf install git make
-
-For Debian or Ubuntu we made a make target to install the required debian packages:
-
-.. code-block:: console
-
-    $ sudo make deb
-
-For Fedora we did the same:
-
-.. code-block:: console
-
-    $ sudo make dnf
-
-You can then continue with installing via e.g. Pip
+    $ sudo dnf install \
+		libnotify \
+		libsecret \
+		gtk3 \
+		python3-dbus \
+		python3-gobject \
+		python3-pytest \
+		python3-cairo-devel \
+		gobject-introspection-devel \
+		cairo-gobject-devel \
+		dbus-python-devel
 
-If you're not installing the rest via Pip, note that since version 4
-of this Linux client, we use the eduvpn-common Go library to provide
-most of the core functionality. Thus these commands cannot provide you
-the complete development dependencies as eduvpn-common is not in the
-official repositories. To install this library manually and to see how it works
-we refer to `their documentation
-<https://eduvpn.github.io/eduvpn-common>`_.
-
-Eduvpn-common, however is available to install with Pip (it includes
-precompiled shared libraries).  The aforementioned repositories
-(e.g. Fedora, Debian) also include the latest stable release of
-eduvpn-common.
-
-Development packages for eduvpn-common and this client will follow later.
-
-Pip
----
+Pip commands
+------------
 
-You can install the client API from pypi:
+You can then continue with installing via Pip:
 
 .. code-block:: console
 
     $ pip install "eduvpn-client[gui]"
 
 Or, if you want to try out the bleeding edge development version:
 
 .. code-block:: console
 
     $ pip install git+https://github.com/eduvpn/python-eduvpn-client.git
 
-.. note::
-
-    This requires the installation of system packages
-    using your distributions package manager. See the previous section for the `Makefile` targets for your system.
-
-
-Development version
--------------------
-
-You first need to obtain the code:
-
-.. code-block:: console
-
-    $ git clone https://github.com/eduvpn/python-eduvpn-client.git
-    $ cd python-eduvpn-client
-
-
-We've made various Makefile targets to quickly get started. For example to start the eduVPN GUI:
-
-.. code-block:: console
-
-    $ make eduvpn-gui
-
-Please have a look in the `Makefile`_ to find out the available targets.
-
 
 Issues
 ======
 
 If you experience any issues you could and should report them at our
 `issue tracker <https://github.com/eduvpn/python-eduvpn-client/issues>`_. Please don't forget to mention your OS,
 method of installation, eduVPN client version and instructions on how to reproduce the problem. If you have a problem
```

### Comparing `eduvpn_client-4.1.0/doc/knownissues.rst` & `eduvpn_client-4.1.1/doc/knownissues.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ============
 Known issues
 ============
 
 This chapter contains some known issues for the Linux client that are not possible or hacky to fix in the client itself
 
 OpenVPN <= 2.5.7 and OpenSSL 3
-=================
+==============================
 
 When your distribution uses OpenSSL 3 and an OpenVPN version before 2.5.8, you might get the following error in the NetworkManager logging after connecting to a server that uses OpenVPN:
 
 .. code-block:: console
 
     $ Cipher BF-CBC not supported
```

### Comparing `eduvpn_client-4.1.0/doc/screenshot.png` & `eduvpn_client-4.1.1/doc/screenshot.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/doc/updating.rst` & `eduvpn_client-4.1.1/doc/updating.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 When upgrading from version 3 to the newest version (currently 4.x), there are some manual steps needed for updating. The main part is that we have moved to a new repository for this major version update. We will go over the distro specific update instructions (distros that are not listed here do not need specific instructions, go to `Installation <./installation.html>`_).
 
 Before you continue, it might be wise to close the client if you have it open. Note that once the new client is installed, you will have to add your servers again.
 
 
 Debian and Ubuntu (both x86_64)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 First we must remove the old files, repository and associated signing keys:
 
 .. code-block:: console
 
     $ rm -r ~/.config/eduvpn
     $ sudo rm /etc/apt/sources.list.d/eduvpn.list
@@ -36,18 +36,25 @@
 
     $ sudo apt install apt-transport-https lsb-release wget
     $ wget -O- https://app.eduvpn.org/linux/v4/deb/app+linux@eduvpn.org.asc | gpg --dearmor | sudo tee /usr/share/keyrings/eduvpn-v4.gpg >/dev/null
     $ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/eduvpn-v4.gpg] https://app.eduvpn.org/linux/v4/deb/ $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/eduvpn-v4.list
     $ sudo apt update
     $ sudo apt upgrade
 
-For other Debian based distros, you can use Pip, see `Pip Installation <./installation.html#pip>`_
+For other Debian based distros, you can use Pip . If you do the upgrade via Pip, remove the old client first with:
+
+.. code-block:: console
+
+    $ sudo apt purge eduvpn-client
+    $ sudo apt autoremove
+
+Then install via Pip, see `Pip Installation <./installation.html#pip-installation>`_
 
 Fedora (36 & 37, both x86_64)
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 First we must remove the old files, repository and associated signing keys:
 
 .. code-block:: console
 
     $ rm -r ~/.config/eduvpn
     $ sudo dnf copr remove @eduvpn/eduvpn-client
```

### Comparing `eduvpn_client-4.1.0/doc/usage.rst` & `eduvpn_client-4.1.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/app.py` & `eduvpn_client-4.1.1/eduvpn/app.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/cli.py` & `eduvpn_client-4.1.1/eduvpn/cli.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/config.py` & `eduvpn_client-4.1.1/eduvpn/config.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/connection.py` & `eduvpn_client-4.1.1/eduvpn/connection.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/i18n.py` & `eduvpn_client-4.1.1/eduvpn/i18n.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/keyring.py` & `eduvpn_client-4.1.1/eduvpn/keyring.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/nm.py` & `eduvpn_client-4.1.1/eduvpn/nm.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/notify.py` & `eduvpn_client-4.1.1/eduvpn/notify.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ovpn.py` & `eduvpn_client-4.1.1/eduvpn/ovpn.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/server.py` & `eduvpn_client-4.1.1/eduvpn/server.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/settings.py` & `eduvpn_client-4.1.1/eduvpn/settings.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/storage.py` & `eduvpn_client-4.1.1/eduvpn/storage.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/__main__.py` & `eduvpn_client-4.1.1/eduvpn/ui/__main__.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/app.py` & `eduvpn_client-4.1.1/eduvpn/ui/app.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/search.py` & `eduvpn_client-4.1.1/eduvpn/ui/search.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/stats.py` & `eduvpn_client-4.1.1/eduvpn/ui/stats.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/ui.py` & `eduvpn_client-4.1.1/eduvpn/ui/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,15 @@
 
     def recreate_profile_combo(self, server_info) -> None:
         # Create a store of profiles
         profile_store = Gtk.ListStore(GObject.TYPE_STRING, GObject.TYPE_PYOBJECT)  # type: ignore
         active_profile = 0
         sorted_profiles = sorted(server_info.profiles.profiles, key=lambda p: str(p))
         for index, profile in enumerate(sorted_profiles):
-            if index == server_info.profiles.current:
+            if server_info.profiles.current is not None and profile.identifier == server_info.profiles.current.identifier:
                 active_profile = index
             profile_store.append([str(profile), profile])  # type: ignore
 
         # Create a new combobox
         # We create a new one every time because Gtk has some weird behaviour regarding the width of the combo box
         # When we add items that are large, the combobox resizes to fit the content
         # However, when we add items again that are all smaller (e.g. for a new server), the combo box does not shrink back
```

### Comparing `eduvpn_client-4.1.0/eduvpn/ui/utils.py` & `eduvpn_client-4.1.1/eduvpn/ui/utils.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/utils.py` & `eduvpn_client-4.1.1/eduvpn/utils.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn/variants.py` & `eduvpn_client-4.1.1/eduvpn/variants.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/eduvpn_client.egg-info/PKG-INFO` & `eduvpn_client-4.1.1/eduvpn_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eduvpn-client
-Version: 4.1.0
+Version: 4.1.1
 Summary: eduVPN client
 Home-page: https://github.com/eduvpn/python-eduvpn-client
 Author: Jeroen Wijenbergh
 Author-email: jeroen.wijenbergh@geant.org
 License: GPL3
 Keywords: vpn openvpn networking security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eduvpn_client-4.1.0/eduvpn_client.egg-info/SOURCES.txt` & `eduvpn_client-4.1.1/eduvpn_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/setup.py` & `eduvpn_client-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from glob import glob
 
 from setuptools import setup, find_packages
 
-__version__ = "4.1.0"
+__version__ = "4.1.1"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 install_requires = [
     'wheel',
```

### Comparing `eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui` & `eduvpn_client-4.1.1/share/eduvpn/builder/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui~` & `eduvpn_client-4.1.1/share/eduvpn/builder/mainwindow.ui~`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/country_codes.json` & `eduvpn_client-4.1.1/share/eduvpn/country_codes.json`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/eduvpn.png` & `eduvpn_client-4.1.1/share/eduvpn/eduvpn.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle.svg` & `eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle.svg`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/app-icon-circle@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/back.png` & `eduvpn_client-4.1.1/share/eduvpn/images/back.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/back@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/back@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/back@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/back@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/chevron-down@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/chevron-right@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/cross@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/cross@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/cross@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/cross@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connected@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-connecting@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-default.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-default@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-default@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/desktop-not-connected@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/earth-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/edu-vpn-logo@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/AZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Artsakh@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Artsakh@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-BO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-BO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BQ-SE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/BZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-BC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-MB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-NU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-ON@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-PE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-QC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-SK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CA-YT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CW@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/CY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DJ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/DZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ER@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ES-CT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ET@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/EU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-MQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-TF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/FR-YT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-SCT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB-Symbol@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE-AB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GE-AB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/GY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/HR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/IO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/JP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/KZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Kurdistan@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Kurdistan@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/LY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/MZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/NZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/OM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/PY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/QA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/RW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SH-HL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ST@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SX@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/SZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Sealand@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/TZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/UG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/VU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@1,5x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/flags/png/ZW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/group@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/group@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/group@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/group@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/institute@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/institute@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/question-icon@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/question-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/server-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/server-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/server-icon@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/server-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/server-icon@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/server-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings@2x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/eduvpn/images/settings@3x.png` & `eduvpn_client-4.1.1/share/eduvpn/images/settings@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/128x128/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/256x256/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/48x48/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/512x512/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.1/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/app-icon-circle.svg` & `eduvpn_client-4.1.1/share/letsconnect/images/app-icon-circle.svg`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect.png` & `eduvpn_client-4.1.1/share/letsconnect/images/letsconnect.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@2x.png` & `eduvpn_client-4.1.1/share/letsconnect/images/letsconnect@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@3x.png` & `eduvpn_client-4.1.1/share/letsconnect/images/letsconnect@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration.png` & `eduvpn_client-4.1.1/share/letsconnect/images/server-illustration.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@2x.png` & `eduvpn_client-4.1.1/share/letsconnect/images/server-illustration@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@3x.png` & `eduvpn_client-4.1.1/share/letsconnect/images/server-illustration@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/eduVPN.mo` & `eduvpn_client-4.1.1/share/locale/de_DE/LC_MESSAGES/eduVPN.mo`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/eduVPN.mo` & `eduvpn_client-4.1.1/share/locale/es_LA/LC_MESSAGES/eduVPN.mo`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/tests/mock_config.py` & `eduvpn_client-4.1.1/tests/mock_config.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/tests/test_nm.py` & `eduvpn_client-4.1.1/tests/test_nm.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.1.0/tests/test_stats.py` & `eduvpn_client-4.1.1/tests/test_stats.py`

 * *Files identical despite different names*

