# Comparing `tmp/ats_case-0.4.6.tar.gz` & `tmp/ats_case-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.6.tar", last modified: Wed Apr 19 08:19:03 2023, max compression
+gzip compressed data, was "ats_case-0.5.0.tar", last modified: Thu Apr 20 08:36:57 2023, max compression
```

## Comparing `ats_case-0.4.6.tar` & `ats_case-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.100308 ats_case-0.4.6/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-19 08:19:03.098312 ats_case-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.618795 ats_case-0.4.6/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.6/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.885468 ats_case-0.4.6/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.6/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    16757 2023-04-19 08:16:19.000000 ats_case-0.4.6/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10234 2023-04-19 08:13:19.000000 ats_case-0.4.6/ats_case/case/context.py
--rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.6/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5441 2023-04-19 06:25:18.000000 ats_case-0.4.6/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.958275 ats_case-0.4.6/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.6/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.6/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.6/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.039705 ats_case-0.4.6/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.6/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.6/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3083 2023-04-19 08:18:35.000000 ats_case-0.4.6/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:03.089337 ats_case-0.4.6/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.6/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.6/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-19 08:19:02.749829 ats_case-0.4.6/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-19 08:19:02.000000 ats_case-0.4.6/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 08:19:01.000000 ats_case-0.4.6/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 08:19:03.100308 ats_case-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-19 08:18:43.000000 ats_case-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.648786 ats_case-0.5.0/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-20 08:36:57.644797 ats_case-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.111681 ats_case-0.5.0/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.0/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.344051 ats_case-0.5.0/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.0/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17372 2023-04-20 03:36:42.000000 ats_case-0.5.0/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.0/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     6444 2023-04-20 08:35:14.000000 ats_case-0.5.0/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5591 2023-04-20 08:34:36.000000 ats_case-0.5.0/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.423838 ats_case-0.5.0/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.0/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.0/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.0/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.539533 ats_case-0.5.0/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.0/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.0/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.0/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.588949 ats_case-0.5.0/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.0/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.0/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.212926 ats_case-0.5.0/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:36:57.648786 ats_case-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-20 05:29:46.000000 ats_case-0.5.0/setup.py
```

### Comparing `ats_case-0.4.6/PKG-INFO` & `ats_case-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.6
+Version: 0.5.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.6/README.md` & `ats_case-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.6/ats_case/case/command.py` & `ats_case-0.5.0/ats_case/case/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import time
 
 from ats_base.common import func
 from ats_base.log.logger import logger
 from ats_base.service import app, pro, em, udm
 
 from ats_case.case.context import Context
-from ats_case.common.enum import ProClazz, OperationClazz
-from ats_case.common.error import APIError, ClientReturnError, MeterOperationError
+from ats_case.common.enum import *
+from ats_case.common.error import *
 
 """
     常用操作命令
 """
 
 
 def send(context: Context, todo: dict, types=2, retry_times: int = 3):
@@ -129,14 +129,33 @@
             sd = sd.replace('&{}'.format(r), v)
         else:
             sd = sd.replace('\'&{}\''.format(r), str(v))
 
     return eval(sd)
 
 
+def step_annotation(**param):
+    """
+    测试步骤方法注释 - 装饰器
+    :param param: desc-测试步骤描述
+    :return:
+    """
+    desc = param.get('desc')
+
+    def decorate(callback):
+        def fn(*args, **kwargs):
+            client().message(desc).show(args[0])
+            r = callback(*args, **kwargs)
+            return r
+        
+        return fn
+
+    return decorate
+
+
 """
     通讯协议篇
 """
 
 
 def meter(protocol: str):
     return Meter(protocol)
@@ -209,15 +228,15 @@
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context, index=0):
         # 异常判断 - 客户端返回结果
         if self._frame is None or len(self._frame) <= 0:
-            raise ClientReturnError(self._frame)
+            raise ClientError(self._frame)
 
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(
             func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.test_sn))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         # 异常判断 - 协议服务返回结果
@@ -454,40 +473,38 @@
 
 class App(object):
     def __init__(self):
         self._name = 'app'
         self._operation = None
         self._message = None
         self._parameter = None
