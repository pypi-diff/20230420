# Comparing `tmp/mss-9.0.0.tar.gz` & `tmp/mss-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-9.0.0.tar", last modified: Tue Apr 18 20:19:43 2023, max compression
+gzip compressed data, was "mss-9.0.1.tar", last modified: Thu Apr 20 05:46:26 2023, max compression
```

## Comparing `mss-9.0.0.tar` & `mss-9.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    11521 2023-04-18 20:18:15.000000 mss-9.0.0/CHANGELOG.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5769 2023-04-18 20:16:57.000000 mss-9.0.0/CHANGES.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      668 2023-04-10 12:52:20.000000 mss-9.0.0/CONTRIBUTORS.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-10 14:19:05.000000 mss-9.0.0/LICENSE.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      276 2023-04-14 22:47:09.000000 mss-9.0.0/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-18 20:19:43.514272 mss-9.0.0/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2110 2023-04-14 22:55:26.000000 mss-9.0.0/README.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       43 2023-04-11 07:35:16.000000 mss-9.0.0/dev-requirements.txt
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.506272 mss-9.0.0/docs/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/docs/source/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8757 2023-04-18 20:16:41.000000 mss-9.0.0/docs/source/api.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-15 20:14:16.000000 mss-9.0.0/docs/source/conf.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      858 2023-04-10 20:36:40.000000 mss-9.0.0/docs/source/developers.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/docs/source/examples/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/callback.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/custom_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-9.0.0/docs/source/examples/fps.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-9.0.0/docs/source/examples/fps_multiprocessing.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/from_pil_tuple.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/linux_display_keyword.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/opencv_numpy.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/part_of_screen.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/part_of_screen_monitor_2.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/pil.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/pil_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     4332 2022-10-27 01:33:30.000000 mss-9.0.0/docs/source/examples.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1689 2023-04-10 19:48:35.000000 mss-9.0.0/docs/source/index.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      494 2022-10-27 01:33:30.000000 mss-9.0.0/docs/source/installation.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      735 2023-04-09 20:16:52.000000 mss-9.0.0/docs/source/support.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2216 2023-04-09 20:16:52.000000 mss-9.0.0/docs/source/usage.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3293 2023-04-09 22:30:36.000000 mss-9.0.0/docs/source/where.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2439 2023-04-18 20:19:43.514272 mss-9.0.0/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-9.0.0/setup.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-18 20:16:57.000000 mss-9.0.0/src/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-15 20:54:55.000000 mss-9.0.0/src/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7430 2023-04-18 20:16:16.000000 mss-9.0.0/src/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    16967 2023-04-18 20:16:30.000000 mss-9.0.0/src/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/py.typed
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/screenshot.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-15 20:55:26.000000 mss-9.0.0/src/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8818 2023-04-15 21:57:39.000000 mss-9.0.0/src/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1647 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/top_level.txt
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/src/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1629 2023-04-15 22:58:23.000000 mss-9.0.0/src/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/src/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/res/monitor-1024x768.raw.zip
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      508 2023-04-15 22:57:30.000000 mss-9.0.0/src/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1517 2023-04-15 22:57:30.000000 mss-9.0.0/src/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5439 2023-04-15 20:13:59.000000 mss-9.0.0/src/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6612 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1366 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_issue_220.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3470 2023-04-15 20:13:59.000000 mss-9.0.0/src/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6674 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2920 2023-04-15 21:55:33.000000 mss-9.0.0/src/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      101 2023-04-16 08:23:38.000000 mss-9.0.0/tests-requirements.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.812763 mss-9.0.1/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    11604 2023-04-20 05:45:55.000000 mss-9.0.1/CHANGELOG.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5769 2023-04-20 05:03:07.000000 mss-9.0.1/CHANGES.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      668 2023-04-10 12:52:20.000000 mss-9.0.1/CONTRIBUTORS.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-10 14:19:05.000000 mss-9.0.1/LICENSE.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      276 2023-04-14 22:47:09.000000 mss-9.0.1/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-20 05:46:26.812763 mss-9.0.1/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2110 2023-04-14 22:55:26.000000 mss-9.0.1/README.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       43 2023-04-11 07:35:16.000000 mss-9.0.1/dev-requirements.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.804763 mss-9.0.1/docs/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.808763 mss-9.0.1/docs/source/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8757 2023-04-18 20:16:41.000000 mss-9.0.1/docs/source/api.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-15 20:14:16.000000 mss-9.0.1/docs/source/conf.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      858 2023-04-10 20:36:40.000000 mss-9.0.1/docs/source/developers.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.808763 mss-9.0.1/docs/source/examples/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/callback.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/custom_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-9.0.1/docs/source/examples/fps.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-9.0.1/docs/source/examples/fps_multiprocessing.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/from_pil_tuple.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/linux_display_keyword.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/opencv_numpy.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/part_of_screen.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/part_of_screen_monitor_2.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/pil.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2023-04-10 11:55:20.000000 mss-9.0.1/docs/source/examples/pil_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     4332 2022-10-27 01:33:30.000000 mss-9.0.1/docs/source/examples.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1689 2023-04-10 19:48:35.000000 mss-9.0.1/docs/source/index.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      494 2022-10-27 01:33:30.000000 mss-9.0.1/docs/source/installation.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      735 2023-04-09 20:16:52.000000 mss-9.0.1/docs/source/support.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2216 2023-04-09 20:16:52.000000 mss-9.0.1/docs/source/usage.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3293 2023-04-09 22:30:36.000000 mss-9.0.1/docs/source/where.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2439 2023-04-20 05:46:26.812763 mss-9.0.1/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-9.0.1/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.808763 mss-9.0.1/src/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.812763 mss-9.0.1/src/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-18 20:20:34.000000 mss-9.0.1/src/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-20 05:45:52.000000 mss-9.0.1/src/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-15 20:54:55.000000 mss-9.0.1/src/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7430 2023-04-18 20:16:16.000000 mss-9.0.1/src/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-14 22:47:09.000000 mss-9.0.1/src/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-14 22:47:09.000000 mss-9.0.1/src/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    16967 2023-04-18 20:16:30.000000 mss-9.0.1/src/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-04-14 22:47:09.000000 mss-9.0.1/src/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:47:09.000000 mss-9.0.1/src/mss/py.typed
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-14 22:47:09.000000 mss-9.0.1/src/mss/screenshot.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-15 20:55:26.000000 mss-9.0.1/src/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8818 2023-04-15 21:57:39.000000 mss-9.0.1/src/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.812763 mss-9.0.1/src/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-20 05:46:26.000000 mss-9.0.1/src/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1647 2023-04-20 05:46:26.000000 mss-9.0.1/src/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-20 05:46:26.000000 mss-9.0.1/src/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-20 05:46:26.000000 mss-9.0.1/src/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-20 05:46:26.000000 mss-9.0.1/src/mss.egg-info/top_level.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.812763 mss-9.0.1/src/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1629 2023-04-15 22:58:23.000000 mss-9.0.1/src/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-20 05:46:26.812763 mss-9.0.1/src/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/res/monitor-1024x768.raw.zip
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      508 2023-04-15 22:57:30.000000 mss-9.0.1/src/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1517 2023-04-15 22:57:30.000000 mss-9.0.1/src/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5439 2023-04-15 20:13:59.000000 mss-9.0.1/src/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7275 2023-04-20 05:45:52.000000 mss-9.0.1/src/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1366 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3470 2023-04-15 20:13:59.000000 mss-9.0.1/src/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6674 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-14 22:47:09.000000 mss-9.0.1/src/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2920 2023-04-15 21:55:33.000000 mss-9.0.1/src/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      101 2023-04-16 08:23:38.000000 mss-9.0.1/tests-requirements.txt
```

### Comparing `mss-9.0.0/CHANGELOG.md` & `mss-9.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # History
 
 See Git checking messages for full history.
 
