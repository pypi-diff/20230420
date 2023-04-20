# Comparing `tmp/ducc0-0.8.0.tar.gz` & `tmp/ducc0-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducc0-0.8.0.tar", last modified: Fri Jan 15 12:53:31 2021, max compression
+gzip compressed data, was "ducc0-0.9.0.tar", last modified: Tue Mar 16 13:48:28 2021, max compression
```

## Comparing `ducc0-0.8.0.tar` & `ducc0-0.9.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.433414 ducc0-0.8.0/
--rw-r--r--   0 martin    (1000) martin    (1000)     3076 2021-01-15 10:50:00.000000 ducc0-0.8.0/ChangeLog
--rw-r--r--   0 martin    (1000) martin    (1000)    15188 2020-06-19 13:21:06.000000 ducc0-0.8.0/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)     2637 2021-01-14 15:08:48.000000 ducc0-0.8.0/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     8161 2021-01-15 12:53:31.433414 ducc0-0.8.0/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     6534 2020-11-10 20:02:40.000000 ducc0-0.8.0/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.421414 ducc0-0.8.0/ducc0.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     8161 2021-01-15 12:53:31.000000 ducc0-0.8.0/ducc0.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     2232 2021-01-15 12:53:31.000000 ducc0-0.8.0/ducc0.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2021-01-15 12:53:31.000000 ducc0-0.8.0/ducc0.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       14 2021-01-15 12:53:31.000000 ducc0-0.8.0/ducc0.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        6 2021-01-15 12:53:31.000000 ducc0-0.8.0/ducc0.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)      131 2020-11-10 20:02:40.000000 ducc0-0.8.0/pyproject.toml
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.425414 ducc0-0.8.0/python/
--rw-r--r--   0 martin    (1000) martin    (1000)    11113 2021-01-14 15:08:48.000000 ducc0-0.8.0/python/alm.h
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.425414 ducc0-0.8.0/python/demos/
--rw-r--r--   0 martin    (1000) martin    (1000)     4911 2020-12-18 21:10:46.000000 ducc0-0.8.0/python/demos/fft_bench.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6951 2020-06-19 13:21:06.000000 ducc0-0.8.0/python/demos/fft_stress.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3615 2020-06-19 13:21:06.000000 ducc0-0.8.0/python/demos/healpix_perftest.py
--rw-r--r--   0 martin    (1000) martin    (1000)     4679 2020-12-10 08:38:40.000000 ducc0-0.8.0/python/demos/totalconvolve_demo.py
--rw-r--r--   0 martin    (1000) martin    (1000)     2875 2020-06-19 13:21:06.000000 ducc0-0.8.0/python/demos/totalconvolve_usage.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1115 2020-12-04 10:38:25.000000 ducc0-0.8.0/python/ducc.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    24010 2021-01-14 22:09:34.000000 ducc0-0.8.0/python/fft.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    55246 2021-01-15 09:50:04.000000 ducc0-0.8.0/python/gridder_cxx.h
--rw-r--r--   0 martin    (1000) martin    (1000)    13104 2021-01-14 22:21:58.000000 ducc0-0.8.0/python/healpix.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     6934 2021-01-14 22:09:38.000000 ducc0-0.8.0/python/misc.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    10479 2021-01-14 15:36:58.000000 ducc0-0.8.0/python/pointingprovider.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     7991 2020-11-10 20:02:40.000000 ducc0-0.8.0/python/sht.cc
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.425414 ducc0-0.8.0/python/test/
--rw-r--r--   0 martin    (1000) martin    (1000)     9915 2021-01-14 15:08:48.000000 ducc0-0.8.0/python/test/test_fft.py
--rw-r--r--   0 martin    (1000) martin    (1000)     2974 2020-06-19 13:21:06.000000 ducc0-0.8.0/python/test/test_healpix.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3298 2021-01-14 15:08:48.000000 ducc0-0.8.0/python/test/test_pointing.py
--rw-r--r--   0 martin    (1000) martin    (1000)     2885 2020-06-19 13:21:06.000000 ducc0-0.8.0/python/test/test_sht.py
--rw-r--r--   0 martin    (1000) martin    (1000)     8710 2021-01-14 15:08:48.000000 ducc0-0.8.0/python/test/test_totalconvolve.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6913 2021-01-15 10:46:24.000000 ducc0-0.8.0/python/test/test_wgridder.py
--rw-r--r--   0 martin    (1000) martin    (1000)    30687 2021-01-14 15:08:49.000000 ducc0-0.8.0/python/totalconvolve.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    33234 2021-01-14 15:36:58.000000 ducc0-0.8.0/python/totalconvolve.h
--rw-r--r--   0 martin    (1000) martin    (1000)    16798 2021-01-15 09:50:04.000000 ducc0-0.8.0/python/wgridder.cc
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2021-01-15 12:53:31.433414 ducc0-0.8.0/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     4061 2021-01-15 09:50:04.000000 ducc0-0.8.0/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.421414 ducc0-0.8.0/src/
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.421414 ducc0-0.8.0/src/ducc0/
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.425414 ducc0-0.8.0/src/ducc0/bindings/
--rw-r--r--   0 martin    (1000) martin    (1000)     4839 2020-11-14 16:38:57.000000 ducc0-0.8.0/src/ducc0/bindings/pybind_utils.h
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.429414 ducc0-0.8.0/src/ducc0/healpix/
--rw-r--r--   0 martin    (1000) martin    (1000)    40668 2020-11-29 11:56:24.000000 ducc0-0.8.0/src/ducc0/healpix/healpix_base.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    20715 2020-11-27 09:35:11.000000 ducc0-0.8.0/src/ducc0/healpix/healpix_base.h
--rw-r--r--   0 martin    (1000) martin    (1000)     5466 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/healpix/healpix_tables.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     2048 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/healpix/healpix_tables.h
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.429414 ducc0-0.8.0/src/ducc0/infra/
--rw-r--r--   0 martin    (1000) martin    (1000)     2944 2020-11-20 18:25:53.000000 ducc0-0.8.0/src/ducc0/infra/aligned_array.h
--rw-r--r--   0 martin    (1000) martin    (1000)     4151 2021-01-14 15:36:58.000000 ducc0-0.8.0/src/ducc0/infra/bucket_sort.h
--rw-r--r--   0 martin    (1000) martin    (1000)    10296 2020-11-10 20:02:40.000000 ducc0-0.8.0/src/ducc0/infra/communication.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     5953 2020-11-10 20:02:40.000000 ducc0-0.8.0/src/ducc0/infra/communication.h
--rw-r--r--   0 martin    (1000) martin    (1000)     2553 2020-11-28 18:07:54.000000 ducc0-0.8.0/src/ducc0/infra/error_handling.h
--rw-r--r--   0 martin    (1000) martin    (1000)    24287 2021-01-14 15:36:58.000000 ducc0-0.8.0/src/ducc0/infra/mav.h
--rw-r--r--   0 martin    (1000) martin    (1000)     1541 2020-11-10 20:02:40.000000 ducc0-0.8.0/src/ducc0/infra/misc_utils.h
--rw-r--r--   0 martin    (1000) martin    (1000)    18039 2020-11-27 09:29:37.000000 ducc0-0.8.0/src/ducc0/infra/simd.h
--rw-r--r--   0 martin    (1000) martin    (1000)    10002 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/infra/string_utils.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     4885 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/infra/string_utils.h
--rw-r--r--   0 martin    (1000) martin    (1000)     2087 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/infra/system.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     1244 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/infra/system.h
--rw-r--r--   0 martin    (1000) martin    (1000)    14664 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/infra/threading.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     2928 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/infra/threading.h
--rw-r--r--   0 martin    (1000) martin    (1000)     6349 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/infra/timers.h
--rw-r--r--   0 martin    (1000) martin    (1000)     5380 2020-11-23 17:01:18.000000 ducc0-0.8.0/src/ducc0/infra/transpose.h
--rw-r--r--   0 martin    (1000) martin    (1000)     1493 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/infra/types.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     1698 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/infra/types.h
--rw-r--r--   0 martin    (1000) martin    (1000)      569 2021-01-04 20:09:34.000000 ducc0-0.8.0/src/ducc0/infra/useful_macros.h
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.433414 ducc0-0.8.0/src/ducc0/math/
--rw-r--r--   0 martin    (1000) martin    (1000)     2670 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/cmplx.h
--rw-r--r--   0 martin    (1000) martin    (1000)     3101 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/constants.h
--rw-r--r--   0 martin    (1000) martin    (1000)    42816 2020-12-04 14:29:41.000000 ducc0-0.8.0/src/ducc0/math/fft.h
--rw-r--r--   0 martin    (1000) martin    (1000)    59993 2021-01-14 15:19:24.000000 ducc0-0.8.0/src/ducc0/math/fft1d.h
--rw-r--r--   0 martin    (1000) martin    (1000)     2413 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/geom_utils.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     3170 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/geom_utils.h
--rw-r--r--   0 martin    (1000) martin    (1000)     4103 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/gl_integrator.h
--rw-r--r--   0 martin    (1000) martin    (1000)    27166 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/math/gridding_kernel.h
--rw-r--r--   0 martin    (1000) martin    (1000)     6453 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/math/math_utils.h
--rw-r--r--   0 martin    (1000) martin    (1000)     1906 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/pointing.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     2670 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/pointing.h
--rw-r--r--   0 martin    (1000) martin    (1000)     3154 2020-11-10 20:02:40.000000 ducc0-0.8.0/src/ducc0/math/quaternion.h
--rw-r--r--   0 martin    (1000) martin    (1000)    14711 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/rangeset.h
--rw-r--r--   0 martin    (1000) martin    (1000)    14126 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/math/space_filling.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     6331 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/math/space_filling.h
--rw-r--r--   0 martin    (1000) martin    (1000)     3267 2020-12-10 08:38:40.000000 ducc0-0.8.0/src/ducc0/math/unity_roots.h
--rw-r--r--   0 martin    (1000) martin    (1000)     4782 2020-11-10 20:02:40.000000 ducc0-0.8.0/src/ducc0/math/vec3.h
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-01-15 12:53:31.433414 ducc0-0.8.0/src/ducc0/sharp/
--rw-r--r--   0 martin    (1000) martin    (1000)    13732 2021-01-14 15:36:58.000000 ducc0-0.8.0/src/ducc0/sharp/sharp.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     6855 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp.h
--rw-r--r--   0 martin    (1000) martin    (1000)     4886 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_almhelpers.cc
--rw-r--r--   0 martin    (1000) martin    (1000)     4588 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_almhelpers.h
--rw-r--r--   0 martin    (1000) martin    (1000)     3842 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_core.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    37956 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_core_inc.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    12062 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_geomhelpers.cc
--rw-r--r--   0 martin    (1000) martin    (1000)    10480 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_geomhelpers.h
--rw-r--r--   0 martin    (1000) martin    (1000)     4438 2021-01-14 15:08:48.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_internal.h
--rw-r--r--   0 martin    (1000) martin    (1000)     6212 2020-06-19 13:21:06.000000 ducc0-0.8.0/src/ducc0/sharp/sharp_ylmgen.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.353366 ducc0-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2021-03-16 13:43:56.000000 ducc0-0.9.0/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)    15188 2021-03-16 11:31:06.000000 ducc0-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2021-03-16 13:48:23.000000 ducc0-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8085 2021-03-16 13:48:28.353366 ducc0-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6458 2021-03-16 11:31:06.000000 ducc0-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.341367 ducc0-0.9.0/ducc0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8085 2021-03-16 13:48:28.000000 ducc0-0.9.0/ducc0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2232 2021-03-16 13:48:28.000000 ducc0-0.9.0/ducc0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-16 13:48:28.000000 ducc0-0.9.0/ducc0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-03-16 13:48:28.000000 ducc0-0.9.0/ducc0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2021-03-16 13:48:28.000000 ducc0-0.9.0/ducc0.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      131 2021-03-16 11:31:06.000000 ducc0-0.9.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.341367 ducc0-0.9.0/python/
+-rw-rw-rw-   0 root         (0) root         (0)    16345 2021-03-16 13:04:22.000000 ducc0-0.9.0/python/alm.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.341367 ducc0-0.9.0/python/demos/
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/demos/fft_bench.py
+-rw-rw-rw-   0 root         (0) root         (0)     6951 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/demos/fft_stress.py
+-rw-rw-rw-   0 root         (0) root         (0)     3615 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/demos/healpix_perftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/demos/totalconvolve_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/demos/totalconvolve_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2021-03-16 13:48:23.000000 ducc0-0.9.0/python/ducc.cc
+-rw-rw-rw-   0 root         (0) root         (0)    24010 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/fft.cc
+-rw-rw-rw-   0 root         (0) root         (0)    55241 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/gridder_cxx.h
+-rw-rw-rw-   0 root         (0) root         (0)    13104 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/healpix.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6934 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/misc.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10479 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/pointingprovider.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7991 2021-03-16 13:48:23.000000 ducc0-0.9.0/python/sht.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.345366 ducc0-0.9.0/python/test/
+-rw-rw-rw-   0 root         (0) root         (0)     9915 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_fft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2974 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_healpix.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_pointing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_sht.py
+-rw-rw-rw-   0 root         (0) root         (0)     8710 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_totalconvolve.py
+-rw-rw-rw-   0 root         (0) root         (0)    10176 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/test/test_wgridder.py
+-rw-rw-rw-   0 root         (0) root         (0)    30687 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/totalconvolve.cc
+-rw-rw-rw-   0 root         (0) root         (0)    33234 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/totalconvolve.h
+-rw-rw-rw-   0 root         (0) root         (0)    16798 2021-03-16 11:31:06.000000 ducc0-0.9.0/python/wgridder.cc
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-16 13:48:28.353366 ducc0-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4103 2021-03-16 13:48:23.000000 ducc0-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.337367 ducc0-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.337367 ducc0-0.9.0/src/ducc0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.345366 ducc0-0.9.0/src/ducc0/bindings/
+-rw-rw-rw-   0 root         (0) root         (0)     4839 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/bindings/pybind_utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.345366 ducc0-0.9.0/src/ducc0/healpix/
+-rw-rw-rw-   0 root         (0) root         (0)    40668 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/healpix/healpix_base.cc
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/healpix/healpix_base.h
+-rw-rw-rw-   0 root         (0) root         (0)     5466 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/healpix/healpix_tables.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/healpix/healpix_tables.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.349366 ducc0-0.9.0/src/ducc0/infra/
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/aligned_array.h
+-rw-rw-rw-   0 root         (0) root         (0)     4151 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/bucket_sort.h
+-rw-rw-rw-   0 root         (0) root         (0)    10296 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/communication.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5953 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/communication.h
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/error_handling.h
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/mav.h
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/misc_utils.h
+-rw-rw-rw-   0 root         (0) root         (0)    18039 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/simd.h
+-rw-rw-rw-   0 root         (0) root         (0)    10002 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/string_utils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4885 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/string_utils.h
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/system.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/system.h
+-rw-rw-rw-   0 root         (0) root         (0)    14664 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/threading.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/threading.h
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/timers.h
+-rw-rw-rw-   0 root         (0) root         (0)     5380 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/transpose.h
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/types.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/types.h
+-rw-rw-rw-   0 root         (0) root         (0)      569 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/infra/useful_macros.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.349366 ducc0-0.9.0/src/ducc0/math/
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/cmplx.h
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/constants.h
+-rw-rw-rw-   0 root         (0) root         (0)    44781 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/fft.h
+-rw-rw-rw-   0 root         (0) root         (0)    62092 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/fft1d.h
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/geom_utils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/geom_utils.h
+-rw-rw-rw-   0 root         (0) root         (0)    11259 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/gl_integrator.h
+-rw-rw-rw-   0 root         (0) root         (0)    27169 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/gridding_kernel.h
+-rw-rw-rw-   0 root         (0) root         (0)     6453 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/math_utils.h
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/pointing.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/pointing.h
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/quaternion.h
+-rw-rw-rw-   0 root         (0) root         (0)    14711 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/rangeset.h
+-rw-rw-rw-   0 root         (0) root         (0)    14126 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/space_filling.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6331 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/space_filling.h
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/unity_roots.h
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/math/vec3.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 13:48:28.353366 ducc0-0.9.0/src/ducc0/sharp/
+-rw-rw-rw-   0 root         (0) root         (0)    13732 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6855 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp.h
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_almhelpers.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4588 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_almhelpers.h
+-rw-rw-rw-   0 root         (0) root         (0)     3842 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_core.cc
+-rw-rw-rw-   0 root         (0) root         (0)    37956 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_core_inc.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12062 2021-03-16 13:48:23.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_geomhelpers.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10480 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_geomhelpers.h
+-rw-rw-rw-   0 root         (0) root         (0)     4438 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)     6212 2021-03-16 11:31:06.000000 ducc0-0.9.0/src/ducc0/sharp/sharp_ylmgen.cc
```

### Comparing `ducc0-0.8.0/ChangeLog` & `ducc0-0.9.0/ChangeLog`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+0.9.0:
+- general:
+  - improved and faster computation of Gauss-Legendre nodes and weights
+    using Ignace Bogaert's implementation (https://doi.org/10.1137/140954969,
+    https://sourceforge.net/projects/fastgausslegendrequadrature/)
+  - Intel OneAPI compilers are now supported
+  - new accepted value "none-debug" for DUCC0_OPTIMIZATION
+
+- wgridder:
+  - fixed a bug which could cause memory accesses beyond the end of an array
+
+- fft:
+  - slightly improved buffer re-use
+
+- misc:
+  - substantially faster a_lm rotation code based on the Mikael Slevinsky's
+    FastTransforms package (https://github.com/MikaelSlevinsky/FastTransforms)
+
+
 0.8.0:
 - general:
   - compiles and runs on MacOS 11
   - choice of various optimization and debugging levels by setting
     the DUCC0_OPTIMIZATION variable before compilation.
     Valid choices are
     "none":
@@ -16,22 +35,22 @@
       same as above, with debugging information
     Default is "native".
 
 - wgridder:
   - more careful treatment of u,v,w-coordinates and phase angles, leading to
     better achievable accuracies for single-precision runs
   - performance improvements by making the computed interval in "n-1" symmetric
-    around 0. This reduces the number of required w planed significantly.
+    around 0. This reduces the number of required w planes significantly.
     Speedups are bigger for large FOVs and when FFT is dominating.
   - allow working with dirty images that are shifted with respect to the phase
     center. This can be used for faceting and incorporating DDEs.
   - new optional flag "double_precision_accumulation" for gridding routines,
     which causes accumulation onto the uv grid to be done in double precision,
     regardless of input and output precision. This can be helpful to avoid
-    accumulation errors in speciel circumstances.
+    accumulation errors in special circumstances.
 
 - pointingprovider:
   - improved performance via vectorized trigonometric functions
 
 
 0.7.0:
 - general:
```

