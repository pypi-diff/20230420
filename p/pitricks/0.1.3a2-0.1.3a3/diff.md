# Comparing `tmp/pitricks-0.1.3a2.tar.gz` & `tmp/pitricks-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitricks-0.1.3a2.tar", last modified: Mon Apr  3 03:52:59 2023, max compression
+gzip compressed data, was "pitricks-0.1.3a3.tar", last modified: Tue Apr  4 04:37:18 2023, max compression
```

## Comparing `pitricks-0.1.3a2.tar` & `pitricks-0.1.3a3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.276780 pitricks-0.1.3a2/
--rw-rw-rw-   0        0        0    35823 2023-01-19 08:44:48.000000 pitricks-0.1.3a2/LICENSE
--rw-rw-rw-   0        0        0      219 2023-04-03 03:52:59.276780 pitricks-0.1.3a2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.218722 pitricks-0.1.3a2/pitricks/
--rw-rw-rw-   0        0        0      121 2023-04-01 07:52:08.000000 pitricks-0.1.3a2/pitricks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.230723 pitricks-0.1.3a2/pitricks/odd_tools/
--rw-rw-rw-   0        0        0        0 2023-01-20 04:15:03.000000 pitricks-0.1.3a2/pitricks/odd_tools/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-01 07:39:29.000000 pitricks-0.1.3a2/pitricks/odd_tools/file_batch_replace.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.234919 pitricks-0.1.3a2/pitricks/odd_tools/method_chain/
--rw-rw-rw-   0        0        0       41 2023-01-25 11:00:42.000000 pitricks-0.1.3a2/pitricks/odd_tools/method_chain/__init__.py
--rw-rw-rw-   0        0        0     4496 2023-04-01 07:54:45.000000 pitricks-0.1.3a2/pitricks/odd_tools/method_chain/main.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.238721 pitricks-0.1.3a2/pitricks/operations/
--rw-rw-rw-   0        0        0        0 2023-01-19 02:49:31.000000 pitricks-0.1.3a2/pitricks/operations/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-03-28 13:56:40.000000 pitricks-0.1.3a2/pitricks/operations/ops.py
--rw-rw-rw-   0        0        0      125 2023-04-01 07:48:40.000000 pitricks-0.1.3a2/pitricks/path.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.240721 pitricks-0.1.3a2/pitricks/tmp/
--rw-rw-rw-   0        0        0       34 2023-01-24 15:08:53.000000 pitricks-0.1.3a2/pitricks/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.244721 pitricks-0.1.3a2/pitricks/tmp/classes/
--rw-rw-rw-   0        0        0       86 2023-01-25 01:34:13.000000 pitricks-0.1.3a2/pitricks/tmp/classes/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-01-25 02:00:15.000000 pitricks-0.1.3a2/pitricks/tmp/classes/chain.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.273646 pitricks-0.1.3a2/pitricks/utils/
--rw-rw-rw-   0        0        0      369 2023-04-03 03:52:19.000000 pitricks-0.1.3a2/pitricks/utils/__init__.py
--rw-rw-rw-   0        0        0     1108 2023-01-25 00:49:09.000000 pitricks-0.1.3a2/pitricks/utils/code_generater.py
--rw-rw-rw-   0        0        0        0 2023-02-16 06:58:34.000000 pitricks-0.1.3a2/pitricks/utils/daemon.py
--rw-rw-rw-   0        0        0     2287 2023-03-28 13:54:02.000000 pitricks-0.1.3a2/pitricks/utils/handle_exp.py
--rw-rw-rw-   0        0        0        0 2023-02-22 13:22:41.000000 pitricks-0.1.3a2/pitricks/utils/lock.py
--rw-rw-rw-   0        0        0     1085 2023-04-01 07:36:28.000000 pitricks-0.1.3a2/pitricks/utils/log.py
--rw-rw-rw-   0        0        0     4613 2023-04-01 07:37:12.000000 pitricks-0.1.3a2/pitricks/utils/mp_workflow.py
--rw-rw-rw-   0        0        0     1930 2023-04-01 07:37:28.000000 pitricks-0.1.3a2/pitricks/utils/reflect.py
--rw-rw-rw-   0        0        0      956 2023-03-28 13:50:09.000000 pitricks-0.1.3a2/pitricks/utils/relative_import_everywhere.py
--rw-rw-rw-   0        0        0     4368 2023-01-24 13:32:50.000000 pitricks-0.1.3a2/pitricks/utils/retry.py
--rw-rw-rw-   0        0        0      602 2023-01-24 13:34:04.000000 pitricks-0.1.3a2/pitricks/utils/sync.py
--rw-rw-rw-   0        0        0      860 2023-01-23 10:37:27.000000 pitricks-0.1.3a2/pitricks/utils/test.py
--rw-rw-rw-   0        0        0      528 2023-04-01 07:51:06.000000 pitricks-0.1.3a2/pitricks/utils/types.py
--rw-rw-rw-   0        0        0     2061 2023-03-24 02:00:01.000000 pitricks-0.1.3a2/pitricks/utils/use_pool.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:52:59.226724 pitricks-0.1.3a2/pitricks.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-03 03:52:58.000000 pitricks-0.1.3a2/pitricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-04-03 03:52:59.000000 pitricks-0.1.3a2/pitricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 03:52:58.000000 pitricks-0.1.3a2/pitricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-03 03:52:58.000000 pitricks-0.1.3a2/pitricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 03:52:59.277779 pitricks-0.1.3a2/setup.cfg
--rw-rw-rw-   0        0        0      263 2023-04-03 03:52:45.000000 pitricks-0.1.3a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.170634 pitricks-0.1.3a3/
+-rw-rw-rw-   0        0        0    35823 2023-01-19 08:44:48.000000 pitricks-0.1.3a3/LICENSE
+-rw-rw-rw-   0        0        0      219 2023-04-04 04:37:18.168632 pitricks-0.1.3a3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.048139 pitricks-0.1.3a3/pitricks/
+-rw-rw-rw-   0        0        0      121 2023-04-01 07:52:08.000000 pitricks-0.1.3a3/pitricks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.072135 pitricks-0.1.3a3/pitricks/odd_tools/
+-rw-rw-rw-   0        0        0        0 2023-01-20 04:15:03.000000 pitricks-0.1.3a3/pitricks/odd_tools/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 07:39:29.000000 pitricks-0.1.3a3/pitricks/odd_tools/file_batch_replace.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.081136 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/
+-rw-rw-rw-   0        0        0       41 2023-01-25 11:00:42.000000 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/__init__.py
+-rw-rw-rw-   0        0        0     4496 2023-04-01 07:54:45.000000 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/main.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.089137 pitricks-0.1.3a3/pitricks/operations/
+-rw-rw-rw-   0        0        0        0 2023-01-19 02:49:31.000000 pitricks-0.1.3a3/pitricks/operations/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-03-28 13:56:40.000000 pitricks-0.1.3a3/pitricks/operations/ops.py
+-rw-rw-rw-   0        0        0      125 2023-04-01 07:48:40.000000 pitricks-0.1.3a3/pitricks/path.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.094154 pitricks-0.1.3a3/pitricks/tmp/
+-rw-rw-rw-   0        0        0       34 2023-01-24 15:08:53.000000 pitricks-0.1.3a3/pitricks/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.104136 pitricks-0.1.3a3/pitricks/tmp/classes/
+-rw-rw-rw-   0        0        0       86 2023-01-25 01:34:13.000000 pitricks-0.1.3a3/pitricks/tmp/classes/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-01-25 02:00:15.000000 pitricks-0.1.3a3/pitricks/tmp/classes/chain.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.162632 pitricks-0.1.3a3/pitricks/utils/
+-rw-rw-rw-   0        0        0      369 2023-04-03 03:52:19.000000 pitricks-0.1.3a3/pitricks/utils/__init__.py
+-rw-rw-rw-   0        0        0     1108 2023-01-25 00:49:09.000000 pitricks-0.1.3a3/pitricks/utils/code_generater.py
+-rw-rw-rw-   0        0        0        0 2023-02-16 06:58:34.000000 pitricks-0.1.3a3/pitricks/utils/daemon.py
+-rw-rw-rw-   0        0        0     2304 2023-04-03 09:46:38.000000 pitricks-0.1.3a3/pitricks/utils/handle_exp.py
+-rw-rw-rw-   0        0        0        0 2023-02-22 13:22:41.000000 pitricks-0.1.3a3/pitricks/utils/lock.py
+-rw-rw-rw-   0        0        0     1088 2023-04-03 08:01:37.000000 pitricks-0.1.3a3/pitricks/utils/log.py
+-rw-rw-rw-   0        0        0     4613 2023-04-01 07:37:12.000000 pitricks-0.1.3a3/pitricks/utils/mp_workflow.py
+-rw-rw-rw-   0        0        0     1930 2023-04-01 07:37:28.000000 pitricks-0.1.3a3/pitricks/utils/reflect.py
+-rw-rw-rw-   0        0        0      956 2023-03-28 13:50:09.000000 pitricks-0.1.3a3/pitricks/utils/relative_import_everywhere.py
+-rw-rw-rw-   0        0        0     4368 2023-04-03 08:54:39.000000 pitricks-0.1.3a3/pitricks/utils/retry.py
+-rw-rw-rw-   0        0        0      602 2023-01-24 13:34:04.000000 pitricks-0.1.3a3/pitricks/utils/sync.py
+-rw-rw-rw-   0        0        0      860 2023-01-23 10:37:27.000000 pitricks-0.1.3a3/pitricks/utils/test.py
+-rw-rw-rw-   0        0        0      528 2023-04-01 07:51:06.000000 pitricks-0.1.3a3/pitricks/utils/types.py
+-rw-rw-rw-   0        0        0     2167 2023-04-03 07:37:13.000000 pitricks-0.1.3a3/pitricks/utils/use_pool.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.065136 pitricks-0.1.3a3/pitricks.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-04 04:37:18.171633 pitricks-0.1.3a3/setup.cfg
+-rw-rw-rw-   0        0        0      263 2023-04-03 09:48:36.000000 pitricks-0.1.3a3/setup.py
```

### Comparing `pitricks-0.1.3a2/LICENSE` & `pitricks-0.1.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/odd_tools/method_chain/main.py` & `pitricks-0.1.3a3/pitricks/odd_tools/method_chain/main.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/operations/ops.py` & `pitricks-0.1.3a3/pitricks/operations/ops.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/tmp/classes/chain.py` & `pitricks-0.1.3a3/pitricks/tmp/classes/chain.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/code_generater.py` & `pitricks-0.1.3a3/pitricks/utils/code_generater.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/handle_exp.py` & `pitricks-0.1.3a3/pitricks/utils/handle_exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,23 @@
   if echo:
     traceback.print_exc()
   
   if log_level!=-1:
     logging.log(log_level, traceback.format_exc())
 
 
