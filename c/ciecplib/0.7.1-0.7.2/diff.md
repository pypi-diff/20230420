# Comparing `tmp/ciecplib-0.7.1.tar.gz` & `tmp/ciecplib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciecplib-0.7.1.tar", last modified: Tue Nov 15 16:04:22 2022, max compression
+gzip compressed data, was "ciecplib-0.7.2.tar", last modified: Thu Apr 20 11:23:18 2023, max compression
```

## Comparing `ciecplib-0.7.1.tar` & `ciecplib-0.7.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-09-17 12:57:58.000000 ciecplib-0.7.1/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2022-11-14 23:16:49.000000 ciecplib-0.7.1/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2777 2022-11-15 16:04:22.748178 ciecplib-0.7.1/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1567 2022-01-12 10:36:58.000000 ciecplib-0.7.1/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/ciecplib/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1121 2022-11-15 16:02:45.000000 ciecplib-0.7.1/ciecplib/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2531 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/conftest.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4156 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/cookies.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1852 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3587 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1782 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/logging.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4114 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/requests.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2536 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/sessions.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/ciecplib/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      814 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3808 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tests/test_cookies.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1181 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tests/test_env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/tests/test_kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1116 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/tests/test_requests.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2204 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/tests/test_sessions.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4991 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6143 2022-11-15 15:28:45.000000 ciecplib-0.7.1/ciecplib/tests/test_x509.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/ciecplib/tool/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      827 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tool/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5201 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/tool/ecp_cert_info.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3610 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/tool/ecp_curl.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5883 2022-11-15 13:27:59.000000 ciecplib-0.7.1/ciecplib/tool/ecp_get_cert.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5858 2022-11-14 20:46:26.000000 ciecplib-0.7.1/ciecplib/tool/ecp_get_cookie.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/ciecplib/tool/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      819 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tool/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2010 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/tool/tests/test_common.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2309 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_cert_info.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_curl.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2700 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_get_cert.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2688 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tool/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8910 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/tool/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2022-11-14 23:16:49.000000 ciecplib-0.7.1/ciecplib/ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6961 2022-06-13 15:22:20.000000 ciecplib-0.7.1/ciecplib/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13419 2022-11-15 15:28:45.000000 ciecplib-0.7.1/ciecplib/x509.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/ciecplib.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2777 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1341 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      204 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      233 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2022-11-15 16:04:22.000000 ciecplib-0.7.1/ciecplib.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5193 2022-11-15 16:02:45.000000 ciecplib-0.7.1/ciecplib.spec
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2975 2022-11-15 16:02:45.000000 ciecplib-0.7.1/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)       31 2020-09-17 12:57:58.000000 ciecplib-0.7.1/debian/ciecp-utils.install
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-09-17 12:57:58.000000 ciecplib-0.7.1/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1515 2022-11-14 23:16:49.000000 ciecplib-0.7.1/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2020-09-17 12:57:58.000000 ciecplib-0.7.1/debian/copyright
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/debian/patches/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       26 2022-11-14 23:16:49.000000 ciecplib-0.7.1/debian/patches/series
--rw-r--r--   0 duncan    (1000) duncan    (1000)      290 2022-11-14 23:16:49.000000 ciecplib-0.7.1/debian/patches/setup.cfg-pyopenssl.patch
--rw-r--r--   0 duncan    (1000) duncan    (1000)       29 2020-09-17 12:57:58.000000 ciecplib-0.7.1/debian/python3-ciecplib.install
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      157 2022-11-14 23:16:49.000000 ciecplib-0.7.1/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-11-15 16:04:22.748178 ciecplib-0.7.1/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-09-17 12:57:58.000000 ciecplib-0.7.1/debian/source/format
--rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-13 15:22:20.000000 ciecplib-0.7.1/debian/watch
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-11-15 12:53:44.000000 ciecplib-0.7.1/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2022-11-15 16:04:22.748178 ciecplib-0.7.1/setup.cfg
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2022-11-15 14:40:17.000000 ciecplib-0.7.1/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-09-17 12:57:58.000000 ciecplib-0.7.2/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2022-11-14 23:16:49.000000 ciecplib-0.7.2/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-04-20 11:23:18.609881 ciecplib-0.7.2/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1569 2023-02-14 15:31:52.000000 ciecplib-0.7.2/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.579881 ciecplib-0.7.2/ciecplib/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1121 2023-04-20 11:20:08.000000 ciecplib-0.7.2/ciecplib/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2531 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/conftest.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4156 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/cookies.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1852 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3589 2023-04-20 11:00:56.000000 ciecplib-0.7.2/ciecplib/kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1782 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/logging.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4114 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/requests.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2536 2023-02-14 15:17:22.000000 ciecplib-0.7.2/ciecplib/sessions.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.589881 ciecplib-0.7.2/ciecplib/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      814 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3808 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_cookies.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1181 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-20 09:13:39.000000 ciecplib-0.7.2/ciecplib/tests/test_kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1116 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tests/test_requests.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2204 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tests/test_sessions.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4991 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6143 2022-11-15 15:28:45.000000 ciecplib-0.7.2/ciecplib/tests/test_x509.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.599881 ciecplib-0.7.2/ciecplib/tool/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      827 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5217 2023-04-20 11:00:56.000000 ciecplib-0.7.2/ciecplib/tool/ecp_cert_info.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3610 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tool/ecp_curl.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5883 2022-11-15 13:27:59.000000 ciecplib-0.7.2/ciecplib/tool/ecp_get_cert.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5858 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tool/ecp_get_cookie.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.599881 ciecplib-0.7.2/ciecplib/tool/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      819 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2010 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_common.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2309 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_cert_info.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_curl.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2700 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_get_cert.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2688 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8910 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6961 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13419 2022-11-15 15:28:45.000000 ciecplib-0.7.2/ciecplib/x509.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.579881 ciecplib-0.7.2/ciecplib.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1341 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      204 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      233 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5282 2023-04-20 11:20:08.000000 ciecplib-0.7.2/ciecplib.spec
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3118 2023-04-20 11:20:08.000000 ciecplib-0.7.2/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       31 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/ciecp-utils.install
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1515 2023-04-20 09:13:39.000000 ciecplib-0.7.2/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/copyright
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/patches/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       26 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/patches/series
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      290 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/patches/setup.cfg-pyopenssl.patch
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       29 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/python3-ciecplib.install
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      157 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/source/format
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-13 15:22:20.000000 ciecplib-0.7.2/debian/watch
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-11-15 12:53:44.000000 ciecplib-0.7.2/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2023-04-20 11:23:18.609881 ciecplib-0.7.2/setup.cfg
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2022-11-15 14:40:17.000000 ciecplib-0.7.2/setup.py
```

### Comparing `ciecplib-0.7.1/LICENSE` & `ciecplib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/PKG-INFO` & `ciecplib-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciecplib
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python client for SAML/ECP authentication
 Home-page: https://pypi.org/project/ciecplib
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/ciecplib/issues
 Project-URL: Documentation, https://ciecplib.readthedocs.io/