### Comparing `ducc0-0.8.0/LICENSE` & `ducc0-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/MANIFEST.in` & `ducc0-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/PKG-INFO` & `ducc0-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducc0
-Version: 0.8.0
+Version: 0.9.0
 Summary: Distinctly useful code collection
 Home-page: https://gitlab.mpcdf.mpg.de/mtr/ducc
 Author: Martin Reinecke
 Author-email: martin@mpa-garching.mpg.de
 License: GPLv2
 Description: Distinctly Useful Code Collection (DUCC)
         ========================================
@@ -17,16 +17,16 @@
         The code is written in C++17, but provides a simple and comprehensive Python
         interface.
         
         ### Requirements
         
         - [Python >= 3.6](https://www.python.org/)
         - [pybind11](https://github.com/pybind/pybind11)
-        - a C++17-capable compiler (tested with g++ version 7 or newer and clang++;
-          recent versions of MSVC on Windows also work, but are tested less frequently)
+        - a C++17-capable compiler (tested with g++ version 7 or newer, clang++,
+          MSVC 2019 and Intel icpx 2021.1.2)
         
         ### Sources
         
         The latest version of DUCC can be obtained by cloning the repository via
         
             git clone https://gitlab.mpcdf.mpg.de/mtr/ducc.git
         
@@ -154,15 +154,15 @@
         - kernel computation is performed on the fly, avoiding inaccuracies
           due to table lookup and reducing overall memory bandwidth
         
         ### Numerical aspects
         - uses the analytical gridding kernel presented in
           <https://arxiv.org/abs/1808.06736>
         - uses the "improved W-stacking method" described in
-          <https://www.repository.cam.ac.uk/handle/1810/292298> (p. 139ff)
+          <https://arxiv.org/abs/2101.11172>
         - in combination these two aspects allow extremely accurate gridding/degridding
           operations (L2 error compared to explicit DFTs can go below 1e-12) with
           reasonable resource consumption
         
         
         ducc.misc
         ---------
```

### Comparing `ducc0-0.8.0/README.md` & `ducc0-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 The code is written in C++17, but provides a simple and comprehensive Python
 interface.
 
 ### Requirements
 
 - [Python >= 3.6](https://www.python.org/)
 - [pybind11](https://github.com/pybind/pybind11)
-- a C++17-capable compiler (tested with g++ version 7 or newer and clang++;
-  recent versions of MSVC on Windows also work, but are tested less frequently)
+- a C++17-capable compiler (tested with g++ version 7 or newer, clang++,
+  MSVC 2019 and Intel icpx 2021.1.2)
 
 ### Sources
 
 The latest version of DUCC can be obtained by cloning the repository via
 
     git clone https://gitlab.mpcdf.mpg.de/mtr/ducc.git
 
@@ -146,15 +146,15 @@
 - kernel computation is performed on the fly, avoiding inaccuracies
   due to table lookup and reducing overall memory bandwidth
 
 ### Numerical aspects
 - uses the analytical gridding kernel presented in
   <https://arxiv.org/abs/1808.06736>
 - uses the "improved W-stacking method" described in
-  <https://www.repository.cam.ac.uk/handle/1810/292298> (p. 139ff)
+  <https://arxiv.org/abs/2101.11172>
 - in combination these two aspects allow extremely accurate gridding/degridding
   operations (L2 error compared to explicit DFTs can go below 1e-12) with
   reasonable resource consumption
 
 
 ducc.misc
 ---------
```

### Comparing `ducc0-0.8.0/ducc0.egg-info/PKG-INFO` & `ducc0-0.9.0/ducc0.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducc0
-Version: 0.8.0
+Version: 0.9.0
 Summary: Distinctly useful code collection
 Home-page: https://gitlab.mpcdf.mpg.de/mtr/ducc
 Author: Martin Reinecke
 Author-email: martin@mpa-garching.mpg.de
 License: GPLv2
 Description: Distinctly Useful Code Collection (DUCC)
         ========================================
@@ -17,16 +17,16 @@
         The code is written in C++17, but provides a simple and comprehensive Python
         interface.
         
         ### Requirements
         
         - [Python >= 3.6](https://www.python.org/)
         - [pybind11](https://github.com/pybind/pybind11)
-        - a C++17-capable compiler (tested with g++ version 7 or newer and clang++;
-          recent versions of MSVC on Windows also work, but are tested less frequently)
+        - a C++17-capable compiler (tested with g++ version 7 or newer, clang++,
+          MSVC 2019 and Intel icpx 2021.1.2)
         
         ### Sources
         
         The latest version of DUCC can be obtained by cloning the repository via
         
             git clone https://gitlab.mpcdf.mpg.de/mtr/ducc.git
         
@@ -154,15 +154,15 @@
         - kernel computation is performed on the fly, avoiding inaccuracies
           due to table lookup and reducing overall memory bandwidth
         
         ### Numerical aspects
         - uses the analytical gridding kernel presented in
           <https://arxiv.org/abs/1808.06736>
         - uses the "improved W-stacking method" described in
-          <https://www.repository.cam.ac.uk/handle/1810/292298> (p. 139ff)
+          <https://arxiv.org/abs/2101.11172>
         - in combination these two aspects allow extremely accurate gridding/degridding
           operations (L2 error compared to explicit DFTs can go below 1e-12) with
           reasonable resource consumption
         
         
         ducc.misc
         ---------
```

### Comparing `ducc0-0.8.0/ducc0.egg-info/SOURCES.txt` & `ducc0-0.9.0/ducc0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/demos/fft_bench.py` & `ducc0-0.9.0/python/demos/fft_bench.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/demos/fft_stress.py` & `ducc0-0.9.0/python/demos/fft_stress.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/demos/healpix_perftest.py` & `ducc0-0.9.0/python/demos/healpix_perftest.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/demos/totalconvolve_demo.py` & `ducc0-0.9.0/python/demos/totalconvolve_demo.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/demos/totalconvolve_usage.py` & `ducc0-0.9.0/python/demos/totalconvolve_usage.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/ducc.cc` & `ducc0-0.9.0/python/ducc.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/fft.cc` & `ducc0-0.9.0/python/fft.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/gridder_cxx.h` & `ducc0-0.9.0/python/gridder_cxx.h`

 * *Files 1% similar despite different names*

```diff
@@ -718,15 +718,15 @@
         static constexpr size_t vlen = mysimd<Tacc>::size();
         static constexpr size_t nvec = (supp+vlen-1)/vlen;
 
       private:
         static constexpr int nsafe = (supp+1)/2;
         static constexpr int su = 2*nsafe+(1<<logsquare);
         static constexpr int sv = 2*nsafe+(1<<logsquare);
-        static constexpr int svvec = ((sv+vlen-1)/vlen)*vlen;
+        static constexpr int svvec = sv+vlen-1;
         static constexpr double xsupp=2./supp;
         const Params *parent;
         TemplateKernel<supp, mysimd<Tacc>> tkrn;
         mav<complex<Tcalc>,2> &grid;
         int iu0, iv0; // start index of the current visibility
         int bu0, bv0; // start index of the current buffer
 
@@ -818,15 +818,15 @@
         static constexpr size_t vlen = mysimd<Tcalc>::size();
         static constexpr size_t nvec = (supp+vlen-1)/vlen;
 
       private:
         static constexpr int nsafe = (supp+1)/2;
         static constexpr int su = 2*nsafe+(1<<logsquare);
         static constexpr int sv = 2*nsafe+(1<<logsquare);
-        static constexpr int svvec = ((sv+vlen-1)/vlen)*vlen;
+        static constexpr int svvec = sv+vlen-1;
         static constexpr double xsupp=2./supp;
         const Params *parent;
 
         TemplateKernel<supp, mysimd<Tcalc>> tkrn;
         const mav<complex<Tcalc>,2> &grid;
         int iu0, iv0; // start index of the current visibility
         int bu0, bv0; // start index of the current buffer
@@ -1417,15 +1417,15 @@
         nydirty(gridding ? dirty_out.shape(1) : dirty_in.shape(1)),
         epsilon(epsilon_),
         do_wgridding(do_wgridding_),
         nthreads((nthreads_==0) ? get_default_nthreads() : nthreads_),
         verbosity(verbosity_),
         negate_v(negate_v_), divide_by_n(divide_by_n_),
         sigma_min(sigma_min_), sigma_max(sigma_max_),
-        lshift(center_x), mshift(center_y),
+        lshift(center_x), mshift(negate_v ? -center_y : center_y),
         lmshift((lshift!=0) || (mshift!=0)),
         no_nshift(!allow_nshift)
       {
       timers.push("Baseline construction");
       bl = Baselines(uvw, freq, negate_v);
       MR_assert(bl.Nrows()<(size_t(1)<<32), "too many rows in the MS");
       MR_assert(bl.Nchannels()<(size_t(1)<<16), "too many channels in the MS");
```

### Comparing `ducc0-0.8.0/python/healpix.cc` & `ducc0-0.9.0/python/healpix.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/misc.cc` & `ducc0-0.9.0/python/misc.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/pointingprovider.cc` & `ducc0-0.9.0/python/pointingprovider.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/sht.cc` & `ducc0-0.9.0/python/sht.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_fft.py` & `ducc0-0.9.0/python/test/test_fft.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_healpix.py` & `ducc0-0.9.0/python/test/test_healpix.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_pointing.py` & `ducc0-0.9.0/python/test/test_pointing.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_sht.py` & `ducc0-0.9.0/python/test/test_sht.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_totalconvolve.py` & `ducc0-0.9.0/python/test/test_totalconvolve.py`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/test/test_wgridder.py` & `ducc0-0.9.0/python/test/test_wgridder.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Copyright(C) 2020 Max-Planck-Society
 
+from itertools import product
+
 import ducc0.wgridder as ng
 try:
     import finufft
     have_finufft = True
 except ImportError:
     have_finufft = False
 import numpy as np
@@ -88,27 +90,69 @@
     plan = finufft.Plan(1, (nxdirty, nydirty), eps=eps)
     plan.setpts(u.ravel(), v.ravel())
     res1 = plan.execute(ms.ravel()).real
     np.testing.assert_allclose(res0, res1)
     return res0
 
 
-@pmp("nxdirty", (30, 128))
-@pmp("nydirty", (128, 250))
+def vis2dirty_with_faceting(nfacets_x, nfacets_y, npix_x, npix_y, **kwargs):
+    if npix_x % nfacets_x != 0:
+        raise ValueError("nfacets_x needs to be divisor of npix_x.")
+    if npix_y % nfacets_y != 0:
+        raise ValueError("nfacets_y needs to be divisor of npix_y.")
+    nx = npix_x // nfacets_x
+    ny = npix_y // nfacets_y
+    dtype = np.float32 if kwargs["vis"].dtype == np.complex64 else np.float64
+    res = np.zeros((npix_x, npix_y), dtype)
+    for xx, yy in product(range(nfacets_x), range(nfacets_y)):
+        cx = ((0.5+xx)/nfacets_x - 0.5) * kwargs["pixsize_x"]*npix_x
+        cy = ((0.5+yy)/nfacets_y - 0.5) * kwargs["pixsize_y"]*npix_y
+        im = ng.experimental.vis2dirty(**kwargs,
+                                       center_x=cx, center_y=cy,
+                                       npix_x=nx, npix_y=ny)
+        res[nx*xx:nx*(xx+1), ny*yy:ny*(yy+1)] = im
+    return res
+
+
+def dirty2vis_with_faceting(nfacets_x, nfacets_y, dirty, **kwargs):
+    npix_x, npix_y = dirty.shape
+    if npix_x % nfacets_x != 0:
+        raise ValueError("nfacets_x needs to be divisor of npix_x.")
+    if npix_y % nfacets_y != 0:
+        raise ValueError("nfacets_y needs to be divisor of npix_y.")
+    nx = npix_x // nfacets_x
+    ny = npix_y // nfacets_y
+    vis = None
+    for xx, yy in product(range(nfacets_x), range(nfacets_y)):
+        cx = ((0.5+xx)/nfacets_x - 0.5) * kwargs["pixsize_x"]*npix_x
+        cy = ((0.5+yy)/nfacets_y - 0.5) * kwargs["pixsize_y"]*npix_y
+        facet = dirty[nx*xx:nx*(xx+1), ny*yy:ny*(yy+1)]
+        foo = ng.experimental.dirty2vis(**kwargs, dirty=facet,
+                                        center_x=cx, center_y=cy)
+        if vis is None:
+            vis = foo
+        else:
+            vis += foo
+    return vis
+
+
+@pmp('nx', [(30, 3), (128, 2)])
+@pmp('ny', [(128, 2), (250, 5)])
 @pmp("nrow", (1, 2, 27))
 @pmp("nchan", (1, 5))
 @pmp("epsilon", (1e-1, 1e-3, 3e-5, 2e-13))
 @pmp("singleprec", (True, False))
 @pmp("wstacking", (True, False))
 @pmp("use_wgt", (True, False))
 @pmp("use_mask", (False, True))
 @pmp("nthreads", (1, 2, 7))
-def test_adjointness_ms2dirty(nxdirty, nydirty, nrow, nchan, epsilon,
+def test_adjointness_ms2dirty(nx, ny, nrow, nchan, epsilon,
                               singleprec, wstacking, use_wgt, nthreads,
                               use_mask):
+    (nxdirty, nxfacets), (nydirty, nyfacets) = nx, ny
     if singleprec and epsilon < 1e-6:
         pytest.skip()
     rng = np.random.default_rng(42)
     pixsizex = np.pi/180/60/nxdirty*0.2398
     pixsizey = np.pi/180/60/nxdirty
     f0 = 1e9
     freq = f0 + np.arange(nchan)*(f0/nchan)
@@ -120,39 +164,58 @@
     dirty = rng.random((nxdirty, nydirty))-0.5
     nu = nv = 0
     if singleprec:
         ms = ms.astype("c8")
         dirty = dirty.astype("f4")
         if wgt is not None:
             wgt = wgt.astype("f4")
+
+    def check(d2, m2):
+        ref = max(my_vdot(ms, ms).real, my_vdot(m2, m2).real,
+                  my_vdot(dirty, dirty).real, my_vdot(d2, d2).real)
+        tol = 3e-5*ref if singleprec else 2e-13*ref
+        assert_allclose(my_vdot(ms, m2).real, my_vdot(d2, dirty), rtol=tol)
+
     dirty2 = ng.ms2dirty(uvw, freq, ms, wgt, nxdirty, nydirty, pixsizex,
                          pixsizey, nu, nv, epsilon, wstacking, nthreads, 0,
                          mask).astype("f8")
     ms2 = ng.dirty2ms(uvw, freq, dirty, wgt, pixsizex, pixsizey, nu, nv,
                       epsilon, wstacking, nthreads+1, 0, mask).astype("c16")
-    ref = max(my_vdot(ms, ms).real, my_vdot(ms2, ms2).real,
-              my_vdot(dirty, dirty).real, my_vdot(dirty2, dirty2).real)
-    tol = 3e-5*ref if singleprec else 2e-13*ref
-    assert_allclose(my_vdot(ms, ms2).real, my_vdot(dirty2, dirty), rtol=tol)
+    check(dirty2, ms2)
+
 
+    dirty2 = vis2dirty_with_faceting(nxfacets, nyfacets, uvw=uvw, freq=freq,
+                                     vis=ms, wgt=wgt, npix_x=nxdirty,
+                                     npix_y=nydirty, pixsize_x=pixsizex,
+                                     pixsize_y=pixsizey, epsilon=epsilon,
+                                     do_wgridding=wstacking, nthreads=nthreads,
+                                     mask=mask).astype("f8")
+    ms2 = dirty2vis_with_faceting(nxfacets, nyfacets, uvw=uvw, freq=freq,
+                                  dirty=dirty, wgt=wgt, pixsize_x=pixsizex,
+                                  pixsize_y=pixsizey, epsilon=epsilon,
+                                  do_wgridding=wstacking, nthreads=nthreads+1,
+                                  mask=mask).astype("c16")
+    check(dirty2, ms2)
 
-@pmp('nxdirty', [16, 64])
-@pmp('nydirty', [64])
+
+@pmp('nx', [(16, 2), (64, 4)])
+@pmp('ny', [(64, 2)])
 @pmp("nrow", (1, 2, 27))
 @pmp("nchan", (1, 5))
 @pmp("epsilon", (1e-2, 1e-3, 1e-4, 1e-7))
 @pmp("singleprec", (False,))
 @pmp("wstacking", (False, True))
 @pmp("use_wgt", (True,))
 @pmp("use_mask", (True,))
 @pmp("nthreads", (1, 2, 7))
 @pmp("fov", (0.001, 0.01, 0.1, 1., 20.))
-def test_ms2dirty_against_wdft2(nxdirty, nydirty, nrow, nchan, epsilon,
+def test_ms2dirty_against_wdft2(nx, ny, nrow, nchan, epsilon,
                                 singleprec, wstacking, use_wgt, use_mask, fov,
                                 nthreads):
+    (nxdirty, nxfacets), (nydirty, nyfacets) = nx, ny
     if singleprec and epsilon < 1e-6:
         pytest.skip()
     rng = np.random.default_rng(42)
     pixsizex = fov*np.pi/180/nxdirty
     pixsizey = fov*np.pi/180/nydirty*1.1
     f0 = 1e9
     freq = f0 + np.arange(nchan)*(f0/nchan)
@@ -170,12 +233,20 @@
     dirty = ng.ms2dirty(uvw, freq, ms, wgt, nxdirty, nydirty, pixsizex,
                         pixsizey, nu, nv, epsilon, wstacking, nthreads,
                         0, mask).astype("f8")
     ref = explicit_gridder(uvw, freq, ms, wgt, nxdirty, nydirty, pixsizex,
                            pixsizey, wstacking, mask)
     assert_allclose(_l2error(dirty, ref), 0, atol=epsilon)
 
+    dirty2 = vis2dirty_with_faceting(nxfacets, nyfacets, uvw=uvw, freq=freq,
+                                     vis=ms, wgt=wgt, npix_x=nxdirty,
+                                     npix_y=nydirty, pixsize_x=pixsizex,
+                                     pixsize_y=pixsizey, epsilon=epsilon,
+                                     do_wgridding=wstacking, nthreads=nthreads,
+                                     mask=mask).astype("f8")
+    assert_allclose(_l2error(dirty2, ref), 0, atol=epsilon)
+
     if wstacking or (not have_finufft):
         return
     dirty = with_finufft(uvw, freq, ms, wgt, nxdirty, nydirty, pixsizex,
                          pixsizey, mask, epsilon)
     assert_allclose(_l2error(dirty, ref), 0, atol=epsilon)
```

### Comparing `ducc0-0.8.0/python/totalconvolve.cc` & `ducc0-0.9.0/python/totalconvolve.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/totalconvolve.h` & `ducc0-0.9.0/python/totalconvolve.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/python/wgridder.cc` & `ducc0-0.9.0/python/wgridder.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/setup.py` & `ducc0-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from glob import iglob
 import os
 
 from setuptools import setup, Extension
 import pybind11
 
 pkgname = 'ducc0'
-version = '0.8.0'
+version = '0.9.0'
 
 user_cflags = os.getenv("DUCC0_CFLAGS", "").split(" ")
 user_cflags = [x for x in user_cflags if x != ""]
 user_lflags = os.getenv("DUCC0_LFLAGS", "").split(" ")
 user_lflags = [x for x in user_lflags if x != ""]
 
 compilation_strategy = os.getenv('DUCC0_OPTIMIZATION', 'native')
-if compilation_strategy not in ['none', 'portable', 'portable-debug', 'native', 'native-debug']:
+if compilation_strategy not in ['none', 'none-debug', 'portable', 'portable-debug', 'native', 'native-debug']:
     raise RuntimeError('unknown compilation strategy')
-do_debug = compilation_strategy in ['portable-debug', 'native-debug']
-do_optimize = compilation_strategy not in ['none']
+do_debug = compilation_strategy in ['none-debug', 'portable-debug', 'native-debug']
+do_optimize = compilation_strategy not in ['none', 'none-debug']
 do_native = compilation_strategy in ['native', 'native-debug']
 
 def _get_files_by_suffix(directory, suffix):
     path = directory
     iterable_sources = (iglob(os.path.join(root, '*.'+suffix))
                         for root, dirs, files in os.walk(path))
     return list(itertools.chain.from_iterable(iterable_sources))
```

### Comparing `ducc0-0.8.0/src/ducc0/bindings/pybind_utils.h` & `ducc0-0.9.0/src/ducc0/bindings/pybind_utils.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/healpix/healpix_base.cc` & `ducc0-0.9.0/src/ducc0/healpix/healpix_base.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/healpix/healpix_base.h` & `ducc0-0.9.0/src/ducc0/healpix/healpix_base.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/healpix/healpix_tables.cc` & `ducc0-0.9.0/src/ducc0/healpix/healpix_tables.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/healpix/healpix_tables.h` & `ducc0-0.9.0/src/ducc0/healpix/healpix_tables.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/aligned_array.h` & `ducc0-0.9.0/src/ducc0/infra/aligned_array.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/bucket_sort.h` & `ducc0-0.9.0/src/ducc0/infra/bucket_sort.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/communication.cc` & `ducc0-0.9.0/src/ducc0/infra/communication.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/communication.h` & `ducc0-0.9.0/src/ducc0/infra/communication.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/error_handling.h` & `ducc0-0.9.0/src/ducc0/infra/error_handling.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/mav.h` & `ducc0-0.9.0/src/ducc0/infra/mav.h`

 * *Files 0% similar despite different names*

```diff
@@ -555,15 +555,15 @@
 
     template<size_t nd2> auto subdata(const shape_t &i0, const shape_t &extent) const
       {
       array<size_t, nd2> nshp;
       array<ptrdiff_t, nd2> nstr;
       ptrdiff_t nofs;
       size_t n0=0;
-      for (auto x:extent) if (x==0)++n0;
+      for (auto x:extent) if (x==0) ++n0;
       MR_assert(n0+nd2==ndim, "bad extent");
       nofs=0;
       for (size_t i=0, i2=0; i<ndim; ++i)
         {
         MR_assert(i0[i]<shp[i], "bad subset");
         nofs+=i0[i]*str[i];
         if (extent[i]!=0)
```

### Comparing `ducc0-0.8.0/src/ducc0/infra/misc_utils.h` & `ducc0-0.9.0/src/ducc0/infra/misc_utils.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/simd.h` & `ducc0-0.9.0/src/ducc0/infra/simd.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/string_utils.cc` & `ducc0-0.9.0/src/ducc0/infra/string_utils.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/string_utils.h` & `ducc0-0.9.0/src/ducc0/infra/string_utils.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/system.cc` & `ducc0-0.9.0/src/ducc0/infra/system.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/system.h` & `ducc0-0.9.0/src/ducc0/infra/system.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/threading.cc` & `ducc0-0.9.0/src/ducc0/infra/threading.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/threading.h` & `ducc0-0.9.0/src/ducc0/infra/threading.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/timers.h` & `ducc0-0.9.0/src/ducc0/infra/timers.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/transpose.h` & `ducc0-0.9.0/src/ducc0/infra/transpose.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/types.cc` & `ducc0-0.9.0/src/ducc0/infra/types.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/types.h` & `ducc0-0.9.0/src/ducc0/infra/types.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/infra/useful_macros.h` & `ducc0-0.9.0/src/ducc0/infra/useful_macros.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/cmplx.h` & `ducc0-0.9.0/src/ducc0/math/cmplx.h`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  *  GNU General Public License for more details.
  *
  *  You should have received a copy of the GNU General Public License
  *  along with this code; if not, write to the Free Software
  *  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
  */
 
-/* Copyright (C) 2019-2020 Max-Planck-Society
+/* Copyright (C) 2019-2021 Max-Planck-Society
    Author: Martin Reinecke */
 
 #ifndef DUCC0_CMPLX_H
 #define DUCC0_CMPLX_H
 
 namespace ducc0 {
 
@@ -39,14 +39,15 @@
   template<typename T2>Cmplx &operator*= (const Cmplx<T2> &other)
     {
     T tmp = r*other.r - i*other.i;
     i = r*other.i + i*other.r;
     r = tmp;
     return *this;
     }
+  Cmplx conj() const { return {r, -i}; }
   template<typename T2>Cmplx &operator+= (const Cmplx<T2> &other)
     { r+=other.r; i+=other.i; return *this; }
   template<typename T2>Cmplx &operator-= (const Cmplx<T2> &other)
     { r-=other.r; i-=other.i; return *this; }
   template<typename T2> auto operator* (const T2 &other) const
     -> Cmplx<decltype(r*other)>
     { return {r*other, i*other}; }
```

### Comparing `ducc0-0.8.0/src/ducc0/math/constants.h` & `ducc0-0.9.0/src/ducc0/math/constants.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/fft.h` & `ducc0-0.9.0/src/ducc0/math/fft.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
 This file is part of pocketfft.
 
-Copyright (C) 2010-2020 Max-Planck-Society
+Copyright (C) 2010-2021 Max-Planck-Society
 Copyright (C) 2019 Peter Bell
 
 For the odd-sized DCT-IV transforms:
   Copyright (C) 2003, 2007-14 Matteo Frigo
   Copyright (C) 2003, 2007-14 Massachusetts Institute of Technology
 
 Authors: Martin Reinecke, Peter Bell
@@ -134,59 +134,75 @@
   private:
     pocketfft_r<T0> fftplan;
 
   public:
     DUCC0_NOINLINE T_dct1(size_t length)
       : fftplan(2*(length-1)) {}
 
-    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct, bool ortho,
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T buf[], T0 fct, bool ortho,
       int /*type*/, bool /*cosine*/) const
       {
       constexpr T0 sqrt2=T0(1.414213562373095048801688724209698L);
       size_t N=fftplan.length(), n=N/2+1;
       if (ortho)
         { c[0]*=sqrt2; c[n-1]*=sqrt2; }
-      aligned_array<T> tmp(N);
+      auto tmp=&buf[0];
       tmp[0] = c[0];
       for (size_t i=1; i<n; ++i)
         tmp[i] = tmp[N-i] = c[i];
-      fftplan.exec(tmp.data(), fct, true);
-      c[0] = tmp[0];
+      auto res = fftplan.exec(tmp, &buf[N], fct, true);
+      c[0] = res[0];
       for (size_t i=1; i<n; ++i)
-        c[i] = tmp[2*i-1];
+        c[i] = res[2*i-1];
       if (ortho)
         { c[0]*=sqrt2*T0(0.5); c[n-1]*=sqrt2*T0(0.5); }
+      return c;
+      }
+    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct, bool ortho,
+      int /*type*/, bool /*cosine*/) const
+      {
+      aligned_array<T> buf(bufsize());
+      exec(c, buf.data(), fct, ortho, 1, true);
       }
 
     size_t length() const { return fftplan.length()/2+1; }
+    size_t bufsize() const { return fftplan.length()+fftplan.bufsize(); }
   };
 
 template<typename T0> class T_dst1
   {
   private:
     pocketfft_r<T0> fftplan;
 
   public:
     DUCC0_NOINLINE T_dst1(size_t length)
       : fftplan(2*(length+1)) {}
 
-    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct,
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T buf[], T0 fct,
       bool /*ortho*/, int /*type*/, bool /*cosine*/) const
       {
       size_t N=fftplan.length(), n=N/2-1;
-      aligned_array<T> tmp(N);
+      auto tmp = &buf[0];
       tmp[0] = tmp[n+1] = c[0]*0;
       for (size_t i=0; i<n; ++i)
         { tmp[i+1]=c[i]; tmp[N-1-i]=-c[i]; }
-      fftplan.exec(tmp.data(), fct, true);
+      auto res = fftplan.exec(tmp, buf+N, fct, true);
       for (size_t i=0; i<n; ++i)
-        c[i] = -tmp[2*i+2];
+        c[i] = -res[2*i+2];
+      return c;
+      }
+    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct,
+      bool /*ortho*/, int /*type*/, bool /*cosine*/) const
+      {
+      aligned_array<T> buf(bufsize());
+      exec(c, buf.data(), fct, true, 1, false);
       }
 
     size_t length() const { return fftplan.length()/2-1; }
+    size_t bufsize() const { return fftplan.length()+fftplan.bufsize(); }
   };
 
 template<typename T0> class T_dcst23
   {
   private:
     pocketfft_r<T0> fftplan;
     std::vector<T0> twiddle;
@@ -196,38 +212,39 @@
       : fftplan(length), twiddle(length)
       {
       UnityRoots<T0,Cmplx<T0>> tw(4*length);
       for (size_t i=0; i<length; ++i)
         twiddle[i] = tw[i+1].r;
       }
 
-    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct, bool ortho,
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T buf[], T0 fct, bool ortho,
       int type, bool cosine) const
       {
       constexpr T0 sqrt2=T0(1.414213562373095048801688724209698L);
       size_t N=length();
       size_t NS2 = (N+1)/2;
       if (type==2)
         {
         if (!cosine)
           for (size_t k=1; k<N; k+=2)
             c[k] = -c[k];
         c[0] *= 2;
         if ((N&1)==0) c[N-1]*=2;
         for (size_t k=1; k<N-1; k+=2)
           MPINPLACE(c[k+1], c[k]);
-        fftplan.exec(c, fct, false);
+        auto res = fftplan.exec(c, buf, fct, false);
+        c[0] = res[0];
         for (size_t k=1, kc=N-1; k<NS2; ++k, --kc)
           {
-          T t1 = twiddle[k-1]*c[kc]+twiddle[kc-1]*c[k];
-          T t2 = twiddle[k-1]*c[k]-twiddle[kc-1]*c[kc];
+          T t1 = twiddle[k-1]*res[kc]+twiddle[kc-1]*res[k];
+          T t2 = twiddle[k-1]*res[k]-twiddle[kc-1]*res[kc];
           c[k] = T0(0.5)*(t1+t2); c[kc]=T0(0.5)*(t1-t2);
           }
         if ((N&1)==0)
-          c[NS2] *= twiddle[NS2-1];
+          c[NS2] = res[NS2]*twiddle[NS2-1];
         if (!cosine)
           for (size_t k=0, kc=N-1; k<kc; ++k, --kc)
             std::swap(c[k], c[kc]);
         if (ortho) c[0]*=sqrt2*T0(0.5);
         }
       else
         {
@@ -239,24 +256,34 @@
           {
           T t1=c[k]+c[kc], t2=c[k]-c[kc];
           c[k] = twiddle[k-1]*t2+twiddle[kc-1]*t1;
           c[kc]= twiddle[k-1]*t1-twiddle[kc-1]*t2;
           }
         if ((N&1)==0)
           c[NS2] *= 2*twiddle[NS2-1];
-        fftplan.exec(c, fct, true);
+        auto res = fftplan.exec(c, buf, fct, true);
+        if (res != c) // FIXME: not yet optimal
+          memcpy(c, res, N*sizeof(T));
         for (size_t k=1; k<N-1; k+=2)
           MPINPLACE(c[k], c[k+1]);
         if (!cosine)
           for (size_t k=1; k<N; k+=2)
             c[k] = -c[k];
         }
+      return c;
+      }
+    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct, bool ortho,
+      int type, bool cosine) const
+      {
+      aligned_array<T> buf(bufsize());
+      exec(c, &buf[0], fct, ortho, type, cosine);
       }
 
     size_t length() const { return fftplan.length(); }
+    size_t bufsize() const { return fftplan.bufsize(); }
   };
 
 template<typename T0> class T_dcst4
   {
   private:
     size_t N;
     std::unique_ptr<pocketfft_c<T0>> fft;
@@ -274,15 +301,15 @@
         {
         UnityRoots<T0,Cmplx<T0>> tw(16*N);
         for (size_t i=0; i<N/2; ++i)
           C2[i] = conj(tw[8*i+1]);
         }
       }
 
-    template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct,
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T /*buf*/[], T0 fct,
       bool /*ortho*/, int /*type*/, bool cosine) const
       {
       size_t n2 = N/2;
       if (!cosine)
         for (size_t k=0, kc=N-1; k<n2; ++k, --kc)
           std::swap(c[k], c[kc]);
       if (N&1)
@@ -346,17 +373,25 @@
           c[2*i  ] = T0( 2)*(y[i ].r*C2[i ].r-y[i ].i*C2[i ].i);
           c[2*i+1] = T0(-2)*(y[ic].i*C2[ic].r+y[ic].r*C2[ic].i);
           }
         }
       if (!cosine)
         for (size_t k=1; k<N; k+=2)
           c[k] = -c[k];
