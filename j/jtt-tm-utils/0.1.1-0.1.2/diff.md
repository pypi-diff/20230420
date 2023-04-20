# Comparing `tmp/jtt-tm-utils-0.1.1.tar.gz` & `tmp/jtt-tm-utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtt-tm-utils-0.1.1.tar", last modified: Fri Mar 17 07:32:43 2023, max compression
+gzip compressed data, was "jtt-tm-utils-0.1.2.tar", last modified: Thu Apr 20 07:07:58 2023, max compression
```

## Comparing `jtt-tm-utils-0.1.1.tar` & `jtt-tm-utils-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 07:32:43.157158 jtt-tm-utils-0.1.1/
--rw-rw-rw-   0        0        0       62 2019-01-09 08:06:40.000000 jtt-tm-utils-0.1.1/.gitignore
--rw-rw-rw-   0        0        0      665 2023-03-17 07:32:43.157158 jtt-tm-utils-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-03-17 07:32:18.000000 jtt-tm-utils-0.1.1/README.md
--rw-rw-rw-   0        0        0      502 2018-12-10 02:54:33.000000 jtt-tm-utils-0.1.1/gencodeFile.yml
-drwxrwxrwx   0        0        0        0 2023-03-17 07:32:43.125907 jtt-tm-utils-0.1.1/jtt_tm_utils/
--rw-rw-rw-   0        0        0      284 2023-03-17 07:32:27.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/__init__.py
--rw-rw-rw-   0        0        0     9281 2022-08-08 08:12:08.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/consul_handle.py
--rw-rw-rw-   0        0        0     9481 2023-03-17 07:26:06.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/kong.py
--rw-rw-rw-   0        0        0       56 2018-12-19 08:06:50.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/log.py
--rw-rw-rw-   0        0        0     9179 2023-03-16 03:32:19.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/sync_basedata.py
--rw-rw-rw-   0        0        0      530 2020-12-25 03:25:07.000000 jtt-tm-utils-0.1.1/jtt_tm_utils/timeutil.py
-drwxrwxrwx   0        0        0        0 2023-03-17 07:32:43.141534 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/
--rw-rw-rw-   0        0        0      665 2023-03-17 07:32:43.000000 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-03-17 07:32:43.000000 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 07:32:43.000000 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-12-10 08:00:22.000000 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-03-17 07:32:43.000000 jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       40 2023-02-03 08:01:46.000000 jtt-tm-utils-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 07:32:43.157158 jtt-tm-utils-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1783 2019-01-11 02:03:22.000000 jtt-tm-utils-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-17 07:32:43.157158 jtt-tm-utils-0.1.1/tests/
--rw-rw-rw-   0        0        0      547 2023-03-16 03:36:27.000000 jtt-tm-utils-0.1.1/tests/test_consul.py
--rw-rw-rw-   0        0        0      307 2018-12-10 07:45:03.000000 jtt-tm-utils-0.1.1/tests/test_sync.py
--rw-rw-rw-   0        0        0     3929 2023-03-16 03:14:50.000000 jtt-tm-utils-0.1.1/tests/test_syncdata.py
--rw-rw-rw-   0        0        0     1849 2023-03-16 03:36:27.000000 jtt-tm-utils-0.1.1/tests/test_task.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:07:58.356964 jtt-tm-utils-0.1.2/
+-rw-rw-rw-   0        0        0       62 2019-01-09 08:06:40.000000 jtt-tm-utils-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0      665 2023-04-20 07:07:58.356964 jtt-tm-utils-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-04-20 07:02:05.000000 jtt-tm-utils-0.1.2/README.md
+-rw-rw-rw-   0        0        0      502 2018-12-10 02:54:33.000000 jtt-tm-utils-0.1.2/gencodeFile.yml
+drwxrwxrwx   0        0        0        0 2023-04-20 07:07:58.350895 jtt-tm-utils-0.1.2/jtt_tm_utils/
+-rw-rw-rw-   0        0        0      284 2023-04-20 07:00:44.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/__init__.py
+-rw-rw-rw-   0        0        0     9281 2022-08-08 08:12:08.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/consul_handle.py
+-rw-rw-rw-   0        0        0     9481 2023-03-17 07:26:06.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/kong.py
+-rw-rw-rw-   0        0        0       56 2018-12-19 08:06:50.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/log.py
+-rw-rw-rw-   0        0        0     9663 2023-04-20 03:36:22.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/sync_basedata.py
+-rw-rw-rw-   0        0        0      530 2020-12-25 03:25:07.000000 jtt-tm-utils-0.1.2/jtt_tm_utils/timeutil.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:07:58.356964 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-04-20 07:07:58.000000 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-04-20 07:07:58.000000 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 07:07:58.000000 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-12-10 08:00:22.000000 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-20 07:07:58.000000 jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       40 2023-02-03 08:01:46.000000 jtt-tm-utils-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 07:07:58.356964 jtt-tm-utils-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1783 2019-01-11 02:03:22.000000 jtt-tm-utils-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:07:58.356964 jtt-tm-utils-0.1.2/tests/
+-rw-rw-rw-   0        0        0      547 2023-03-16 03:36:27.000000 jtt-tm-utils-0.1.2/tests/test_consul.py
+-rw-rw-rw-   0        0        0      307 2018-12-10 07:45:03.000000 jtt-tm-utils-0.1.2/tests/test_sync.py
+-rw-rw-rw-   0        0        0     3929 2023-03-16 03:14:50.000000 jtt-tm-utils-0.1.2/tests/test_syncdata.py
+-rw-rw-rw-   0        0        0     1849 2023-03-16 03:36:27.000000 jtt-tm-utils-0.1.2/tests/test_task.py
```

### Comparing `jtt-tm-utils-0.1.1/PKG-INFO` & `jtt-tm-utils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtt-tm-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: jtt common tools
 Home-page: UNKNOWN
 Author: candyabc
 Author-email: hfcandyabc@163.com
 License: maxwin
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jtt-tm-utils-0.1.1/README.md` & `jtt-tm-utils-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -53,8 +53,13 @@
 fix update line_config bug。
 ```
 * 2023/03/17
 ```text
 v 0.1.1
 
 kong register add host param
