# Comparing `tmp/dg-itest-0.0.3.tar.gz` & `tmp/dg-itest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg-itest-0.0.3.tar", last modified: Thu Apr 20 10:42:13 2023, max compression
+gzip compressed data, was "dg-itest-0.0.4.tar", last modified: Thu Apr 20 10:57:41 2023, max compression
```

## Comparing `dg-itest-0.0.3.tar` & `dg-itest-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.269011 dg-itest-0.0.3/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      150 2023-04-20 10:13:24.000000 dg-itest-0.0.3/MANIFEST.in
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:42:13.268900 dg-itest-0.0.3/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     6266 2023-04-20 09:12:27.000000 dg-itest-0.0.3/README.md
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.267603 dg-itest-0.0.3/dg_itest/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1567 2023-04-20 08:51:12.000000 dg-itest-0.0.3/dg_itest/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.268391 dg-itest-0.0.3/dg_itest/servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.3/dg_itest/servers/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.264119 dg-itest-0.0.3/dg_itest/servers/dg_servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:34:49.000000 dg-itest-0.0.3/dg_itest/servers/dg_servers/__init__
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/dg_servers/dg_requsts.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/dg_servers/dg_singleton.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.265186 dg-itest-0.0.3/dg_itest/servers/file_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.3/dg_itest/servers/file_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/file_handler/file_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/file_handler/xlsx_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/file_handler/yaml_handler.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.266210 dg-itest-0.0.3/dg_itest/servers/test_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.3/dg_itest/servers/test_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-20 08:25:46.000000 dg-itest-0.0.3/dg_itest/servers/test_handler/test_file.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     3477 2023-04-20 07:15:06.000000 dg-itest-0.0.3/dg_itest/servers/test_handler/test_item.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.267282 dg-itest-0.0.3/dg_itest/utils/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.3/dg_itest/utils/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-18 13:18:59.000000 dg-itest-0.0.3/dg_itest/utils/cache.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-20 09:01:39.000000 dg-itest-0.0.3/dg_itest/utils/diff_helper.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-20 08:19:36.000000 dg-itest-0.0.3/dg_itest/utils/env_generater.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-18 13:18:59.000000 dg-itest-0.0.3/dg_itest/utils/string_helper.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:42:13.268300 dg-itest-0.0.3/dg_itest.egg-info/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1329 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/SOURCES.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/dependency_links.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/not-zip-safe
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/requires.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-20 10:42:13.000000 dg-itest-0.0.3/dg_itest.egg-info/top_level.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-20 10:42:13.269044 dg-itest-0.0.3/setup.cfg
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-20 10:42:10.000000 dg-itest-0.0.3/setup.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.268612 dg-itest-0.0.4/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      150 2023-04-20 10:13:24.000000 dg-itest-0.0.4/MANIFEST.in
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:57:41.268482 dg-itest-0.0.4/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     6266 2023-04-20 09:12:27.000000 dg-itest-0.0.4/README.md
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267008 dg-itest-0.0.4/dg_itest/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1579 2023-04-20 10:57:05.000000 dg-itest-0.0.4/dg_itest/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267896 dg-itest-0.0.4/dg_itest/servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.261618 dg-itest-0.0.4/dg_itest/servers/dg_servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:34:49.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_requsts.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_singleton.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.264030 dg-itest-0.0.4/dg_itest/servers/file_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/file_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/xlsx_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/yaml_handler.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.265193 dg-itest-0.0.4/dg_itest/servers/test_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-20 08:25:46.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/test_file.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     3477 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/test_item.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.266747 dg-itest-0.0.4/dg_itest/utils/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/utils/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-18 13:18:59.000000 dg-itest-0.0.4/dg_itest/utils/cache.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-20 09:01:39.000000 dg-itest-0.0.4/dg_itest/utils/diff_helper.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-20 08:19:36.000000 dg-itest-0.0.4/dg_itest/utils/env_generater.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-18 13:18:59.000000 dg-itest-0.0.4/dg_itest/utils/string_helper.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267794 dg-itest-0.0.4/dg_itest.egg-info/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1458 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/not-zip-safe
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/requires.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/top_level.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-20 10:57:41.268646 dg-itest-0.0.4/setup.cfg
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-20 10:57:06.000000 dg-itest-0.0.4/setup.py
```

### Comparing `dg-itest-0.0.3/README.md` & `dg-itest-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/__init__.py` & `dg-itest-0.0.4/dg_itest/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         local_test_res = test_res
         self.test_src = test_src
 
     def run(self):
         test_report = 'test_report/result/'
 
         if not Path(test_report).exists():
