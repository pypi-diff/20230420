# Comparing `tmp/cool_cache-0.3.0.tar.gz` & `tmp/cool_cache-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_cache-0.3.0.tar", last modified: Wed Apr 19 04:11:24 2023, max compression
+gzip compressed data, was "cool_cache-0.3.1.tar", last modified: Thu Apr 20 04:08:34 2023, max compression
```

## Comparing `cool_cache-0.3.0.tar` & `cool_cache-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.466011 cool_cache-0.3.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-19 04:11:24.465872 cool_cache-0.3.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.464931 cool_cache-0.3.0/cool_cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7189 2023-04-19 04:10:44.000000 cool_cache-0.3.0/cool_cache/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.465706 cool_cache-0.3.0/cool_cache.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       57 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-19 04:11:24.466052 cool_cache-0.3.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1208 2022-11-09 13:57:56.000000 cool_cache-0.3.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.173319 cool_cache-0.3.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-20 04:08:34.173138 cool_cache-0.3.1/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.172066 cool_cache-0.3.1/cool_cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7261 2023-04-20 03:52:36.000000 cool_cache-0.3.1/cool_cache/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.172969 cool_cache-0.3.1/cool_cache.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-20 04:08:33.000000 cool_cache-0.3.1/cool_cache.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-20 04:08:33.000000 cool_cache-0.3.1/cool_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       57 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-20 04:08:34.173378 cool_cache-0.3.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1208 2022-11-09 13:57:56.000000 cool_cache-0.3.1/setup.py
```

### Comparing `cool_cache-0.3.0/PKG-INFO` & `cool_cache-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_cache
-Version: 0.3.0
+Version: 0.3.1
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.0/cool_cache/__init__.py` & `cool_cache-0.3.1/cool_cache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,19 +147,19 @@
                 if arg_hash in data.cache:
                     return data.cache[arg_hash]
                 # if args not in cache, run the function
                 else:
                     result = input_func(*args, **kwargs)
                     data.cache[arg_hash] = result # save the output for next time
                     data_to_push = CacheData()
-                    data_to_push = deepcopy(data.calculated)
-                    data_to_push = deepcopy(data.cache_file_name)
-                    data_to_push = deepcopy(data.deep_hash)
-                    data_to_push = deepcopy(data.cache)
-                    worker_que.put(data, block=False) # use a different process for saving to disk to prevent slowdown
+                    data_to_push.calculated      = deepcopy(data.calculated)
+                    data_to_push.cache_file_name = deepcopy(data.cache_file_name)
+                    data_to_push.deep_hash       = deepcopy(data.deep_hash)
+                    data_to_push.cache           = deepcopy(data.cache)
+                    worker_que.put(data_to_push, block=False) # use a different process for saving to disk to prevent slowdown
                     return result
             return wrapper
         return real_decorator
 
 def worker():
     global worker_que
     while threading.main_thread().is_alive():
```

### Comparing `cool_cache-0.3.0/cool_cache.egg-info/PKG-INFO` & `cool_cache-0.3.1/cool_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-cache
-Version: 0.3.0
+Version: 0.3.1
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.0/setup.py` & `cool_cache-0.3.1/setup.py`

 * *Files identical despite different names*

