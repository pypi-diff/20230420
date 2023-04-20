# Comparing `tmp/m-abac-anhnt-1.0.3.tar.gz` & `tmp/m-abac-anhnt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-anhnt-1.0.3.tar", last modified: Thu Apr 20 10:05:14 2023, max compression
+gzip compressed data, was "m-abac-anhnt-1.0.4.tar", last modified: Thu Apr 20 10:27:00 2023, max compression
```

## Comparing `m-abac-anhnt-1.0.3.tar` & `m-abac-anhnt-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,89 @@
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/PKG-INFO
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1115 2023-04-13 06:35:19.000000 m-abac-anhnt-1.0.3/README.md
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/PKG-INFO
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      212 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/SOURCES.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/dependency_links.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/requires.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/top_level.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.3/pyproject.toml
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/setup.cfg
--rw-r--r--   0 mobio     (1000) mobio     (1000)     9779 2023-04-20 10:05:03.000000 m-abac-anhnt-1.0.3/setup.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/PKG-INFO
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1115 2023-04-13 06:35:19.000000 m-abac-anhnt-1.0.4/README.md
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/PKG-INFO
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     3378 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/requires.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        6 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/top_level.txt
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       70 2023-04-20 10:26:41.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-20 08:11:29.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     8187 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/call_api.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    13365 2023-04-12 06:41:17.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/pdp.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/base.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1934 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/schema.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2762 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/result_access.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.4/pyproject.toml
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/setup.cfg
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     9780 2023-04-20 10:23:54.000000 m-abac-anhnt-1.0.4/setup.py
```

### Comparing `m-abac-anhnt-1.0.3/PKG-INFO` & `m-abac-anhnt-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.3/README.md` & `m-abac-anhnt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/PKG-INFO` & `m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.3/setup.py` & `m-abac-anhnt-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.3',  # Required
+    version='1.0.4',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -139,26 +139,26 @@
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
     keywords="mobio, mobio-engine, m-abac",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
-    package_dir={'mobio.libs.abac': 'm_abac'},  # Optional
+    # package_dir={'mobio.libs.abac': 'm_abac'},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    # packages=find_namespace_packages(include=["m_abac.*"]),  # Required
-    packages = find_packages(where="m_abac.*"),
+    packages=find_namespace_packages(include=["mobio.*"]),  # Required
+    # packages = find_packages(where="m_abac.*"),
     # namespace_packages=["mobio"],  # Optional
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires=">=3",
     # This field lists other packages that your project depends on to run.
```