-            Path(test_report).mkdir()
+            Path(test_report).mkdir(parents=True)
 
         pytest.main(['-s', self.test_src, '--alluredir', Path(test_report).resolve().as_posix()])
 
         try:
             # 生成allure report中environment相关配置
             EnvGenerater.generate_env_file(host_url, Path(test_report))
```

### Comparing `dg-itest-0.0.3/dg_itest/servers/dg_servers/dg_requsts.py` & `dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_requsts.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/servers/dg_servers/dg_singleton.py` & `dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_singleton.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/servers/file_handler/file_handler.py` & `dg-itest-0.0.4/dg_itest/servers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/servers/file_handler/xlsx_handler.py` & `dg-itest-0.0.4/dg_itest/servers/file_handler/xlsx_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/servers/test_handler/test_file.py` & `dg-itest-0.0.4/dg_itest/servers/test_handler/test_file.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/servers/test_handler/test_item.py` & `dg-itest-0.0.4/dg_itest/servers/test_handler/test_item.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/utils/diff_helper.py` & `dg-itest-0.0.4/dg_itest/utils/diff_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/utils/env_generater.py` & `dg-itest-0.0.4/dg_itest/utils/env_generater.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest/utils/string_helper.py` & `dg-itest-0.0.4/dg_itest/utils/string_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.3/dg_itest.egg-info/SOURCES.txt` & `dg-itest-0.0.4/dg_itest.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
-./dg_itest/servers/dg_servers/__init__
+./dg_itest/servers/dg_servers/__init__.py
 ./dg_itest/servers/dg_servers/dg_requsts.py
 ./dg_itest/servers/dg_servers/dg_singleton.py
 ./dg_itest/servers/file_handler/__init__.py
 ./dg_itest/servers/file_handler/file_handler.py
 ./dg_itest/servers/file_handler/xlsx_handler.py
 ./dg_itest/servers/file_handler/yaml_handler.py
 ./dg_itest/servers/test_handler/__init__.py
@@ -20,14 +20,17 @@
 dg_itest.egg-info/PKG-INFO
 dg_itest.egg-info/SOURCES.txt
 dg_itest.egg-info/dependency_links.txt
 dg_itest.egg-info/not-zip-safe
 dg_itest.egg-info/requires.txt
 dg_itest.egg-info/top_level.txt
 dg_itest/servers/__init__.py
+dg_itest/servers/dg_servers/__init__.py
+dg_itest/servers/dg_servers/dg_requsts.py
+dg_itest/servers/dg_servers/dg_singleton.py
 dg_itest/servers/file_handler/__init__.py
 dg_itest/servers/file_handler/file_handler.py
 dg_itest/servers/file_handler/xlsx_handler.py
 dg_itest/servers/file_handler/yaml_handler.py
 dg_itest/servers/test_handler/__init__.py
 dg_itest/servers/test_handler/test_file.py
 dg_itest/servers/test_handler/test_item.py
```

### Comparing `dg-itest-0.0.3/setup.py` & `dg-itest-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if not os.path.exists(requirements):  # install from tar
         requirements = 'dg_itest.egg-info/requires.txt'
     with open(requirements) as fp:
         install_requires = fp.read()
     return install_requires.split('\n')
 
 setup(name='dg-itest',
-      version='0.0.3',
+      version='0.0.4',
       description='接口自动化测试框架',
       url='https://github.com/yaitza/dg-itest',
       download_url='https://github.com/yaitza/dg-itest/releases',
       author='yaitza',
       author_email='yaitza@foxmail.com',
       packages=find_packages(),
       package_data={'': ['*.py']},
```