-        self._command = None
 
     def operation(self, command: str):
         self._operation = command
         return self
 
     def message(self, msg: str):
         self._message = msg
         return self
 
     def parameter(self, param=None):
         self._parameter = param
         return self
 
-    def encode(self):
-        logger.info('~ @APP-> operation:{} message:{}'.format(self._operation, self._message))
-        self._command = {'{}:{}'.format(self._name, self._operation): self._message}
-
-        return self._command
-
-    def decode(self):
-        pass
+    def show(self, context: Context, types=2):
+        logger.info('~ @APP-> operation:{} message:{}'.format('show', self._message))
+        send(context, todo={'{}:{}'.format(self._name, 'show'): self._message}, types=types)
+
+    def error(self, context: Context, types=2):
+        logger.info('~ @APP-> operation:{} message:{}'.format('error', self._message))
+        send(context, todo={'{}:{}'.format(self._name, 'error'): self._message}, types=types)
 
     def exec(self, context: Context):
-        self.encode()
-        send(context, todo=self._command)
+        logger.info('~ @APP-> operation:{} message:{}'.format(self._operation, self._message))
+        send(context, todo={'{}:{}'.format(self._name, self._operation): self._message})
 
 
 """
     平台篇
 """
```

### Comparing `ats_case-0.4.6/ats_case/case/context.py` & `ats_case-0.5.0/ats_case/case/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 from ats_base.service import mm
 
+from ats_case.common.enum import WorkMode, ScriptClazz
+
 
 class Context(object):
     """
     测试用例上下文
     """
 
-    def __init__(self, sn, cid, pos):
+    def __init__(self, sn):
         self._test_sn = sn
-        self._case_id = cid
-        self._pos = pos
-        self._script = None
-        self._mode = None
-        self._acd_url = None
         self._parse()
 
     def _parse(self):
-        tl = mm.Dict.get("debug:log", self._test_sn)
+        tl = mm.Dict.get("test:log", self._test_sn)
 
+        self._mode = WorkMode(tl.get('mode'))
         self._tester = self.Tester(tl.get('tester'))
         self._case = self.Case(tl.get('usercase'))
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
+        # 运行时
         self._runtime = self.Runtime()
         self._session = self.Session(self)
         # Debug模式 - 测试开发人员本机调试数据比对服务使用
         self._acd_url = tl.get('acd_url')
 
-    #     self._bench = self.Bench(tl.get('bench'))
-    #     self._case = self.Case(tl.get('cases').get(self.case_id))
-    #     self._meter = tl.get('meter')
-    #     self._runtime = self.Runtime()
-    #
-    #     self._exec_result = None
-    #     if self.rerun == 1:
-    #         # self._exec_result = tl.get('exec_result').get(str(self._case_id))
-    #         # try:
-    #         #     self.runtime.loop_index = self.exec_result.get('loop_index', 0)
-    #         # except:
-    #         try:
-    #             self.runtime.loop_index = int(self._cache.get('loop_index'))
-    #         except:
-    #             self.runtime.loop_index = 0
+    @property
+    def mode(self):
+        return self._mode
 
     @property
     def test_sn(self):
         return self._test_sn
 
     @property
     def tester(self):
@@ -60,18 +47,14 @@
         return self._case
 
     @property
     def meter(self):
         return self._meter
 
     @property
-    def mode(self):
-        return self._mode
-
-    @property
     def runtime(self):
         return self._runtime
 
     @property
     def session(self):
         return self._session
 
@@ -140,16 +123,17 @@
         def __init__(self, data: dict):
             self._id = data.get('id', -1)
             self._name = data.get('name', 'test')
             #         self._code = data.get('code')
             #         self._version = data.get('version')
             #         self._scope = data.get('scope')
             #         self._purpose = data.get('purpose')
+            self._script = ScriptClazz(data.get('script', 1))
             self._control = data.get('control', {})
-            self._steps = data.get('steps', {})
+            self._steps = data.get('steps')
 
         #         self._script = 'script.{}'.format(data.get('script'))
         #         self._bench_step_orders = data.get('bench_step_orders', [])
         #         # 用户发起的参数
         #         self._req_params = self.ReqParams(data.get('req_params'))
         #
         #         lps = data.get('loops')
