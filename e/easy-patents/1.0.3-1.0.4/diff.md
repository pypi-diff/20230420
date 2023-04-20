# Comparing `tmp/easy_patents-1.0.3.tar.gz` & `tmp/easy_patents-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_patents-1.0.3.tar", last modified: Thu Apr 20 12:20:11 2023, max compression
+gzip compressed data, was "dist/easy_patents-1.0.4.tar", last modified: Thu Apr 20 13:16:59 2023, max compression
```

## Comparing `easy_patents-1.0.3.tar` & `easy_patents-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/config/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/config/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/sample/
--rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/mail_notify.py
--rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample.py
--rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample_check_due_date.py
--rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample_update_monitor_excel.py
--rw-r--r--   0 root         (0) root         (0)     2808 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/auth_info.py
--rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/delete_caches.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/errors.py
--rw-r--r--   0 root         (0) root         (0)      934 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/get_apitoken.py
--rw-r--r--   0 root         (0) root         (0)    34816 2023-04-20 12:14:28.000000 easy_patents-1.0.3/easy_patents/get_info.py
--rw-r--r--   0 root         (0) root         (0)     1321 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/update_authinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 12:17:12.000000 easy_patents-1.0.3/setup.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 12:20:11.000000 easy_patents-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 12:20:11.000000 easy_patents-1.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/config/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/config/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/sample/
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/mail_notify.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample_check_due_date.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample_update_monitor_excel.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/auth_info.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/delete_caches.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/errors.py
+-rw-r--r--   0 root         (0) root         (0)      934 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/get_apitoken.py
+-rw-r--r--   0 root         (0) root         (0)    35935 2023-04-20 13:15:55.000000 easy_patents-1.0.4/easy_patents/get_info.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/update_authinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 13:16:58.000000 easy_patents-1.0.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 13:16:59.000000 easy_patents-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 13:16:59.000000 easy_patents-1.0.4/setup.cfg
```

### Comparing `easy_patents-1.0.3/easy_patents/sample/mail_notify.py` & `easy_patents-1.0.4/easy_patents/sample/mail_notify.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/sample/sample.py` & `easy_patents-1.0.4/easy_patents/sample/sample.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/sample/sample_check_due_date.py` & `easy_patents-1.0.4/easy_patents/sample/sample_check_due_date.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/sample/sample_update_monitor_excel.py` & `easy_patents-1.0.4/easy_patents/sample/sample_update_monitor_excel.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/auth_info.py` & `easy_patents-1.0.4/easy_patents/auth_info.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/delete_caches.py` & `easy_patents-1.0.4/easy_patents/delete_caches.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/errors.py` & `easy_patents-1.0.4/easy_patents/errors.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/get_apitoken.py` & `easy_patents-1.0.4/easy_patents/get_apitoken.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents/get_info.py` & `easy_patents-1.0.4/easy_patents/get_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,23 +197,48 @@
     '2020008423'
     >>> convert_key("特開２０２０／８４２３号")
     '2020008423'
     >>> convert_key("2020008423")
     '2020008423'
     >>> convert_key("特許第1234567号")
     '1234567'
+    >>> convert_key("意願２０２０－８４２３号")
+    '意願2020008423'
+    >>> convert_key("商願２０２０－８４２３号")
+    '商願2020008423'
+    >>> convert_key("特願２０２０－８４２３号", law="design")
+    '特願2020008423'
+    >>> convert_key("商願２０２０－８４２３号", law="design")
+    '商願2020008423'
+    >>> convert_key("意願２０２０－８４２３号", law="design")
+    '2020008423'
+    >>> convert_key("意匠登録２０２０８４２３号", law="design")
+    '20208423'
+    >>> convert_key("商願２０２０－８４２３号", law="trademark")
+    '2020008423'
+    >>> convert_key("商標登録２０２０８４２３号", law="trademark")
+    '20208423'
+    >>> convert_key("特願２０２０－８４２３号", law="trademark")
+    '特願2020008423'
+    >>> convert_key("意願２０２０－８４２３号", law="trademark")
+    '意願2020008423'
     '''
     key = mojimoji.zen_to_han(key)
     if law == "patent":
         key = key.replace("特願", "")
         key = key.replace("特開", "")
         key = key.replace("特表", "")
         key = key.replace("特許", "")
     if law == "design":
-        pass
+        key = key.replace("意願", "")
+        key = key.replace("意匠登録", "")
+    if law == "trademark":
+        key = key.replace("商願", "")
+        key = key.replace("商標登録", "")
+
     key = key.replace("第", "")
     key = key.replace("号", "")
     key = key.replace("公報", "")
     key = zfill_key(key, "-")
     key = zfill_key(key, "/")
     return key
```

### Comparing `easy_patents-1.0.3/easy_patents/update_authinfo.py` & `easy_patents-1.0.4/easy_patents/update_authinfo.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.3/easy_patents.egg-info/SOURCES.txt` & `easy_patents-1.0.4/easy_patents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

