# Comparing `tmp/osc-fish-complete-0.0.1.tar.gz` & `tmp/osc-fish-complete-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osc-fish-complete-0.0.1.tar", last modified: Fri Apr 10 13:06:46 2020, max compression
+gzip compressed data, was "osc-fish-complete-0.2.0.tar", last modified: Thu Apr 20 04:07:34 2023, max compression
```

## Comparing `osc-fish-complete-0.0.1.tar` & `osc-fish-complete-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 ykky     (899402263) domain users (899400513)        0 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/
--rw-r--r--   0 ykky     (899402263) domain users (899400513)      349 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/PKG-INFO
--rw-r--r--   0 ykky     (899402263) domain users (899400513)       56 2020-04-07 04:52:41.000000 osc-fish-complete-0.0.1/README.md
-drwxr-xr-x   0 ykky     (899402263) domain users (899400513)        0 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete/
--rw-r--r--   0 ykky     (899402263) domain users (899400513)        0 2020-04-10 11:13:07.000000 osc-fish-complete-0.0.1/osc_fish_complete/__init__.py
--rw-r--r--   0 ykky     (899402263) domain users (899400513)     1027 2020-04-10 12:35:55.000000 osc-fish-complete-0.0.1/osc_fish_complete/complete.py
-drwxr-xr-x   0 ykky     (899402263) domain users (899400513)        0 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/
--rw-r--r--   0 ykky     (899402263) domain users (899400513)      349 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/PKG-INFO
--rw-r--r--   0 ykky     (899402263) domain users (899400513)      296 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/SOURCES.txt
--rw-r--r--   0 ykky     (899402263) domain users (899400513)        1 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/dependency_links.txt
--rw-r--r--   0 ykky     (899402263) domain users (899400513)       77 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/entry_points.txt
--rw-r--r--   0 ykky     (899402263) domain users (899400513)       18 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/osc_fish_complete.egg-info/top_level.txt
--rw-r--r--   0 ykky     (899402263) domain users (899400513)      440 2020-04-10 13:06:46.000000 osc-fish-complete-0.0.1/setup.cfg
--rw-r--r--   0 ykky     (899402263) domain users (899400513)       37 2020-04-10 11:16:05.000000 osc-fish-complete-0.0.1/setup.py
+drwxr-xr-x   0 ykky      (1000) ykky      (1000)        0 2023-04-20 04:07:34.579381 osc-fish-complete-0.2.0/
+-rw-r--r--   0 ykky      (1000) ykky      (1000)     1065 2022-10-19 01:42:18.000000 osc-fish-complete-0.2.0/LICENSE
+-rw-r--r--   0 ykky      (1000) ykky      (1000)      499 2023-04-20 04:07:34.579381 osc-fish-complete-0.2.0/PKG-INFO
+-rw-r--r--   0 ykky      (1000) ykky      (1000)      231 2023-04-20 03:14:35.000000 osc-fish-complete-0.2.0/README.md
+drwxr-xr-x   0 ykky      (1000) ykky      (1000)        0 2023-04-20 04:07:34.579381 osc-fish-complete-0.2.0/osc_fish_complete/
+-rw-r--r--   0 ykky      (1000) ykky      (1000)        0 2022-10-19 01:42:18.000000 osc-fish-complete-0.2.0/osc_fish_complete/__init__.py
+-rw-r--r--   0 ykky      (1000) ykky      (1000)     1532 2023-04-20 04:01:52.000000 osc-fish-complete-0.2.0/osc_fish_complete/complete.py
+drwxr-xr-x   0 ykky      (1000) ykky      (1000)        0 2023-04-20 04:07:34.579381 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/
+-rw-r--r--   0 ykky      (1000) ykky      (1000)      499 2023-04-20 04:07:34.000000 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/PKG-INFO
+-rw-r--r--   0 ykky      (1000) ykky      (1000)      304 2023-04-20 04:07:34.000000 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 ykky      (1000) ykky      (1000)        1 2023-04-20 04:07:34.000000 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 ykky      (1000) ykky      (1000)       76 2023-04-20 04:07:34.000000 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/entry_points.txt
+-rw-r--r--   0 ykky      (1000) ykky      (1000)       18 2023-04-20 04:07:34.000000 osc-fish-complete-0.2.0/osc_fish_complete.egg-info/top_level.txt
+-rw-r--r--   0 ykky      (1000) ykky      (1000)      440 2023-04-20 04:07:34.579381 osc-fish-complete-0.2.0/setup.cfg
+-rw-r--r--   0 ykky      (1000) ykky      (1000)       37 2022-10-19 01:42:18.000000 osc-fish-complete-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