+```
+* 2023/04/20
+```text
+v 0.1.2
+sync basedata 同步支持 key_type='set' 方式
 ```
```

### Comparing `jtt-tm-utils-0.1.1/jtt_tm_utils/consul_handle.py` & `jtt-tm-utils-0.1.2/jtt_tm_utils/consul_handle.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/jtt_tm_utils/kong.py` & `jtt-tm-utils-0.1.2/jtt_tm_utils/kong.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/jtt_tm_utils/sync_basedata.py` & `jtt-tm-utils-0.1.2/jtt_tm_utils/sync_basedata.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 re+=list(filter(lambda name:name.startswith(condition),self.names))
 
         return re
 
     def config(self,redis,names=DEFAULT_NAMES,loop=None):
         def make_func(name):
             def _method(self,key):
-                return self.get_bdobj(name,key)
+                return self.get_bdobj(name,key )
 
             return _method
 
         self._redis =redis
         for cname in names:
             if type(cname)==tuple:
                 name, fields = cname
@@ -116,14 +116,16 @@
                                 handled = self.custom_reload()
                                 if not handled:
                                     self.clear_all()
 
                             else:
                                 if name =='line_config': # line.config的 update name 是line_config 所以要调整一下
                                     name = 'line.config'
+                                elif name =='vehiclegroup_vehicles':
+                                    name ='vehiclegroup.vehicles'
                                 logger.info(f'notify update {name} {key}')
                                 bd_names = self.update_associations(name)
                                 for bd_name in bd_names:
                                     handled =self.custom_reload_item(bd_name,key)
                                     if not handled :
                                         self.remove_bdobj(bd_name,key)
 
@@ -153,14 +155,21 @@
             elif key_type =='string':
                 data = await self.rds.get(rds_key)
                 if data is not None:
                     try:
                         obj = json.loads(data.decode())
                     except Exception as e:
                         logger.error('key:%s load error:%s' %(rds_key,str(e)))
+            elif key_type =='set':
+                data = await self.rds.smembers(rds_key)
+                if data is not None:
+                    try:
+                        obj =[item.decode() for item in data]
+                    except Exception as e:
+                        logger.error('key:%s load error:%s' % (rds_key, str(e)))
             else:
                 logger.error('key:%s not support key_type:%s' %(rds_key,key_type))
             if data_isnull(obj):
                 logger.warning('the %s(%s) is not exist!' % (name, key))
                 obj =None
             # if self.cache.get(name) is None:
             #     self.cache[name] = {}
```

### Comparing `jtt-tm-utils-0.1.1/jtt_tm_utils/timeutil.py` & `jtt-tm-utils-0.1.2/jtt_tm_utils/timeutil.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/jtt_tm_utils.egg-info/PKG-INFO` & `jtt-tm-utils-0.1.2/jtt_tm_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtt-tm-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: jtt common tools
 Home-page: UNKNOWN
 Author: candyabc
 Author-email: hfcandyabc@163.com
 License: maxwin
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jtt-tm-utils-0.1.1/setup.py` & `jtt-tm-utils-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/tests/test_consul.py` & `jtt-tm-utils-0.1.2/tests/test_consul.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/tests/test_syncdata.py` & `jtt-tm-utils-0.1.2/tests/test_syncdata.py`

 * *Files identical despite different names*

### Comparing `jtt-tm-utils-0.1.1/tests/test_task.py` & `jtt-tm-utils-0.1.2/tests/test_task.py`

 * *Files identical despite different names*