@@ -172,14 +156,18 @@
             return self._id
 
         @property
         def name(self):
             return self._name
 
         @property
+        def script(self):
+            return self._script
+
+        @property
         def control(self):
             return self._control
 
         @property
         def steps(self):
             return self._steps
```

### Comparing `ats_case-0.4.6/ats_case/case/executor.py` & `ats_case-0.5.0/ats_case/case/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from importlib import import_module
 
+from ats_base.common import func
 from ats_base.log.logger import logger
 
 from ats_case.case import translator, command
 from ats_case.case.context import Context
 from ats_case.common.enum import *
 from ats_case.common.error import *
 
@@ -13,35 +14,51 @@
         if context.mode == WorkMode.FORMAL:
             FormalExecutor(context).exec()
         else:
             DebugExecutor(context).exec()
     except APIError as ae:
         logger.info(str(ae))
         raise AssertionError(str(ae))
-    except ClientReturnError as ce:
+    except ClientError as ce:
         logger.info(str(ce))
-        command.client().operation("app:error").message(str(ce))
+        command.client().message(str(ce)).error(context)
         raise AssertionError(str(ce))
     except MeterOperationError as pe:
         logger.info(str(pe))
-        command.client().operation("app:error").message(str(pe))
+        command.client().message(str(pe)).error(context)
         raise AssertionError(str(pe))
     except Exception as e:
         logger.error(str(e))
-        command.client().operation("app:error").message(str(e))
+        command.client().message(str(e)).error(context)
         raise AssertionError(str(e))
 
 
 class Executor(object):
     def __init__(self, context: Context):
         self._context = context
         self._model = None
 
     def exec(self):
-        pass
+        steps = self.handle()
+
+        index = 0
+        while index < len(steps):
+            self._context.runtime.step = steps[index]
+            if self.loop_meet():
+                self.loop_exec()
+            else:
+                self.step_exec()
+
+            if self._context.runtime.step > (index + 1):
+                index = self._context.runtime.step
+            else:
+                index += 1
+
+    def handle(self):
+        return []
 
     def is_exec(self):
         ifs = self._context.case.control.get('ifs')
         if ifs is not None and type(ifs) is dict and len(ifs) > 0:
             for func, values in ifs.items():
                 if command.ats().operation(func).parameter(values).exec(self._context):
                     return False
@@ -84,54 +101,68 @@
         return False
 
     def loop_exec(self):
         logger.info('~ @TCC-LOOP-> loops[#{}] start. -range {}:{}  -count {}'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
             self._context.runtime.loop_end_step, self._context.runtime.loop_count))
 
-        command.client().operation('show').message('循环[#{}]开始, 步骤范围[{}-{}], 共{}次'.format(
+        command.client().message('循环[#{}]开始, 步骤范围[{}-{}], 共{}次'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
-            self._context.runtime.loop_end_step, self._context.runtime.loop_count)).exec(self._context)
+            self._context.runtime.loop_end_step, self._context.runtime.loop_count)).show(self._context)
 
         # while self._context.runtime.loop_index < self._context.runtime.loop_count:
         for i in range(1, self._context.runtime.loop_count + 1):
             self._context.runtime.loop_index = i
 
             logger.info('~ @TCC-LOOP-> loops[#{}], -count {}, -index {}'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
                 self._context.runtime.loop_index))
-            command.client().operation('show').message('循环[#{}], 共{}次, 当前第{}次'.format(
+            command.client().message('循环[#{}], 共{}次, 当前第{}次'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
-                self._context.runtime.loop_index)).exec(self._context)
+                self._context.runtime.loop_index)).show(self._context)
 
             for j in range(self._context.runtime.loop_start_step, self._context.runtime.loop_end_step + 1):
                 self._context.runtime.step = j
                 self.step_exec()
 
-        command.client().operation('show').message("循环结束...").exec(self._context)
+        command.client().message("循环结束...").show(self._context)
         logger.info('~ @TCC-LOOP-> loops[#{}] end.'.format(self._context.runtime.loop_sn))
         self._context.runtime.loop_sn += 1
 
 