-def catch_exp(func: Callable[..., T1],
+def catch_exp(func: Callable[..., T1], 
+              *args, 
               _echo=False,
               _log_level=-1,
               _raise_exp=False,
               _catch_classes: Exps = Exception,
               _catch_regex: Union[str, re.Pattern] = ".*",
               _failed_return: Optional[T2] = None,
-              *args, **kwargs) -> Union[T1, Optional[T2]]:
+              **kwargs) -> Union[T1, Optional[T2]]:
   """执行func函数, 参数给args和kwargs, 如果发生异常, 则根据其他参数处理异常
   如果log_level为-1, 则不记录日志, 否则记录日志, 且日志级别为log_level; 可以传入logging.DEBUG等常量"""
   if not isinstance(_catch_classes, tuple):
     _catch_classes = (_catch_classes, )
 
   try:
     return func(*args, **kwargs)
```

### Comparing `pitricks-0.1.3a2/pitricks/utils/mp_workflow.py` & `pitricks-0.1.3a3/pitricks/utils/mp_workflow.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/reflect.py` & `pitricks-0.1.3a3/pitricks/utils/reflect.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/relative_import_everywhere.py` & `pitricks-0.1.3a3/pitricks/utils/relative_import_everywhere.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/retry.py` & `pitricks-0.1.3a3/pitricks/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/sync.py` & `pitricks-0.1.3a3/pitricks/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/test.py` & `pitricks-0.1.3a3/pitricks/utils/test.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/types.py` & `pitricks-0.1.3a3/pitricks/utils/types.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a2/pitricks/utils/use_pool.py` & `pitricks-0.1.3a3/pitricks/utils/use_pool.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,40 +3,42 @@
 from queue import Queue, Empty
 
 T = TypeVar('T')
 T1 = TypeVar('T1')
 
 class PoolProtocol(Protocol[T]):
   "Of course you can add more parameters to the get methods without reporting an error"