+      return c;
+      }
+
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T0 fct,
+      bool /*ortho*/, int /*type*/, bool cosine) const
+      {
+      exec(c, nullptr, fct, true, 4, cosine);
       }
 
     size_t length() const { return N; }
+    size_t bufsize() const { return 0; }
   };
 
 
 //
 // multi-D infrastructure
 //
 
@@ -552,17 +587,27 @@
   };
 
 template<typename T, typename T0> DUCC0_NOINLINE aligned_array<T> alloc_tmp
   (const fmav_info &info, size_t axsize)
   {
   auto othersize = info.size()/axsize;
   constexpr auto vlen = native_simd<T0>::size();
+  // FIXME: when switching to C++20, use bit_floor(othersize)
   return aligned_array<T>(axsize*std::min(vlen, othersize));
   }
 
+template<typename T, typename T0> DUCC0_NOINLINE aligned_array<T> alloc_tmp
+  (const fmav_info &info, size_t axsize, size_t bufsize)
+  {
+  auto othersize = info.size()/axsize;
+  constexpr auto vlen = native_simd<T0>::size();
+  // FIXME: when switching to C++20, use bit_floor(othersize)
+  return aligned_array<T>((axsize+bufsize)*std::min(vlen, othersize));
+  }
+
 template <typename Tsimd, typename Titer> DUCC0_NOINLINE void copy_input(const Titer &it,
   const fmav<Cmplx<typename Tsimd::Ts>> &src, Cmplx<Tsimd> *DUCC0_RESTRICT dst)
   {
   constexpr auto vlen=Tsimd::size();
   if (it.uniform_i())
     {
     auto ptr = &src.craw(it.iofs_uni(0,0));
@@ -729,30 +774,30 @@
 template <typename T, size_t vlen> struct add_vec { using type = simd<T, vlen>; };
 template <typename T, size_t vlen> struct add_vec<Cmplx<T>, vlen>
   { using type = Cmplx<simd<T, vlen>>; };
 template <typename T, size_t vlen> using add_vec_t = typename add_vec<T, vlen>::type;
 
 template<typename Tplan, typename T, typename T0, typename Exec>
 DUCC0_NOINLINE void general_nd(const fmav<T> &in, fmav<T> &out,
-  const shape_t &axes, T0 fct, size_t nthreads, const Exec & exec,
-  const bool allow_inplace=true)
+  const shape_t &axes, T0 fct, size_t nthreads, const Exec &exec,
+  const bool /*allow_inplace*/=true)
   {
   std::unique_ptr<Tplan> plan;
 
   for (size_t iax=0; iax<axes.size(); ++iax)
     {
     size_t len=in.shape(axes[iax]);
     if ((!plan) || (len!=plan->length()))
       plan = std::make_unique<Tplan>(len);
 
     execParallel(
       util::thread_count(nthreads, in, axes[iax], native_simd<T0>::size()),
       [&](Scheduler &sched) {
         constexpr auto vlen = native_simd<T0>::size();
-        auto storage = alloc_tmp<T,T0>(in, len);
+        auto storage = alloc_tmp<T,T0>(in, len, plan->bufsize());
         const auto &tin(iax==0? in : out);
         multi_iter<vlen> it(tin, out, axes[iax], sched.num_threads(), sched.thread_num());
 #ifndef DUCC0_NO_SIMD
         if constexpr (vlen>1)
           while (it.remaining()>=vlen)
             {
             it.advance(vlen);
@@ -773,34 +818,33 @@
             auto tdatav = reinterpret_cast<add_vec_t<T, vlen/4> *>(storage.data());
             exec(it, tin, out, tdatav, *plan, fct);
             }
 #endif
         while (it.remaining()>0)
           {
           it.advance(1);
-          auto buf = allow_inplace && it.stride_out() == 1 ?
-            &out.vraw(it.oofs(0)) : reinterpret_cast<T *>(storage.data());
-          exec(it, tin, out, buf, *plan, fct);
+          exec(it, tin, out, storage.data(), *plan, fct);
           }
       });  // end of parallel region
     fct = T0(1); // factor has been applied, use 1 for remaining axes
     }
   }
 
 struct ExecC2C
   {
   bool forward;
 
   template <typename T0, typename T, typename Titer> DUCC0_NOINLINE void operator() (
     const Titer &it, const fmav<Cmplx<T0>> &in,
     fmav<Cmplx<T0>> &out, T *buf, const pocketfft_c<T0> &plan, T0 fct) const
     {
-    copy_input(it, in, buf);
-    plan.exec(buf, fct, forward);
-    copy_output(it, buf, out);
+    T *buf1=buf, *buf2=buf+plan.bufsize(); 
+    copy_input(it, in, buf2);
+    auto res = plan.exec(buf2, buf1, fct, forward);
+    copy_output(it, res, out);
     }
   };
 
 template <typename Tsimd, typename Titer> DUCC0_NOINLINE void copy_hartley(const Titer &it,
   const Tsimd *DUCC0_RESTRICT src, fmav<typename Tsimd::Ts> &dst)
   {
   constexpr auto vlen=Tsimd::size();
@@ -888,49 +932,51 @@
     ptr[it.oofs(i1)] = src[i];
   }
 
 struct ExecHartley
   {
   template <typename T0, typename T, typename Titer> DUCC0_NOINLINE void operator () (
     const Titer &it, const fmav<T0> &in, fmav<T0> &out,
-    T * buf, const pocketfft_r<T0> &plan, T0 fct) const
+    T *buf, const pocketfft_r<T0> &plan, T0 fct) const
     {
-    copy_input(it, in, buf);
-    plan.exec(buf, fct, true);
-    copy_hartley(it, buf, out);
+    T *buf1=buf, *buf2=buf+plan.bufsize(); 
+    copy_input(it, in, buf2);
+    auto res = plan.exec(buf2, buf1, fct, true);
+    copy_hartley(it, res, out);
     }
   };
 
 struct ExecDcst
   {
   bool ortho;
   int type;
   bool cosine;
 
   template <typename T0, typename T, typename Tplan, typename Titer>
   DUCC0_NOINLINE void operator () (const Titer &it, const fmav<T0> &in,
     fmav <T0> &out, T * buf, const Tplan &plan, T0 fct) const
     {
-    copy_input(it, in, buf);
-    plan.exec(buf, fct, ortho, type, cosine);
-    copy_output(it, buf, out);
+    T *buf1=buf, *buf2=buf+plan.bufsize(); 
+    copy_input(it, in, buf2);
+    auto res = plan.exec(buf2, buf1, fct, ortho, type, cosine);
+    copy_output(it, res, out);
     }
   };
 
 template<typename T> DUCC0_NOINLINE void general_r2c(
   const fmav<T> &in, fmav<Cmplx<T>> &out, size_t axis, bool forward, T fct,
   size_t nthreads)
   {
   auto plan = std::make_unique<pocketfft_r<T>>(in.shape(axis));
   size_t len=in.shape(axis);
   execParallel(
     util::thread_count(nthreads, in, axis, native_simd<T>::size()),
     [&](Scheduler &sched) {
     constexpr auto vlen = native_simd<T>::size();
-    auto storage = alloc_tmp<T,T>(in, len);
+    auto storage = alloc_tmp<T,T>(in, len, plan->bufsize());
     multi_iter<vlen> it(in, out, axis, sched.num_threads(), sched.thread_num());
 #ifndef DUCC0_NO_SIMD
     if constexpr (vlen>1)
       while (it.remaining()>=vlen)
         {
         it.advance(vlen);
         auto tdatav = reinterpret_cast<simd<T,vlen> *>(storage.data());
@@ -1025,15 +1071,15 @@
   {
   auto plan = std::make_unique<pocketfft_r<T>>(out.shape(axis));
   size_t len=out.shape(axis);
   execParallel(
     util::thread_count(nthreads, in, axis, native_simd<T>::size()),
     [&](Scheduler &sched) {
       constexpr auto vlen = native_simd<T>::size();
-      auto storage = alloc_tmp<T,T>(out, len);
+      auto storage = alloc_tmp<T,T>(out, len, plan->bufsize());
       multi_iter<vlen> it(in, out, axis, sched.num_threads(), sched.thread_num());
 #ifndef DUCC0_NO_SIMD
       if constexpr (vlen>1)
         while (it.remaining()>=vlen)
           {
           it.advance(vlen);
           auto tdatav = reinterpret_cast<native_simd<T> *>(storage.data());
@@ -1152,26 +1198,27 @@
   }
 
 struct ExecR2R
   {
   bool r2c, forward;
 
   template <typename T0, typename T, typename Titer> DUCC0_NOINLINE void operator () (
-    const Titer &it, const fmav<T0> &in, fmav<T0> &out, T * buf,
+    const Titer &it, const fmav<T0> &in, fmav<T0> &out, T *buf,
     const pocketfft_r<T0> &plan, T0 fct) const
     {
-    copy_input(it, in, buf);
+    T *buf1=buf, *buf2=buf+plan.bufsize();
+    copy_input(it, in, buf2);
     if ((!r2c) && forward)
       for (size_t i=2; i<it.length_out(); i+=2)
-        buf[i] = -buf[i];
-    plan.exec(buf, fct, r2c);
+        buf2[i] = -buf2[i];
+    auto res = plan.exec(buf2, buf1, fct, r2c);
     if (r2c && (!forward))
       for (size_t i=2; i<it.length_out(); i+=2)
-        buf[i] = -buf[i];
-    copy_output(it, buf, out);
+        res[i] = -res[i];
+    copy_output(it, res, out);
     }
   };
 
 template<typename T> DUCC0_NOINLINE void c2c(const fmav<std::complex<T>> &in,
   fmav<std::complex<T>> &out, const shape_t &axes, bool forward,
   T fct, size_t nthreads=1)
   {
```

### Comparing `ducc0-0.8.0/src/ducc0/math/fft1d.h` & `ducc0-0.9.0/src/ducc0/math/fft1d.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
 This file is part of pocketfft.
 
-Copyright (C) 2010-2020 Max-Planck-Society
+Copyright (C) 2010-2021 Max-Planck-Society
 Copyright (C) 2019 Peter Bell
 
 Authors: Martin Reinecke, Peter Bell
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
@@ -668,19 +668,14 @@
   auto CX = [cc, ido, l1](size_t a, size_t b, size_t c) -> T&
     { return cc[a+ido*(b+l1*c)]; };
   auto CX2 = [cc, idl1](size_t a, size_t b) -> T&
     { return cc[a+idl1*b]; };
   auto CH2 = [ch, idl1](size_t a, size_t b) -> const T&
     { return ch[a+idl1*b]; };
 
-  aligned_array<Cmplx<T0>> wal(ip);
-  wal[0] = Cmplx<T0>(1., 0.);
-  for (size_t i=1; i<ip; ++i)
-    wal[i]=Cmplx<T0>(csarr[i].r,fwd ? -csarr[i].i : csarr[i].i);
-
   for (size_t k=0; k<l1; ++k)
     for (size_t i=0; i<ido; ++i)
       CH(i,k,0) = CC(i,0,k);
   for (size_t j=1, jc=ip-1; j<ipph; ++j, --jc)
     for (size_t k=0; k<l1; ++k)
       for (size_t i=0; i<ido; ++i)
         PM(CH(i,k,j),CH(i,k,jc),CC(i,j,k),CC(i,jc,k));
@@ -693,40 +688,42 @@
       CX(i,k,0) = tmp;
       }
   for (size_t l=1, lc=ip-1; l<ipph; ++l, --lc)
     {
     // j=0
     for (size_t ik=0; ik<idl1; ++ik)
       {
-      CX2(ik,l).r = CH2(ik,0).r+wal[l].r*CH2(ik,1).r+wal[2*l].r*CH2(ik,2).r;
-      CX2(ik,l).i = CH2(ik,0).i+wal[l].r*CH2(ik,1).i+wal[2*l].r*CH2(ik,2).i;
-      CX2(ik,lc).r=-wal[l].i*CH2(ik,ip-1).i-wal[2*l].i*CH2(ik,ip-2).i;
-      CX2(ik,lc).i=wal[l].i*CH2(ik,ip-1).r+wal[2*l].i*CH2(ik,ip-2).r;
+      auto wal  = fwd ? csarr[  l].conj() : csarr[  l];
+      auto wal2 = fwd ? csarr[2*l].conj() : csarr[2*l];
+      CX2(ik,l ).r = CH2(ik,0).r+wal.r*CH2(ik,1).r+wal2.r*CH2(ik,2).r;
+      CX2(ik,l ).i = CH2(ik,0).i+wal.r*CH2(ik,1).i+wal2.r*CH2(ik,2).i;
+      CX2(ik,lc).r =-wal.i*CH2(ik,ip-1).i-wal2.i*CH2(ik,ip-2).i;
+      CX2(ik,lc).i = wal.i*CH2(ik,ip-1).r+wal2.i*CH2(ik,ip-2).r;
       }
 
     size_t iwal=2*l;
     size_t j=3, jc=ip-3;
     for (; j<ipph-1; j+=2, jc-=2)
       {
       iwal+=l; if (iwal>ip) iwal-=ip;
-      Cmplx<T0> xwal=wal[iwal];
+      Cmplx<T0> xwal=fwd ? csarr[iwal].conj() : csarr[iwal];
       iwal+=l; if (iwal>ip) iwal-=ip;
-      Cmplx<T0> xwal2=wal[iwal];
+      Cmplx<T0> xwal2=fwd ? csarr[iwal].conj() : csarr[iwal];
       for (size_t ik=0; ik<idl1; ++ik)
         {
         CX2(ik,l).r += CH2(ik,j).r*xwal.r+CH2(ik,j+1).r*xwal2.r;
         CX2(ik,l).i += CH2(ik,j).i*xwal.r+CH2(ik,j+1).i*xwal2.r;
         CX2(ik,lc).r -= CH2(ik,jc).i*xwal.i+CH2(ik,jc-1).i*xwal2.i;
         CX2(ik,lc).i += CH2(ik,jc).r*xwal.i+CH2(ik,jc-1).r*xwal2.i;
         }
       }
     for (; j<ipph; ++j, --jc)
       {
       iwal+=l; if (iwal>ip) iwal-=ip;
-      Cmplx<T0> xwal=wal[iwal];
+      Cmplx<T0> xwal=fwd ? csarr[iwal].conj() : csarr[iwal];
       for (size_t ik=0; ik<idl1; ++ik)
         {
         CX2(ik,l).r += CH2(ik,j).r*xwal.r;
         CX2(ik,l).i += CH2(ik,j).i*xwal.r;
         CX2(ik,lc).r -= CH2(ik,jc).i*xwal.i;
         CX2(ik,lc).i += CH2(ik,jc).r*xwal.i;
         }
@@ -757,20 +754,19 @@
           idij=(jc-1)*(ido-1)+i-1;
           special_mul<fwd>(x2,wa[idij],CX(i,k,jc));
           }
         }
     }
   }
 
-template<bool fwd, typename T> void pass_all(T c[], T0 fct) const
+template<bool fwd, typename T> T *pass_all(T c[], T ch[], T0 fct) const
   {
-  if (length==1) { c[0]*=fct; return; }
+  if (length==1) { c[0]*=fct; return c; }
   size_t l1=1;
-  aligned_array<T> ch(length);
-  T *p1=c, *p2=ch.data();
+  T *p1=c, *p2=ch;
 
   for(size_t k1=0; k1<fact.size(); k1++)
     {
     size_t ip=fact[k1].fct;
     size_t l2=ip*l1;
     size_t ido = length/l2;
     if     (ip==4)
@@ -791,14 +787,25 @@
       {
       passg<fwd>(ido, ip, l1, p1, p2, fact[k1].tw, fact[k1].tws);
       std::swap(p1,p2);
       }
     std::swap(p1,p2);
     l1=l2;
     }
+  if (fct!=1.)
+    for (size_t i=0; i<length; ++i)
+      p1[i] *= fct;
+  return p1;
+  }
+
+template<bool fwd, typename T> void pass_all(T c[], T0 fct) const
+  {
+  if (length==1) { c[0]*=fct; return; }
+  aligned_array<T> ch(length);
+  auto p1 = pass_all<fwd>(c, ch.data(), T0(1));
   if (p1!=c)
     {
     if (fct!=1.)
       for (size_t i=0; i<length; ++i)
         c[i] = ch[i]*fct;
     else
       memcpy (c,p1,length*sizeof(T));
@@ -808,14 +815,16 @@
       for (size_t i=0; i<length; ++i)
         c[i] *= fct;
   }
 
   public:
     template<typename T> void exec(T c[], T0 fct, bool fwd) const
       { fwd ? pass_all<true>(c, fct) : pass_all<false>(c, fct); }
+    template<typename T> T *exec(T c[], T ch[], T0 fct, bool fwd) const
+      { return fwd ? pass_all<true>(c, ch, fct) : pass_all<false>(c, ch, fct); }
 
   private:
     DUCC0_NOINLINE void factorize()
       {
       size_t len=length;
       while ((len&7)==0)
         { add_factor(8); len>>=3; }
@@ -881,14 +890,16 @@
       {
       if (length==0) throw std::runtime_error("zero-length FFT requested");
       if (length==1) return;
       factorize();
       mem.resize(twsize());
       comp_twiddle();
       }
+
+    size_t bufsize() const { return length; }
   };
 
 //
 // real-valued FFTPACK transforms
 //
 
 template<typename T0> class rfftp
@@ -1562,20 +1573,19 @@
       else
         if (fct!=1.)
           for (size_t i=0; i<n; ++i)
             c[i] *= fct;
       }
 
   public:
-    template<typename T> void exec(T c[], T0 fct, bool r2hc) const
+    template<typename T> T *exec(T c[], T ch[], T0 fct, bool r2hc) const
       {
-      if (length==1) { c[0]*=fct; return; }
+      if (length==1) { c[0]*=fct; return c; }
       size_t n=length, nf=fact.size();
-      aligned_array<T> ch(n);
-      T *p1=c, *p2=ch.data();
+      T *p1=c, *p2=ch;
 
       if (r2hc)
         for(size_t k1=0, l1=n; k1<nf;++k1)
           {
           size_t k=nf-k1-1;
           size_t ip=fact[k].fct;
           size_t ido=n / l1;
@@ -1606,16 +1616,24 @@
           else if(ip==5)
             radb5(ido, l1, p1, p2, fact[k].tw);
           else
             radbg(ido, ip, l1, p1, p2, fact[k].tw, fact[k].tws);
           std::swap (p1,p2);
           l1*=ip;
           }
+      copy_and_norm(p1, p1, length, fct);
+      return p1;
+      }
 
-      copy_and_norm(c,p1,n,fct);
+    template<typename T> void exec(T c[], T0 fct, bool r2hc) const
+      {
+      if (length==1) { c[0]*=fct; return; }
+      aligned_array<T> ch(length);
+      auto p1 = exec(c, ch.data(), T0(1), r2hc);
+      copy_and_norm(c,p1,length,fct);
       }
 
   private:
     void factorize()
       {
       size_t len=length;
       while ((len%4)==0)
@@ -1690,57 +1708,66 @@
       {
       if (length==0) throw std::runtime_error("zero-length FFT requested");
       if (length==1) return;
       factorize();
       mem.resize(twsize());
       comp_twiddle();
       }
+
+    size_t bufsize() const { return length; }
 };
 
 //
 // complex Bluestein transforms
 //
 
 template<typename T0> class fftblue
   {
   private:
     size_t n, n2;
     cfftp<T0> plan;
     aligned_array<Cmplx<T0>> mem;
     Cmplx<T0> *bk, *bkf;
 
-    template<bool fwd, typename T> void fft(Cmplx<T> c[], T0 fct) const
+    template<bool fwd, typename T> void fft(Cmplx<T> c[], Cmplx<T> buf[], T0 fct) const
       {
-      aligned_array<Cmplx<T>> akf(n2);
+      auto akf = &buf[0];
+      auto akf2 = &buf[n2];
 
       /* initialize a_k and FFT it */
       for (size_t m=0; m<n; ++m)
         special_mul<fwd>(c[m],bk[m],akf[m]);
       auto zero = akf[0]*T0(0);
       for (size_t m=n; m<n2; ++m)
         akf[m]=zero;
 
-      plan.exec (akf.data(),1.,true);
+      auto res = plan.exec (akf,akf2,T0(1),true);
 
       /* do the convolution */
-      akf[0] = akf[0].template special_mul<!fwd>(bkf[0]);
+      res[0] = res[0].template special_mul<!fwd>(bkf[0]);
       for (size_t m=1; m<(n2+1)/2; ++m)
         {
-        akf[m] = akf[m].template special_mul<!fwd>(bkf[m]);
-        akf[n2-m] = akf[n2-m].template special_mul<!fwd>(bkf[m]);
+        res[m] = res[m].template special_mul<!fwd>(bkf[m]);
+        res[n2-m] = res[n2-m].template special_mul<!fwd>(bkf[m]);
         }
       if ((n2&1)==0)
-        akf[n2/2] = akf[n2/2].template special_mul<!fwd>(bkf[n2/2]);
+        res[n2/2] = res[n2/2].template special_mul<!fwd>(bkf[n2/2]);
 
       /* inverse FFT */
-      plan.exec (akf.data(),1.,false);
+      res = plan.exec (res, (res==akf) ? akf2 : akf, T0(1), false);
 
       /* multiply by b_k */
       for (size_t m=0; m<n; ++m)
-        c[m] = akf[m].template special_mul<fwd>(bk[m])*fct;
+        c[m] = res[m].template special_mul<fwd>(bk[m])*fct;
+      }
+
+    template<bool fwd, typename T> void fft(Cmplx<T> c[], T0 fct) const
+      {
+      aligned_array<Cmplx<T>> buf(2*n2);
+      fft<fwd>(c, buf.data(), fct);
       }
 
   public:
     DUCC0_NOINLINE fftblue(size_t length)
       : n(length), n2(util1d::good_size_cmplx(n*2-1)), plan(n2), mem(n+n2/2+1),
         bk(mem.data()), bkf(mem.data()+n)
       {
@@ -1765,42 +1792,57 @@
       for (size_t m=n;m<=(n2-n);++m)
         tbkf[m].Set(0.,0.);
       plan.exec(tbkf.data(),1.,true);
       for (size_t i=0; i<n2/2+1; ++i)
         bkf[i] = tbkf[i];
       }
 
+    size_t bufsize_c() const { return 2*n2; }
+    size_t bufsize_r() const { return 2*bufsize_c(); }
+
     template<typename T> void exec(Cmplx<T> c[], T0 fct, bool fwd) const
       { fwd ? fft<true>(c,fct) : fft<false>(c,fct); }
+    template<typename T> Cmplx<T> *exec(Cmplx<T> c[], Cmplx<T> *buf, T0 fct, bool fwd) const
+      {
+      fwd ? fft<true>(c,buf,fct) : fft<false>(c,buf,fct);
+      return c;
+      }
 
-    template<typename T> void exec_r(T c[], T0 fct, bool fwd)
+    template<typename T> T *exec_r(T c[], T buf[], T0 fct, bool fwd)
       {
-      aligned_array<Cmplx<T>> tmp(n);
+      auto tmp = reinterpret_cast<Cmplx<T> *>(&buf[2*n2]);
+      auto buf2 = reinterpret_cast<Cmplx<T> *>(&buf[0]);
       if (fwd)
         {
         auto zero = T0(0)*c[0];
         for (size_t m=0; m<n; ++m)
           tmp[m].Set(c[m], zero);
-        fft<true>(tmp.data(),fct);
+        fft<true>(tmp,buf2,fct);
         c[0] = tmp[0].r;
-        memcpy (reinterpret_cast<void *>(c+1),
-                reinterpret_cast<void *>(tmp.data()+1), (n-1)*sizeof(T));
+        memcpy (reinterpret_cast<void *>(&c[1]),
+                reinterpret_cast<void *>(&tmp[1]), (n-1)*sizeof(T));
         }
       else
         {
         tmp[0].Set(c[0],c[0]*0);
-        memcpy (reinterpret_cast<void *>(tmp.data()+1),
+        memcpy (reinterpret_cast<void *>(&tmp[1]),
                 reinterpret_cast<void *>(c+1), (n-1)*sizeof(T));
         if ((n&1)==0) tmp[n/2].i=T0(0)*c[0];
         for (size_t m=1; 2*m<n; ++m)
           tmp[n-m].Set(tmp[m].r, -tmp[m].i);
-        fft<false>(tmp.data(),fct);
+        fft<false>(tmp,buf2,fct);
         for (size_t m=0; m<n; ++m)
           c[m] = tmp[m].r;
         }
+      return c;
+      }
+    template<typename T> void exec_r(T c[], T0 fct, bool fwd)
+      {
+      aligned_array<T> buf(4*n2);
+      exec_r(c, buf.data(), fct, fwd);
       }
   };
 
 //
 // flexible (FFTPACK/Bluestein) complex 1D transform
 //
 
@@ -1829,16 +1871,20 @@
         blueplan=std::unique_ptr<fftblue<T0>>(new fftblue<T0>(length));
       else
         packplan=std::unique_ptr<cfftp<T0>>(new cfftp<T0>(length));
       }
 
     template<typename T> DUCC0_NOINLINE void exec(Cmplx<T> c[], T0 fct, bool fwd) const
       { packplan ? packplan->exec(c,fct,fwd) : blueplan->exec(c,fct,fwd); }
+    template<typename T> DUCC0_NOINLINE Cmplx<T> *exec(Cmplx<T> c[], Cmplx<T> buf[], T0 fct, bool fwd) const
+      { return packplan ? packplan->exec(c,buf,fct,fwd) : blueplan->exec(c,buf,fct,fwd); }
 
     size_t length() const { return len; }
+    size_t bufsize() const
+      { return packplan ? packplan->bufsize() : blueplan->bufsize_c(); }
   };
 
 //
 // flexible (FFTPACK/Bluestein) real-valued 1D transform
 //
 
 template<typename T0> class pocketfft_r
@@ -1866,16 +1912,20 @@
         blueplan=std::unique_ptr<fftblue<T0>>(new fftblue<T0>(length));
       else
         packplan=std::unique_ptr<rfftp<T0>>(new rfftp<T0>(length));
       }
 
     template<typename T> DUCC0_NOINLINE void exec(T c[], T0 fct, bool fwd) const
       { packplan ? packplan->exec(c,fct,fwd) : blueplan->exec_r(c,fct,fwd); }
+    template<typename T> DUCC0_NOINLINE T *exec(T c[], T buf[], T0 fct, bool fwd) const
+      { return packplan ? packplan->exec(c,buf,fct,fwd) : blueplan->exec_r(c,buf,fct,fwd); }
 
     size_t length() const { return len; }
+    size_t bufsize() const
+      { return packplan ? packplan->bufsize() : blueplan->bufsize_r(); }
   };
 
 }
 
 using detail_fft::pocketfft_c;
 using detail_fft::pocketfft_r;
 inline size_t good_size_complex(size_t n)
```

### Comparing `ducc0-0.8.0/src/ducc0/math/geom_utils.cc` & `ducc0-0.9.0/src/ducc0/math/geom_utils.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/geom_utils.h` & `ducc0-0.9.0/src/ducc0/math/geom_utils.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/gridding_kernel.h` & `ducc0-0.9.0/src/ducc0/math/gridding_kernel.h`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  *  GNU General Public License for more details.
  *
  *  You should have received a copy of the GNU General Public License
  *  along with this code; if not, write to the Free Software
  *  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
  */
 
-/* Copyright (C) 2020 Max-Planck-Society
+/* Copyright (C) 2020-2021 Max-Planck-Society
    Author: Martin Reinecke */
 
 #ifndef DUCC0_GRIDDING_KERNEL_H
 #define DUCC0_GRIDDING_KERNEL_H
 
 #include <vector>
 #include <memory>
@@ -139,15 +139,15 @@
 class GLFullCorrection: public KernelCorrection
   {
   public:
     GLFullCorrection(size_t W, const function<double(double)> &func)
       {
       supp = W;
       size_t p = size_t(1.5*W)+2;
-      GL_Integrator integ(2*p,1);
+      GL_Integrator integ(2*p);
       x = integ.coordsSymmetric();
       wgtpsi = integ.weightsSymmetric();
       for (size_t i=0; i<x.size(); ++i)
         wgtpsi[i] *= func(x[i])*supp*0.5;
       }
   };
```

### Comparing `ducc0-0.8.0/src/ducc0/math/math_utils.h` & `ducc0-0.9.0/src/ducc0/math/math_utils.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/pointing.cc` & `ducc0-0.9.0/src/ducc0/math/pointing.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/pointing.h` & `ducc0-0.9.0/src/ducc0/math/pointing.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/quaternion.h` & `ducc0-0.9.0/src/ducc0/math/quaternion.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/rangeset.h` & `ducc0-0.9.0/src/ducc0/math/rangeset.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/space_filling.cc` & `ducc0-0.9.0/src/ducc0/math/space_filling.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/space_filling.h` & `ducc0-0.9.0/src/ducc0/math/space_filling.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/unity_roots.h` & `ducc0-0.9.0/src/ducc0/math/unity_roots.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/math/vec3.h` & `ducc0-0.9.0/src/ducc0/math/vec3.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp.h` & `ducc0-0.9.0/src/ducc0/sharp/sharp.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_almhelpers.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp_almhelpers.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_almhelpers.h` & `ducc0-0.9.0/src/ducc0/sharp/sharp_almhelpers.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_core.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp_core.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_core_inc.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp_core_inc.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_geomhelpers.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp_geomhelpers.cc`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_geomhelpers.h` & `ducc0-0.9.0/src/ducc0/sharp/sharp_geomhelpers.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_internal.h` & `ducc0-0.9.0/src/ducc0/sharp/sharp_internal.h`

 * *Files identical despite different names*

### Comparing `ducc0-0.8.0/src/ducc0/sharp/sharp_ylmgen.cc` & `ducc0-0.9.0/src/ducc0/sharp/sharp_ylmgen.cc`

 * *Files identical despite different names*