+def extract_steps(content: list):
+    n_s = []
+    for s in content:
+        if s.upper().find('STEP_') >= 0:
+            num = func.extract_digit(s)
+            n_s.append(int(num))
+
+    sorted_n_s = sorted(n_s)
+
+    return sorted_n_s
+
+
 class FormalExecutor(Executor):
-    def exec(self):
+    def handle(self):
         # 分为两种情况: 1. 手动编写脚本 2.自动编写脚本
-        pass
+        if self._context.case.script == ScriptClazz.AUTO:
+            steps = translator.translate(self._context)
+            self._model = import_module('script.auto.{}.tsm_{}'.format(self._context.tester.username.lower()
+                                                                       , self._context.meter.pos))
+        else:
+            self._model = import_module('script.manual.formal.{}'.format(self._context.case.steps))
+            steps = extract_steps(dir(self._model))
 
+        return steps
 
-class DebugExecutor(Executor):
-    def exec(self):
-        steps = translator.translate(self._context)
-        self._model = import_module('script.debug.{}.steps'.format(self._context.tester.username.lower()))
 
-        index = 0
-        while index < len(steps):
-            self._context.runtime.step = steps[index]
-            if self.loop_meet():
-                self.loop_exec()
-            else:
-                self.step_exec()
+class DebugExecutor(Executor):
+    def handle(self):
+        if self._context.case.script == ScriptClazz.AUTO:
+            steps = translator.translate(self._context)
+            self._model = import_module('script.auto.{}.tsm_{}'.format(self._context.tester.username.lower()
+                                                                       , self._context.meter.pos))
+        else:
+            self._model = import_module('script.manual.debug.{}'.format(self._context.case.steps))
+            steps = extract_steps(dir(self._model))
 
-            if self._context.runtime.step > (index + 1):
-                index = self._context.runtime.step
-            else:
-                index += 1
+        return steps
```

### Comparing `ats_case-0.4.6/ats_case/case/translator.py` & `ats_case-0.5.0/ats_case/case/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,39 +23,40 @@
 
         with open(self._script(), "w", encoding='utf-8') as f:
             f.write(self._gen_import())
             f.write(self._gen_line(2))
 
             for step, operations in self._context.case.steps.items():
                 steps.append(int(step))
-                f.write(self._gen_step(int(step)))
+                f.write(self._gen_step(int(step), operations))
 
                 tab_count = 1
                 # for op in operations:
                 f.write(self._gen_tab(tab_count) + self._gen_operation(operations) + self._gen_line(1))
                 # if self._contain_keyword(step):
                 #     tab_count += 1
                 f.write(self._gen_line(2))
 
             return steps
 
     def _script(self):
-        user_dir = func.makeDir(func.project_dir(), 'script', 'debug', self._context.tester.username)
-        script_file = os.path.join(user_dir, 'steps.py')
+        user_dir = func.makeDir(func.project_dir(), 'script', 'auto', self._context.tester.username)
+        script_file = os.path.join(user_dir, 'tsm_{}.py'.format(self._context.meter.pos))
 
         if not os.path.exists(user_dir):
             Path(user_dir).mkdir(parents=True, exist_ok=True)
 
         return script_file
 
     def _gen_import(self):
         return 'from ats_case.case import command' + self.LINE + 'from ats_case.case.context import Context' + self.LINE
 
-    def _gen_step(self, step: int):
-        return 'def step_{}(context: Context):{}'.format(step, self.LINE)
+    def _gen_step(self, step: int, op: dict):
+        return '@command.step_annotation(desc={}){}'.format(op.get('desc', ''), self.LINE) + \
+               'def step_{}(context: Context):{}'.format(step, self.LINE)
 
     def _gen_tab(self, count: int):
         ts = ''
         for i in range(count):
             ts += self.TAB
 
         return ts
```

### Comparing `ats_case-0.4.6/ats_case/common/error.py` & `ats_case-0.5.0/ats_case/common/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return "MeterOperationError - 电表操作错误, {}".format(repr(self.value))
 
 
-class ClientReturnError(Exception):
+class ClientError(Exception):
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return "ClientReturnError - 客户端返回结果为空. {}".format(repr(self.value))
```

### Comparing `ats_case-0.4.6/ats_case/manage/core.py` & `ats_case-0.5.0/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.6/ats_case/manage/start.py` & `ats_case-0.5.0/ats_case/manage/start.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,22 +23,19 @@
         pass
 
 
 class ExecMode(object):
     def __init__(self, data: dict):
         self._data = data
         self._username = self._data.get('tester').get('username', '')