-  def put(self, obj: T): pass
-  def get(self) -> Union[T, None]: pass
+  def put(self, obj: T, /): ...
+  def get_or_none(self) -> Union[T, None]: ...
 
 class ExamplePool(Generic[T]):
   def __init__(self) -> None:
     super().__init__()
     self.q = Queue()
   
   def put(self, obj: T):
     self.q.put(obj)
   
-  def get(self) -> Union[T, None]:
+  def get_or_none(self) -> Union[T, None]:
     try:
       return self.q.get_nowait()
     except Empty:
       return None
 
-def use_pool(Tp: Type[T], pool: PoolProtocol[T1]) -> Type[T]:
+def use_pool(Tp: Type[T], 
+             pool: Optional[PoolProtocol[T1]] = None) -> Type[T]:
   "请自行在__init__中检测是否需要重新初始化实例"
+  pool: PoolProtocol[T1] = pool or ExamplePool()
   class NewTp:
     def __new__(cls, *args, **kwargs):
-      obj = pool.get()
+      obj = pool.get_or_none()
       if obj is None:
         obj = object.__new__(Tp, *args, **kwargs)
       new_tp = super().__new__(cls)
-      super().__setattr__(new_tp, 'me', obj)
+      object.__setattr__(new_tp, 'me', obj)
       return new_tp
     
     def __init__(self, *args, **kwargs):
       super().__init__()
       super().__getattribute__('me').__init__(*args, **kwargs)
     
     def __del__(self):
```

### Comparing `pitricks-0.1.3a2/pitricks.egg-info/SOURCES.txt` & `pitricks-0.1.3a3/pitricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

