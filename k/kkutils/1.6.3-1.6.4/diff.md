# Comparing `tmp/kkutils-1.6.3.tar.gz` & `tmp/kkutils-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkutils-1.6.3.tar", last modified: Tue Apr 18 08:52:44 2023, max compression
+gzip compressed data, was "kkutils-1.6.4.tar", last modified: Thu Apr 20 03:35:51 2023, max compression
```

## Comparing `kkutils-1.6.3.tar` & `kkutils-1.6.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/
--rw-r--r--   0 root         (0) root         (0)      703 2023-04-18 08:52:44.391119 kkutils-1.6.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.387119 kkutils-1.6.3/kkutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.3/processor.py
--rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 08:52:44.391119 kkutils-1.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-18 08:52:41.000000 kkutils-1.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/tornado_utils/
--rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.3/tornado_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.3/tornado_utils/application.py
--rw-r--r--   0 root         (0) root         (0)    10043 2023-03-06 03:11:06.000000 kkutils-1.6.3/tornado_utils/basehandler.py
--rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.3/tornado_utils/userhandler.py
--rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.3/tornado_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/utils/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.3/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10382 2023-03-19 08:31:21.000000 kkutils-1.6.3/utils/base_utils.py
--rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/cached_property.py
--rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-02-19 15:22:17.000000 kkutils-1.6.3/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)    10693 2022-11-04 03:27:22.000000 kkutils-1.6.3/utils/curl_utils.py
--rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.3/utils/db_utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4007 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/email_utils.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.3/utils/fire.py
--rw-r--r--   0 root         (0) root         (0)    26362 2023-02-19 15:22:17.000000 kkutils-1.6.3/utils/http_utils.py
--rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.3/utils/log_utils.py
--rw-r--r--   0 root         (0) root         (0)     6577 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.3/utils/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.3/utils/xdb_searcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.044617 kkutils-1.6.4/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-20 03:35:51.044617 kkutils-1.6.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.040617 kkutils-1.6.4/kkutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-20 03:35:51.000000 kkutils-1.6.4/kkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.4/processor.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 03:35:51.044617 kkutils-1.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-04-20 03:35:48.000000 kkutils-1.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.040617 kkutils-1.6.4/tornado_utils/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.4/tornado_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.4/tornado_utils/application.py
+-rw-r--r--   0 root         (0) root         (0)    10043 2023-03-06 03:11:06.000000 kkutils-1.6.4/tornado_utils/basehandler.py
+-rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.4/tornado_utils/userhandler.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.4/tornado_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.044617 kkutils-1.6.4/utils/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.4/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10413 2023-04-20 03:33:38.000000 kkutils-1.6.4/utils/base_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/cached_property.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-02-19 15:22:17.000000 kkutils-1.6.4/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    10693 2022-11-04 03:27:22.000000 kkutils-1.6.4/utils/curl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.4/utils/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/email_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.4/utils/fire.py
+-rw-r--r--   0 root         (0) root         (0)    26362 2023-02-19 15:22:17.000000 kkutils-1.6.4/utils/http_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.4/utils/log_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.4/utils/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.4/utils/xdb_searcher.py
```

### Comparing `kkutils-1.6.3/PKG-INFO` & `kkutils-1.6.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.3
+Version: 1.6.4
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.3/kkutils.egg-info/PKG-INFO` & `kkutils-1.6.4/kkutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.3
+Version: 1.6.4
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.3/kkutils.egg-info/SOURCES.txt` & `kkutils-1.6.4/kkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/processor.py` & `kkutils-1.6.4/processor.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/setup.py` & `kkutils-1.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Last modified: 2019-04-07 00:07:43
 '''
 
 from setuptools import setup
 
 setup(
     name="kkutils",
-    version="1.6.3",
+    version="1.6.4",
     description="python utils",
     author="digua",
     author_email="zkdfbb@qq.com",
     url="https://www.ishield.cn",
     license="MIT",
     python_requires='>=3.6',
     data_files=[('', ['requirements.txt'])],
```

### Comparing `kkutils-1.6.3/tornado_utils/application.py` & `kkutils-1.6.4/tornado_utils/application.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/tornado_utils/basehandler.py` & `kkutils-1.6.4/tornado_utils/basehandler.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/tornado_utils/userhandler.py` & `kkutils-1.6.4/tornado_utils/userhandler.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/tornado_utils/utils.py` & `kkutils-1.6.4/tornado_utils/utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/__init__.py` & `kkutils-1.6.4/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/base_utils.py` & `kkutils-1.6.4/utils/base_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 
 
 yaml.add_constructor('!include', _include_yaml)
 
 
 class tqdm(tqdm):
 
-    def __init__(self, iterable=None, **kwargs):
+    def __init__(self, iterable=None, colour='green', **kwargs):
         if not kwargs.get('total') and isinstance(iterable, Cursor):
             kwargs.setdefault('total', iterable.count())
         kwargs.setdefault('disable', not sys.stdout.isatty())
-        super().__init__(iterable, **kwargs)
+        super().__init__(iterable, colour=colour, **kwargs)
 
     def update(self, n=None, total=None, incr=None):
         if total is not None:
             self.total = total
         if n is not None:
             super().update(max(0, n - self.n))
         elif incr is not None:
```

### Comparing `kkutils-1.6.3/utils/cached_property.py` & `kkutils-1.6.4/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/config_utils.py` & `kkutils-1.6.4/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/crypto.py` & `kkutils-1.6.4/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/curl_utils.py` & `kkutils-1.6.4/utils/curl_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/db_utils.py` & `kkutils-1.6.4/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/decorator.py` & `kkutils-1.6.4/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/email_utils.py` & `kkutils-1.6.4/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/fire.py` & `kkutils-1.6.4/utils/fire.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/http_utils.py` & `kkutils-1.6.4/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/log_utils.py` & `kkutils-1.6.4/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/rabbitmq.py` & `kkutils-1.6.4/utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/stopwatch.py` & `kkutils-1.6.4/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.3/utils/xdb_searcher.py` & `kkutils-1.6.4/utils/xdb_searcher.py`

 * *Files identical despite different names*