-        self._sn = self.gen_sn()
+        self._sn = self._username.upper() + self._now()
 
     def run(self):
         pass
 
-    def gen_sn(self):
-        return self._username.upper() + self._now()
-
     def _now(self):
         return datetime.now().strftime('%y%m%d%H%M%S%f')
 
     def _save(self):
         pass
 
     def _flush(self, **kwargs):
@@ -66,39 +63,39 @@
         self._save()
         cases = self._data.pop('cases')
         meters = self._data.pop('meters')
 
         for case in cases:
             for meter in meters:
                 self._flush(case=case, meter=meter)
-                # 客户端出来的参数需要缓存case, meter，context从数据库里去原始数据
                 # i = 0 执行操作表台 传入参数index
-                th = threading.Thread(target=self._exec, daemon=True)
-                th.start()
+                # th = threading.Thread(target=self._exec, daemon=True)
+                # th.start()
+                self._exec()
 
     def _exec(self):
         pytest.main(
             ["-sv", self._build(WorkMode.FORMAL), '--sn={}'.format(self._sn)])
 
     def _save(self):
         pass  # 存数据库
 
     def _flush(self, **kwargs):
         self._data['usercase'] = kwargs['case']
         self._data['meter'] = kwargs['meter']
         self._sn += ':{}:{}'.format(kwargs['case']['id'], kwargs['meter']['pos'])
-        mm.Dict.put('debug:log', self._sn, self._data)
+        mm.Dict.put('test:log', self._sn, self._data)
 
 
 class DebugMode(ExecMode):
     def __init__(self, data: dict):
         super().__init__(data)
 
     def run(self):
         self._flush()
         pytest.main(["-sv", self._build(WorkMode.DEBUG), '--sn={}'.format(self._sn)])
 
     def _flush(self):
         case = self._data.get('usercase')
         meter = self._data.get('meter')
         self._sn += ':{}:{}'.format(case['id'], meter['pos'])
-        mm.Dict.put('debug:log', self._sn, self._data)
+        mm.Dict.put('test:log', self._sn, self._data)
```

### Comparing `ats_case-0.4.6/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.0/ats_case/template/testcase_v1.tmp`

 * *Files 7% similar despite different names*

```diff
@@ -9,31 +9,31 @@
         测试用例前置步骤
         :return:
         """
         logger.info('~ @TCC-MSG-> TEST CASE[{}-{}] METER[{}] START...'.format(CaseContext.case.id,
                                                                               CaseContext.case.name,
                                                                               CaseContext.meter.no))
         try:
-            command.send(CaseContext, todo={
-                              'app:show': {'msg': '[{}]开始测试 - 测试用例[{}], 电表[{}]...'.format(
-                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}}, types=0)
+            msg = {'msg': '[{}]开始测试 - 测试用例[{}], 电表[{}]...'.format(
+                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}
+            command.client().message(msg).show(CaseContext, types=0)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
 
     @pytest.mark.run(order=3)
     def test_after(self, CaseContext):
         """
         测试用例后置步骤
         :return:
         """
         try:
-            command.send(CaseContext, todo={
-                              'app:show': {'msg': '[{}]结束测试 - 测试用例[{}], 电表[{}].'.format(
-                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}}, types=1)
+            msg = {'msg': '[{}]结束测试 - 测试用例[{}], 电表[{}].'.format(
+                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}
+            command.client().message(msg).show(CaseContext, types=1)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
 
         logger.info('~ @TCC-MSG-> TEST CASE[{}-{}] METER[{}] END.'.format(CaseContext.case.id,
                                                                           CaseContext.case.name,
                                                                           CaseContext.meter.no))
```

### Comparing `ats_case-0.4.6/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.0/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.6
+Version: 0.5.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.6/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.0/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.6/setup.py` & `ats_case-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.6",
+    version="0.5.0",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