+## 9.0.1 (2023/04/20)
+- CLI: fixed entry point not taking into account arguments
+
 ## 9.0.0 (2023/04/18)
 - Linux: add failure handling to `XOpenDisplay()` call (fixes #246)
-- Mac: tiny improvement in moniors finding
+- Mac: tiny improvement in monitors finding
 - Windows: refactored how internal handles are stored (fixes #198)
 - Windows: removed side effects when leaving the context manager, resources are all freed (fixes #209)
 - CI: run tests via `xvfb-run` on GitHub Actions (#248)
 - tests: enhance `test_get_pixels.py`, and try to fix a random failure at the same time (related to #251)
 - tests: use `PyVirtualDisplay` instead of `xvfbwrapper` (#249)
 - tests: automatic rerun in case of failure (related to #251)
 - :heart: contributors: @mgorny, @CTPaHHuK-HEbA
```

### Comparing `mss-9.0.0/CHANGES.md` & `mss-9.0.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/CONTRIBUTORS.md` & `mss-9.0.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/LICENSE.txt` & `mss-9.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/PKG-INFO` & `mss-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 9.0.0
+Version: 9.0.1
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-9.0.0/README.md` & `mss-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/api.rst` & `mss-9.0.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/conf.py` & `mss-9.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/developers.rst` & `mss-9.0.1/docs/source/developers.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/callback.py` & `mss-9.0.1/docs/source/examples/callback.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/custom_cls_image.py` & `mss-9.0.1/docs/source/examples/custom_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/fps.py` & `mss-9.0.1/docs/source/examples/fps.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/fps_multiprocessing.py` & `mss-9.0.1/docs/source/examples/fps_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/from_pil_tuple.py` & `mss-9.0.1/docs/source/examples/from_pil_tuple.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/opencv_numpy.py` & `mss-9.0.1/docs/source/examples/opencv_numpy.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/part_of_screen.py` & `mss-9.0.1/docs/source/examples/part_of_screen.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/part_of_screen_monitor_2.py` & `mss-9.0.1/docs/source/examples/part_of_screen_monitor_2.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/pil.py` & `mss-9.0.1/docs/source/examples/pil.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples/pil_pixels.py` & `mss-9.0.1/docs/source/examples/pil_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/examples.rst` & `mss-9.0.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/index.rst` & `mss-9.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/support.rst` & `mss-9.0.1/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/usage.rst` & `mss-9.0.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/docs/source/where.rst` & `mss-9.0.1/docs/source/where.rst`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/setup.cfg` & `mss-9.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mss
-version = 9.0.0
+version = 9.0.1
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
```

### Comparing `mss-9.0.0/src/mss/__init__.py` & `mss-9.0.1/src/mss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "9.0.0"
+__version__ = "9.0.1"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
```

### Comparing `mss-9.0.0/src/mss/__main__.py` & `mss-9.0.1/src/mss/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import os.path
+import sys
 from argparse import ArgumentParser
 
 from . import __version__
 from .exception import ScreenShotError
 from .factory import mss
 from .tools import to_png
 
 
 def main(*args: str) -> int:
     """Main logic."""
 
-    cli_args = ArgumentParser()
+    cli_args = ArgumentParser(prog="mss")
     cli_args.add_argument(
         "-c",
         "--coordinates",
         default="",
         type=str,
         help="the part of the screen to capture: top, left, width, height",
     )
@@ -38,15 +39,15 @@
         "--quiet",
         default=False,
         action="store_true",
         help="do not print created files",
     )
     cli_args.add_argument("-v", "--version", action="version", version=__version__)
 
-    options = cli_args.parse_args(args)
+    options = cli_args.parse_args(args or None)
     kwargs = {"mon": options.monitor, "output": options.output}
     if options.coordinates:
         try:
             top, left, width, height = options.coordinates.split(",")
         except ValueError:
             print("Coordinates syntax: top, left, width, height")
             return 2
@@ -76,10 +77,8 @@
     except ScreenShotError:
         if options.quiet:
             return 1
         raise
 
 
 if __name__ == "__main__":  # pragma: nocover
-    import sys
-
-    sys.exit(main(*sys.argv[1:]))
+    sys.exit(main())
```

### Comparing `mss-9.0.0/src/mss/base.py` & `mss-9.0.1/src/mss/base.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/darwin.py` & `mss-9.0.1/src/mss/darwin.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/factory.py` & `mss-9.0.1/src/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/linux.py` & `mss-9.0.1/src/mss/linux.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/screenshot.py` & `mss-9.0.1/src/mss/screenshot.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/tools.py` & `mss-9.0.1/src/mss/tools.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss/windows.py` & `mss-9.0.1/src/mss/windows.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/mss.egg-info/PKG-INFO` & `mss-9.0.1/src/mss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 9.0.0
+Version: 9.0.1
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-9.0.0/src/mss.egg-info/SOURCES.txt` & `mss-9.0.1/src/mss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/bench_bgra2rgb.py` & `mss-9.0.1/src/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/bench_general.py` & `mss-9.0.1/src/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/conftest.py` & `mss-9.0.1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/res/monitor-1024x768.raw.zip` & `mss-9.0.1/src/tests/res/monitor-1024x768.raw.zip`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_cls_image.py` & `mss-9.0.1/src/tests/test_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_find_monitors.py` & `mss-9.0.1/src/tests/test_find_monitors.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_get_pixels.py` & `mss-9.0.1/src/tests/test_get_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_gnu_linux.py` & `mss-9.0.1/src/tests/test_gnu_linux.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_implementation.py` & `mss-9.0.1/src/tests/test_implementation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import os
 import os.path
 import platform
-from unittest.mock import patch
+import sys
+from datetime import datetime
+from unittest.mock import Mock, patch
 
 import pytest
 
 import mss.tools
 from mss import mss
+from mss.__main__ import main as entry_point
 from mss.base import MSSBase
 from mss.exception import ScreenShotError
 from mss.screenshot import ScreenShot
 
 
 class MSS0(MSSBase):
     """Nothing implemented."""
@@ -74,104 +77,113 @@
         mss()
     monkeypatch.undo()
 
     error = exc.value.args[0]
     assert error == "System 'chuck norris' not (yet?) implemented."
 
 
+@patch.object(sys, "argv", new=[])  # Prevent side effects while testing
 @pytest.mark.parametrize("with_cursor", [False, True])
 def test_entry_point(with_cursor: bool, capsys):
-    from datetime import datetime
-
-    from mss.__main__ import main as entry_point
-
     def main(*args: str, ret: int = 0) -> None:
         if with_cursor:
             args = args + ("--with-cursor",)
         assert entry_point(*args) == ret
 
     # No arguments
     main()
-    out, _ = capsys.readouterr()
-    for mon, line in enumerate(out.splitlines(), 1):
+    captured = capsys.readouterr()
+    for mon, line in enumerate(captured.out.splitlines(), 1):
         filename = f"monitor-{mon}.png"
         assert line.endswith(filename)
         assert os.path.isfile(filename)
         os.remove(filename)
 
     for opt in ("-m", "--monitor"):
         main(opt, "1")
-        out, _ = capsys.readouterr()
-        assert out.endswith("monitor-1.png\n")
+        captured = capsys.readouterr()
+        assert captured.out.endswith("monitor-1.png\n")
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
 
     for opt in zip(["-m 1", "--monitor=1"], ["-q", "--quiet"]):
         main(*opt)
-        out, _ = capsys.readouterr()
-        assert not out
+        captured = capsys.readouterr()
+        assert not captured.out
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
 
     fmt = "sct-{mon}-{width}x{height}.png"
     for opt in ("-o", "--out"):
         main(opt, fmt)
-        out, _ = capsys.readouterr()
+        captured = capsys.readouterr()
         with mss(display=os.getenv("DISPLAY")) as sct:
-            for mon, (monitor, line) in enumerate(zip(sct.monitors[1:], out.splitlines()), 1):
+            for mon, (monitor, line) in enumerate(zip(sct.monitors[1:], captured.out.splitlines()), 1):
                 filename = fmt.format(mon=mon, **monitor)
                 assert line.endswith(filename)
                 assert os.path.isfile(filename)
                 os.remove(filename)
 
     fmt = "sct_{mon}-{date:%Y-%m-%d}.png"
     for opt in ("-o", "--out"):
         main("-m 1", opt, fmt)
         filename = fmt.format(mon=1, date=datetime.now())
-        out, _ = capsys.readouterr()
-        assert out.endswith(filename + "\n")
+        captured = capsys.readouterr()
+        assert captured.out.endswith(filename + "\n")
         assert os.path.isfile(filename)
         os.remove(filename)
 
     coordinates = "2,12,40,67"
     filename = "sct-2x12_40x67.png"
     for opt in ("-c", "--coordinates"):
         main(opt, coordinates)
-        out, _ = capsys.readouterr()
-        assert out.endswith(filename + "\n")
+        captured = capsys.readouterr()
+        assert captured.out.endswith(filename + "\n")
         assert os.path.isfile(filename)
         os.remove(filename)
 
     coordinates = "2,12,40"
     for opt in ("-c", "--coordinates"):
         main(opt, coordinates, ret=2)
-        out, _ = capsys.readouterr()
-        assert out == "Coordinates syntax: top, left, width, height\n"
+        captured = capsys.readouterr()
+        assert captured.out == "Coordinates syntax: top, left, width, height\n"
 
 
+@patch.object(sys, "argv", new=[])  # Prevent side effects while testing
 @patch("mss.base.MSSBase.monitors", new=[])
 @pytest.mark.parametrize("quiet", [False, True])
 def test_entry_point_error(quiet: bool, capsys):
-    from mss.__main__ import main as entry_point
-
     def main(*args: str) -> int:
         if quiet:
             args = args + ("--quiet",)
         return entry_point(*args)
 
     if quiet:
         assert main() == 1
-        out, err = capsys.readouterr()
-        assert not out
-        assert not err
+        captured = capsys.readouterr()
+        assert not captured.out
+        assert not captured.err
     else:
         with pytest.raises(ScreenShotError):
             main()
 
 
+def test_entry_point_with_no_argument(capsys):
+    # Make sure to fail if arguments are not handled
+    with patch("mss.factory.mss", new=Mock(side_effect=RuntimeError("Boom!"))):
+        with patch.object(sys, "argv", ["mss", "--help"]):
+            with pytest.raises(SystemExit) as exc:
+                entry_point()
+            assert exc.value.code == 0
+
+    captured = capsys.readouterr()
+    assert not captured.err
+    assert "usage: mss" in captured.out
+
+
 def test_grab_with_tuple(pixel_ratio: int):
     left = 100
     top = 100
     right = 500
     lower = 500
     width = right - left  # 400px width
     height = lower - top  # 400px height
```

### Comparing `mss-9.0.0/src/tests/test_issue_220.py` & `mss-9.0.1/src/tests/test_issue_220.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_leaks.py` & `mss-9.0.1/src/tests/test_leaks.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_macos.py` & `mss-9.0.1/src/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_save.py` & `mss-9.0.1/src/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_setup.py` & `mss-9.0.1/src/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_third_party.py` & `mss-9.0.1/src/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_tools.py` & `mss-9.0.1/src/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mss-9.0.0/src/tests/test_windows.py` & `mss-9.0.1/src/tests/test_windows.py`

 * *Files identical despite different names*