@@ -40,15 +40,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/ciecplib.svg)](https://anaconda.org/conda-forge/ciecplib/)  
 [![DOI](https://zenodo.org/badge/33156275.svg)](https://zenodo.org/badge/latestdoi/33156275)
 [![License](https://img.shields.io/pypi/l/ciecplib.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/ciecplib.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml)
 [![Codecov](https://img.shields.io/codecov/c/gh/duncanmmacleod/ciecplib?logo=codecov)](https://codecov.io/gh/duncanmmacleod/ciecplib)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9e777f5fe160d1e3e7b6/maintainability)](https://codeclimate.com/github/duncanmmacleod/ciecplib/maintainability)
 [![Documentation](https://readthedocs.org/projects/ciecplib/badge/?version=latest)](https://ciecplib.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://ciecplib.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `ciecplib-0.7.1/README.md` & `ciecplib-0.7.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/ciecplib.svg)](https://anaconda.org/conda-forge/ciecplib/)  
 [![DOI](https://zenodo.org/badge/33156275.svg)](https://zenodo.org/badge/latestdoi/33156275)
 [![License](https://img.shields.io/pypi/l/ciecplib.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/ciecplib.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml)
 [![Codecov](https://img.shields.io/codecov/c/gh/duncanmmacleod/ciecplib?logo=codecov)](https://codecov.io/gh/duncanmmacleod/ciecplib)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9e777f5fe160d1e3e7b6/maintainability)](https://codeclimate.com/github/duncanmmacleod/ciecplib/maintainability)
 [![Documentation](https://readthedocs.org/projects/ciecplib/badge/?version=latest)](https://ciecplib.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://ciecplib.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `ciecplib-0.7.1/ciecplib/__init__.py` & `ciecplib-0.7.2/ciecplib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 from .ui import (
     get_cert,
     get_cookie,
 )
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 __credits__ = "Scott Koranda, Dave Dykstra"
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `ciecplib-0.7.1/ciecplib/conftest.py` & `ciecplib-0.7.2/ciecplib/conftest.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/cookies.py` & `ciecplib-0.7.2/ciecplib/cookies.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/env.py` & `ciecplib-0.7.2/ciecplib/env.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/kerberos.py` & `ciecplib-0.7.2/ciecplib/kerberos.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import re
 import subprocess
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 KLIST_EXE = "klist"
 KLIST_PRINCIPAL_RE = re.compile(
-    r"\nDefault principal: ([\w\.@]+)",
+    r"\nDefault principal: ([\w\\./@]+)",
     re.M,
 )
 
 
 def has_credential(*args, klist=KLIST_EXE):
     """Run ``klist`` to determine whether a kerberos credential is available.
```

### Comparing `ciecplib-0.7.1/ciecplib/logging.py` & `ciecplib-0.7.2/ciecplib/logging.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/requests.py` & `ciecplib-0.7.2/ciecplib/requests.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/sessions.py` & `ciecplib-0.7.2/ciecplib/sessions.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/__init__.py` & `ciecplib-0.7.2/ciecplib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_cookies.py` & `ciecplib-0.7.2/ciecplib/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_env.py` & `ciecplib-0.7.2/ciecplib/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_kerberos.py` & `ciecplib-0.7.2/ciecplib/tests/test_kerberos.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_requests.py` & `ciecplib-0.7.2/ciecplib/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_sessions.py` & `ciecplib-0.7.2/ciecplib/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_utils.py` & `ciecplib-0.7.2/ciecplib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tests/test_x509.py` & `ciecplib-0.7.2/ciecplib/tests/test_x509.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/__init__.py` & `ciecplib-0.7.2/ciecplib/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/ecp_cert_info.py` & `ciecplib-0.7.2/ciecplib/tool/ecp_cert_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 .B "X509_USER_PROXY"
 The default path for the credential file """,
      },
 ]
 
 
 def _hours_minutes(argstring):
-    """Parse the --valid argument as hours:minutes
+    """Parse the --valid argument as hours:minutes.
 
-    Returns the argument as a float in seconds
+    Returns the argument as a float in seconds.
     """
     try:
         hrs, minutes = argstring.split(":")
     except TypeError as exc:
         exc.args = ("--valid argument must be in the format H:M",)
         raise
     return float(hrs) * 3600. + float(minutes) * 60.
@@ -90,14 +90,15 @@
         default=DEFAULT_X509_USER_FILE,
         help="certificate file to read (must exist)",
     )
     parser.add_argument(
         "-v",
         "-valid",
         "--valid",
+        metavar="HH:MM",
         type=_hours_minutes,
         help="time requirement for proxy to be valid",
     )
     parser.add_argument(
         "--verbose",
         action="store_true",
         default=False,
@@ -156,15 +157,15 @@
     dispargs.add_argument(
         "-path",
         "--path",
         action="append_const",
         const="path",
         dest="display",
         default=argparse.SUPPRESS,
-        help="time left until certificate expires",
+        help="path to certificate file",
     )
 
     return parser
 
 
 def parse_args(parser, args=None):
     """Parse and validate the command-line arguments
```

### Comparing `ciecplib-0.7.1/ciecplib/tool/ecp_curl.py` & `ciecplib-0.7.2/ciecplib/tool/ecp_curl.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/ecp_get_cert.py` & `ciecplib-0.7.2/ciecplib/tool/ecp_get_cert.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/ecp_get_cookie.py` & `ciecplib-0.7.2/ciecplib/tool/ecp_get_cookie.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/__init__.py` & `ciecplib-0.7.2/ciecplib/tool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/test_common.py` & `ciecplib-0.7.2/ciecplib/tool/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_cert_info.py` & `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_cert_info.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_curl.py` & `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_curl.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/test_ecp_get_cert.py` & `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_get_cert.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/tests/test_utils.py` & `ciecplib-0.7.2/ciecplib/tool/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/tool/utils.py` & `ciecplib-0.7.2/ciecplib/tool/utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/ui.py` & `ciecplib-0.7.2/ciecplib/ui.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/utils.py` & `ciecplib-0.7.2/ciecplib/utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib/x509.py` & `ciecplib-0.7.2/ciecplib/x509.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib.egg-info/PKG-INFO` & `ciecplib-0.7.2/ciecplib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciecplib
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python client for SAML/ECP authentication
 Home-page: https://pypi.org/project/ciecplib
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/ciecplib/issues
 Project-URL: Documentation, https://ciecplib.readthedocs.io/
@@ -40,15 +40,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/ciecplib.svg)](https://anaconda.org/conda-forge/ciecplib/)  
 [![DOI](https://zenodo.org/badge/33156275.svg)](https://zenodo.org/badge/latestdoi/33156275)
 [![License](https://img.shields.io/pypi/l/ciecplib.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/ciecplib.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/ciecplib/actions/workflows/python.yml)
 [![Codecov](https://img.shields.io/codecov/c/gh/duncanmmacleod/ciecplib?logo=codecov)](https://codecov.io/gh/duncanmmacleod/ciecplib)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9e777f5fe160d1e3e7b6/maintainability)](https://codeclimate.com/github/duncanmmacleod/ciecplib/maintainability)
 [![Documentation](https://readthedocs.org/projects/ciecplib/badge/?version=latest)](https://ciecplib.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://ciecplib.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `ciecplib-0.7.1/ciecplib.egg-info/SOURCES.txt` & `ciecplib-0.7.2/ciecplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/ciecplib.spec` & `ciecplib-0.7.2/ciecplib.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname ciecplib
-%define version 0.7.1
+%define version 0.7.2
 %define release 1
 
 # -- metadata ---------------
 
 Name:      %{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
@@ -122,14 +122,17 @@
 %if 0%{?fedora} >= 26 || 0%{?rhel} >= 8
 %{_mandir}/man1/*.1*
 %endif
 
 # -- changelog --------------
 
 %changelog
+* Thu Apr 20 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.2-1
+- update for 0.7.2
+
 * Tue Nov 15 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.1-1
 - update for 0.7.1
 
 * Wed Nov 02 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.0-2
 - fix metadata sed hack for RHEL<9
 
 * Thu Oct 27 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.0-1
```

### Comparing `ciecplib-0.7.1/debian/changelog` & `ciecplib-0.7.2/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+ciecplib (0.7.2-1) unstable; urgency=low
+
+  * Update for 0.7.2
+
+ -- Duncan Macleod <duncan.macleod@ligo.org>  Thu, 20 Apr 2023 12:02:00 +0100
+
 ciecplib (0.7.1-1) unstable; urgency=low
 
   * Update for 0.7.1
 
  -- Duncan Macleod <duncan.macleod@ligo.org>  Tue, 15 Nov 2022 15:47:00 +0000
 
 ciecplib (0.7.0-1) unstable; urgency=low
```

### Comparing `ciecplib-0.7.1/debian/control` & `ciecplib-0.7.2/debian/control`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/debian/copyright` & `ciecplib-0.7.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/setup.cfg` & `ciecplib-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.1/setup.py` & `ciecplib-0.7.2/setup.py`

 * *Files identical despite different names*

